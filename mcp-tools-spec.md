# MCP Tools Required for Wiki Maintenance

This document specifies every MCP tool the wiki-maintainer agent needs to fulfil the workflows defined in `CLAUDE.md`, assuming **no terminal/shell access**.

---

## 1. Filesystem — Read

### `filesystem_read_file`

Read the full contents of a file given its path.

| Field | Value |
|---|---|
| **Used in** | Every workflow (ingest, query, lint, session start) |
| **Why** | Read raw sources from `raw/`, read existing wiki pages, read `index.md`, `log.md`, `glossary.md`, `overview.md`, `CLAUDE.md` |
| **Input** | `{ "path": "string" }` |
| **Output** | File contents as string |

### `filesystem_read_directory` (or `filesystem_list_directory`)

List files and subdirectories at a given path.

| Field | Value |
|---|---|
| **Used in** | Lint (enumerate all pages), ingest (discover existing pages), session start |
| **Why** | Enumerate `wiki/steps/`, `wiki/controls/`, `raw/`, etc. to know what exists |
| **Input** | `{ "path": "string" }` |
| **Output** | Array of file/directory names |

---

## 2. Filesystem — Write

### `filesystem_write_file`

Create a new file or overwrite an existing file at a given path.

| Field | Value |
|---|---|
| **Used in** | Ingest (create source summaries, new entity pages), query (file answers to `analyses/`), lint (apply fixes) |
| **Why** | Create new wiki pages in `wiki/sources/`, `wiki/steps/`, `wiki/controls/`, `wiki/outcomes/`, `wiki/analyses/`, etc. |
| **Input** | `{ "path": "string", "content": "string" }` |
| **Output** | Confirmation |

### `filesystem_edit_file` (or `filesystem_patch_file`)

Apply a targeted edit (search-and-replace or line-range patch) to an existing file without rewriting the whole thing.

| Field | Value |
|---|---|
| **Used in** | Ingest (update existing pages, append to `log.md`, update `index.md`, update `glossary.md`, update `overview.md`), lint (fix inconsistencies), query (append log entry) |
| **Why** | Append entries to `log.md`, add terms to `glossary.md`, add backlinks to existing pages, update frontmatter `updated` dates |
| **Input** | `{ "path": "string", "old_text": "string", "new_text": "string" }` or `{ "path": "string", "insert_at": "end", "content": "string" }` |
| **Output** | Confirmation |

### `filesystem_create_directory`

Create a new directory (including nested paths).

| Field | Value |
|---|---|
| **Used in** | Ingest (when a new entity category is needed) |
| **Why** | CLAUDE.md says "Create subdirectories as needed." New categories may require new folders under `wiki/` |
| **Input** | `{ "path": "string" }` |
| **Output** | Confirmation |

---

## 3. Search

### `filesystem_search_files` (or `grep`)

Search for a text pattern across files in a directory tree. Returns matching file paths and line numbers.

| Field | Value |
|---|---|
| **Used in** | Lint, ingest, query, cross-referencing |
| **Why** | Find all pages that mention a term (terminology discipline), find orphan pages (no `[[page-name]]` links pointing to them), find contradictions, check if a concept already has a page, scan for backlinks |
| **Input** | `{ "path": "string", "pattern": "string", "recursive": true }` |
| **Output** | Array of `{ file, line_number, line_content }` |

### `filesystem_glob` (or `filesystem_find`)

Find files matching a glob pattern (e.g., `wiki/**/*.md`).

| Field | Value |
|---|---|
| **Used in** | Lint (read all pages), ingest (discover all existing pages) |
| **Why** | Get a complete list of every `.md` file in the wiki to iterate over |
| **Input** | `{ "base_path": "string", "pattern": "string" }` |
| **Output** | Array of matching file paths |

---

## 4. Summary: Tool-to-Workflow Matrix

| Tool | Session Start | Ingest | Query | Lint |
|---|---|---|---|---|
| `filesystem_read_file` | x | x | x | x |
| `filesystem_read_directory` | x | x | | x |
| `filesystem_write_file` | | x | x | x |
| `filesystem_edit_file` | | x | x | x |
| `filesystem_create_directory` | | x | | |
| `filesystem_search_files` | | x | x | x |
| `filesystem_glob` | | x | | x |

---

## 5. Optional / Nice-to-Have

These are not strictly required but would improve the agent's capabilities:

### `filesystem_file_info`

Get metadata about a file (size, last modified date, etc.).

| Field | Value |
|---|---|
| **Used in** | Lint (detect stale pages) |
| **Why** | Compare file modification dates against `updated` frontmatter to find pages that may be stale |

### `filesystem_move_file` (or `filesystem_rename`)

Rename or move a file.

| Field | Value |
|---|---|
| **Used in** | Lint, restructuring |
| **Why** | Rename pages to match kebab-case convention, move pages between categories if they were miscategorized |

### `filesystem_delete_file`

Delete a file.

| Field | Value |
|---|---|
| **Used in** | Lint (remove orphan/duplicate pages after user confirmation) |
| **Why** | Clean up pages the user confirms should be removed |

---

## 6. Minimum Viable Toolset

If constrained to the absolute minimum, these **5 tools** cover all CLAUDE.md workflows:

1. **`filesystem_read_file`** — read sources and wiki pages
2. **`filesystem_read_directory`** — list directory contents
3. **`filesystem_write_file`** — create new pages
4. **`filesystem_edit_file`** — update existing pages (append to log, add glossary terms, insert backlinks)
5. **`filesystem_search_files`** — find text across the wiki (cross-referencing, lint, terminology checks)

Without `filesystem_edit_file`, you could fall back to read-then-write-whole-file, reducing the minimum to **4 tools** — but targeted edits are strongly preferred for `log.md` appends and backlink insertions.

# Topology Diagnostics - Extended Conversation

---

**User:** Hi, I need some help with my mechanical model. I've been having issues with meshing and someone mentioned I should check my topology first. Where do I even start?

---

**Chatbot:** Hello! You're on the right track. Before surface meshing, it's highly recommended to validate your model's topology to catch problematic geometry that could cause meshing failures downstream.

The tool you're looking for is called **Topology Diagnostics**. It's a control that diagnoses your model to detect common topology issues including:

- **Thin stripes** – narrow sliver regions on faces
- **Small edges** – edges below a minimum length threshold
- **Overlapping faces** – faces that overlap within a tolerance
- **Intersecting faces** – faces that cross each other

Would you like me to walk you through how to set it up?

---

**User:** Yes please. What kind of control is this exactly? Is it a mesh control or something else?

---

**Chatbot:** Good clarifying question! **Topology Diagnostics** is a **pre-meshing diagnostic control**, not a mesh control itself. It doesn't generate or modify a mesh — instead, it inspects the underlying CAD topology so you can fix problems *before* meshing.

You'll typically find it used in two contexts:

- **Pre-meshing topology diagnostic steps** – to catch problems before surface meshing runs
- **Geometry validation steps** – as part of a broader CAD cleanup workflow

Think of it as a "health check" for your geometry. It flags issues, reports them, and lets you decide whether to clean them up manually or with repair tools.

---

**User:** Got it. So what parameters does it need? I want to make sure I configure it properly.

---

**Chatbot:** The Topology Diagnostics control has five key parameters you'll want to be aware of:

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Defines what the control applies to (Part, Label, or Zone) | — |
| **Thin Stripes Width** | Width threshold for thin stripe detection | 5.0 mm |
| **Small Edges Length** | Minimum edge length for diagnosis | 1.0 mm |
| **Overlapping Face Tolerance** | Tolerance for face overlap detection | 0.1 mm |
| **Intersecting Face Tolerance** | Angle tolerance for face intersection detection | 25 degrees |

A few things worth knowing:

- **Scoping Method** determines *where* the diagnostic runs. You can target a specific **Part**, a **Label**, or a **Zone**.
- The four tolerance parameters (Thin Stripes Width, Small Edges Length, Overlapping Face Tolerance, Intersecting Face Tolerance) are all **parametrizable and publishable**, meaning you can expose them for design studies or reuse across projects.

Do you already know which part you want to diagnose?

---

**User:** Yes, I have a part called "abc" that's been giving me trouble. That's the one I want to scope this to.

---

**Chatbot:** Perfect — scoping to a single part is the cleanest way to isolate the diagnostic. Here's what that looks like:

1. Set **Scoping Method** to `Part`
2. Select the part named **"abc"** from your geometry tree

This will limit the diagnostic to only evaluate the topology within part "abc", ignoring the rest of the assembly. That makes the results much easier to interpret and faster to run.

Do you also want to customize any of the tolerance values, or use defaults for those?

---

**User:** Yes, I want to change two of them. I need the thin face width set to 3 inches and the overlapping face tolerance set to 0.5 mm. The others can stay at default.

---

**Chatbot:** Got it. Here's your full configuration:

## Configuration Summary

| Parameter | Your Value | Notes |
|---|---|---|
| Scoping Method | `Part` → **abc** | Limits diagnostic to part "abc" |
| Thin Stripes Width | **3 in** | Overriding default of 5.0 mm |
| Small Edges Length | 1.0 mm | *Default* |
| Overlapping Face Tolerance | **0.5 mm** | Overriding default of 0.1 mm |
| Intersecting Face Tolerance | 25° | *Default* |

A quick note on your values:

- **3 inches** for Thin Stripes Width is significantly larger than the 5.0 mm default (≈76.2 mm vs 5.0 mm). This will flag much wider stripes as "thin," so expect more hits. That's fine if you're intentionally looking for broader sliver regions.
- **0.5 mm** for Overlapping Face Tolerance is 5× the default (0.1 mm), meaning it will be more permissive in flagging overlaps. Faces that are close but not quite coincident will still show up.

Make sure your units are set correctly in the project before entering `3 in` — some interfaces will auto-convert, but it's worth double-checking.

---

**User:** Good point on the units. Okay, now walk me through actually executing it step by step.

---

**Chatbot:** Here's the full step-by-step workflow:

## Execution Steps

1. **Open your pre-meshing or geometry validation step** in the workflow tree.

2. **Insert a Topology Diagnostics control** under that step.

3. **Configure Scoping:**
   - Scoping Method → `Part`
   - Select part → `abc`

4. **Set tolerance parameters:**
   - Thin Stripes Width → `3 in`
   - Small Edges Length → `1.0 mm` *(leave as default)*
   - Overlapping Face Tolerance → `0.5 mm`
   - Intersecting Face Tolerance → `25 deg` *(leave as default)*

5. **Verify your inputs** — double-check the unit on Thin Stripes Width reads `in` and not `mm`.

6. **Execute the control.**

7. **Review the diagnostic output**, which will list any detected:
   - Thin stripes wider than 3 inches
   - Small edges shorter than 1.0 mm
   - Overlapping faces within 0.5 mm
   - Intersecting faces within 25°

Once it runs, you'll get a report of all flagged entities on part "abc".

---

**User:** What should I do with the results once I see them? Does this control fix the issues automatically?

---

**Chatbot:** Great question — and an important distinction. **Topology Diagnostics only detects issues; it does not repair them automatically.** It's a diagnostic tool, not a repair tool.

Here's how to handle the results:

- **Review each flagged entity** in the diagnostic report. The tool will typically highlight them in the graphics window.
- **Decide severity:** Not every flagged item is necessarily a problem. For example, an intentionally thin feature may be flagged but is still valid for your simulation.
- **Remediate problematic items** using the appropriate geometry repair or cleanup tools in your workflow (e.g., merging small edges, removing overlapping faces, splitting intersecting faces).
- **Re-run Topology Diagnostics** after cleanup to confirm the issues are resolved.

The typical loop looks like: **Diagnose → Inspect → Repair → Re-diagnose → Mesh.**

---

**User:** Makes sense. One more thing — you mentioned the parameters are "parametrizable and publishable." What does that actually mean in practice?

---

**Chatbot:** Good follow-up — this is a useful feature many people overlook.

**Parametrizable** means you can drive the parameter's value from a variable or expression rather than a hardcoded number. For example, instead of typing `3 in` directly, you could link Thin Stripes Width to a project variable like `min_feature_size` that's defined elsewhere.

**Publishable** means you can expose the parameter to a higher level — for instance, to a design study, optimization run, or parent workflow — so it can be varied or controlled externally.

### Practical benefits

- **Design studies:** Run the same diagnostic across multiple geometries with different tolerance sweeps.
- **Consistency:** Define a single tolerance at the project level and have all diagnostic controls inherit it.
- **Reusability:** Share a validated configuration across teams or projects without rebuilding it each time.

For your case with part "abc", if you think you'll re-run this diagnostic on similar parts later, it's worth parameterizing the `3 in` and `0.5 mm` values so you can tweak them once globally rather than editing each control individually.

---

**User:** Awesome, this has been super helpful. Just to make sure I have everything — can you give me a final recap?

---

**Chatbot:** Absolutely! Here's your complete recap:

## Final Recap: Topology Diagnostics for Part "abc"

### What it is
A **pre-meshing diagnostic control** that detects topology issues (thin stripes, small edges, overlapping faces, intersecting faces) before surface meshing.

### Where it's used
- Pre-meshing topology diagnostic steps
- Geometry validation steps

### Your configuration

| Parameter | Value |
|---|---|
| Scoping Method | `Part` → **abc** |
| Thin Stripes Width | **3 in** *(custom)* |
| Small Edges Length | 1.0 mm *(default)* |
| Overlapping Face Tolerance | **0.5 mm** *(custom)* |
| Intersecting Face Tolerance | 25° *(default)* |

### Execution workflow
1. Insert Topology Diagnostics under a pre-meshing/validation step
2. Set scoping to part "abc"
3. Enter your custom tolerances (watch units!)
4. Execute the control
5. Review flagged entities in the report
6. Repair issues with separate cleanup tools
7. Re-run to confirm, then proceed to meshing

### Key reminders
- This control **detects only** — it does not repair
- Verify Thin Stripes Width unit is `in`, not `mm`
- Consider **parametrizing** your custom values if you'll reuse this configuration

Good luck with your meshing — let me know if anything comes up when you run it!

---

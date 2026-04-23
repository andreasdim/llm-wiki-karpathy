query: how can I ensure, that direct morphing preserves symetry settings?                                                                                                
                                                                            
  Searched for 1 pattern, read 1 file (ctrl+o to expand)                                                                                                                   
                                                                                                                                                                         
⏺ Let me read the relevant pages.                                                                                                                                          
                              
  Read 5 files (ctrl+o to expand)                                                                                                                                          
                                                                                                                                                                           
⏺ Let me search the raw sources for symmetry-related information.                                                                                                          
                                                                                                                                                                           
  Searched for 1 pattern (ctrl+o to expand)                                                                                                                                
                                                                                                                                                                           
⏺ The wiki currently has no information about symmetry settings in the context of direct morphing. The only mentions of "symmetry" in the entire knowledge base relate to  
  axisymmetric body decomposition in MultiZone volume meshing — which is unrelated.                                                                                        
                                                                                                                                                                           
  Based on what the wiki documents about Direct Morphing:                                                                                                                  
                                                                                                                                                                           
  The wiki does not cover a symmetry preservation mechanism for morphing operations. The morphing controls documented are:                                                 
  - Scope controls: Control Scope, Fixed Scope, Rigid Scope, Morphable Scope ([[morphing]])
  - Advanced Scope: Rings/Distance-based morphable region, Free Edges as Fixed ([[advanced-scope]])                                                                        
  - Advanced Solver: Fast/Smooth/Linear solver, Biasing Type, Preserve Boundary Layers ([[advanced-solver]])
                                                                                                                                                                           
  None of these pages mention symmetry.                                                                                                                                    
                                                                                                                                                                           
  Possible approaches based on what is documented:                                                                                                                         
                  
  1. Fixed Scope — You could scope symmetric counterpart faces as "Fixed" so they don't deform during the morph. Then apply matching morph operations to both symmetric    
  halves separately.
  2. Free Edges as Fixed (Advanced Scope) — Freezing free edges can prevent boundary distortion, but this isn't symmetry-specific.                                         
  3. Morph Recording — Record the morph to an .mrd file ([[morph-recording]]), then apply the mirrored transformation to the symmetric side. This is the closest mechanism 
  to ensuring consistent symmetric modifications.                                                                                                                          
                                                                                                                                                                           
  However, I'm uncertain whether the product has a dedicated symmetry constraint for morphing that simply hasn't been ingested yet, or whether symmetry preservation must  
  be handled manually through the approaches above.
                                                                                                                                                                           
  Do you have a raw source covering symmetry settings in morphing that I should ingest? That would let me give a definitive answer and update the wiki. Otherwise, should I
   file what I've synthesized here as an analysis page?
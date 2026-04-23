query: how can I ensure, that direct morphing preserves symetry settings?                                                                                                
                                                                             
  Read 1 file (ctrl+o to expand)                                                                                                                                           
                                                                                                                                                                         
⏺ The relevant pages are: symmetry-definition, morphing, direct-morphing, direct-morph, and the source pages new and new2. Let me read them.                               
                           
  Read 4 files (ctrl+o to expand)                                                                                                                                          
                                                                                                                                                                           
⏺ How to preserve symmetry settings during Direct Morphing                                                                                                                 
                                                                                                                                                                           
  To ensure Direct Morphing preserves symmetry, you need to add a Symmetry Definition control to the Direct Morph step. Here's the process:                                
                                                                                                                                                                           
  1. Prepare matching scopes                                                                                                                                               
                                                                                                                                                                           
  Before morphing, ensure you have defined scopes for the symmetric boundary faces. These can be Labels (Named Selections), Zones, or a mix:                               
                                                                                                                                                                         
  - Side A — the source periodic/symmetric face                                                                                                                            
  - Side B — the target face (must have a matching node pattern with Side A)                                                                                             
  - Axis (periodic only) — the axis of revolution                                                                                                                          
  - Symmetry Plane (planar only) — the mirror plane                                                                                                                        
                                                                                                                                                                           
  Critical: The paired faces must already have matching node patterns (e.g., from a cyclic mesh or match control). The symmetry definition preserves node pairing — it does
   not create it.                                                                                                                                                        
                                                                                                                                                                           
  2. Insert the Symmetry Definition                                                                                                                                      

  Right-click the Direct Morphing step → Insert → Symmetry Definition. Then configure:                                                                                     
   
  ┌─────────────────────┬────────────────────┬────────────────────┐                                                                                                        
  │      Property       │      Periodic      │       Planar       │
  ├─────────────────────┼────────────────────┼────────────────────┤                                                                                                        
  │ Type                │ Periodic           │ Planar             │
  ├─────────────────────┼────────────────────┼────────────────────┤
  │ Side A / Side B     │ paired face scopes │ paired face scopes │
  ├─────────────────────┼────────────────────┼────────────────────┤                                                                                                        
  │ Axis + Sector Angle │ required           │ —                  │
  ├─────────────────────┼────────────────────┼────────────────────┤                                                                                                        
  │ Symmetry Plane      │ —                  │ required           │
  └─────────────────────┴────────────────────┴────────────────────┘                                                                                                        
                  
  3. How it works

  - Periodic: any displacement on a Side A node is reproduced on its paired Side B node after rotation through the sector angle. Node pairing is maintained.               
  - Planar: normal-to-plane displacements are mirrored; in-plane components are duplicated on the paired node.
  - Interior nodes are smoothed consistently with the boundary constraints to preserve element quality.                                                                    
                                                                                                                                                                           
  You can add multiple symmetry definitions to one morph step (e.g., one periodic + one planar for a cyclic sector with a hub mid-plane).                                  
                                                                                                                                                                           
  4. Validate after morphing                                                                                                                                               
                  
  1. Check paired node distance after rotation — should be within ~1e-6 of model characteristic length                                                                     
  2. Inspect element quality (skewness, orthogonal quality) near periodic faces
  3. Visually copy the sector rotationally — the seam should be invisible                                                                                                  
  4. Confirm the solver accepts the periodic/cyclic BC without mismatch warnings
                                                                                                                                                                           
  Common pitfalls 
                                                                                                                                                                           
  - Non-matching Side A / Side B meshes → create a cyclic match control before morphing                                                                                    
  - Wrong axis or sector angle → silently produces asymmetric results
  - Forgetting to update Named Selections after a CAD change                                                                                                               
                  
  Sources: [[symmetry-definition]], [[morphing]], [[direct-morph]], [[direct-morphing]]                                                                                    
                  
  ---                                                                                                                                                                      
  Should I file this answer as a wiki page in wiki/analyses/?
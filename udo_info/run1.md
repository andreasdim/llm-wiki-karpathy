query: how can I ensure, that direct morphing preserves symetry settings?                                                                                                
                                                                                 
  Read 5 files (ctrl+o to expand)                                                                                                                                          
                                                                                                                                                                         
⏺ Here's how to ensure Direct Morphing preserves symmetry settings:                                                                                                        
                           
  Add a Symmetry Definition control to the Direct Morph step                                                                                                               
                                                                                                                                                                           
  Right-click the Direct Morphing step → Insert → Symmetry Definition. Two types are available:                                                                            
                                                                                                                                                                           
  ┌──────────┬────────────────────────────────────────────────────┬───────────────────────────────────────────────────┐                                                    
  │   Type   │                      Use case                      │                  Key properties                   │                                                  
  ├──────────┼────────────────────────────────────────────────────┼───────────────────────────────────────────────────┤
  │ Periodic │ Cyclic/rotational symmetry (e.g., turbine sectors) │ Axis of revolution, Sector Angle, Side A / Side B │
  ├──────────┼────────────────────────────────────────────────────┼───────────────────────────────────────────────────┤
  │ Planar   │ Mirror symmetry                                    │ Symmetry Plane, Side A / Side B                   │                                                    
  └──────────┴────────────────────────────────────────────────────┴───────────────────────────────────────────────────┘                                                    
                                                                                                                                                                           
  Prerequisites                                                                                                                                                            
                                                                                                                                                                         
  Before adding the control, you need these Named Selections in place:                                                                                                     
   
  - sym_side_A — source symmetric face                                                                                                                                     
  - sym_side_B — target symmetric face (must have a matching node pattern with Side A)                                                                                   
  - sym_axis (periodic only) — axis of revolution                                                                                                                          
  - sym_plane (planar only) — mirror plane                                                                                                                               
                                                                                                                                                                           
  Critical: The paired faces must already have matching nodes (e.g., from a cyclic mesh or match control). The Symmetry Definition preserves node pairing — it does not    
  create it.                                                                                                                                                               
                                                                                                                                                                           
  How it works                                                                                                                                                           

  - Periodic: any displacement on a Side A node is reproduced on its paired Side B node after rotation through the sector angle. Interior nodes are smoothed consistently. 
  - Planar: normal-to-plane displacements are mirrored; in-plane components are duplicated on the paired node.
                                                                                                                                                                           
  Validation after morphing                                                                                                                                                
                                                                                                                                                                           
  1. Check paired node distance after rotation (should be ~1e-6 tolerance)                                                                                                 
  2. Inspect element quality near periodic faces (skewness, orthogonal quality)                                                                                          
  3. Visually copy the sector rotationally — the seam should be invisible                                                                                                  
  4. Confirm the solver accepts the periodic/cyclic BC without mismatch warnings                                                                                           
                                                                                                                                                                           
  Common pitfalls                                                                                                                                                          
                                                                                                                                                                           
  - Non-matching meshes on Side A / Side B — create a cyclic match control before morphing                                                                                 
  - Wrong axis or sector angle — silently produces asymmetric results
  - Stale Named Selections after CAD changes — labels may scope different geometry silently                                                                                
                                                                                                                                                                           
  You can also stack multiple Symmetry Definitions on one step (e.g., periodic + planar for a hub mid-plane).                                                              
                                                                                                                                                                           
  Sources: [[symmetry-definition]], [[morphing]], [[direct-morph]], [[direct-morphing]]                                                                                    
                                                                                                                                                                         
  ---                                                                                                                                                                      
  Should I file this answer as a wiki analysis page?
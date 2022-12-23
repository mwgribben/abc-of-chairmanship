---
mermaid: true
---
## Procedure on a motion which is put to the vote

<div class="mermaid">

graph TB

    A[Motion Moved & Seconded] --> B[No Amendment Proposed]
    
    B --Vote--> C[Carried] & D[Defeated]
    
    C --> E[Resolution]
    
    A --> F[Amendment Proposed and Seconded]
    
    F --Vote--> G[Amendment Carried] & H[Amendment Lost]
    
    G --> I[No further amendment]
    
    I --Vote--> C & D
    
    G --> J[Amended Motion]
    
    J --> K[Further Amendment]
    
    K --Vote--> L[Lost] & M[Carried] --> I
    
    H --> N[Original Motion] & O[Original Motion]
    
    N --> I
    
    O --> K

</div>

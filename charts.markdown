---
chapter_num : Appendix B
mermaid: true
last_modified_at: 2023-01-02
canonical_url: 'https://chair.guide/charts'
---

# Flow charts of Procedure

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

## Procedure on a motion in any event
<div class="mermaid">
graph LR
A[Motion] --> B[No Amendment proposed] & C[Amendment proposed]

B --Vote--> D([Carried]) & E([Defeated])

B --No Vote--> F([Withdrawn, Adjourned, Next Business Moved, Previous Question])

C --Vote--> J[Amendment lost] & K[Amendment carried]

J --> L[Original Motion]

L --No Vote--> F

L --Vote--> D & E

L --> M[Further Amendment]

M --> C

K --> N[Amended Motion]

N --Vote--> O([Carried]) & P([Defeated])

N --No Vote--> Q([Withdrawn, Adjourned, Next Business Moved, Previous Question])

D & O --> R([Resolution])
</div>

## Simplified flowchart (editor's addition)

<div class="mermaid">
graph TB
A[/Original Motion/] --> B[Moved and seconded]

B --> C{Amendments moved and seconded?}

C --No--> D{Put to the vote?}

D --Yes--> E{Result}

E --Carried--> F[/Resolution/]

E --Lost--> G([Defeated])

D --No--> H([Withdrawn/Adjourned/Next Business Moved/Previous Question])

C --Yes--> I{Vote on Amendment}

I --Carried--> J[/Amended Motion/]

I --Lost--> K[/Original Motion/]

J & K --> L{Further Amendment?}

L --Yes--> I

L --No--> D
</div>

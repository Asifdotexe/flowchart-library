---
config:
  theme: redux-color
---
%% Merge conflict
graph TD
    Start[File: fit_regression.py] --> Main(main)
    Start --> Feat(update-params)
    
    Main -->|Line 10: import pandas as pd| Merge{GIT MERGE}
    Feat -->|Line 10: import pandas as np| Merge
    
    Merge -->|Git gets confused!| Output["<<<<<<< HEAD (main)<br>import pandas as pd<br>=======<br>import pandas as np<br>>>>>>>> update-params"]
    
    style Merge fill:#ffcccc,stroke:#ff0000,stroke-width:2px

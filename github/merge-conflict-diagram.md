---
config:
  theme: redux-color
  layout: dagre
---
flowchart LR
    Start["File: fit_regression.py"] --> Main("main") & Feat("update-params")
    Main -- Line 10: import pandas as pd --> Merge{"GIT MERGE"}
    Feat -- Line 10: import pandas as np --> Merge
    Merge -- Git gets confused! --> Output["&lt;&lt;&lt;&lt;&lt;&lt;&lt; HEAD (main)<br>import pandas as pd<br>=======<br>import pandas as np<br>&gt;&gt;&gt;&gt;&gt;&gt;&gt; update-params"]

    style Merge fill:#ffcccc,stroke:#ff0000,stroke-width:2px

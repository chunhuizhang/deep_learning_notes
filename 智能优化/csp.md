
```python

from ortools.sat.python import cp_model

model = cp_model.CpModel()

model.add...
model.Maximize()

solver = cp_model.CpSolver()
solver.parameters.log_search_progress = True

status = solver.Solve(model)


```

## 1. constraints


- allDifferent
- addCircuit
    - 汉密尔顿环，所有的点，走且仅走一次；

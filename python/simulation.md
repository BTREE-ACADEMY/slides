---
title: "Simulation"
date: "2021-03-03"
post_type: "lecture"
---

# Simulation, not calculation

Computers are so fast that it's often feasible to simulate a difficult task without knowing the mathematics behind it. For example, the sum of the series 1 + 2 + 3 + ... 100 is simply (100) * (101) / 2 = 5050. However, the following loop can also do the trick

```python
s = 0
for i in range(1, 101):
  s += i
```
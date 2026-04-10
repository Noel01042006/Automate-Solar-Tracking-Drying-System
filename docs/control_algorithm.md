# Control Algorithm

1. Read LDR left value
2. Read LDR right value
3. Calculate difference
4. Compare with threshold
5. Rotate motor accordingly
6. Stop when balanced

Pseudo Code:

if abs(left-right) < threshold
    stop
else if left > right
    rotate left
else
    rotate right

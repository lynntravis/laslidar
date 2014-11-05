las.py
======

python functions for reading lidar point clouds from .las files

returns a list containing all points as dictionarys each having the keys:
  * x
  * y
  * z
  * intensity
  * classification
  * returnnum
  * numreturns

basic usage:
```
points = read_las(filename)
```

"optimized" mode returns only x, y, and z values in a tuple to save memory:
```
mode="normal"
mode="optimized"
```

option to center points around 0 and scale to ~ -1 - 1 range:
```
center="False"
center="True"
```

Maybe I'll make a version that is object based and uses generators, someday.

# GeometryPy

**GeometryPy** is a math library for compute analytic geometry problem. 

In 2D or 3D analytic geometry , this library isn't needing another third-party library such as Sympy or Numpy.

However, if you need to solve N-dimensional analytic geometry, you must use matrix. 
Therefore, **GeometryPy** will import other libraries (such as Numpy) to solve the matrix problem.

# Simple Example

In the plane, judge that two lines are vertical to each other:

```
from geometrypy.geometry2d.line2d import Line2d

# x + 2y + 3 = 0 
line1 = Line2d(1, 2, 3)

# 3x + 4y + 5 = 0
line2 = Line2d(3, 4, 5)

line1.vertical(line2) # result is False
```

line1 and line2 intersect:

```
line1.intersect(line2) # result is Point(1.0, -2.0)
```
# cookie-learning

Here collected different chips in different languages. Why am I doing this? Fuck I these geese, that would be remembered formula, algorithms and everything else. If to whom it is useful I will be very happy :D With love sedrew

### Lemniscate of Bernoulli
```C
scale = 2 / (3 - cos(2*t));
x = scale * cos(t);
y = scale * sin(2*t) / 2;
```
In Blender 2.8 with primative cube

```py
import bpy
import math

z = 0
size = (0.2,0.2,0.2)

for t in range(100):
    scale = 20 / (3- math.cos(2*t))
    x = scale * math.cos(t);
    y = scale * math.sin(2*t) / 2
    z += 0.01
    bpy.ops.mesh.primitive_cube_add(enter_editmode=False, location=(x, y, 1))
    bpy.ops.transform.resize(value=(size))
```

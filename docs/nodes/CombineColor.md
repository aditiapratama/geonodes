
# Node CombineColor

> Geometry node name: [Combine Color](https://docs.blender.org/manual/en/latest/modeling/geometry_nodes/color/combine_color.html)<br>
  Blender type: [Combine Color](https://docs.blender.org/api/current/bpy.types.FunctionNodeCombineColor.html)
  
<sub>go to [index](/docs/index.md)</sub>

## Initialization

```python
from geonodes import nodes
node = nodes.CombineColor(red=None, green=None, blue=None, alpha=None, mode='RGB', label=None, node_color=None)
```



## Arguments


### Input sockets

- red : Float
- green : Float
- blue : Float
- alpha : Float

### Parameters

- mode : str (default = 'RGB') in ('RGB', 'HSV', 'HSL')

### Node label

- label : Geometry node display label (default=None)
- node_color : Geometry node color (default=None)

## Output sockets

- color : Color

## Data sockets

> Data socket classes implementing this node.
  
  
- [Color](/docs/sockets/Color.md).[Combine](/docs/sockets/Color.md#combine) : Constructor
- [Color](/docs/sockets/Color.md).[CombineHSL](/docs/sockets/Color.md#combinehsl) : Constructor
- [Color](/docs/sockets/Color.md).[CombineHSV](/docs/sockets/Color.md#combinehsv) : Constructor
- [Color](/docs/sockets/Color.md).[CombineRGB](/docs/sockets/Color.md#combinergb) : Constructor
  

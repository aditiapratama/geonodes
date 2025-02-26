
# Data socket Color

> Inherits from dsock.Color
  
<sub>go to [index](/docs/index.md)</sub>



## Constructors

- [Combine](#combine) : color (Color)
- [CombineHSL](#combinehsl) : color (Color)
- [CombineHSV](#combinehsv) : color (Color)
- [CombineRGB](#combinergb) : color (Color)

## Methods

- [add](#add) : color (Color)
- [brighter](#brighter) : result (Boolean)
- [burn](#burn) : color (Color)
- [capture_attribute](#capture_attribute) : Sockets      [geometry (Geometry), attribute (Color)]
- [curves](#curves) : color (Color)
- [darken](#darken) : color (Color)
- [darker](#darker) : result (Boolean)
- [difference](#difference) : color (Color)
- [divide](#divide) : color (Color)
- [dodge](#dodge) : color (Color)
- [equal](#equal) : result (Boolean)
- [field_at_index](#field_at_index) : value (Color)
- [lighten](#lighten) : color (Color)
- [linear_light](#linear_light) : color (Color)
- [mix](#mix) : color (Color)
- [mix](#mix) : color (Color)
- [mix_color](#mix_color) : color (Color)
- [mix_hue](#mix_hue) : color (Color)
- [mix_saturation](#mix_saturation) : color (Color)
- [mix_value](#mix_value) : color (Color)
- [multiply](#multiply) : color (Color)
- [not_equal](#not_equal) : result (Boolean)
- [overlay](#overlay) : color (Color)
- [raycast](#raycast) : Sockets      [is_hit (Boolean), hit_position (Vector), hit_normal (Vector), hit_distance (Float), attribute (Color)]
- [screen](#screen) : color (Color)
- [separate_color](#separate_color) : Sockets      [red (Float), green (Float), blue (Float), alpha (Float)]
- [soft_light](#soft_light) : color (Color)
- [subtract](#subtract) : color (Color)
- [switch](#switch) : output (Color)

## Combine

Geometry node [*Combine Color*].


  Args:
    red: Float
    green: Float
    blue: Float
    alpha: Float
    mode (str): 'RGB' in [RGB, HSV, HSL]
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.CombineColor`
  
  
  .. blid:: FunctionNodeCombineColor
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.CombineColor(red=red, green=green, blue=blue, alpha=alpha, mode=mode, label=node_label, node_color=node_color)
    

## CombineRGB

Geometry node [*Combine Color*].


  Args:
    red: Float
    green: Float
    blue: Float
    alpha: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.CombineColor`
  
  - mode = 'RGB'
    
  .. blid:: FunctionNodeCombineColor
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.CombineColor(red=red, green=green, blue=blue, alpha=alpha, mode='RGB', label=node_label, node_color=node_color)
    

## CombineHSV

Geometry node [*Combine Color*].


  Args:
    red: Float
    green: Float
    blue: Float
    alpha: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.CombineColor`
  
  - mode = 'HSV'
    
  .. blid:: FunctionNodeCombineColor
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.CombineColor(red=hue, green=saturation, blue=value, alpha=alpha, mode='HSV', label=node_label, node_color=node_color)
    

## CombineHSL

Geometry node [*Combine Color*].


  Args:
    red: Float
    green: Float
    blue: Float
    alpha: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.CombineColor`
  
  - mode = 'HSL'
    
  .. blid:: FunctionNodeCombineColor
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.CombineColor(red=hue, green=saturation, blue=lightness, alpha=alpha, mode='HSL', label=node_label, node_color=node_color)
    

## capture_attribute

Geometry node [*Capture Attribute*].


  Args:
    geometry: Geometry
    domain (str): 'POINT' in [POINT, EDGE, FACE, CORNER, CURVE, INSTANCE]
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Sockets [geometry (Geometry), attribute (Color)]
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.CaptureAttribute`
  
  - data_type = 'FLOAT_COLOR'
    
  .. blid:: GeometryNodeCaptureAttribute
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.CaptureAttribute(value=self, geometry=geometry, data_type='FLOAT_COLOR', domain=domain, label=node_label, node_color=node_color)
    

## field_at_index

Geometry node [*Field at Index*].


  Args:
    index: Integer
    domain (str): 'POINT' in [POINT, EDGE, FACE, CORNER, CURVE, INSTANCE]
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.FieldAtIndex`
  
  - data_type = 'FLOAT_COLOR'
    
  .. blid:: GeometryNodeFieldAtIndex
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.FieldAtIndex(value=self, index=index, data_type='FLOAT_COLOR', domain=domain, label=node_label, node_color=node_color)
    

## raycast

Geometry node [*Raycast*].


  Args:
    target_geometry: Geometry
    source_position: Vector
    ray_direction: Vector
    ray_length: Float
    mapping (str): 'INTERPOLATED' in [INTERPOLATED, NEAREST]
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Sockets [is_hit (Boolean), hit_position (Vector), hit_normal (Vector), hit_distance (Float), attribute (Color)]
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Raycast`
  
  - data_type = 'FLOAT_COLOR'
    
  .. blid:: GeometryNodeRaycast
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Raycast(attribute=self, target_geometry=target_geometry, source_position=source_position, ray_direction=ray_direction, ray_length=ray_length, data_type='FLOAT_COLOR', mapping=mapping, label=node_label, node_color=node_color)
    

## switch

Geometry node [*Switch*].


  Args:
    switch: Boolean
    true: Color
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Switch`
  
  - input_type = 'RGBA'
    
  .. blid:: GeometryNodeSwitch
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Switch(false=self, switch=switch, true=true, input_type='RGBA', label=node_label, node_color=node_color)
    

## equal

Geometry node [*Compare*].


  Args:
    b: Color
    epsilon: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Boolean
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Compare`
  
  - data_type = 'RGBA'
  - mode = 'ELEMENT'
  - operation = 'EQUAL'
    
  .. blid:: FunctionNodeCompare
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Compare(a=self, b=b, epsilon=epsilon, data_type='RGBA', mode='ELEMENT', operation='EQUAL', label=node_label, node_color=node_color)
    

## not_equal

Geometry node [*Compare*].


  Args:
    b: Color
    epsilon: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Boolean
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Compare`
  
  - data_type = 'RGBA'
  - mode = 'ELEMENT'
  - operation = 'NOT_EQUAL'
    
  .. blid:: FunctionNodeCompare
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Compare(a=self, b=b, epsilon=epsilon, data_type='RGBA', mode='ELEMENT', operation='NOT_EQUAL', label=node_label, node_color=node_color)
    

## brighter

Geometry node [*Compare*].


  Args:
    b: Color
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Boolean
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Compare`
  
  - data_type = 'RGBA'
  - mode = 'ELEMENT'
  - operation = 'BRIGHTER'
    
  .. blid:: FunctionNodeCompare
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Compare(a=self, b=b, data_type='RGBA', mode='ELEMENT', operation='BRIGHTER', label=node_label, node_color=node_color)
    

## darker

Geometry node [*Compare*].


  Args:
    b: Color
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Boolean
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Compare`
  
  - data_type = 'RGBA'
  - mode = 'ELEMENT'
  - operation = 'DARKER'
    
  .. blid:: FunctionNodeCompare
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Compare(a=self, b=b, data_type='RGBA', mode='ELEMENT', operation='DARKER', label=node_label, node_color=node_color)
    

## mix

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'MIX'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='MIX', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## darken

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'DARKEN'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='DARKEN', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## multiply

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'MULTIPLY'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='MULTIPLY', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## burn

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'BURN'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='BURN', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## lighten

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'LIGHTEN'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='LIGHTEN', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## screen

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'SCREEN'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='SCREEN', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## dodge

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'DODGE'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='DODGE', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## add

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'ADD'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='ADD', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## overlay

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'OVERLAY'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='OVERLAY', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## soft_light

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'SOFT_LIGHT'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='SOFT_LIGHT', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## linear_light

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'LINEAR_LIGHT'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='LINEAR_LIGHT', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## difference

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'DIFFERENCE'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='DIFFERENCE', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## subtract

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'SUBTRACT'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='SUBTRACT', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## divide

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'DIVIDE'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='DIVIDE', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## mix_hue

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'HUE'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='HUE', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## mix_saturation

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'SATURATION'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='SATURATION', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## mix_color

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'COLOR'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='COLOR', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## mix_value

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  - blend_type = 'VALUE'
    
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type='VALUE', use_alpha=use_alpha, label=node_label, node_color=node_color)
    

## separate_color

Geometry node [*Separate Color*].


  Args:
    mode (str): 'RGB' in [RGB, HSV, HSL]
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Sockets [red (Float), green (Float), blue (Float), alpha (Float)]
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.SeparateColor`
  
  
  .. blid:: FunctionNodeSeparateColor
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.SeparateColor(color=self, mode=mode, label=node_label, node_color=node_color)
    

## curves

Geometry node [*RGB Curves*].


  Args:
    fac: Float
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.RgbCurves`
  
  
  .. blid:: ShaderNodeRGBCurve
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.RgbCurves(color=self, fac=fac, label=node_label, node_color=node_color)
    

## mix

Geometry node [*Mix*].


  Args:
    color2: Color
    fac: Float
    blend_type (str): 'MIX' in [MIX, DARKEN, MULTIPLY, BURN, LIGHTEN,... , SATURATION, COLOR, VALUE]
    use_alpha (bool): False
    node_label (str): Node label
    node_color (color): Node background color
    
  Returns:
    Color
    
  **Node creation**
  
  Node :class:`~geonodes.nodes.nodes.Mix`
  
  
  .. blid:: ShaderNodeMixRGB
  
  .. code-block:: python
  
    from geonodes import nodes
    nodes.Mix(color1=self, color2=color2, fac=fac, blend_type=blend_type, use_alpha=use_alpha, label=node_label, node_color=node_color)
    

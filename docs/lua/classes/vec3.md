# Class: vec3

Class representing a 3D vector.
<!-- 这是一个表示三维向量的类，用于在3D空间中表示位置、方向或运动。 -->

## Fields (3)

### `x`

x component of the vector.
<!-- x轴分量，表示向量在x轴上的投影值 -->

- Type: `float`

### `y`

y component of the vector.
<!-- y轴分量，表示向量在y轴上的投影值 -->

- Type: `float`

### `z`

z component of the vector.
<!-- z轴分量，表示向量在z轴上的投影值 -->

- Type: `float`

## Constructors (1)

### `new(x, y, z)`

Returns: vec3: a vector that contains the x, y, and z values.
<!-- 返回一个包含x、y、z值的新向量实例 -->

- **Parameters:**
  - `x` (float): x component of the vector.
  <!-- x参数：向量的x轴分量，浮点数类型 -->
  - `y` (float): y component of the vector.
  <!-- y参数：向量的y轴分量，浮点数类型 -->
  - `z` (float): z component of the vector.
  <!-- z参数：向量的z轴分量，浮点数类型 -->

**Example Usage:**
<!-- 使用示例：创建一个新的三维向量实例 -->
```lua
myInstance = vec3:new(x, y, z)
```


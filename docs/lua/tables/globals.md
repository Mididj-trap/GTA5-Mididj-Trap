# Table: globals

Table containing functions for manipulating gta script globals.
<!-- 该表包含用于操作GTA脚本全局变量的函数。 -->

## Functions (11)

### `get_int(global)`

Retrieves an int global value.
<!-- 获取一个整数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `integer`: value of the global
  <!-- 返回整数类型的全局变量值 -->

**Example Usage:**
```lua
integer = globals.get_int(global)
```

### `get_uint(global)`

Retrieves an uint global value.
<!-- 获取一个无符号整数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `integer`: value of the global
  <!-- 返回无符号整数类型的全局变量值 -->

**Example Usage:**
```lua
integer = globals.get_uint(global)
```

### `get_float(global)`

Retrieves a float global value.
<!-- 获取一个浮点数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `float`: value of the global
  <!-- 返回浮点数类型的全局变量值 -->

**Example Usage:**
```lua
float = globals.get_float(global)
```

### `get_string(global)`

Retrieves a string global value.
<!-- 获取一个字符串类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `string`: value of the global
  <!-- 返回字符串类型的全局变量值 -->

**Example Usage:**
```lua
string = globals.get_string(global)
```

### `get_vec3(global)`

Retrieves a Vector3 global value.
<!-- 获取一个三维向量类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `Vector3`: value of the global
  <!-- 返回三维向量类型的全局变量值 -->

**Example Usage:**
```lua
Vector3 = globals.get_vec3(global)
```

### `set_int(global, val)`

Sets an int global value.
<!-- 设置一个整数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->
  - `val` (integer): new value for the global
  <!-- val参数为整数类型，表示要设置的新值 -->

**Example Usage:**
```lua
globals.set_int(global, val)
```

### `set_uint(global, val)`

Sets an uint global value.
<!-- 设置一个无符号整数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->
  - `val` (integer): new value for the global
  <!-- val参数为无符号整数类型，表示要设置的新值 -->

**Example Usage:**
```lua
globals.set_uint(global, val)
```

### `set_float(global, val)`

Sets a float global value.
<!-- 设置一个浮点数类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->
  - `val` (float): new value for the global
  <!-- val参数为浮点数类型，表示要设置的新值 -->

**Example Usage:**
```lua
globals.set_float(global, val)
```

### `set_string(global, str)`

Sets a string global value.
<!-- 设置一个字符串类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->
  - `str` (string): new value for the global
  <!-- str参数为字符串类型，表示要设置的新值 -->

**Example Usage:**
```lua
globals.set_string(global, str)
```

### `set_vec3(global, param)`

Sets a Vector3 global value.
<!-- 设置一个三维向量类型的全局变量值。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->
  - `param` (Vector3): new value for the global
  <!-- param参数为三维向量类型，表示要设置的新值 -->

**Example Usage:**
```lua
globals.set_vec3(global, param)
```

### `get_pointer(global)`

Retrieves a pointer global.
<!-- 获取一个指针类型的全局变量。 -->

- **Parameters:**
  - `global` (integer): index of the global
  <!-- global参数为整数类型，表示全局变量的索引 -->

- **Returns:**
  - `pointer`: value of the global
  <!-- 返回指针类型的全局变量值 -->

**Example Usage:**
```lua
pointer = globals.get_pointer(global)
```



# Table: locals

Table for manipulating GTA scripts locals.
用于操作GTA脚本局部变量的表。

## Functions (9)

### `get_int(script, index)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引

- **Returns:**
  - `integer`: The value of the given local. | 返回指定局部变量的整数值

**Example Usage:**
```lua
integer = locals.get_int(script, index)
```

### `get_uint(script, index)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引

- **Returns:**
  - `unsigned integer`: The value of the given local. | 返回指定局部变量的无符号整数值

**Example Usage:**
```lua
unsigned integer = locals.get_uint(script, index)
```

### `get_float(script, index)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引

- **Returns:**
  - `float`: The value of the given local. | 返回指定局部变量的浮点数值

**Example Usage:**
```lua
float = locals.get_float(script, index)
```

### `get_vec3(script, index)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引

- **Returns:**
  - `Vector3`: The value of the given local. | 返回指定局部变量的三维向量值

**Example Usage:**
```lua
Vector3 = locals.get_vec3(script, index)
```

### `set_int(script, index, val)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引
  - `val` (integer): The new value of the given local. | 要设置的新整数值

**Example Usage:**
```lua
locals.set_int(script, index, val)
```

### `set_uint(script, index, val)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引
  - `val` (unsigned integer): The new value of the given local. | 要设置的新无符号整数值

**Example Usage:**
```lua
locals.set_uint(script, index, val)
```

### `set_float(script, index, val)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引
  - `val` (float): The new value of the given local. | 要设置的新浮点数值

**Example Usage:**
```lua
locals.set_float(script, index, val)
```

### `set_vec3(script, index, val)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引
  - `val` (Vector3): The new value of the given local. | 要设置的新三维向量值

**Example Usage:**
```lua
locals.set_vec3(script, index, val)
```

### `get_pointer(script, index)`

- **Parameters:**
  - `script` (string): The name of the script | 脚本的名称
  - `index` (index): Index of the script local. | 脚本局部变量的索引

- **Returns:**
  - `pointer`: The pointer to the given local. | 返回指定局部变量的指针

**Example Usage:**
```lua
pointer = locals.get_pointer(script, index)
```



# Table: tunables

Table for manipulating gta tunables.
可调节参数表，用于操作GTA中的可调节参数。

## Functions (12)

### `get_int(tunable_name)`

获取指定名称的整数类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。

- **Returns:**
  - `integer`: The value of the given tunable.
  - `integer`: 返回指定可调节参数的整数值。

**Example Usage:**
**使用示例：**
```lua
integer = tunables.get_int(tunable_name)
```

### `get_float(tunable_name)`

获取指定名称的浮点数类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。

- **Returns:**
  - `float`: The value of the given tunable.
  - `float`: 返回指定可调节参数的浮点数值。

**Example Usage:**
**使用示例：**
```lua
float = tunables.get_float(tunable_name)
```

### `get_bool(tunable_name)`

获取指定名称的布尔类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。

- **Returns:**
  - `boolean`: The value of the given tunable.
  - `boolean`: 返回指定可调节参数的布尔值。

**Example Usage:**
**使用示例：**
```lua
boolean = tunables.get_bool(tunable_name)
```

### `get_int(tunable_joaated_value)`

通过joaated值获取整数类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。

- **Returns:**
  - `integer`: The value of the given tunable.
  - `integer`: 返回指定可调节参数的整数值。

**Example Usage:**
**使用示例：**
```lua
integer = tunables.get_int(tunable_joaated_value)
```

### `get_float(tunable_joaated_value)`

通过joaated值获取浮点数类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。

- **Returns:**
  - `float`: The value of the given tunable.
  - `float`: 返回指定可调节参数的浮点数值。

**Example Usage:**
**使用示例：**
```lua
float = tunables.get_float(tunable_joaated_value)
```

### `get_bool(tunable_joaated_value)`

通过joaated值获取布尔类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。

- **Returns:**
  - `boolean`: The value of the given tunable.
  - `boolean`: 返回指定可调节参数的布尔值。

**Example Usage:**
**使用示例：**
```lua
boolean = tunables.get_bool(tunable_joaated_value)
```

### `set_int(tunable_name, val)`

设置指定名称的整数类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。
  - `val` (integer): The new value of the given tunable.
  - `val` (integer): 要设置的新整数值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_int(tunable_name, val)
```

### `set_float(tunable_name, val)`

设置指定名称的浮点数类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。
  - `val` (float): The new value of the given tunable.
  - `val` (float): 要设置的新浮点数值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_float(tunable_name, val)
```

### `set_bool(tunable_name, val)`

设置指定名称的布尔类型可调节参数值。

- **Parameters:**
  - `tunable_name` (string): The name of the tunable.
  - `tunable_name` (string): 可调节参数的名称。
  - `val` (boolean): The new value of the given tunable.
  - `val` (boolean): 要设置的新布尔值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_bool(tunable_name, val)
```

### `set_int(tunable_joaated_value, val)`

通过joaated值设置整数类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。
  - `val` (integer): The new value of the given tunable.
  - `val` (integer): 要设置的新整数值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_int(tunable_joaated_value, val)
```

### `set_float(tunable_joaated_value, val)`

通过joaated值设置浮点数类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。
  - `val` (float): The new value of the given tunable.
  - `val` (float): 要设置的新浮点数值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_float(tunable_joaated_value, val)
```

### `set_bool(tunable_joaated_value, val)`

通过joaated值设置布尔类型可调节参数值。

- **Parameters:**
  - `tunable_joaated_value` (integer): The joaated value of the tunable.
  - `tunable_joaated_value` (integer): 可调节参数的joaated值。
  - `val` (boolean): The new value of the given tunable.
  - `val` (boolean): 要设置的新布尔值。

**Example Usage:**
**使用示例：**
```lua
tunables.set_bool(tunable_joaated_value, val)
```



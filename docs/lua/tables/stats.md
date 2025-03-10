# Table: stats

Table for manipulating GTA stats.
为操作GTA统计数据提供的功能表。
For stats that get prefixed by either `MP0` or `MP1`, you can use `MPX` instead and the menu will resolve to the correct number automatically.
对于以`MP0`或`MP1`为前缀的统计数据，你可以使用`MPX`代替，菜单会自动解析为正确的数字。

## Functions (25)

### `get_character_index()`

获取当前多人游戏角色索引。

- **Returns:**
  - `integer`: The current multiplayer character index (0 or 1).
  - `integer`: 当前多人游戏角色的索引值（0或1）。

**Example Usage:**
**使用示例：**
```lua
integer = stats.get_character_index()
```

### `get_bool(stat_hash)`

通过统计数据哈希值获取布尔类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。

- **Returns:**
  - `boolean`: The value of the given stat.
  - `boolean`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.get_bool(stat_hash)
```

### `get_bool(stat_name)`

通过统计数据名称获取布尔类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。

- **Returns:**
  - `boolean`: The value of the given stat.
  - `boolean`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.get_bool(stat_name)
```

### `get_bool_masked(stat_hash, bit_index)`

通过统计数据哈希值获取指定位的布尔类型统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `bit_index` (integer): bit index.
  - `bit_index` (integer): 位索引。

- **Returns:**
  - `boolean`: The value of the given stat.
  - `boolean`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.get_bool_masked(stat_hash, bit_index)
```

### `get_bool_masked(stat_name, bit_index)`

通过统计数据名称获取指定位的布尔类型统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `bit_index` (integer): bit index.
  - `bit_index` (integer): 位索引。

- **Returns:**
  - `boolean`: The value of the given stat.
  - `boolean`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.get_bool_masked(stat_name, bit_index)
```

### `get_float(stat_hash)`

通过统计数据哈希值获取浮点类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。

- **Returns:**
  - `float`: The value of the given stat.
  - `float`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
float = stats.get_float(stat_hash)
```

### `get_float(stat_name)`

通过统计数据名称获取浮点类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。

- **Returns:**
  - `float`: The value of the given stat.
  - `float`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
float = stats.get_float(stat_name)
```

### `get_int(stat_hash)`

通过统计数据哈希值获取整数类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。

- **Returns:**
  - `integer`: The value of the given stat.
  - `integer`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
integer = stats.get_int(stat_hash)
```

### `get_int(stat_name)`

通过统计数据名称获取整数类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。

- **Returns:**
  - `integer`: The value of the given stat.
  - `integer`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
integer = stats.get_int(stat_name)
```

### `get_masked_int(stat_hash, bit_start, bit_size)`

通过统计数据哈希值获取指定位范围的整数类型统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `bit_start` (integer): bit start.
  - `bit_start` (integer): 起始位。
  - `bit_size` (integer): bit size.
  - `bit_size` (integer): 位长度。

- **Returns:**
  - `integer`: The value of the given stat.
  - `integer`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
integer = stats.get_masked_int(stat_hash, bit_start, bit_size)
```

### `get_masked_int(stat_name, bit_index, bit_size)`

通过统计数据名称获取指定位范围的整数类型统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `bit_index` (integer): bit index.
  - `bit_index` (integer): 位索引。
  - `bit_size` (integer): bit size.
  - `bit_size` (integer): 位长度。

- **Returns:**
  - `integer`: The value of the given stat.
  - `integer`: 指定统计数据的值。

**Example Usage:**
**使用示例：**
```lua
integer = stats.get_masked_int(stat_name, bit_index, bit_size)
```

### `set_bool(stat_hash, new_value)`

通过统计数据哈希值设置布尔类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `new_value` (boolean): the new value for the stat.
  - `new_value` (boolean): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_bool(stat_hash, new_value)
```

### `set_bool(stat_name, new_value)`

通过统计数据名称设置布尔类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `new_value` (boolean): the new value for the stat.
  - `new_value` (boolean): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_bool(stat_name, new_value)
```

### `set_bool_masked(stat_hash, new_value, bit_index)`

通过统计数据哈希值设置指定位的布尔类型统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `new_value` (boolean): the new value for the stat.
  - `new_value` (boolean): 要设置的新值。
  - `bit_index` (integer): bit_index.
  - `bit_index` (integer): 位索引。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_bool_masked(stat_hash, new_value, bit_index)
```

### `set_bool_masked(stat_name, new_value, bit_index)`

通过统计数据名称设置指定位的布尔类型统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `new_value` (boolean): the new value for the stat.
  - `new_value` (boolean): 要设置的新值。
  - `bit_index` (integer): bit_index.
  - `bit_index` (integer): 位索引。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_bool_masked(stat_name, new_value, bit_index)
```

### `set_float(stat_hash, new_value)`

通过统计数据哈希值设置浮点类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `new_value` (float): the new value for the stat.
  - `new_value` (float): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_float(stat_hash, new_value)
```

### `set_float(stat_name, new_value)`

通过统计数据名称设置浮点类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `new_value` (float): the new value for the stat.
  - `new_value` (float): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_float(stat_name, new_value)
```

### `set_int(stat_hash, new_value)`

通过统计数据哈希值设置整数类型的统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `new_value` (integer): the new value for the stat.
  - `new_value` (integer): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_int(stat_hash, new_value)
```

### `set_int(stat_name, new_value)`

通过统计数据名称设置整数类型的统计数据。

- **Parameters:**
  - `stat_name` (string): the stat name.
  - `stat_name` (string): 统计数据的名称。
  - `new_value` (integer): the new value for the stat.
  - `new_value` (integer): 要设置的新值。

- **Returns:**
  - `boolean`: True if succeeded.
  - `boolean`: 如果设置成功则返回true。

**Example Usage:**
**使用示例：**
```lua
boolean = stats.set_int(stat_name, new_value)
```

### `set_masked_int(stat_hash, new_value, bit_start, bit_size)`

通过统计数据哈希值设置指定位范围的整数类型统计数据。

- **Parameters:**
  - `stat_hash` (integer): the stat hash.
  - `stat_hash` (integer): 统计数据的哈希值。
  - `new_value` (integer): the new value for the stat.
  - `new_value` (integer):



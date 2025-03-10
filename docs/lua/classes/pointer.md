# Class: pointer

<!-- 这个类用于表示64位内存地址 -->
Class representing a 64-bit memory address.

## Constructors (1)

### `new(address)`

<!-- 创建一个新的内存实例，使用给定的地址 -->
Returns a memory instance, with the given address.

- **Parameters:**
  - `address` (integer): Address

**Example Usage:**
```lua
myInstance = pointer:new(address)
```

## Functions (26)

### `add(offset)`

<!-- 将给定的偏移量添加到当前内存地址，并返回一个新的指针对象 -->
Adds an offset to the current memory address and returns a new pointer object.

- **Parameters:**
  - `offset` (integer): offset

- **Returns:**
  - `pointer`: new pointer object.

**Example Usage:**
```lua
pointer = pointer:add(offset)
```

### `sub(offset)`

<!-- 从当前内存地址减去给定的偏移量，并返回一个新的指针对象 -->
Subs an offset to the current memory address and returns a new pointer object.

- **Parameters:**
  - `offset` (integer): offset

- **Returns:**
  - `pointer`: new pointer object.

**Example Usage:**
```lua
pointer = pointer:sub(offset)
```

### `rip(offset)`

<!-- 对当前内存地址进行RIP相对寻址，并返回一个新的指针对象 -->
Rips the current memory address and returns a new pointer object.

- **Parameters:**
  - `offset` (integer): offset

- **Returns:**
  - `pointer`: new pointer object.

**Example Usage:**
```lua
pointer = pointer:rip(offset)
```

### `get_byte()`

<!-- 从内存地址读取一个字节的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `number`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
number = pointer:get_byte()
```

### `get_word()`

<!-- 从内存地址读取一个字（2字节）的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `number`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
number = pointer:get_word()
```

### `get_int()`

<!-- 从内存地址读取一个整数（4字节）的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `number`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
number = pointer:get_int()
```

### `get_dword()`

<!-- 从内存地址读取一个双字（4字节）的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `number`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
number = pointer:get_dword()
```

### `get_float()`

<!-- 从内存地址读取一个浮点数的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `float`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
float = pointer:get_float()
```

### `get_qword()`

<!-- 从内存地址读取一个四字（8字节）的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `number`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
number = pointer:get_qword()
```

### `set_byte(value)`

<!-- 向内存地址写入一个字节的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (number): new value.

**Example Usage:**
```lua
pointer:set_byte(value)
```

### `set_word(value)`

<!-- 向内存地址写入一个字（2字节）的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (number): new value.

**Example Usage:**
```lua
pointer:set_word(value)
```

### `set_int(value)`

<!-- 向内存地址写入一个整数（4字节）的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (number): new value.

**Example Usage:**
```lua
pointer:set_int(value)
```

### `set_dword(value)`

<!-- 向内存地址写入一个双字（4字节）的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (number): new value.

**Example Usage:**
```lua
pointer:set_dword(value)
```

### `set_float(value)`

<!-- 向内存地址写入一个浮点数的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (float): new value.

**Example Usage:**
```lua
pointer:set_float(value)
```

### `set_qword(value)`

<!-- 向内存地址写入一个四字（8字节）的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (number): new value.

**Example Usage:**
```lua
pointer:set_qword(value)
```

### `get_string()`

<!-- 从内存地址读取一个字符串的值 -->
Retrieves the value stored at the memory address as the specified type.

- **Returns:**
  - `string`: the value stored at the memory address as the specified type.

**Example Usage:**
```lua
string = pointer:get_string()
```

### `set_string(value)`

<!-- 向内存地址写入一个字符串的值 -->
Sets the value at the memory address to the specified value of the given type.

- **Parameters:**
  - `value` (string): new value.

**Example Usage:**
```lua
pointer:set_string(value)
```

### `patch_byte(value)`

<!-- 创建一个内存补丁，用于修改内存地址中的字节值。
调用lua_patch对象的apply函数时应用修改的值，
调用restore函数时恢复原始值。 -->
Creates a memory patch for modifying the value at the memory address with the specified value.
The modified value is applied when you call the apply function on the lua_patch object.
The original value is restored when you call the restore function on the lua_patch object.

- **Parameters:**
  - `value` (number): new value.

- **Returns:**
  - `lua_patch`: memory patch instance for modifying the value at the memory address with the specified value. Can call apply / restore on the object.

**Example Usage:**
```lua
lua_patch = pointer:patch_byte(value)
```

### `patch_word(value)`

<!-- 创建一个内存补丁，用于修改内存地址中的字（2字节）值。
调用lua_patch对象的apply函数时应用修改的值，
调用restore函数时恢复原始值。 -->
Creates a memory patch for modifying the value at the memory address with the specified value.
The modified value is applied when you call the apply function on the lua_patch object.
The original value is restored when you call the restore function on the lua_patch object.

- **Parameters:**
  - `value` (number): new value.

- **Returns:**
  - `lua_patch`: memory patch instance for modifying the value at the memory address with the specified value. Can call apply / restore on the object.

**Example Usage:**
```lua
lua_patch = pointer:patch_word(value)
```

### `patch_dword(value)`

<!-- 创建一个内存补丁，用于修改内存地址中的双字（4字节）值。
调用lua_patch对象的apply函数时应用修改的值，
调用restore函数时恢复原始值。 -->
Creates a memory patch for modifying the value at the memory address with the specified value.
The modified value is applied when you call the apply function on the lua_patch object.
The original value is restored when you call the restore function on the lua_patch object.

- **Parameters:**
  - `value` (number): new value.

- **Returns:**
  - `lua_patch`: memory patch instance for modifying the value at the memory address with the specified value. Can call apply / restore on the object.

**Example Usage:**
```lua
lua_patch = pointer:patch_dword(value)
```

### `patch_qword(value)`

<!-- 创建一个内存补丁，用于修改内存地址中的四字（8字节）值。
调用lua_patch对象的apply函数时应用修改的值，
调用restore函数时恢复原始值。 -->
Creates a memory patch for modifying the value at the memory address with the specified value.
The modified value is applied when you call the apply function on the lua_patch object.
The original value is restored when you call the restore function on the lua_patch object.

- **Parameters:**
  - `value` (number): new value.

- **Returns:**
  - `lua_patch`: memory patch instance for modifying the value at the memory address with the specified value. Can call apply / restore on the object.

**Example Usage:**
```lua
lua_patch = pointer:patch_qword(value)
```

### `is_null()`

<!-- 检查当前内存地址是否为空（null） -->
- **Returns:**
  - `boolean`: Returns true if the address is null.

**Example Usage:**
```lua
boolean = pointer:is_null()
```

### `is_valid()`

<!-- 检查当前内存地址是否有效（非null） -->
- **Returns:**
  - `boolean`: Returns true if the address is not null.

**Example Usage:**
```lua
boolean = pointer:is_valid()
```

### `deref()`

<!-- 解引用当前内存地址，返回一个指向该地址存储的值的新指针对象 -->
Dereferences the memory address and returns a new pointer object pointing to the value at that address.

- **Returns:**
  - `pointer`: A new pointer object pointing to the value at that address.

**Example Usage:**
```lua
pointer = pointer:deref()
```

### `get_address()`

<!-- 获取指针对象中存储的内存地址值 -->
Retrieves the memory address stored in the pointer object.

- **Returns:**
  - `number`: The memory address stored in the pointer object as a number.

**Example Usage:**
```lua
number = pointer:get_address()
```

### `set_address(address)`

<!-- 设置指针对象中存储的内存地址值 -->
Sets the memory address stored in the pointer object.

- **Parameters:**
  - `address` (integer): new address.

**Example Usage:**
```lua
pointer:set_address(address)
```



# Table: scr_function

> 用于调用GTA脚本函数的表。需要在fiber池中调用。仅在必要时调用该函数。

Table for calling GTA script functions. Needs to be called in the fiber pool. Only call the function when necessary.

## Functions (2)

### `call_script_function(script_name, function_name, pattern, return_type_string, args_)`

> 通过模式扫描方式调用脚本函数。使用给定的参数调用脚本函数，并按指定类型返回返回值。

Calls a script function with the given arguments. Returns the return value as the given type.
**Example Usage:**
```lua
local value = scr_function.call_script_function("freemode", "wear_sunglasses_at_night", "69 42 06 66", "bool", {
   { "int", 69 },
   { "float", 4.20 },
   { "int", 666 }
})
```

- **Parameters:**
  > **参数说明：**
  > - `script_name` (string): 脚本名称
  > - `function_name` (string): 函数名称，此参数需要是唯一的
  > - `pattern` (string): 在脚本中扫描的模式
  > - `return_type_string` (string): 函数的返回类型。支持的类型包括 **"int"**（整数）, **"bool"**（布尔值）, **"const char\*/string"**（字符串）, **"ptr/pointer/*"**（指针）, **"float"**（浮点数）, 和 **"vector3"**（三维向量）。其他类型将被拒绝
  > - `args_` (table): 传递给函数的参数表。支持的类型与返回类型相同

- **Parameters:**
  - `script_name` (string): Name of the script.
  - `function_name` (string): Name of the function. This parameter needs to be unique.
  - `pattern` (string): Pattern to scan for within the script.
  - `return_type_string` (string): Return type of the function. Supported types are **"int"**, **"bool"**, **"const char\*/string"**, **"ptr/pointer/*"**, **"float"**, and **"vector3"**. Anything different will be rejected.
  - `args_` (table): Arguments to pass to the function. Supported types are the same as return types.

**Example Usage:**
```lua
scr_function.call_script_function(script_name, function_name, pattern, return_type_string, args_)
```

### `call_script_function(script_name, instruction_pointer, return_type_string, args_)`

> 通过指令指针直接调用脚本函数。使用函数位置和给定参数直接调用脚本函数，并按指定类型返回返回值。

Calls a script function directly using the function position with the given arguments. Returns the return value as the given type.
**Example Usage:**
```lua
local value = scr_function.call_script_function("freemode", 0xE792, "string", {
   { "int", 191 }
})
```

- **Parameters:**
  > **参数说明：**
  > - `script_name` (string): 脚本名称
  > - `instruction_pointer` (integer): 函数在脚本中的位置
  > - `return_type_string` (string): 函数的返回类型。支持的类型包括 **"int"**（整数）, **"bool"**（布尔值）, **"const char\*/string"**（字符串）, **"ptr/pointer/*"**（指针）, **"float"**（浮点数）, 和 **"vector3"**（三维向量）。其他类型将被拒绝
  > - `args_` (table): 传递给函数的参数表。支持的类型与返回类型相同

- **Parameters:**
  - `script_name` (string): Name of the script.
  - `instruction_pointer` (integer): Position of the function within the script.
  - `return_type_string` (string): Return type of the function. Supported types are **"int"**, **"bool"**, **"const char\*/string"**, **"ptr/pointer/*"**, **"float"**, and **"vector3"**. Anything different will be rejected.
  - `args_` (table): Arguments to pass to the function. Supported types are the same as return types.

**Example Usage:**
```lua
scr_function.call_script_function(script_name, instruction_pointer, return_type_string, args_)
```



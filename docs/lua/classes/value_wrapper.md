# Class: value_wrapper

<!-- 
类名：value_wrapper
这是一个用于包装函数参数和返回值的类，主要应用于dynamic_hook系统中。
它提供了一个简单的接口来获取和设置被包装的值。
-->

Class for wrapping parameters and return value of functions, used mostly by the dynamic_hook system.

## Functions (2)

### `get()`

<!-- 
函数：get()
获取当前包装器中存储的值。

返回值：
- 任意类型：返回当前包装器中存储的值
-->

Get the value currently contained by the wrapper.

- **Returns:**
  - `any`: The current value.

**Example Usage:**
```lua
any = value_wrapper:get()
```

### `set(new_value)`

<!-- 
函数：set(new_value)
设置包装器中存储的新值。

参数：
- new_value (任意类型)：要存储在包装器中的新值
-->

Set the new value contained by the wrapper.

- **Parameters:**
  - `new_value` (any): The new value.

**Example Usage:**
```lua
value_wrapper:set(new_value)
```



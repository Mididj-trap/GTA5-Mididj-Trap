# Table: Global Table

<!-- 
全局表(Global Table)是Lua语言中的一个特殊表，它包含了所有的全局变量。
这里列出了添加到Lua全局表中的自定义字段、函数等扩展功能。
-->

Custom fields, functions, etc added to The Lua [Global Table](https://www.lua.org/pil/15.4.html).

## Functions (1)

### `joaat(str)`

<!-- 
joaat函数用于计算字符串的Jenkins one-at-a-time哈希值。
这是GTA5中常用的一种哈希算法，用于将字符串转换为整数标识符。
-->

- **Parameters:**
  - `str` (string): The string that needs to be joaat hashed.
    <!-- 参数str：需要进行joaat哈希计算的字符串 -->

- **Returns:**
  - `integer`: The joaat hashed input string.
    <!-- 返回值：输入字符串的joaat哈希值（整数类型）-->

**Example Usage:**
```lua
integer = joaat(str)
```
<!-- 
使用示例说明：
将字符串变量str进行joaat哈希计算，得到的整数结果存储在integer变量中
-->



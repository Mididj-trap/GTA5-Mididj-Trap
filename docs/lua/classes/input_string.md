# Class: input_string

<!-- 这是一个用于在GUI中创建和管理字符串输入框的类 -->

## Inherit from 1 class: base_text_element

<!-- 继承自base_text_element基础文本元素类 -->

Class for representing an input field for editing a string value within the GUI.

<!-- 该类用于在GUI界面中表示一个可编辑字符串值的输入框 -->

## Functions (2)

### `get_value()`

<!-- 获取输入框中当前输入的字符串值 -->

- **Returns:**
  - `string`: Get the value currently written inside the input field.

<!-- 返回值：
  - string类型：返回输入框中当前输入的字符串内容 -->

**Example Usage:**
```lua
string = input_string:get_value()
```

### `set_value(val)`

<!-- 设置输入框中的字符串值 -->

- **Parameters:**
  - `val` (string): Set the value currently written inside the input field.

<!-- 参数：
  - val (string类型)：要设置到输入框中的字符串值 -->

**Example Usage:**
```lua
input_string:set_value(val)
```



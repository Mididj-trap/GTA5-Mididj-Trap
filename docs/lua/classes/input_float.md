# Class: input_float
<!-- 类名：浮点数输入框 -->

## Inherit from 1 class: base_text_element
<!-- 继承关系：继承自base_text_element基类 -->

Class for representing an input field for editing a float value within the GUI.
<!-- 类描述：表示GUI中用于编辑浮点数值的输入框组件 -->

## Functions (2)
<!-- 方法列表：共2个方法 -->

### `get_value()`
<!-- 方法功能：获取输入框中的当前值 -->

- **Returns:**
  - `float`: Get the value currently written inside the input field.
  <!-- 返回值说明：返回浮点数类型的当前输入值 -->

**Example Usage:**
<!-- 使用示例：调用get_value方法获取输入值 -->
```lua
float = input_float:get_value()
```

### `set_value(val)`
<!-- 方法功能：设置输入框的值 -->

- **Parameters:**
  - `val` (float): Set the value currently written inside the input field.
  <!-- 参数说明：浮点数类型，设置输入框中的值 -->

**Example Usage:**
<!-- 使用示例：调用set_value方法设置输入值 -->
```lua
input_float:set_value(val)
```



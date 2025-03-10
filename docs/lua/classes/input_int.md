# Class: input_int

<!-- input_int类：用于在GUI中创建和管理整数输入框的类 -->

## Inherit from 1 class: base_text_element
<!-- 继承自base_text_element基类 -->

Class for representing an input field for editing an integer value within the GUI.
<!-- 这个类用于在图形用户界面(GUI)中表示一个用于编辑整数值的输入框 -->

## Functions (2)

### `get_value()`
<!-- 获取输入框当前的整数值 -->

- **Returns:**
  - `integer`: Get the value currently written inside the input field.
  <!-- 返回：整数类型，获取输入框中当前输入的整数值 -->

**Example Usage:**
```lua
integer = input_int:get_value()
```

### `set_value(val)`
<!-- 设置输入框的整数值 -->

- **Parameters:**
  - `val` (integer): Set the value currently written inside the input field.
  <!-- 参数：val (整数类型) - 要设置到输入框中的整数值 -->

**Example Usage:**
```lua
input_int:set_value(val)
```



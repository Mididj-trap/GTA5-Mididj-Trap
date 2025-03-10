# Class: checkbox
<!-- 类名：复选框 -->

## Inherit from 1 class: base_text_element
<!-- 继承关系：继承自base_text_element基类 -->

Class representing a gui checkbox.
<!-- 类描述：表示GUI中的复选框组件 -->

## Functions (2)
<!-- 方法列表：共2个方法 -->

### `is_enabled()`
<!-- 方法功能：获取复选框的选中状态 -->

- **Returns:**
  - `boolean`: Is the checkbox checked?
  <!-- 返回值说明：返回布尔值，表示复选框是否被选中 -->

**Example Usage:**
<!-- 使用示例：调用is_enabled方法获取复选框状态 -->
```lua
boolean = checkbox:is_enabled()
```

### `set_enabled(enabled)`
<!-- 方法功能：设置复选框的选中状态 -->

- **Parameters:**
  - `enabled` (boolean): The desired enabled state of the checkbox.
  <!-- 参数说明：布尔值，设置复选框是否选中 -->

**Example Usage:**
<!-- 使用示例：调用set_enabled方法设置复选框状态 -->
```lua
checkbox:set_enabled(enabled)
```



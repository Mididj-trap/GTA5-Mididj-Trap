# Class: base_text_element
<!-- 文本元素基类：表示GUI中的文本元素组件 -->

Class representing a gui text element.

## Functions (2)

### `set_text(new_text)`
<!-- 方法功能：设置文本元素内容 -->

- **Parameters:**
  - `new_text` (string): The new text for that gui text element. <!-- 参数说明：接受字符串类型的新文本 -->

**Example Usage:**
<!-- 使用示例：调用set_text方法更新文本 -->
```lua
base_text_element:set_text(new_text)
```

### `get_text()`
<!-- 方法功能：获取当前文本内容 -->

- **Returns:**
  - `string`: Returns the current text for that gui text element. <!-- 返回值说明：返回字符串类型的当前文本 -->

**Example Usage:**
<!-- 使用示例：调用get_text方法获取文本 -->
```lua
string = base_text_element:get_text()
```

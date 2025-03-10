# Class: text

<!-- 这是一个表示imgui文本元素的类，用于在GUI系统中创建和管理文本显示 -->

## Inherit from 1 class: base_text_element

<!-- 该类继承自base_text_element基类，获得了基本文本元素的所有功能 -->

Class representing an imgui text element.

<!-- 这个类用于表示一个imgui文本元素，可以在界面上显示文字内容 -->

## Functions (1)

### `set_font(font)`

<!-- 设置文本元素的字体，可以改变文本的显示样式 -->

- **Parameters:**
  - `font` (string): The new font name for that imgui text element.

<!-- 参数说明：
  - font：字符串类型，指定要使用的新字体名称，将应用于该imgui文本元素 -->

**Example Usage:**
```lua
text:set_font(font)
```

<!-- 使用示例：
通过调用set_font方法，可以为文本元素设置新的字体。
例如，如果你想将文本改为使用"Arial"字体，可以这样调用：
text:set_font("Arial") -->



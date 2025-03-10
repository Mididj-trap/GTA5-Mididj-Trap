# Class: tab

<!-- 这是一个用于表示GUI中标签页的类。它提供了丰富的方法来添加和管理GUI元素。 -->
Class for representing a tab within the GUI.

## Functions (12)

### `is_selected()`

<!-- 检查当前标签页是否被选中 -->
- **Returns:**
  - `boolean`: Returns true if this tab is the one currently selected in the GUI.
<!-- 返回值：布尔值，如果当前标签页是GUI中被选中的标签页则返回true -->

**Example Usage:**
```lua
boolean = tab:is_selected()
```

### `clear()`

<!-- 清除标签页中所有你拥有的自定义Lua内容 -->
Clear the tab of all its custom lua content that you own.

**Example Usage:**
```lua
tab:clear()
```

### `add_tab(tab_name)`

<!-- 向当前标签页添加一个子标签页 -->
Add a sub tab to this tab.

- **Parameters:**
  - `tab_name` (string): Name of the tab to add.
<!-- 参数：tab_name (字符串类型) - 要添加的标签页名称 -->

- **Returns:**
  - `tab`: A tab instance which corresponds to the new tab in the GUI.
<!-- 返回值：tab对象 - 对应于GUI中新创建的标签页实例 -->

**Example Usage:**
```lua
tab = tab:add_tab(tab_name)
```

### `add_button(name, callback)`

<!-- 向GUI标签页添加一个按钮 -->
Add a button to the gui tab.

- **Parameters:**
  - `name` (string): Text written inside the button.
  - `callback` (function): function that will be called when the button is clicked.
<!-- 参数：
  - name (字符串类型) - 按钮内显示的文本
  - callback (函数类型) - 当按钮被点击时将调用的函数 -->

**Example Usage:**
```lua
tab:add_button(name, callback)
```

### `add_text(name)`

<!-- 向GUI标签页添加文本 -->
Add text to the gui tab.

- **Parameters:**
  - `name` (string): Text that will be written.
<!-- 参数：name (字符串类型) - 要显示的文本内容 -->

- **Returns:**
  - `text`: The text object instance.
<!-- 返回值：text对象 - 文本对象实例 -->

**Example Usage:**
```lua
text = tab:add_text(name)
```

### `add_checkbox(name)`

<!-- 向GUI标签页添加一个复选框部件 -->
Add a checkbox widget to the gui tab.

- **Parameters:**
  - `name` (string): Text that will be written next to the checkbox.
<!-- 参数：name (字符串类型) - 显示在复选框旁边的文本 -->

- **Returns:**
  - `checkbox`: The checkbox object instance.
<!-- 返回值：checkbox对象 - 复选框对象实例 -->

**Example Usage:**
```lua
checkbox = tab:add_checkbox(name)
```

### `add_sameline()`

<!-- 添加ImGui::SameLine效果，使下一个控件在同一行显示 -->
Add a ImGui::SameLine.

- **Returns:**
  - `sameline`: The sameline object instance.
<!-- 返回值：sameline对象 - 同行显示对象实例 -->

**Example Usage:**
```lua
sameline = tab:add_sameline()
```

### `add_separator()`

<!-- 添加ImGui::Separator分隔线 -->
Add a ImGui::Separator.

- **Returns:**
  - `separator`: The separator object instance.
<!-- 返回值：separator对象 - 分隔线对象实例 -->

**Example Usage:**
```lua
separator = tab:add_separator()
```

### `add_input_int(name)`

<!-- 添加ImGui::InputInt整数输入框 -->
Add a ImGui::InputInt.

- **Parameters:**
  - `name` (string): Text that will be written next to the input field.
<!-- 参数：name (字符串类型) - 显示在输入框旁边的文本 -->

- **Returns:**
  - `input_int`: The input_int object instance.
<!-- 返回值：input_int对象 - 整数输入框对象实例 -->

**Example Usage:**
```lua
input_int = tab:add_input_int(name)
```

### `add_input_float(name)`

<!-- 添加ImGui::InputFloat浮点数输入框 -->
Add a ImGui::InputFloat.

- **Parameters:**
  - `name` (string): Text that will be written next to the input field.
<!-- 参数：name (字符串类型) - 显示在输入框旁边的文本 -->

- **Returns:**
  - `input_float`: The input_float object instance.
<!-- 返回值：input_float对象 - 浮点数输入框对象实例 -->

**Example Usage:**
```lua
input_float = tab:add_input_float(name)
```

### `add_input_string(name)`

<!-- 添加ImGui::InputText文本输入框 -->
Add a ImGui::InputText.

- **Parameters:**
  - `name` (string): Text that will be written next to the input field.
<!-- 参数：name (字符串类型) - 显示在输入框旁边的文本 -->

- **Returns:**
  - `input_string`: The input_string object instance.
<!-- 返回值：input_string对象 - 文本输入框对象实例 -->

**Example Usage:**
```lua
input_string = tab:add_input_string(name)
```

### `add_imgui(imgui_rendering)`

<!-- 注册一个在每帧渲染时调用的函数，你可以在其中调用ImGui函数。更多信息请查看ImGui.md文档文件。 -->
Registers a function that will be called every rendering frame, you can call ImGui functions in it, please check the ImGui.md documentation file for more info.
**Example Usage:**
```lua
tab:add_imgui(function()
   if ImGui.Begin("My Custom Window") then
       if ImGui.Button("Label") then
         script.run_in_fiber(function(script)
           -- call natives in there
         end)
       end

       ImGui.End()
   end
end)
```

- **Parameters:**
  - `imgui_rendering` (function): Function that will be called every rendering frame, you can call ImGui functions in it, please check the ImGui.md documentation file for more info.
<!-- 参数：imgui_rendering (函数类型) - 将在每帧渲染时被调用的函数，你可以在其中调用ImGui函数。更多信息请查看ImGui.md文档文件。 -->

**Example Usage:**
```lua
tab:add_imgui(imgui_rendering)
```



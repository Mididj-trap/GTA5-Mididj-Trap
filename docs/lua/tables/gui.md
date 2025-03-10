# Table: gui

<!-- 
此表包含用于修改菜单GUI的函数。
通过这些函数，你可以：
- 管理GUI标签页
- 显示各种类型的消息提示
- 控制GUI的显示和隐藏
- 处理鼠标事件
- 添加自定义ImGui渲染
-->

Table containing functions for modifying the menu GUI.

## Functions (12)

### `get_tab(tab_name)`

<!-- 
获取指定名称的GUI标签页。
-->

- **Parameters:**
  - `tab_name` (string): <!-- 要获取的标签页名称 --> Name of the tab to get.

- **Returns:**
  - `tab`: <!-- 返回与GUI中对应标签页相关联的标签页实例 --> A tab instance which corresponds to the tab in the GUI.

**Example Usage:**
```lua
tab = gui.get_tab(tab_name)
```

### `add_tab(tab_name)`

<!-- 
添加一个新的GUI标签页。
-->

- **Parameters:**
  - `tab_name` (string): <!-- 要添加的新标签页名称 --> Name of the tab to add.

- **Returns:**
  - `tab`: <!-- 返回与新创建的GUI标签页相关联的标签页实例 --> A tab instance which corresponds to the new tab in the GUI.

**Example Usage:**
```lua
tab = gui.add_tab(tab_name)
```

### `show_success(title, message)`

<!-- 
显示一个成功提示消息框，包含指定的标题和内容。
-->

Shows a success to the user with the given title and message.

- **Parameters:**
  - `title` (string): <!-- 成功提示框的标题 -->
  - `message` (string): <!-- 成功提示框的具体内容 -->

**Example Usage:**
```lua
gui.show_success(title, message)
```

### `show_message(title, message)`

<!-- 
显示一个普通消息框，包含指定的标题和内容。
-->

Shows a message to the user with the given title and message.

- **Parameters:**
  - `title` (string): <!-- 消息框的标题 -->
  - `message` (string): <!-- 消息框的具体内容 -->

**Example Usage:**
```lua
gui.show_message(title, message)
```

### `show_warning(title, message)`

<!-- 
显示一个警告提示消息框，包含指定的标题和内容。
-->

Shows a warning to the user with the given title and message.

- **Parameters:**
  - `title` (string): <!-- 警告提示框的标题 -->
  - `message` (string): <!-- 警告提示框的具体内容 -->

**Example Usage:**
```lua
gui.show_warning(title, message)
```

### `show_error(title, message)`

<!-- 
显示一个错误提示消息框，包含指定的标题和内容。
-->

Shows an error to the user with the given title and message.

- **Parameters:**
  - `title` (string): <!-- 错误提示框的标题 -->
  - `message` (string): <!-- 错误提示框的具体内容 -->

**Example Usage:**
```lua
gui.show_error(title, message)
```

### `is_open()`

- **Returns:**
  - `bool`: Returns true if the GUI is open.

**Example Usage:**
```lua
bool = gui.is_open()
```

### `toggle(toggle)`

Opens and closes the gui.

- **Parameters:**
  - `toggle` (boolean)

**Example Usage:**
```lua
gui.toggle(toggle)
```

### `mouse_override()`

- **Returns:**
  - `bool`: Returns true if the mouse is overridden.

**Example Usage:**
```lua
bool = gui.mouse_override()
```

### `override_mouse(override)`

- **Parameters:**
  - `override` (boolean)

**Example Usage:**
```lua
gui.override_mouse(override)
```

### `add_imgui(imgui_rendering)`

Registers a function that will be called every rendering frame, you can call ImGui functions in it, please check the ImGui.md documentation file for more info.
**Example Usage:**
```lua
gui.add_imgui(function()
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

**Example Usage:**
```lua
gui.add_imgui(imgui_rendering)
```

### `add_always_draw_imgui(imgui_rendering)`

<!-- 
注册一个在每个渲染帧中被调用的函数，你可以在其中调用ImGui函数。
即使菜单关闭时该函数也会被调用。
详细信息请查看ImGui.md文档文件。
-->

Registers a function that will be called every rendering frame, you can call ImGui functions in it, please check the ImGui.md documentation file for more info. This function will be called even when the menu is closed.
**Example Usage:**
```lua
gui.add_always_draw_imgui(function()
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
  - `imgui_rendering` (function): <!-- 将在每个渲染帧中被调用的函数，你可以在其中调用ImGui函数。即使菜单关闭时该函数也会被调用。详细信息请查看ImGui.md文档文件。 --> Function that will be called every rendering frame, you can call ImGui functions in it, please check the ImGui.md documentation file for more info.

**Example Usage:**
```lua
gui.add_always_draw_imgui(imgui_rendering)
```



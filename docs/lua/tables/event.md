# Table: event

<!-- 
事件表（event）用于响应各种菜单事件。你可以通过这个表注册事件处理函数，当特定的菜单事件被触发时，相应的处理函数就会被调用。
所有可用的菜单事件类型都定义在menu_event表中。
-->

Table for responding to various events. The list of events is available in the menu_event table.

## Functions (1)

### `register_handler(menu_event, func)`

<!-- 
注册一个事件处理函数。每当指定的菜单事件被触发时，这个处理函数就会被调用。

参数说明：
- menu_event：要响应的菜单事件类型，必须是menu_event表中定义的有效事件类型
- func：事件处理函数，当指定的菜单事件发生时，这个函数会被自动调用
-->

Register a function that will be called each time the corresponding menu_event is triggered.

- **Parameters:**
  - `menu_event` (menu_event): The menu_event that we want to respond to.
  - `func` (function): The function that will be called.

**Example Usage:**
```lua
<!-- 
使用示例：
这行代码演示了如何注册一个事件处理函数。
当menu_event指定的事件发生时，func函数将被调用来处理该事件。
-->
event.register_handler(menu_event, func)
```



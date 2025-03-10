# Table: command

<!-- 用于调用菜单命令的表 -->
Table for calling menu commands.

## Functions (3)

### `call(command_name, _args)`

<!-- 调用一个菜单命令 -->
Call a menu command.

<!-- 参数说明：
  - command_name (字符串)：将要调用的命令名称
  - _args (表)：可选参数。命令的参数列表 -->
- **Parameters:**
  - `command_name` (string): The name of the command that will be called.
  - `_args` (table): Optional. List of arguments for the command.

<!-- 使用示例 -->
**Example Usage:**
```lua
command.call(command_name, _args)
```

### `call_player(player_idx, command_name, _args)`

<!-- 在指定玩家上调用菜单命令 -->
Call a menu command on a given player.

<!-- 参数说明：
  - player_idx (整数)：将执行菜单命令的玩家索引
  - command_name (字符串)：将要调用的命令名称
  - _args (表)：可选参数。命令的参数列表 -->
- **Parameters:**
  - `player_idx` (integer): Index of the player on which the menu command will be executed.
  - `command_name` (string): The name of the command that will be called.
  - `_args` (table): Optional. List of arguments for the command.

<!-- 使用示例 -->
**Example Usage:**
```lua
command.call_player(player_idx, command_name, _args)
```

### `get_all_player_command_names()`

<!-- 返回值说明：
  - table<integer, string>：包含所有玩家命令名称的表 -->
- **Returns:**
  - `table<integer, string>`: Table that contains the names of all the player commands.

<!-- 使用示例 -->
**Example Usage:**
```lua
table<integer, string> = command.get_all_player_command_names()
```



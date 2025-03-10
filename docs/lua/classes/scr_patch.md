# Class: scr_patch

<!-- 这是一个用于修补GTA脚本函数的类 -->
Class for patching GTA script functions.

## Constructors (1)

### `new(script_name, patch_name, pattern, offset, patch_)`

<!-- 为指定的脚本添加一个补丁 -->
Adds a patch for the specified script.

- **Parameters:**
  <!-- 参数说明 -->
  - `script_name` (string): <!-- 脚本名称 --> The name of the script.
  - `patch_name` (string): <!-- 补丁名称 --> The name of the patch.
  - `pattern` (string): <!-- 在脚本中需要扫描的模式 --> The pattern to scan for within the script.
  - `offset` (integer): <!-- 模式中的位置偏移量 --> The position within the pattern.
  - `patch_` (table): <!-- 要写入脚本字节码的字节数据 --> The bytes to be written into the script's bytecode.

**Example Usage:**
<!-- 使用示例 -->
```lua
my_patch = scr_patch:new(script_name, patch_name, pattern, offset, patch_)
```

## Functions (2)

### `enable()`

<!-- 启用当前实例的脚本补丁。当创建新实例时，补丁默认是启用状态 -->
Enables the script patch for the current instance. When a new instance is created, it will be enabled by default.

**Example Usage:**
<!-- 使用示例 -->
```lua
scr_patch:enable()
```

### `disable()`

<!-- 禁用当前实例的脚本补丁 -->
Disables the script patch for the current instance.

**Example Usage:**
<!-- 使用示例 -->
```lua
scr_patch:disable()
```
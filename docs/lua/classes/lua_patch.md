# Class: lua_patch

<!-- 这是一个表示内存补丁的类，用于在运行时修改和恢复内存中的值 -->
Class representing a in-memory patch.

## Functions (2)

### `apply()`

<!-- 应用修改后的值到内存中。当你需要使修改生效时调用此方法 -->
Apply the modified value.

**Example Usage:**
```lua
lua_patch:apply()
```

### `restore()`

<!-- 将内存中的值恢复到原始状态。当你需要撤销修改时调用此方法 -->
Restore the original value.

**Example Usage:**
```lua
lua_patch:restore()
```



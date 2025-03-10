# Table: self

Table for retrieving data or info about our own player object.

用于获取当前玩家对象数据和信息的功能表。

## Functions (5)

### `get_ped()`

获取当前玩家角色的脚本句柄。

- **Returns:**
  - `integer`: Script handle of our ped.
  - `integer`: 返回当前玩家角色的脚本句柄。

**Example Usage:**
```lua
integer = self.get_ped()
```

### `get_id()`

获取当前玩家的ID。

- **Returns:**
  - `integer`: Our player id.
  - `integer`: 返回当前玩家的ID。

**Example Usage:**
```lua
integer = self.get_id()
```

### `get_pos()`

获取当前玩家角色的位置坐标。

- **Returns:**
  - `vec3`: Position of our ped.
  - `vec3`: 返回当前玩家角色的三维位置坐标。

**Example Usage:**
```lua
vec3 = self.get_pos()
```

### `get_rot()`

获取当前玩家角色的旋转角度。

- **Returns:**
  - `vec3`: Rotation of our ped.
  - `vec3`: 返回当前玩家角色的三维旋转角度。

**Example Usage:**
```lua
vec3 = self.get_rot()
```

### `get_veh()`

获取当前玩家所在载具的脚本句柄。

- **Returns:**
  - `integer`: Script handle of our current vehicle.
  - `integer`: 返回当前玩家所在载具的脚本句柄。

**Example Usage:**
```lua
integer = self.get_veh()
```



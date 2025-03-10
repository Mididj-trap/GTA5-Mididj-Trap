# Table: entities

<!-- 用于操作GTA实体的表 -->
Table for manipulating GTA entities.

## Functions (4)

### `get_all_vehicles_as_handles()`

<!-- 获取所有载具的脚本句柄 -->

<!-- 返回值说明：
  - table<int, int>：返回包含所有载具脚本句柄的表 -->
- **Returns:**
  - `table<int, int>`: Returns all vehicles as script handles

<!-- 使用示例 -->
**Example Usage:**
```lua
table<int, int> = entities.get_all_vehicles_as_handles()
```

### `get_all_peds_as_handles()`

<!-- 获取所有行人的脚本句柄 -->

<!-- 返回值说明：
  - table<int, int>：返回包含所有行人脚本句柄的表 -->
- **Returns:**
  - `table<int, int>`: Returns all peds as script handles

<!-- 使用示例 -->
**Example Usage:**
```lua
table<int, int> = entities.get_all_peds_as_handles()
```

### `get_all_objects_as_handles()`

<!-- 获取所有物体的脚本句柄 -->

<!-- 返回值说明：
  - table<int, int>：返回包含所有物体脚本句柄的表 -->
- **Returns:**
  - `table<int, int>`: Returns all objects as script handles

<!-- 使用示例 -->
**Example Usage:**
```lua
table<int, int> = entities.get_all_objects_as_handles()
```

### `take_control_of(entity, try_count)`

<!-- 必须从脚本中调用（例如使用script.run_in_fiber） -->
Must be called from a script (script.run_in_fiber for example)

<!-- 参数说明：
  - entity (实体)：我们尝试获取控制权的实体的脚本句柄
  - try_count (整数)：可选参数。尝试获取实体控制权的次数，默认为300 -->
- **Parameters:**
  - `entity` (Entity): Script handle of the entity we are trying to take control of.
  - `try_count` (integer): Optional. Number of time we'll try taking control of the entity. Default to 300.

<!-- 返回值说明：
  - boolean：如果成功获取实体的控制权则返回true -->
- **Returns:**
  - `boolean`: Returns true if we successfully got control of the entity.

<!-- 使用示例 -->
**Example Usage:**
```lua
boolean = entities.take_control_of(entity, try_count)
```



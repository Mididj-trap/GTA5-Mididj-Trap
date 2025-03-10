# Table: vehicles

# 载具表（Table: vehicles）
Table containing functions for getting information about vehicles in GTA V.
此表包含用于获取GTA5中载具信息的函数。

## Functions (4)

### `get_vehicle_display_name(vehicle_hash)`

> 通过载具哈希值获取载具的显示名称

- **Example Usage (使用示例):**
```lua
log.info(vehicles.get_vehicle_display_name('BTYPE2'))
```

- **Parameters (参数):**
  - `vehicle_hash` (Hash): JOAAT hash of the vehicle.
    载具的JOAAT哈希值。

- **Returns (返回值):**
  - `vehicle_display_string`: String: the in-game display string. If the vehicle is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
    返回游戏中的显示字符串。如果未找到载具或调用时机过早，将返回空字符串。保证返回安全值。

**Example Usage:**
```lua
vehicle_display_string = vehicles.get_vehicle_display_name(vehicle_hash)
```

### `get_vehicle_display_name(vehicle_name)`

> 通过载具名称获取载具的显示名称

- **Example Usage (使用示例):**
```lua
log.info(vehicles.get_vehicle_display_name('BTYPE2'))
```

- **Parameters (参数):**
  - `vehicle_name` (String): Name of the vehicle.
    载具的名称。

- **Returns (返回值):**
  - `vehicle_display_string`: String: the in-game display string. If the vehicle is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
    返回游戏中的显示字符串。如果未找到载具或调用时机过早，将返回空字符串。保证返回安全值。

**Example Usage:**
```lua
vehicle_display_string = vehicles.get_vehicle_display_name(vehicle_name)
```

### `get_all_vehicles_by_class(vehicle_class)`

> 获取指定类别的所有载具列表

- **Example Usage (使用示例):**
```lua
local sports_classics = vehicles.get_all_vehicles_by_class('Sports Classics')
for i = 1, #sports_classics do
    log.info(sports_classics[i])
end
```

- **Parameters (参数):**
  - `vehicle_class` (String): The vehicle class.
    载具类别。

- **Returns (返回值):**
  - `vehicles`: table<int, String>: a list of all vehicles that match the class passed in. The list can contain anything from 0 to n elements.
    返回与指定类别匹配的所有载具列表。列表可能包含0到n个元素。

**Example Usage:**
```lua
vehicles = vehicles.get_all_vehicles_by_class(vehicle_class)
```

### `get_all_vehicles_by_mfr(manufacturer)`

> 获取指定制造商的所有载具列表

- **Example Usage (使用示例):**
```lua
local albanies = vehicles.get_all_vehicles_by_mfr('Albany')
for i = 1, #albanies do
    log.info(albanies[i])
end
```

- **Parameters (参数):**
  - `manufacturer` (String): The vehicle manufacturer.
    载具制造商。

- **Returns (返回值):**
  - `vehicles`: table<int, String>: a list of all vehicles that match the manufacturer passed in. The list can contain anything from 0 to n elements.
    返回与指定制造商匹配的所有载具列表。列表可能包含0到n个元素。

**Example Usage:**
```lua
vehicles = vehicles.get_all_vehicles_by_mfr(manufacturer)
```



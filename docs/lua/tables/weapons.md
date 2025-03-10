# Table: weapons

Table containing functions for getting information about weapons in GTA V.

【中文说明：此表包含用于获取GTA V中武器信息的函数。】

## Functions (10)
【中文说明：共10个函数，用于处理武器相关的各种操作。】

### `get_weapon_display_name(weapon_hash)`
【中文说明：通过武器哈希值获取武器的显示名称。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_display_name(joaat('WEAPON_REVOLVER')))
```

- **Parameters:**
  - `weapon_hash` (Hash): JOAAT hash of the weapon.
  【参数说明：weapon_hash - 武器的JOAAT哈希值】

- **Returns:**
  - `weapon_display_name`: String: the in-game display string. If the weapon is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：weapon_display_name - 字符串类型，返回游戏中武器的显示名称。如果未找到武器或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
weapon_display_name = weapons.get_weapon_display_name(weapon_hash)
```

### `get_weapon_display_name(weapon_name)`
【中文说明：通过武器名称获取武器的显示名称。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_display_name('WEAPON_REVOLVER'))
```

- **Parameters:**
  - `weapon_name` (String): Name of the weapon.
  【参数说明：weapon_name - 字符串类型，武器的名称】

- **Returns:**
  - `weapon_display_name`: String: the in-game display string. If the weapon is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：weapon_display_name - 字符串类型，返回游戏中武器的显示名称。如果未找到武器或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
weapon_display_name = weapons.get_weapon_display_name(weapon_name)
```

### `get_all_weapons_of_group_type(group_hash)`
【中文说明：通过武器组的哈希值获取该组中的所有武器。】

- **Example Usage:**
```lua
local pistols = weapons.get_all_weapons_of_group_type(joaat('GROUP_PISTOL'))
for i = 1, #pistols do
    log.info(pistols[i])
end
```

- **Parameters:**
  - `group_hash` (Hash): The JOAAT hash of the group the weapon(s) belong to.
  【参数说明：group_hash - 武器组的JOAAT哈希值】

- **Returns:**
  - `weapons_of_group_type`: table<int, String>: a list of all weapons that match the group hash passed in. The list can contain anything from 0 to n elements.
  【返回值说明：weapons_of_group_type - 表类型，包含匹配该组哈希值的所有武器列表。列表可能包含0到多个元素。】

**Example Usage:**
```lua
weapons_of_group_type = weapons.get_all_weapons_of_group_type(group_hash)
```

### `get_all_weapons_of_group_type(group_name)`
【中文说明：通过武器组的名称获取该组中的所有武器。】

- **Example Usage:**
```lua
local pistols = weapons.get_all_weapons_of_group_type('GROUP_PISTOL')
for i = 1, #pistols do
	log.info(pistols[i])
end

local pistols = weapons.get_all_weapons_of_group_type('PISTOL')
for i = 1, #pistols do
	log.info(pistols[i])
end
```

- **Parameters:**
  - `group_name` (String): The group the weapon(s) belong to. Can be in either GROUP_ format or not. Parameter is case-insensitive.
  【参数说明：group_name - 字符串类型，武器所属的组名。可以使用GROUP_前缀格式或不使用，参数不区分大小写。】

- **Returns:**
  - `weapons_of_group_type`: table<int, String>: a list of all weapons that match the group hash passed in. The list can contain anything from 0 to n elements.
  【返回值说明：weapons_of_group_type - 表类型，包含匹配该组名称的所有武器列表。列表可能包含0到多个元素。】

**Example Usage:**
```lua
weapons_of_group_type = weapons.get_all_weapons_of_group_type(group_name)
```

### `get_all_weapon_components(weapon_hash)`
【中文说明：通过武器哈希值获取该武器的所有组件。】

- **Example Usage:**
```lua
local pistol_attachments = weapons.get_all_weapon_components(joaat('WEAPON_PISTOL'))
for i = 1, #pistol_attachments do
	log.info(pistol_attachments[i])
end
```

- **Parameters:**
  - `weapon_hash` (Hash): The JOAAT hash of the weapon the component(s) belong to.
  【参数说明：weapon_hash - 武器的JOAAT哈希值，用于获取该武器的组件】

- **Returns:**
  - `weapon_components`: table<int, String>: a list of all components that match the weapon passed in. The list can contain anything from 0 to n elements.
  【返回值说明：weapon_components - 表类型，包含匹配该武器的所有组件列表。列表可能包含0到多个元素。】

**Example Usage:**
```lua
weapon_components = weapons.get_all_weapon_components(weapon_hash)
```

### `get_all_weapon_components(weapon_name)`
【中文说明：通过武器名称获取该武器的所有组件。】

- **Example Usage:**
```lua
local pistol_attachments = weapons.get_all_weapon_components('WEAPON_PISTOL')
for i = 1, #pistol_attachments do
	log.info(pistol_attachments[i])
end
```

- **Parameters:**
  - `weapon_name` (String): The weapon the component(s) belong to.
  【参数说明：weapon_name - 字符串类型，要获取组件的武器名称】

- **Returns:**
  - `weapon_components`: table<int, String>: a list of all components that match the weapon passed in. The list can contain anything from 0 to n elements.
  【返回值说明：weapon_components - 表类型，包含匹配该武器的所有组件列表。列表可能包含0到多个元素。】

**Example Usage:**
```lua
weapon_components = weapons.get_all_weapon_components(weapon_name)
```

### `get_weapon_component_display_name(weapon_component_hash)`
【中文说明：通过武器组件哈希值获取该组件的显示名称。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_component_display_name(joaat('COMPONENT_PISTOL_CLIP_01')))
```

- **Parameters:**
  - `weapon_component_hash` (Hash): JOAAT hash of the weapon component.
  【参数说明：weapon_component_hash - 武器组件的JOAAT哈希值】

- **Returns:**
  - `component_display_name`: String: the in-game display string. If the component is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：component_display_name - 字符串类型，返回游戏中组件的显示名称。如果未找到组件或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
component_display_name = weapons.get_weapon_component_display_name(weapon_component_hash)
```

### `get_weapon_component_display_name(weapon_component)`
【中文说明：通过武器组件名称获取该组件的显示名称。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_component_display_name('COMPONENT_PISTOL_CLIP_01'))
```

- **Parameters:**
  - `weapon_component` (String): The weapon component.
  【参数说明：weapon_component - 字符串类型，武器组件的名称】

- **Returns:**
  - `component_display_name`: String: the in-game display string. If the component is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：component_display_name - 字符串类型，返回游戏中组件的显示名称。如果未找到组件或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
component_display_name = weapons.get_weapon_component_display_name(weapon_component)
```

### `get_weapon_component_display_desc(weapon_component_hash)`
【中文说明：通过武器组件哈希值获取该组件的显示描述。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_component_display_desc(joaat('COMPONENT_PISTOL_CLIP_01')))
```

- **Parameters:**
  - `weapon_component_hash` (Hash): JOAAT hash of the weapon component.
  【参数说明：weapon_component_hash - 武器组件的JOAAT哈希值】

- **Returns:**
  - `component_display_desc`: String: the in-game display string. If the component is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：component_display_desc - 字符串类型，返回游戏中组件的显示描述。如果未找到组件或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
component_display_desc = weapons.get_weapon_component_display_desc(weapon_component_hash)
```

### `get_weapon_component_display_desc(weapon_component)`
【中文说明：通过武器组件名称获取该组件的显示描述。】

- **Example Usage:**
```lua
log.info(weapons.get_weapon_component_display_desc('COMPONENT_PISTOL_CLIP_01'))
```

- **Parameters:**
  - `weapon_component` (String): The weapon component.
  【参数说明：weapon_component - 字符串类型，武器组件的名称】

- **Returns:**
  - `component_display_desc`: String: the in-game display string. If the component is not found, or the call is made too early, a blank string will be returned. It is guranteed to return a safe value.
  【返回值说明：component_display_desc - 字符串类型，返回游戏中组件的显示描述。如果未找到组件或调用时机过早，将返回空字符串。保证返回安全值。】

**Example Usage:**
```lua
component_display_desc = weapons.get_weapon_component_display_desc(weapon_component)
```



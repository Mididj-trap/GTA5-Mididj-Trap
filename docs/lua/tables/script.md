# Table: script

Table containing helper functions related to gta scripts.

> 包含GTA脚本相关辅助函数的表。

## Functions (6)

### `register_looped(name, func)`

Registers a function that will be looped as a gta script.

> 注册一个将作为GTA脚本循环执行的函数。

**Example Usage:**
```lua
script.register_looped("nameOfMyLoopedScript", function (script)
     -- sleep until next game frame
     script:yield()

     local ModelHash = joaat("adder")
     if not STREAMING.IS_MODEL_IN_CDIMAGE(ModelHash) then return end
     STREAMING.REQUEST_MODEL(ModelHash) -- Request the model
     while not STREAMING.HAS_MODEL_LOADED(ModelHash) do -- Waits for the model to load
         script:yield()
     end
     local myPed = PLAYER.PLAYER_PED_ID()
     local myCoords = ENTITY.GET_ENTITY_COORDS(myPed, true)
     -- Spawns a networked vehicle on your current coords
     local spawnedVehicle = VEHICLE.CREATE_VEHICLE(ModelHash, myCoords.x, myCoords.y, myCoords.z, ENTITY.GET_ENTITY_HEADING(myPed), true, false)
     -- removes model from game memory as we no longer need it
     STREAMING.SET_MODEL_AS_NO_LONGER_NEEDED(ModelHash)
     -- sleep for 2s
     script:sleep(2000)
     ENTITY.DELETE_ENTITY(spawnedVehicle)
end)
```

- **Parameters:**
  - `name` (string): name of your new looped script
  - `func` (function): function that will be executed in a forever loop.

> **参数说明：**
> - `name` (string): 新循环脚本的名称
> - `func` (function): 将在永久循环中执行的函数

**Example Usage:**
```lua
script.register_looped(name, func)
```

### `run_in_fiber(func)`

Executes a function once inside the fiber pool, you can call natives inside it and yield or sleep.

> 在fiber池中执行一次函数，你可以在其中调用原生函数并进行yield或sleep操作。

**Example Usage:**
```lua
script.run_in_fiber(function (script)
     -- sleep until next game frame
     script:yield()

     local ModelHash = joaat("adder")
     if not STREAMING.IS_MODEL_IN_CDIMAGE(ModelHash) then return end
     STREAMING.REQUEST_MODEL(ModelHash) -- Request the model
     while not STREAMING.HAS_MODEL_LOADED(ModelHash) do -- Waits for the model to load
         script:yield()
     end
     local myPed = PLAYER.PLAYER_PED_ID()
     local myCoords = ENTITY.GET_ENTITY_COORDS(myPed, true)
     -- Spawns a networked vehicle on your current coords
     local spawnedVehicle = VEHICLE.CREATE_VEHICLE(ModelHash, myCoords.x, myCoords.y, myCoords.z, ENTITY.GET_ENTITY_HEADING(myPed), true, false)
     -- removes model from game memory as we no longer need it
     STREAMING.SET_MODEL_AS_NO_LONGER_NEEDED(ModelHash)
     -- sleep for 2s
     script:sleep(2000)
     ENTITY.DELETE_ENTITY(spawnedVehicle)
end)
```

- **Parameters:**
  - `func` (function): function that will be executed once in the fiber pool.

> **参数说明：**
> - `func` (function): 将在fiber池中执行一次的函数

**Example Usage:**
```lua
script.run_in_fiber(func)
```

### `is_active(script_name)`

Returns true if the specified script is currently active/running.

> 如果指定的脚本当前处于活动/运行状态，则返回true。

**Example Usage:**
```lua
local is_freemode_active = script.is_active("freemode")
```

- **Parameters:**
  - `script_name` (string): The name of the script.

> **参数说明：**
> - `script_name` (string): 脚本的名称

**Example Usage:**
```lua
script.is_active(script_name)
```

### `execute_as_script(script_name, func)`

> 在指定的脚本线程中执行一个函数。

- **Parameters:**
  - `script_name` (string): Target script thread.
  - `func` (function): Function that will be executed once in the script thread.

> **参数说明：**
> - `script_name` (string): 目标脚本线程
> - `func` (function): 将在脚本线程中执行一次的函数

**Example Usage:**
```lua
script.execute_as_script(script_name, func)
```

### `start_launcher_script(script_name)`

Tries to start a launcher script. Needs to be called in the fiber pool or a loop.

> 尝试启动一个启动器脚本。需要在fiber池或循环中调用。

**Example Usage:**
```lua
script.run_in_fiber(function()
     script.start_launcher_script("am_hunt_the_beast")
end)
```

- **Parameters:**
  - `script_name` (string): The name of the script.

> **参数说明：**
> - `script_name` (string): 脚本的名称

**Example Usage:**
```lua
script.start_launcher_script(script_name)
```



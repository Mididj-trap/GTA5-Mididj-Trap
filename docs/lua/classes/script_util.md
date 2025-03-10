# Class: script_util

Class for gta script utils, the instance is usually given to you.

<!-- 
这是一个GTA脚本工具类，通常会自动提供给你一个实例。
这个类提供了一些基础的脚本控制功能，如暂停执行和延时等。
-->

## Functions (2)

### `yield()`

Yield execution.

<!-- 
暂停当前脚本的执行。
这个方法用于让出CPU时间片，允许其他脚本继续执行。
-->

**Example Usage:**
```lua
script_util:yield()
```

### `sleep(ms)`

Sleep for the given amount of time, time is in milliseconds.

<!-- 
使脚本休眠指定的时间。
这个方法会暂停脚本执行指定的毫秒数，常用于控制脚本执行速度或实现定时功能。
-->

- **Parameters:**
  - `ms` (integer): The amount of time in milliseconds that we will sleep for.
  <!-- ms参数是一个整数，表示要休眠的毫秒数 -->

**Example Usage:**
```lua
script_util:sleep(ms)
```
<!-- 
使用示例：
script_util:sleep(1000) -- 暂停执行1秒钟
script_util:sleep(500)  -- 暂停执行0.5秒钟
-->



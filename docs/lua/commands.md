# Commands
<!-- 命令列表 -->

All the current commands from the menu are listed below.
<!-- 以下列出了菜单中所有当前可用的命令。 -->

**Example Usage through Lua:**
<!-- **Lua脚本使用示例：** -->

```lua
command.call("spawn", {joaat("adder")})  <!-- 调用命令生成一辆Adder跑车 -->
command.call_player(somePlayerIndex, "spawn", {joaat("adder")})  <!-- 在指定玩家处生成一辆Adder跑车 -->
```

For a complete list of available command functions, please refer to the command table documentation.
<!-- 有关可用命令函数的完整列表，请参阅命令表文档。 -->

## Command Count: 210
<!-- 命令总数：210个 -->

### breakup 
 BREAKUP_KICK_DESC 
<!-- 断开连接踢出玩家 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### breakupcheating 
 BREAKUP_KICK_SHOW_CHEATING_DESC 
<!-- 以作弊为由断开连接踢出所有玩家 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### desync 
 COMPLAINT_KICK_DESC 
<!-- 使目标玩家与会话脱离同步 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### desyncall 
 COMPLAINT_KICK_DESC 
<!-- 使所有玩家与会话脱离同步 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### endkick 
 END_KICK_DESC 
<!-- 强制结束会话踢出玩家 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### hostkick 
 Host kick that only works when host 
<!-- 主机踢出玩家（仅当你是主机时有效） -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### oomkick 
 OOM_KICK_CMD_DESC 
<!-- 内存溢出踢出玩家 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### shkick 
 SCRIPT_HOST_KICK_DESC 
<!-- 脚本主机踢出玩家 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### clearwanted 
 CLEAR_WANTED_LEVEL_DESC 
<!-- 清除玩家的通缉等级 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### clearwantedall 
 CLEAR_WANTED_LEVEL_DESC 
<!-- 清除所有玩家的通缉等级 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### enterint 
 ENTER_INTERIOR_DESC 
Arg Count:  1

### giveammo 
 GIVE_AMMO_DESC 
<!-- 给予玩家弹药 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### giveammoall 
 GIVE_AMMO_DESC 
<!-- 给予所有玩家弹药 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### givearmor 
 GIVE_ARMOR_DESC 
<!-- 给予玩家护甲 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### givearmorall 
 GIVE_ARMOR_DESC 
<!-- 给予所有玩家护甲 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### givehealth 
 GIVE_HEALTH_DESC 
<!-- 给予玩家生命值 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### givehealthall 
 GIVE_HEALTH_DESC 
<!-- 给予所有玩家生命值 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### joinceo 
 JOIN_CEO_DESC 
<!-- 加入CEO组织 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标CEO -->

### copymodel 
 STEAL_IDENTITY_DESC 
<!-- 复制玩家的角色模型 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### copyoutfit 
 STEAL_OUTFIT_DESC 
<!-- 复制玩家的装扮 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### ceokick 
 CEO_KICK_DESC 
<!-- 将玩家踢出CEO组织 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### ceokickall 
 CEO_KICK_DESC 
<!-- 将所有玩家踢出CEO组织 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### explode 
 EXPLODE_PLAYER_DESC 
<!-- 使玩家爆炸 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### explodeall 
 EXPLODE_PLAYER_DESC 
<!-- 使所有玩家爆炸 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### mission 
 FORCE_INTO_MISSION_DESC 
<!-- 强制玩家进入任务 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### missionall 
 FORCE_INTO_MISSION_DESC 
<!-- 强制所有玩家进入任务 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### giveweaps 
 GIVE_WEAPONS_DESC 
<!-- 给予玩家武器 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### giveweapsall 
 GIVE_WEAPONS_ALL_DESC 
<!-- 给予所有玩家武器 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### intkick 
 KICK_FROM_INTERIOR_DESC 
<!-- 将玩家踢出室内空间 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### intkickall 
 KICK_FROM_INTERIOR_DESC 
<!-- 将所有玩家踢出室内空间 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### vehkick 
 VEHICLE_KICK_DESC 
<!-- 将玩家踢出载具 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### vehkickall 
 VEHICLE_KICK_DESC 
<!-- 将所有玩家踢出载具 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### kill 
 KILL_PLAYER_DESC 
<!-- 杀死玩家 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### killall 
 KILL_PLAYER_DESC 
<!-- 杀死所有玩家 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### ragdoll 
 RAGDOLL_PLAYER_DESC 
<!-- 使玩家进入布娃娃状态 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### ragdollall 
 RAGDOLL_PLAYER_DESC 
<!-- 使所有玩家进入布娃娃状态 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### remweaps 
 REMOVE_ALL_WEAPONS_DESC 
<!-- 移除指定玩家的所有武器 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### remweapsall 
 REMOVE_ALL_WEAPONS_DESC 
<!-- 移除所有玩家的所有武器 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### fakeban 
 FAKE_BAN_MESSAGE_DESC 
<!-- 向指定玩家发送虚假的封禁消息 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### fakebanall 
 FAKE_BAN_MESSAGE_DESC 
<!-- 向所有玩家发送虚假的封禁消息 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### sext 
 SEND_SEXT_DESC 
<!-- 向指定玩家发送短信 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### sextall 
 SEND_SEXT_DESC 
<!-- 向所有玩家发送短信 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### apartmenttp 
 TP_TO_APARTMENT_DESC 
<!-- 将指定玩家传送到公寓 -->
Arg Count:  2
<!-- 参数数量：2个，分别指定目标玩家和公寓ID -->

### apartmenttpall 
 TP_TO_APARTMENT_DESC 
<!-- 将所有玩家传送到公寓 -->
Arg Count:  1
<!-- 参数数量：1个，指定公寓ID -->

### interiortp 
 TP_TO_INTERIOR_DESC 
<!-- 将指定玩家传送到室内场景 -->
Arg Count:  2
<!-- 参数数量：2个，分别指定目标玩家和室内场景ID -->

### interiortpall 
 TP_TO_INTERIOR_DESC 
<!-- 将所有玩家传送到室内场景 -->
Arg Count:  1
<!-- 参数数量：1个，指定室内场景ID -->

### warehousetp 
 TP_TO_WAREHOUSE_DESC 
<!-- 将指定玩家传送到仓库 -->
Arg Count:  2
<!-- 参数数量：2个，分别指定目标玩家和仓库ID -->

### warehousetpall 
 TP_TO_WAREHOUSE_DESC 
<!-- 将所有玩家传送到仓库 -->
Arg Count:  1
<!-- 参数数量：1个，指定仓库ID -->

### wanted 
 SET_WANTED_LEVEL_DESC 
<!-- 设置玩家的通缉等级 -->
Arg Count:  2
<!-- 参数数量：2个，分别指定目标玩家和通缉等级 -->

### error 
 SHOW_TRANSACTION_ERROR_DESC 
<!-- 向指定玩家显示交易错误信息 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### errorall 
 SHOW_TRANSACTION_ERROR_DESC 
<!-- 向所有玩家显示交易错误信息 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### tutorial 
 Plays that unskippable cutscene used in the tutorial 
<!-- 播放无法跳过的教程过场动画 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### tutorialall 
 Plays that unskippable cutscene used in the tutorial 
<!-- 为所有玩家播放无法跳过的教程过场动画 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### golf 
 Starts golf 
<!-- 开始高尔夫游戏 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### golfall 
 Starts golf 
<!-- 让所有玩家开始高尔夫游戏 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### flightschool 
 Teleports player to the airport and starts flight school 
<!-- 将玩家传送到机场并开始飞行学校 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### flightschoolall 
 Teleports player to the airport and starts flight school 
<!-- 将所有玩家传送到机场并开始飞行学校 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### darts 
 Starts darts in a Sandy Shores bar 
<!-- 在沙滩酒吧开始飞镖游戏 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### dartsall 
 Starts darts in a Sandy Shores bar 
<!-- 让所有玩家在沙滩酒吧开始飞镖游戏 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### badlands 
 Starts the arcade game Badlands Revenge II in fullscreen 
<!-- 全屏启动街机游戏《荒野复仇2》 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### badlandsall 
 Starts the arcade game Badlands Revenge II in fullscreen 
<!-- 让所有玩家全屏启动街机游戏《荒野复仇2》 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### spacemonkey 
 Starts the arcade game Space Monkey 3 in fullscreen 
<!-- 全屏启动街机游戏《太空猴子3》 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### spacemonkeyall 
 Starts the arcade game Space Monkey 3 in fullscreen 
<!-- 让所有玩家全屏启动街机游戏《太空猴子3》 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### wizard 
 Starts the arcade game The Wizard's Ruin in fullscreen 
<!-- 全屏启动街机游戏《巫师的毁灭》 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### wizardall 
 Starts the arcade game The Wizard's Ruin in fullscreen 
<!-- 让所有玩家全屏启动街机游戏《巫师的毁灭》 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### qub3d 
 Starts the arcade game Qub3D in fullscreen 
<!-- 全屏启动街机游戏《Qub3D》 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### qub3dall 
 Starts the arcade game Qub3D in fullscreen 
<!-- 让所有玩家全屏启动街机游戏《Qub3D》 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### camhedz 
 Starts the arcade game Camhedz in fullscreen 
<!-- 全屏启动街机游戏《Camhedz》 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### camhedzall 
 Starts the arcade game Camhedz in fullscreen 
<!-- 让所有玩家全屏启动街机游戏《Camhedz》 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### ceoraid 
 TRIGGER_CEO_RAID_DESC 
<!-- 触发CEO组织仓库突袭事件 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### ceoraidall 
 TRIGGER_CEO_RAID_DESC 
<!-- 触发所有CEO组织仓库突袭事件 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### beast 
 TURN_INTO_BEAST_DESC 
<!-- 将玩家变成野兽 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### beastall 
 TURN_INTO_BEAST_ALL_DESC 
<!-- 将所有玩家变成野兽 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### bring 
 BRING_DESC 
<!-- 将玩家传送到自己身边 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### bringall 
 BRING_ALL_DESC 
<!-- 将所有玩家传送到自己身边 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### bounty 
 BOUNTY_DESC 
<!-- 设置玩家悬赏金额 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### bountyall 
 BOUNTY_DESC 
<!-- 设置所有玩家悬赏金额 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### anonbounty 
 BOUNTY_ANON_DESC 
<!-- 匿名设置玩家悬赏金额 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### playertp 
 TELEPORT_DESC 
<!-- 传送到指定玩家身边 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### playervehtp 
 TELEPORT_INTO_VEHICLE_DESC 
<!-- 传送到指定玩家的载具中 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### boostveh 
 Boosts their car very fast. 
<!-- 使玩家的载具快速加速 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### boostvehall 
 Boosts their car very fast. 
<!-- 使所有玩家的载具快速加速 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### burstwheels 
 Removes their tyres. 
<!-- 爆破玩家载具的轮胎 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### burstwheelsall 
 Removes their tyres. 
<!-- 爆破所有玩家载具的轮胎 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### closedoors 
 Closes all vehicle doors 
<!-- 关闭玩家载具的所有车门 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### closedoorsall 
 Closes all vehicle doors 
<!-- 关闭所有玩家载具的所有车门 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### downgradeveh 
 Removes all upgrades 
<!-- 移除玩家载具的所有改装 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### downgradevehall 
 Removes all upgrades 
<!-- 移除所有玩家载具的所有改装 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### flip180 
 Rotates their car around 
<!-- 使玩家的载具旋转180度 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### flip180all 
 Rotates their car around 
<!-- 使所有玩家的载具旋转180度 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### flyingveh 
 Catapults their car to  the sky. 
<!-- 将玩家的载具弹射到空中 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### flyingvehall 
 Catapults their car to  the sky. 
<!-- 将所有玩家的载具弹射到空中 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### killengine 
 Breaks their engine 
<!-- 破坏玩家载具的引擎 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### killengineall 
 Breaks their engine 
<!-- 破坏所有玩家载具的引擎 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### lockveh 
 Locks vehicle doors 
<!-- 锁住玩家载具的车门 -->
Arg Count:  1
<!-- 参数数量：1个，指定目标玩家 -->

### lockvehall 
 Locks vehicle doors 
<!-- 锁住所有玩家载具的车门 -->
Arg Count:  0
<!-- 参数数量：0个，影响所有玩家 -->

### opendoors 
// 打开所有车辆的门
 Opens all vehicle doors 
Arg Count:  1

### opendoorsall 
// 打开所有车辆的门
 Opens all vehicle doors 
Arg Count:  0

### rcplayer 
// 控制玩家的载具。为获得最佳效果，请先观察该玩家
 Take control of the player's vehicle. Spectate the player beforehand for best results 
Arg Count:  1

### smashwindows 
// 打碎所有车窗
 Smashes all their windows 
Arg Count:  1

### smashwindowsall 
// 打碎所有车窗
 Smashes all their windows 
Arg Count:  0

### stopveh 
// 停止玩家的载具
 Stops players vehicle 
Arg Count:  1

### stopvehall 
// 停止玩家的载具
 Stops players vehicle 
Arg Count:  0

### unlockveh 
// 解锁载具门
 Unlocks Vehicle Doors 
Arg Count:  1

### unlockvehall 
// 解锁载具门
 Unlocks Vehicle Doors 
Arg Count:  0

### upgradeveh 
// 升级玩家的载具
 Upgrades players vehicle 
Arg Count:  1

### upgradevehall 
// 升级玩家的载具
 Upgrades players vehicle 
Arg Count:  0

### blacktint 
// 使车窗变黑
 Makes their windows black. 
Arg Count:  1

### blacktintall 
// 使车窗变黑
 Makes their windows black. 
Arg Count:  0

### fillammo 
// 补充所有弹药
 Fills all of your ammo. 
Arg Count:  0

### beastjump 
// 获得野兽模式中的跳跃能力
 Allows you to jump as if you were the beast like in the Hunt the Beast event 
Arg Count:  0

### clean 
// 清除玩家身上的水渍和污渍
 Cleans the player of wetness and decals 
Arg Count:  0

### clearwantedlvl 
// 清除通缉等级
 Clears your wanted level 
Arg Count:  0

### fillsnacks 
// 补充零食和护甲
 Refills snacks and armor 
Arg Count:  0

### heal 
// 恢复生命值
 HEAL_DESC 
Arg Count:  0

### repairpv 
// 修理当前使用的个人载具
 Repairs your currently active personal vehicle 
Arg Count:  0

### boatpickup 
// 请求一艘船来接你
 Request a boat pickup 
Arg Count:  0

### ballisticarmor 
// 请求防弹装备，包括防弹衣和迷你枪
 Requests ballistic equipment which includes ballistic armor and an minigun 
Arg Count:  0

### skipcutscene 
// 跳过当前播放的过场动画
 Skips the currently playing cutscene 
Arg Count:  0

### suicide 
// 自杀
 Kills you 
Arg Count:  0

### superjump 
// 超级跳跃
 Jump really high 
Arg Count:  0

### spawn 
// 生成指定型号的载具
 Spawn a vehicle with the specified model 
Arg Count:  1

### spawnmaxed 
// 控制生成的载具是否自动升级到最高级
 Controls whether the vehicle spawned will have its mods maxed out 
Arg Count:  0

### spawnin 
// 控制载具生成后是否自动将玩家传送进去
 Controls whether the player should be set inside the vehicle after it spawns 
Arg Count:  0

### fastquit 
// 快速退出游戏。当你遇到糟糕情况时使用
 We all have bad times sometimes. Close your GTA instant. 
Arg Count:  0

### bringpv 
// 将你的个人载具传送到你附近
 Teleports your PV near you 
Arg Count:  0

### lastvehtp 
// 传送到你最后驾驶的载具中
 Teleports you into your last driven vehicle 
Arg Count:  0

### objectivetp 
// 传送到任务目标点
 Teleports you to your mission objective 
Arg Count:  0

### pvtp 
// 传送到你的个人载具中
 Teleports you into your PV 
Arg Count:  0

### waypointtp 
// 传送到你设置的导航点
 Teleports you to your waypoint 
Arg Count:  0

### hudcolor 
// 自定义HUD颜色
 Override HUD colors 
Arg Count:  0

### cleanloop 
// 保持玩家清洁
 KEEP_PLAYER_CLEAN_DESC 
Arg Count:  0

### fastrespawn 
// 快速重生
 INSTANT_RESPAWN_DESC 
Arg Count:  0

### freecam 
// 自由视角相机
 FREECAM_DESC 
Arg Count:  0

### godmode 
// 无敌模式
 GODMODE_DESC 
Arg Count:  0

### healthregen 
// 生命值自动恢复
 HEALTH_REGEN_DESC 
Arg Count:  0

### invis 
// 隐身
 INVISIBILITY_DESC 
Arg Count:  0

### localvis 
// 本地可见性
 LOCAL_VISIBILITY_DESC 
Arg Count:  0

### mobileradio 
// 移动电台
 MOBILE_RADIO_DESC 
Arg Count:  0

### nocollision 
// 无碰撞
 NO_COLLISION_DESC 
Arg Count:  0

### noragdoll 
// 禁用布娃娃物理效果
 NO_RAGDOLL_DESC 
Arg Count:  0

### walkunder 
// 水下行走
 WALK_UNDERWATER_DESC 
Arg Count:  0

### noclip 
// 穿墙模式
 NO_CLIP_DESC 
Arg Count:  0

### otr 
// 雷达隐身
 OFF_RADAR_DESC 
Arg Count:  0

### ptfx 
// 粒子特效
 PTFX_CMD_DESC 
Arg Count:  0

### fastrun 
// 超级跑步
 SUPER_RUN_DESC 
Arg Count:  0

### superman 
// 超人模式
 SUPERMAN_DESC 
Arg Count:  0

### infoxy 
// 无限氧气
 UNLIMITED_OXYGEN_DESC 
Arg Count:  0

### autotptowp 
// 设置导航点后自动传送
 Automatically teleports you to a waypoint as soon as you set one 
Arg Count:  0

### vcaudio 
// 通过语音聊天播放项目文件夹中的audio.wav文件。波形文件必须使用单声道16位16kHz PCM格式编码。每次加载菜单时都需要重置语音聊天设置才能播放声音
 Plays the audio.wav file in the project folder through voice chat. The wave file must be encoded with a mono 16 bit 16kHz PCM format. You have to reset voice chat settings whenever you load the menu for the sound to play 
Arg Count:  0

### nophone 
// 屏蔽电话和所有来电
 Blocks phone and stops all phone calls 
Arg Count:  0

### noidlekick 
// 防止因挂机而被踢出
 Prevents you from being kicked while idling. 
Arg Count:  0

### blockhoming 
// 防止追踪导弹锁定你的载具
 Prevents homing missiles from locking on to your vehicle 
Arg Count:  0

### mutesiren 
// 禁用紧急车辆的警笛声
 Disables the siren sound of Emergency vehicles 
Arg Count:  0

### driveonwater 
// 允许在水面上驾驶
 Allows you to drive on water 
Arg Count:  0

### vehiclefly 
// 使任何陆地载具能够飞行
 Fly with any land vehicle 
Arg Count:  0

### hornboost 
// 按喇叭时给载具加速
 Boosts your vehicle forward when you sound the horn 
Arg Count:  0

### instantbrake 
// 按刹车时立即停车
 Makes your vehicle stop instantly when you press the brake 
Arg Count:  0

### invisveh 
// 使你的载具隐形
 Makes your car invisible 
Arg Count:  0

### localinvisveh 
// 使你的载具对你自己可见，其他玩家仍然看不到
 Makes your car visible to yourself, other players will still not be able to see it 
Arg Count:  0

### keepengine 
// 离开载具时保持引擎运转
 Keeps the engine running when you exit the vehicle 
Arg Count:  0

### keeponground 
// 使你的载具始终保持四轮着地
 Makes it so your vehicle is always on the ground on all four wheels 
Arg Count:  0

### keepfixed 
// 保持你的载具免受磨损和损坏
 Keeps your vehicle free of wear and tear 
Arg Count:  0

### vehnocollision 
// 与NPC无碰撞类似，但这是全局性的，也会影响NPC
 Same as Ped No Collision, except this is global and also affects Ped 
Arg Count:  0

### driveunder 
// 允许在水下驾驶
 Allows you to drive underwater 
Arg Count:  0

### rainbowpri 
// 为当前载具的主要颜色应用彩虹效果
 Applies active rainbow effect to the current vehicle's primary color 
Arg Count:  0

### rainbowsec 
// 为当前载具的次要颜色应用彩虹效果
 Applies active rainbow effect to the current vehicle's secondary color 
Arg Count:  0

### rainbowneons 
// 为当前载具的霓虹灯应用彩虹效果
 Applies active rainbow effect to the current vehicle's neon color 
Arg Count:  0

### rainbowsmoke 
// 为当前载具的轮胎烟雾应用彩虹效果
 Applies active rainbow effect to the current vehicle's tire smoke color 
Arg Count:  0

### rainbowspeed 
// 设置彩虹漆效果的速度
 Speed of the rainbow paint effect 
Arg Count:  1

### seatbelt 
// 防止你从摩托车上摔下来或者穿过挡风玻璃飞出去
 Prevent you from falling off bikes or flying through the windshield 
Arg Count:  0

### speedometer 
// 启用/禁用载具速度表
 Enable/disable the speedo meter for vehicles. 
Arg Count:  0

### speedometergears 
// 在速度表上显示当前档位
 Adds the current gear the vehicle is in to the speedo meter. 
Arg Count:  0

### speedometerleftside 
// 将速度表文本对齐到左侧而不是右侧
 Aligns the speedo meter text to the left instead of to the right. 
Arg Count:  0

### turnsignals 
// 使用转向灯
 Makes your car invisible 
Arg Count:  0

### vehallweapons 
// 允许在载具中使用所有武器
 Allows you to use all weapons in vehicle 
Arg Count:  0

### vehgodmode 
// 防止你的载具受到任何形式的伤害
 Prevents your vehicle from taking any form of damage 
Arg Count:  0

### vehjump 
// 按手刹时使载具跳跃
 Makes the vehicle jump when you press the handbrake 
Arg Count:  0

### aimbot 
// 自动瞄准并击杀
 Lock on and kill 
Arg Count:  0

### smoothing 
// 控制自动瞄准的灵敏度
 Controls the snappiness of your lock on 
Arg Count:  0

### aimatplayer 
// 如果你不擅长PVP，这个功能适合你
 If you suck at PVP, this is for you 
Arg Count:  0

### aimatnpc 
// 通常用于击杀普通NPC
 Generally kills normal NPCs 
Arg Count:  0

### aimatpolice 
// 锁定警察进行击杀
 Locks onto cops to kill 
Arg Count:  0

### aimatenemy 
// 消灭你的敌人，赢得任务
 Eliminate your enemies, and win your missions 
Arg Count:  0

### alwaysfullammo 
// 每一帧都补充弹药
 Refills your ammo every tick 
Arg Count:  0

### incrdamage 
// 设置你想要的伤害值
 Sets your damage to whatever you want 
Arg Count:  0

### infammo 
// 永远不会用完弹药
 Never run out of ammo again 
Arg Count:  0

### infclip 
// 无需换弹可以一直射击
 Shoot forever without needing to reload 
Arg Count:  0

### infrange 
// 在任何距离都能击杀目标
 Kill anything at any distance 
Arg Count:  0

### norecoil 
// 射击时移除武器后坐力
 Removes weapon recoil when shooting 
Arg Count:  0

### nospread 
// 射击时移除武器扩散
 Removes weapon spread when shooting 
Arg Count:  0

### rapidfire 
// 使你的武器极快速射击
 Makes your weapon fire insanely fast 
Arg Count:  0

### triggerbot 
// 快速自动射击NPC
 Shoots at a ped with fast ease 
Arg Count:  0

### blackhole 
// 生成一个黑洞，吸引周围的NPC和载具
 Spawns a blackhole that picks up all the peds and vehicles in your area 
Arg Count:  0

### blackholeincpeds 
// 将周围的NPC纳入黑洞的破坏范围
 Includes all nearby peds in the blackhole's path of destruction 
Arg Count:  0

### blackholeincvehs 
// 将周围的载具纳入黑洞的破坏范围
 Includes all nearby vehicles in the blackhole's path of destruction 
Arg Count:  0

### autodisarm 
// 自动解除周围NPC的武装
 Disarm nearby pedestrians 
Arg Count:  0

### riotmode 
// 使周围的NPC互相攻击
 Make nearby peds attack each other 
Arg Count:  0

### highalert 
// 不是使命召唤中的技能
 Not the CoD perk 
Arg Count:  0

### pedsignore 
// 使周围的NPC忽视你的行为
 Nearby peds will ignore you and become oblivious to your actions 
Arg Count:  0

### pedrush 
// 使周围的NPC快速移动
 Makes the nearby peds move with a purpose 
Arg Count:  0

### pedrain 
// 使NPC从天而降
 Will pour down and rain nearby peds 
Arg Count:  0

### vehiclerain 
// 使载具从天而降，注意：载具可能会砸死你！
 Drops surrounding vehicles, vehicles can hit and kill you! 
Arg Count:  0

### timeoverride 
// 覆盖当前时间。这是本地效果，其他玩家看不到
 Overrides current time. This is local and cannot be seen by other players 
Arg Count:  0

### weatheroverride 
// 覆盖当前天气。这是本地效果，其他玩家看不到
 Overrides current weather. This is local and cannot be seen by other players 
Arg Count:  0

### orbitaldrone 
// 启用/禁用轨道无人机
 Enables/Disables the orbital drone 
Arg Count:  0

### player_db_auto_update_states 
// 开启此功能将每5分钟自动更新玩家在线状态
 Toggling this feature will automatically update the player online states every 5minutes. 
Arg Count:  0

### vehiclecontrol 
// 启用/禁用载具控制器
 Enables/Disables the vehicle controller. 
Arg Count:  0

### cmdexecutor 
// 切换命令执行器窗口
 Toggles the command executor window 
Arg Count:  0

### resetweaps
// 重置你的武器装备为默认状态
 Resets your weapon loadout to default.
Arg Count: 0
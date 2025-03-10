# Infraction
<!-- 违规类型 -->

All the infraction from the menu are listed below, used as parameter for adding an infraction to a given player, for flagging them as modder.
<!-- 以下列出了菜单中所有可用的违规类型，这些类型可用作参数来为指定玩家添加违规标记，将其标记为作弊者。 -->

**Example Usage:**
<!-- 使用示例： -->
```lua
network.flag_player_as_modder(player_index, infraction.CUSTOM_REASON, "My custom reason on why the player is flagged as a modder")
```

## Infraction Count: 15
<!-- 违规类型总数：15个 -->

### `DESYNC_PROTECTION`
<!-- 不同步保护触发 -->
### `TRIGGERED_ANTICHEAT`
<!-- 触发反作弊系统 -->
### `TRIED_CRASH_PLAYER`
<!-- 尝试崩溃其他玩家 -->
### `TRIED_KICK_PLAYER`
<!-- 尝试踢出其他玩家 -->
### `ATTACKING_WITH_GODMODE`
<!-- 使用无敌模式进行攻击 -->
### `ATTACKING_WITH_INVISIBILITY`
<!-- 使用隐身模式进行攻击 -->
### `ATTACKING_WHEN_HIDDEN_FROM_PLAYER_LIST`
<!-- 在玩家列表中隐藏时进行攻击 -->
### `SPOOFED_DATA`
<!-- 伪造数据 -->
### `SPOOFED_HOST_TOKEN`
<!-- 伪造主机令牌 -->
### `INVALID_PLAYER_MODEL`
<!-- 无效的玩家模型 -->
### `SUPER_JUMP`
<!-- 超级跳跃 -->
### `UNDEAD_OTR`
<!-- 无敌雷达隐匿 -->
### `CUSTOM_REASON`
<!-- 自定义原因 -->
### `CHAT_SPAM`
<!-- 聊天刷屏 -->
### `SENT_MODDER_BEACONS`
<!-- 发送作弊者信标 -->

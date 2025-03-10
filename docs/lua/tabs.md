# Tabs
<!-- 标签页 -->

All the tabs from the menu are listed below, used as parameter for adding gui elements to them.
<!-- 以下列出了菜单中的所有标签页，可用作向其添加GUI元素的参数。 -->

**Example Usage:**
<!-- 使用示例： -->

```lua
missionsTab = gui.get_tab("GUI_TAB_MISSIONS")
missionsTab:add_button("Click me", function ()
    log.info("You clicked!")
end)
```
<!-- 上面的代码展示了如何获取任务标签页并添加一个按钮。当按钮被点击时，会在日志中输出信息。 -->

For a complete list of available gui functions, please refer to the tab class documentation and the gui table documentation.
<!-- 有关可用的GUI函数的完整列表，请参阅标签页类文档和GUI表文档。 -->

## Tab Count: 50
<!-- 标签页总数：50个 -->

### `GUI_TAB_SELF`
### `GUI_TAB_WEAPONS`
### `GUI_TAB_WEAPONS_AMMUNATION`
### `GUI_TAB_TELEPORT`
### `GUI_TAB_CUSTOM_TELEPORT`
### `GUI_TAB_MOBILE`
### `GUI_TAB_OUTFIT_EDITOR`
### `GUI_TAB_OUTFIT_SLOTS`
### `GUI_TAB_ANIMATIONS`
### `GUI_TAB_VEHICLE`
### `GUI_TAB_HANDLING`
### `GUI_TAB_HANDLING_SEARCH`
### `GUI_TAB_HANDLING_SAVED_PROFILE`
### `GUI_TAB_HANDLING_MY_PROFILES`
### `GUI_TAB_HANDLING_CURRENT_PROFILE`
### `GUI_TAB_LSC`
### `GUI_TAB_SPAWN_VEHICLE`
### `GUI_TAB_FUN_VEHICLE`
### `GUI_TAB_WORLD`
### `GUI_TAB_SPAWN_PED`
### `GUI_TAB_SQUAD_SPAWNER`
### `GUI_TAB_CREATOR`
### `GUI_TAB_TRAIN`
### `GUI_TAB_BLACKHOLE`
### `GUI_TAB_MODEL_SWAPPER`
### `GUI_TAB_VFX`
### `GUI_TAB_XML_MAPS`
### `GUI_TAB_NETWORK`
### `GUI_TAB_CHAT`
### `GUI_TAB_NETWORK_CONTROLS`
### `GUI_TAB_MISSIONS`
### `GUI_TAB_SPOOFING`
### `GUI_TAB_PLAYER_DATABASE`
### `GUI_TAB_SESSION_BROWSER`
### `GUI_TAB_STAT_EDITOR`
### `GUI_TAB_SETTINGS`
### `GUI_TAB_LUA_SCRIPTS`
### `GUI_TAB_CONTEXT_MENU_SETTINGS`
### `GUI_TAB_ESP_SETTINGS`
### `GUI_TAB_GTA_CACHE_SETTINGS`
### `GUI_TAB_GUI_SETTINGS`
### `GUI_TAB_HOTKEY_SETTINGS`
### `GUI_TAB_REACTION_SETTINGS`
### `GUI_TAB_PROTECTION_SETTINGS`
### `GUI_TAB_TRANSLATION_SETTINGS`
### `GUI_TAB_PROXY_SETTINGS`
### `GUI_TAB_DEBUG`
### `GUI_TAB_PLAYER`

# utils

### Functions

### world\_to\_screen(pos): [vec2\_t](../types/vec2\_t.md)

| Argument | Type                                       | Description |
| -------- | ------------------------------------------ | ----------- |
| **pos**  | ****[**vec3\_t**](../types/vec3\_t.md)**** | 3D Position |

Returns screen coordinates (vec2\_t) or nil if the position is off screen

```lua
local screen = utils.world_to_screen(pos)
if screen ~= nil then
    -- do something nice with screen.x and/or screen.y
end
```

### find\_netvar(table, prop): number (integer)

| Argument  | Type       | Description |
| --------- | ---------- | ----------- |
| **table** | **string** | Table name  |
| **prop**  | **string** | Prop name   |

Returns the netvar offset, or 0 if failed. Netvars are [here](../netvars.md).

```lua
local m_iHealth = utils.find_netvar("DT_BasePlayer", "m_iHealth")
```

### find\_signature(mod, sig): number (integer)

| Argument | Type       | Description     |
| -------- | ---------- | --------------- |
| **mod**  | **string** | Module name     |
| **sig**  | **string** | Pattern to scan |

Returns the pattern address as an integer (unsigned int), or 0 if failed&#x20;

```lua
local clantag_change_fn_addr = utils.find_signature("engine.dll", "53 56 57 8B DA 8B F9 FF 15")
```

### create\_interface(module\_name, interface\_version): void\*

| Argument               | Type       | Description              |
| ---------------------- | ---------- | ------------------------ |
| **module\_name**       | **string** | Module name              |
| **interface\_version** | **string** | Interface version (name) |

Returns a pointer to the interface, or nil if failed

```lua
local game_movement = utils.create_interface("client.dll", "GameMovement001")
```

### set\_clantag(tag, name)

| Argument | Type       | Description |
| -------- | ---------- | ----------- |
| **tag**  | **string** | Clan-tag    |
| **name** | **string** | Clan name   |

Sets local clan-tag

```lua
utils.set_clantag("leito", "leito")
```

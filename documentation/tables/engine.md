# engine

### Functions

### exec\_client\_cmd(cmd)

Execute Console Command

| Argument | Type       | Description |
| -------- | ---------- | ----------- |
| **cmd**  | **string** | Command     |

```lua
engine.exec_client_cmd("say Hello World!")
```

### get\_net\_channel\_info(): [nci\_t](../types/nci\_t.md)

Returns net channel info ([nci\_t](../types/nci\_t.md)), or nil.

```lua
local nci = engine.get_net_channel_info()
```

### get\_player\_for\_user\_id(userid): number (integer)

| Argument   | Type                 | Description      |
| ---------- | -------------------- | ---------------- |
| **userid** | **number (integer)** | Player's User ID |

Returns player index by their user id (usually used in game events)

```lua
local ent_idx = engine.get_player_for_user_id(userid)
```

### get\_local\_player\_idx(): number (integer)

Returns local player index

```lua
local lp_index = engine.get_local_player_idx()
```

### get\_view\_angles(): [vec3\_t](../types/vec3\_t.md)

Returns the camera angles

```lua
local view_ang = engine.get_view_angles()
```

### set\_view\_angles(angles)

| Argument   | Type                                       | Description |
| ---------- | ------------------------------------------ | ----------- |
| **angles** | ****[**vec3\_t**](../types/vec3\_t.md)**** | View Angles |

Setting the viewangles

```lua
engine.set_view_angles(vec3_t.new(0, 0, 0))
```

### get\_max\_clients(): number (integer)

Returns maximum clients number

```lua
local max_clients = engine.get_max_clients()
```

### is\_in\_game(): boolean

Returns true if in game

```lua
local is_in_game = engine.is_in_game()
```

### is\_connected(): boolean

Returns true if connected

```lua
local is_connected = engine.is_connected()
```

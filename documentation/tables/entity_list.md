# entity\_list

### Functions

### get\_local\_player(): [player\_t](../types/player\_t.md)

Returns local player

```lua
local local_player = entity_list.get_local_player()
```

### get\_player\_by\_index(index): [player\_t](../types/player\_t.md)

Returns player by index

| Argument  | Type             | Description  |
| --------- | ---------------- | ------------ |
| **index** | number (integer) | Player Index |

```lua
local player = entity_list.get_player_by_index(engine.get_local_player_idx())
```

### get\_highest\_entity\_index(): number (integer)

Returns highest entity index

```lua
local highest_ent_idx = entity_list.get_highest_entity_index()
```

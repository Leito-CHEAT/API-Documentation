# weapon\_t

## Based of class: [entity\_t](entity\_t.md)

### Functions

### get\_item\_definition\_index(): number

Returns weapon item definition index

```lua
local weapon = player:get_weapon()
local item_def_idx = weapon:get_item_definition_index()
```

### get\_next\_primary\_attack(): number (float)

Returns weapon next primary attack time

### get\_next\_secondary\_attack(): number (float)

Returns weapon next secondary attack time

### get\_ammo(): number (integer)

Returns weapon ammo count

### get\_postpone\_fire\_time(): number (float)

Returns weapon postpone fire time

### get\_throw\_time(): number (float)

Returns weapon throw time (ONLY for GRENADES!)

### get\_pin\_pulled(): boolean

Returns true if grenade has pin pulled (ONLY for GRENADES!)

### get\_last\_shot\_time(): number (float)

Returns weapon last shot time

### get\_zoom(): number (integer)

Returns weapon zoom level

### get\_burst\_shots\_remaining(): number (integer)

Returns weapon burst shots left (ONLY for BURST WEAPONS!)

### get\_next\_burst\_shot(): number (float)

Returns weapon next burst shot time (ONLY for BURST WEAPONS!)

### get\_accuracy\_penalty(): number (float)

Returns weapon accuracy penalty

### get\_inaccuracy(): number (float)

Returns weapon inaccuracy

### get\_spread(): number (float)

Returns weapon spread

### get\_max\_speed(): number (float)

Returns player's max speed with the weapon

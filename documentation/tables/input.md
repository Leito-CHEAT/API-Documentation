# input

A list with key codes can be found [here](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes).

### Functions

### get\_cursor\_position(): [position\_t](../types/position\_t.md)

Returns cursor [position](../types/position\_t.md)

```lua
local cursor_position = input.get_cursor_position()
```

### key\_preesed(key): boolean

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **key**  | **number (integer)** | Key Code    |

Returns true if the key just got pressed

```lua
local click_pressed = input.key_pressed(1) 
```

### key\_down(key): boolean

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **key**  | **number (integer)** | Key Code    |

Returns true if the key is hold

```lua
local click_hold = input.key_down(1) -- this doesn't return true if it just got pressed 
```

### key\_released(key): boolean

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **key**  | **number (integer)** | Key Code    |

Returns true if the key is not being held anymore

```lua
local click_released = input.key_released(1)
```

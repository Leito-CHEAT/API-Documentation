# color\_t

| Type                           | Name |
| ------------------------------ | ---- |
| number (integer) (range 0-255) | r    |
| number (integer) (range 0-255) | g    |
| number (integer) (range 0-255) | b    |
| number (integer) (range 0-255) | a    |

### Functions

### new(red, green, blue): color\_t

| Type                           | Name  |
| ------------------------------ | ----- |
| number (integer) (range 0-255) | red   |
| number (integer) (range 0-255) | green |
| number (integer) (range 0-255) | blue  |

#### Constructor

```lua
local white_color = color_t.new(255, 255, 255) -- the alpha is automatically 255
```

### new(red, green, blue, alpha): color\_t

| Type                           | Name  |
| ------------------------------ | ----- |
| number (integer) (range 0-255) | red   |
| number (integer) (range 0-255) | green |
| number (integer) (range 0-255) | blue  |
| number (integer) (range 0-255) | alpha |

#### Constructor

```lua
local white_color = color_t.new(255, 255, 255, 255)
```


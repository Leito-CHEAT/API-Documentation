# render

### create\_font(family, height): [font\_t](../types/font\_t.md)

Returns a [font\_t ](../types/font\_t.md)object

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **family** | **string**           | Font Family |
| **height** | **number (integer)** | Font Height |

```lua
local font = render.create_font("tahoma" , 32)
```

### draw\_text(font, pos, text, col)

Draws text with font

| Argument | Type                                               | Description   |
| -------- | -------------------------------------------------- | ------------- |
| **font** | ****[**font\_t**](../types/font\_t.md)****         | Font          |
| **pos**  | ****[**position\_t**](../types/position\_t.md)**** | Text Position |
| **text** | **string**                                         | Text          |
| **col**  | ****[**color\_t**](../types/color\_t.md)****       | Text Color    |

```lua
local font = render.create_font("tahoma" , 32)
render.draw_text(font, position_t.new(20, 20), "TEXT", color_t.new(255, 255, 255))
```

### draw\_text\_outlined(font, pos, text, col)

Draws outlined text with font

| Argument | Type                                               | Description   |
| -------- | -------------------------------------------------- | ------------- |
| **font** | ****[**font\_t**](../types/font\_t.md)****         | Font          |
| **pos**  | ****[**position\_t**](../types/position\_t.md)**** | Text Position |
| **text** | **string**                                         | Text          |
| **col**  | ****[**color\_t**](../types/color\_t.md)****       | Text Color    |

```lua
local font = render.create_font("tahoma" , 32)
render.draw_text_outlined(font, position_t.new(20, 20), "TEXT", color_t.new(255, 255, 255))
```

### text\_size(font, text): [dimensions\_t](../types/dimensions\_t.md)

Returns text size as [dimensions\_t](../types/dimensions\_t.md)

| Argument | Type                                       | Description |
| -------- | ------------------------------------------ | ----------- |
| **font** | ****[**font\_t**](../types/font\_t.md)**** | Font        |
| **text** | **string**                                 | Text        |

```lua
local font = render.create_font("tahoma" , 32)
local text_size = render.text_size(font, "TEXT")
```

### draw\_filled\_rect(pos, dim, col)

Draws a filled rectangle

| Argument | Type                                                   | Description          |
| -------- | ------------------------------------------------------ | -------------------- |
| **pos**  | [**position\_t**](../types/position\_t.md)****         | Rectangle position   |
| **dim**  | ****[**dimensions\_t**](../types/dimensions\_t.md)**** | Rectangle dimensions |
| **col**  | ****[**color\_t**](../types/color\_t.md)****           | Rectangle Color      |

```lua
render.draw_filled_rect(position_t.new(20, 20), dimensions_t.new(100, 30), color_t.new(255,255,255))
```

### draw\_outlined\_rect(pos, dim, col)

Draws an outlined rectangle

| Argument | Type                                                   | Description          |
| -------- | ------------------------------------------------------ | -------------------- |
| **pos**  | [**position\_t**](../types/position\_t.md)****         | Rectangle position   |
| **dim**  | ****[**dimensions\_t**](../types/dimensions\_t.md)**** | Rectangle dimensions |
| **col**  | ****[**color\_t**](../types/color\_t.md)****           | Rectangle Color      |

```lua
render.draw_outlined_rect(position_t.new(20, 20), dimensions_t.new(100, 30), color_t.new(255,255,255))
```

### draw\_multi\_color\_rect(pos, dim, **col\_upr\_left, col\_upr\_right, col\_bot\_right, col\_bot\_left**)

Draws a multi colored rectangle

| Argument            | Type                                                   | Description          |
| ------------------- | ------------------------------------------------------ | -------------------- |
| **pos**             | [**position\_t**](../types/position\_t.md)****         | Rectangle position   |
| **dim**             | ****[**dimensions\_t**](../types/dimensions\_t.md)**** | Rectangle dimensions |
| **col\_upr\_left**  | ****[**color\_t**](../types/color\_t.md)****           | Upper left color     |
| **col\_upr\_right** | [**color\_t**](../types/color\_t.md)****               | Upper right color    |
| **col\_bot\_right** | [**color\_t**](../types/color\_t.md)****               | Bottom right color   |
| **col\_bot\_left**  | [**color\_t**](../types/color\_t.md)****               | Bottom left color    |

```lua
render.draw_multi_color_rect(position_t.new(20, 20), dimensions_t.new(100, 30), color_t.new(255,255,255), color_t.new(0,0,0), color_t.new(255,255,255), color_t.new(0,0,0))
```

### draw\_line(posA, posB, col)

Draws line from position A to position B

| Argument | Type                                               | Description |
| -------- | -------------------------------------------------- | ----------- |
| **posA** | [**position\_t**](../types/position\_t.md)****     | Position A  |
| **posB** | ****[**position\_t**](../types/position\_t.md)**** | Position B  |
| **col**  | ****[**color\_t**](../types/color\_t.md)****       | Line Color  |

```lua
render.draw_line(position_t.new(20, 20), position_t.new(60, 20), color_t.new(255, 255, 255))
```

### draw\_filled\_triangle(posA, posB, posC, col)

Draws a triangle filled with color

| Argument | Type                                               | Description    |
| -------- | -------------------------------------------------- | -------------- |
| **posA** | [**position\_t**](../types/position\_t.md)****     | Position A     |
| **posB** | ****[**position\_t**](../types/position\_t.md)**** | Position B     |
| **posC** | [**position\_t**](../types/position\_t.md)****     | Position C     |
| **col**  | ****[**color\_t**](../types/color\_t.md)****       | Triangle Color |

```lua
render.draw_filled_triangle(position_t.new(5, 5), position_t.new(15, 5), position_t.new(10, 15), color_t.new(255, 255, 255))
```

### draw\_outlined\_triangle(posA, posB, posC, col)

Draws a triangle outlined with color

| Argument | Type                                               | Description    |
| -------- | -------------------------------------------------- | -------------- |
| **posA** | [**position\_t**](../types/position\_t.md)****     | Position A     |
| **posB** | ****[**position\_t**](../types/position\_t.md)**** | Position B     |
| **posC** | [**position\_t**](../types/position\_t.md)****     | Position C     |
| **col**  | ****[**color\_t**](../types/color\_t.md)****       | Triangle Color |

```lua
render.draw_outlined_triangle(position_t.new(5, 5), position_t.new(15, 5), position_t.new(10, 15), color_t.new(255, 255, 255))
```

### draw\_filled\_circle(pos, radius, col)

Draws a circle filled with color

| Argument   | Type                                           | Description   |
| ---------- | ---------------------------------------------- | ------------- |
| **pos**    | [**position\_t**](../types/position\_t.md)**** | Position      |
| **radius** | number (float)                                 | Circle Radius |
| **col**    | ****[**color\_t**](../types/color\_t.md)****   | Circle Color  |

```lua
render.draw_filled_circle(position_t.new(100, 100), 50, color_t.new(255, 255, 255))
```

### draw\_outlined\_circle(pos, radius, col)

Draws a circle outlined with color

| Argument   | Type                                           | Description   |
| ---------- | ---------------------------------------------- | ------------- |
| **pos**    | [**position\_t**](../types/position\_t.md)**** | Position      |
| **radius** | number (float)                                 | Circle Radius |
| **col**    | ****[**color\_t**](../types/color\_t.md)****   | Circle Color  |

```lua
render.draw_outlined_circle(position_t.new(100, 100), 50, color_t.new(255, 255, 255))
```

### draw\_world\_circle(pos, radius, col, filled)

Draws a 3D Circle

| Argument   | Type                                         | Description                |
| ---------- | -------------------------------------------- | -------------------------- |
| **pos**    | ****[**vec3\_t**](../types/vec3\_t.md)****   | Position                   |
| **radius** | **number (float)**                           | Circle Radius              |
| **col**    | ****[**color\_t**](../types/color\_t.md)**** | Circle Color               |
| **filled** | **boolean**                                  | Filled if true or Outlined |

```lua
render.draw_world_circle(vec3_t.new(100, 100, 0), 50, color_t.new(255, 255, 255), true)
```

### get\_screen\_size(): [dimensions\_t](../types/dimensions\_t.md)

Returns screen [dimensions](../types/dimensions\_t.md)

```lua
local screen_size = render.get_screen_size()
```


# ui

### Functions

### add\_check\_box(label, var\_name, def\_value): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument       | Type        | Description    |
| -------------- | ----------- | -------------- |
| **label**      | **string**  | Checkbox label |
| **var\_name**  | **string**  | Variable key   |
| **def\_value** | **boolean** | Default value  |

Creates checkbox in menu

```lua
local checkbox = ui.add_check_box("lua checkbox", "lua_boolean", false)
```

### add\_slider\_int(label, var\_name, def\_value, min\_value, max\_value): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument       | Type                 | Description   |
| -------------- | -------------------- | ------------- |
| **label**      | **string**           | Slider label  |
| **var\_name**  | **string**           | Variable key  |
| **def\_value** | **number (integer)** | Default value |
| **min\_value** | **number (integer)** | Min value     |
| **max\_value** | **number (integer)** | Max value     |

Creates int slider in menu

```lua
local slider_int = ui.add_slider_int("lua int slider", "lua_integer", 50, 0, 100)
```

### add\_slider\_float(label, var\_name, def\_value, min\_value, max\_value): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument       | Type               | Description   |
| -------------- | ------------------ | ------------- |
| **label**      | **string**         | Slider label  |
| **var\_name**  | **string**         | Variable key  |
| **def\_value** | **number (float)** | Default value |
| **min\_value** | **number (float)** | Min value     |
| **max\_value** | **number (float)** | Max value     |

Creates float slider in menu

```lua
local slider_float = ui.add_slider_float("lua float slider", "lua_float", 0.0, 1.0, 0.3)
```

### add\_key\_bind(label, var\_name, def\_key, def\_mode): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument      | Type                 | Description   |
| ------------- | -------------------- | ------------- |
| **label**     | **string**           | Keybind label |
| **var\_name** | **string**           | Variable key  |
| **def\_key**  | **number (integer)** | Default key   |
| **def\_mode** | **number (integer)** | Default mode  |

Creates key bind in menu

```lua
local keybind = ui.add_key_bind("lua key bind", "lua_keybind", 0, 0)
```

### add\_combo\_box(label, var\_name, items, def\_value): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument       | Type                 | Description                          |
| -------------- | -------------------- | ------------------------------------ |
| **label**      | **string**           | Combo label                          |
| **var\_name**  | **string**           | Variable key                         |
| **items**      | **string array**     | Items                                |
| **def\_value** | **number (integer)** | Default item index (starting from 0) |

Creates simple combo box in menu

```lua
local combo = ui.add_combo_box("combo", "lua_combo", { "item1", "item2", "item3" }, 0)
```

### add\_multi\_combo\_box(label, var\_name, items, def\_values): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument        | Type              | Description       |
| --------------- | ----------------- | ----------------- |
| **label**       | **string**        | Multi-Combo label |
| **var\_name**   | **string**        | Variable key      |
| **items**       | **string array**  | Items             |
| **def\_values** | **boolean array** | Default values    |

Creates multi combo box in menu

```lua
local multi_combo = ui.add_multi_combo_box("multi combo", "lua_multi_combo", { "item1", "item2", "item3" }, { false, false, false })
```

### add\_color\_picker(label, var\_name, def\_value): [menu\_item\_t](../types/menu\_item\_t.md)

| Argument       | Type                                         | Description        |
| -------------- | -------------------------------------------- | ------------------ |
| **label**      | **string**                                   | Color picker label |
| **var\_name**  | **string**                                   | Variable key       |
| **def\_value** | ****[**color\_t**](../types/color\_t.md)**** | Default value      |

Creates color picker in menu

```lua
local color_picker = ui.add_color_picker("lua color picker", "lua_color", color_t.new(255, 255, 255, 255))
```

### get\_variable\_reference(var\_name): [VarReference\_t](../types/varreference\_t.md)

| Argument      | Type       | Description  |
| ------------- | ---------- | ------------ |
| **var\_name** | **string** | Variable key |

Gets reference to cheat's variable. Variables can be found [here](../variables.md).

```lua
local antiaim_enabled = ui.get_variable_reference("anti_aim.enable")
client.log(antiaim_enabled:get() and "true" or "false")
```

### get\_cheat\_keybind\_state(keybind\_name): boolean

| Argument          | Type       | Description  |
| ----------------- | ---------- | ------------ |
| **keybind\_name** | **string** | Keybind name |

Gets cheat keybind state. Keybinds can be found [here](../keybinds.md).

```lua
local dt_activated = ui.get_cheat_keybind_state("DT")
```

### is\_menu\_visible(): boolean

Returns true if the menu is currently visible

```lua
local menu_visible = ui.is_menu_visible()
```

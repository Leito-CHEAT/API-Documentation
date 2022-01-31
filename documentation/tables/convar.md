# convar

### Functions

### get\_int(convar\_name): number (integer)

Returns convar integer value

| Argument         | Type       | Description           |
| ---------------- | ---------- | --------------------- |
| **convar\_name** | **string** | Console Variable Name |

```lua
local value = convar.get_int("r_jiggle_bones")
```

### get\_float(convar\_name): number (float)

Returns convar float value

| Argument         | Type       | Description           |
| ---------------- | ---------- | --------------------- |
| **convar\_name** | **string** | Console Variable Name |

```lua
local value = convar.get_float("r_aspectratio")
```

### get\_string(convar\_name): string

Returns convar string value

| Argument         | Type       | Description           |
| ---------------- | ---------- | --------------------- |
| **convar\_name** | **string** | Console Variable Name |

```lua
local value = convar.get_string("sv_skyname")
```

### set\_value(convar\_name, value):

Sets convar value

| Argument         | Type                  | Description                                              |
| ---------------- | --------------------- | -------------------------------------------------------- |
| **convar\_name** | **string**            | Console Variable Name                                    |
| **value**        | boolean/number/string | New Value, can be either a boolean, a number or a string |

```lua
convar.set_value("sv_skyname", "sky");
```

### null\_callback(convar\_name)

Invalidates convar callback (allows you to modify it in-case)

| Argument         | Type       | Description           |
| ---------------- | ---------- | --------------------- |
| **convar\_name** | **string** | Console Variable Name |

```lua
convar.null_callback("sv_skyname")
```


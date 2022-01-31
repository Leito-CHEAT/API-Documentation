# menu\_item\_t

### Functions

### get(): variable type

Returns the variable value (if it's a keybind, returns true or false depending if it's active)

### get(index): boolean

Returns the variable at index value, <mark style="color:red;">**used for multi combo boxes**</mark>

### get\_key(): number (integer)

Returns the key of the keybind, <mark style="color:red;">**only allowed to use for keybinds**</mark>

### get\_key(): number (integer)

Returns the key mode (Disabled, On Hold, etc..) of the keybind, <mark style="color:red;">**only allowed to use for keybinds**</mark>

### set(value)

| Argument  | Type              | Description                                         |
| --------- | ----------------- | --------------------------------------------------- |
| **value** | **variable type** | New value, should be the same type as the variable! |

Sets the variable value

### set(index, value)

| Argument  | Type                 | Description                                         |
| --------- | -------------------- | --------------------------------------------------- |
| **index** | **number (integer)** | Element index                                       |
| **value** | **variable type**    | New value, should be the same type as the variable! |

Sets the variable at index value, <mark style="color:red;">**used for multi combo boxes**</mark>

### set\_key(value)

| Argument  | Type                 | Description |
| --------- | -------------------- | ----------- |
| **value** | **number (integer)** | New key     |

Sets the key, <mark style="color:red;">**only allowed to use for keybinds**</mark>

### set\_key\_mode(value)

| Argument  | Type                 | Description        |
| --------- | -------------------- | ------------------ |
| **value** | **number (integer)** | New key mode (0-3) |

Sets the key mode, <mark style="color:red;">**only allowed to use for keybinds**</mark>

### set\_visible(visible)

| Argument    | Type        | Description     |
| ----------- | ----------- | --------------- |
| **visible** | **boolean** | Item visibility |

Sets the item visibility

### set\_label(label)

| Argument  | Type       | Description    |
| --------- | ---------- | -------------- |
| **label** | **string** | New item label |

Sets the item label

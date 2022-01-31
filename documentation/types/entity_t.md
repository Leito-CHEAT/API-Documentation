# entity\_t

### Offsets

To get prop you need an offset. you can either use [utils.find\_netvar](../tables/utils.md#find\_netvar-table-prop-number-integer) either find it yourself.&#x20;

### Functions

### get\_address(): number

Returns the entity address

```lua
local addr = entity:get_address()
```

### get\_prop\_int(offset): number (integer)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the integer value by offset

### get\_prop\_float(offset): number (float)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the float value by offset

### get\_prop\_short(offset): short

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the number (short) value by offset

### get\_prop\_double(offset): number (double)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the number (double) value by offset

### get\_prop\_bool(offset): boolean

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the boolean value by offset

### get\_prop\_vector(offset): [vec3\_t](vec3\_t.md)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |

Returns the [vec3\_t](vec3\_t.md) value by offset

### set\_prop\_int(offset, value)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |
| **value**  | **number (integer)** | New Value   |

Setting the integer value by offset

### set\_prop\_short(offset, value)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |
| **value**  | **number (short)**   | New Value   |

Setting the number (short) **** value by offset

### set\_prop\_double(offset, value)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |
| **value**  | **number (double)**  | New Value   |

Setting the number (double) **** value by offset

### set\_prop\_float(offset, value)

| Argument | Type             | Description |
| -------- | ---------------- | ----------- |
| offset   | number (integer) | Prop offset |
| value    | number (float)   | New Value   |

Setting the float value by offset

### set\_prop\_bool(offset, value)

| Argument   | Type                 | Description |
| ---------- | -------------------- | ----------- |
| **offset** | **number (integer)** | Prop offset |
| **value**  | **boolean**          | New Value   |

Setting the boolean value by offset

### set\_prop\_vector(offset, value)

| Argument   | Type                              | Description |
| ---------- | --------------------------------- | ----------- |
| **offset** | **number (integer)**              | Prop offset |
| **value**  | ****[**vec3\_t**](vec3\_t.md)**** | New Value   |

Setting the [vec3\_t](vec3\_t.md) value by offset

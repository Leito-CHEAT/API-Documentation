# client

### Functions

### log(text)

Logs a Text into console

| Argument | Type       | Description |
| -------- | ---------- | ----------- |
| **text** | **string** | Log Text    |

```lua
client.log("Hello World!")
```

### add\_callback(callback\_name, callback\_function)

Adds a callback. List of callbacks can be found [here](../callbacks.md).

| Argument               | Type     | Description           |
| ---------------------- | -------- | --------------------- |
| **callback\_name**     | string   | The callback name     |
| **callback\_function** | function | The callback function |

```lua
client.add_callback("on_paint", function()
    render.draw_filled_rect(position_t.new(30, 30), dimensions_t.new(60, 60), color_t.new(255, 255, 255))
end);
```

### get\_username()

Returns the user current name (string).

```lua
local user_name = client.get_username()
```

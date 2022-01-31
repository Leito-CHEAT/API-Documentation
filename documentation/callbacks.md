# callbacks

To add a callback to the list, use [client.add\_callback(callback\_name, callback\_function)](tables/client.md#add\_callback-callback\_name-callback\_function)

### Callback List

* **on\_unload** - when the lua script gets unloaded
* **on\_paint** - used for drawing
* **on\_pre\_prediction(**[**cmd**](types/ucmd\_t.md)**)** - on create move before calling movement and aimbot
* **on\_prediction(**[**cmd**](types/ucmd\_t.md)**)** - on create move after calling movement and aimbot
* **on\_create\_move(**[**cmd**](types/ucmd\_t.md)**)** - at the very end of create move
* Game Events (can be found [here](https://wiki.alliedmods.net/Counter-Strike:\_Global\_Offensive\_Events)); Example: weapon\_zoom([event](types/event\_t.md))

### Example

```lua
client.add_callback("on_paint", function()
    --renderer
end);
```

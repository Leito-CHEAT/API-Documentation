# fakelag

{% hint style="warning" %}
Everything here should be called inside the [`on_pre_prediction`](../callbacks.md) callback or inside the [`on_prediction`](../callbacks.md) callback.&#x20;
{% endhint %}

### Functions

### get\_choked\_commands(): number (integer)

Returns the current choked commands.

```lua
local choked_commands = fakelag.get_choked_commands()
```

### get\_send\_packet(): boolean

Returns the bSendPacket state.

```lua
local bSendPacket = fakelag.get_send_packet()
```

### set\_send\_packet(value)

| Argument  | Type        | Description           |
| --------- | ----------- | --------------------- |
| **value** | **boolean** | New bSendPacket value |

Sets the bSendPacket state.&#x20;

* <mark style="color:red;">**WARNINGS:**</mark>
* This also overrides exploits and fake-duck.&#x20;
* For fake-duck you must choke 14 ticks.
* If you don't send packets while shooting, the bullet may have some delay on the server.

```lua
-- fakelag each 14 ticks
fakelag.set_send_packet(fakelag.get_choked_commands() >= 14)
```

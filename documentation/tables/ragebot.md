# ragebot

{% hint style="warning" %}
Everything here should be called inside the [`on_pre_prediction`](../callbacks.md) callback or inside the [`on_prediction`](../callbacks.md) callback.&#x20;
{% endhint %}

### Functions

### override\_min\_damage(ent\_index, min\_damage)

| Argument        | Type                 | Description                      |
| --------------- | -------------------- | -------------------------------- |
| **ent\_index**  | **number (integer)** | Entity index                     |
| **min\_damage** | **number (integer)** | New minimum damage (range 0-130) |

Overrides minimum damage

```lua
for i=0,65,1 do
    ragebot.override_min_damage(i, 1)
end
```

### override\_hitchance(ent\_index, hitchance)

| Argument       | Type                 | Description                  |
| -------------- | -------------------- | ---------------------------- |
| **ent\_index** | **number (integer)** | Entity index                 |
| **hitchance**  | **number (integer)** | New hit chance (range 0-100) |

Overrides minimum hit chance

```lua
for i=0,65,1 do
    ragebot.override_hitchance(i, 80)
end
```

### override\_hitscan(ent\_index, hitbox, value)

| Argument       | Type                 | Description  |
| -------------- | -------------------- | ------------ |
| **ent\_index** | **number (integer)** | Entity index |
| **hitbox**     | **number (integer)** | Hitbox index |
| **value**      | **boolean**          | Scan value   |

Overrides hit scan

```lua
local SCAN_HEAD = 0
local SCAN_NECK = 1
local SCAN_CHEST = 2
local SCAN_PELVIS = 3
local SCAN_ARMS = 4
local SCAN_LEGS = 5
local SCAN_FEET = 6
                
for i=0,65,1 do
    ragebot.override_hitscan(i, SCAN_HEAD, true)
    ragebot.override_hitscan(i, SCAN_NECK, false)
    ragebot.override_hitscan(i, SCAN_CHEST, false)
    ragebot.override_hitscan(i, SCAN_PELVIS, false)
    ragebot.override_hitscan(i, SCAN_ARMS, false)
    ragebot.override_hitscan(i, SCAN_LEGS, false)
    ragebot.override_hitscan(i, SCAN_FEET, false)
end
```

### override\_head\_scale(ent\_index, percentage)

| Argument       | Type                 | Description            |
| -------------- | -------------------- | ---------------------- |
| **ent\_index** | **number (integer)** | Entity index           |
| **percentage** | **number (integer)** | New head scale (0-100) |

Overrides head point scale

```lua
for i=0,65,1 do
    ragebot.override_head_scale(i, 50)
end
```

### override\_body\_scale(ent\_index, percentage)

| Argument       | Type                 | Description            |
| -------------- | -------------------- | ---------------------- |
| **ent\_index** | **number (integer)** | Entity index           |
| **percentage** | **number (integer)** | New head scale (0-100) |

Overrides body point scale

```lua
for i=0,65,1 do
    ragebot.override_body_scale(i, 50)
end
```

### ignore\_target(ent\_index)

| Argument       | Type                 | Description  |
| -------------- | -------------------- | ------------ |
| **ent\_index** | **number (integer)** | Entity index |

Rage aim-bot will ignore the target

```lua
local entity_index = player:get_index()
ragebot.ignore_target(entity_index)
```

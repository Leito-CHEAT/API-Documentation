# vec2\_t

| Type           | Name |
| -------------- | ---- |
| number (float) | x    |
| number (float) | y    |

### Functions

### new(x, y) : vec2\_t

| Type           | Name |
| -------------- | ---- |
| number (float) | x    |
| number (float) | y    |

#### Constructor

```lua
local vector_2d = vec2_t.new(0, 0)
```

### length(): number (float)

Returns the length of vector

```lua
local vector = vec2_t.new(100, 100)
local vec_length = vector:length()
```

### dist\_to(point): number (float)

Returns the distance between two vectors

| Argument | Type    | Description                                    |
| -------- | ------- | ---------------------------------------------- |
| point    | vec2\_t | The point we want to calculate the distance to |

```lua
local vector = vec2_t.new(100, 100)
local second_vector = vec2_t.new(200, 200)
local dist = vector.dist_to(second_vector)
```

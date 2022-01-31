# vec3\_t

| Type           | Name |
| -------------- | ---- |
| number (float) | x    |
| number (float) | y    |
| number (float) | z    |

### Functions

### new(x, y, z): vec3\_t

| Type           | Name |
| -------------- | ---- |
| number (float) | x    |
| number (float) | y    |
| number (float) | z    |

#### Constructor

```lua
local vector_3d = vec3_t.new(0, 0, 0)
```

### length(): number (float)

Returns the length of vector

```lua
local vector = vec3_t.new(100, 100, 0)
local vec_length = vector:length()
```

### dist\_to(point): number (float)

Returns the distance between two vectors

| Argument | Type    | Description                                    |
| -------- | ------- | ---------------------------------------------- |
| point    | vec3\_t | The point we want to calculate the distance to |

```lua
local vector = vec3_t.new(100, 100, 0)
local second_vector = vec3_t.new(200, 200, 0)
local dist = vector.dist_to(second_vector)
```

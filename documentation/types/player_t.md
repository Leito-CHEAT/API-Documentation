# player\_t

## Based of class: [entity\_t](entity\_t.md)

### Functions

### get\_index(): number

Returns the entity index

```lua
local idx = player:get_index()
```

### is\_dormant(): boolean

Returns true if the entity is dormant

### get\_name(): string

Returns the entity name (it's supposed to be a player)

### get\_team(): number

Returns the entity team number

### is\_alive(): boolean

Returns true if the entity is alive

### get\_eye\_pos(): [vec3\_t](vec3\_t.md)

Returns the entity eye position (also equals to head position)

### get\_aim\_punch(): [vec3\_t](vec3\_t.md)

Returns the entity aim punch angle

### get\_view\_punch(): [vec3\_t](vec3\_t.md)

Returns the entity view punch angle

### get\_velocity(): [vec3\_t](vec3\_t.md)

Returns the entity velocity

### get\_abs\_velocity(): [vec3\_t](vec3\_t.md)

Returns the entity absolute velocity

### get\_origin(): [vec3\_t](vec3\_t.md)

Returns the entity origin

### get\_abs\_origin(): [vec3\_t](vec3\_t.md)

Returns the entity absolute origin

### get\_eye\_angles(): [vec3\_t](vec3\_t.md)

Returns the entity eye angles

### has\_helmet(): boolean

Returns true if entity has helmet

### has\_heavy\_armor(): boolean

Returns true if entity has heavy armor

### is\_scoped(): boolean

Returns true if entity is scoped

### get\_health(): number (integer)

Returns entity health

### get\_weapon(): [weapon\_t](weapon\_t.md)

Returns the entity weapon

# nci\_t

### Flow types

| Value | Outgoing | Incoming |
| ----- | -------- | -------- |
| 0     | Yes      | No       |
| 1     | No       | Yes      |
| 2     | Yes      | Yes      |

### Functions

### get\_name(): string

Returns the channel name

### get\_address(): string

Returns the channel address

### is\_loopback(): boolean

\-

### is\_playback(): boolean

\-

### get\_latency(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns current latency

### get\_avg\_latency(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns current average latency

### get\_avg\_loss(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns current average packet loss \[0-1]

### get\_avg\_choke(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns current average choke \[0-1]

### get\_avg\_data(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns data flow in bytes/sec

### get\_avg\_data(flow): number (float)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns data flow in bytes/sec

### get\_total\_data(flow): number (integer)

| Argument | Type                 | Description |
| -------- | -------------------- | ----------- |
| **flow** | **number (integer)** | Flow type   |

Returns total flow in/out in bytes/sec

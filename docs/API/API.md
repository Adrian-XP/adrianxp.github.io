---
title: API
---

The Hub acts as a middle node in the project. It receives messages from the chain, sends messages when needed, and passes messages to the other subsystems.


## Team Members
| **Individual** | **No.**|
|----------------|--------|
| Sam B          | 1      |
| Adrian P (Me)  | 2      |
| Andrew I       | 3      |
| Jacob D        | 4      |
| Sam M          | 5      |
| Mo A           | 6      |


# Messages That Are Directed to The Hub

## Message Type 12 - Request Subsystem Status 

| **Byte** | **Variable Name** | **Variable Type** | **Min** | **Max** |
|----------|-------------------|-------------------|---------|---------|
| 1        | message_type      | uni8_t            | 12      | 12      |
| 2        | subsystem_number  | uni8_t            | 0       | 15      |
| 3        | request_code      | uni8_t            | 0       | 5       |

- Purpose:
  - Requests status from the hub
- Behavior:
  - If subsystem_number = 3 → process
  - Otherwise → forward message


## Message Type 20 - Hub Command Message 

| **Byte** | **Variable Name** | **Variable Type** | **Min** | **Max** |
|----------|-------------------|-------------------|---------|---------|
| 1        | message_type      | uni8_t            | 20      | 20      |
| 2        | subsystem_number  | uni8_t            | 0       | 15      |
| 3        | command_code      | uni8_t            | 0       | 10      |
| 4        | command_code      | int8_t            | -100    | 100     |

- Purpose:
  - Send control commands to the hub
- Behavior:
  - Execute the command if addressed to the hub
  - Ignore invalid values



# Messages Sent by The Hub

## Message Type 2 - Status Response

| **Byte** | **Variable Name** | **Variable Type** | **Min** | **Max** |
|----------|-------------------|-------------------|---------|---------|
| 1        | message_type      | uni8_t            | 2       | 2       |
| 2        | subsystem_number  | uni8_t            | 3       | 3       |
| 3        | status_code       | uni8_t            | 0       | 10      |
| 4        | data_value        | int8_t            | -100    | 100     |

- Purpose:
  - Send status data back to the controller


## Message Type 14 - Error Message

| **Byte** | **Variable Name** | **Variable Type** | **Min** | **Max** |
|----------|-------------------|-------------------|---------|---------|
| 1        | message_type      | uni8_t            | 14      | 14      |
| 2        | subsystem_number  | uni8_t            | 3       | 3       |
| 3        | error_code        | int8_t            | 0       | 10      |
| 4        | sensor_id         | uni8_t            | 0       | 15      |

- Purpose:
  - Report errors to the controller or the team


















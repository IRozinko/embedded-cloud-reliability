# Device State Model — Draft

## Core states

| State | Meaning | Key risks |
|---|---|---|
| Provisioned | Device registered but not active | Wrong identity, duplicate registration |
| Online | Device is connected and sending data | False online status, stale heartbeat |
| Offline | Device is not reachable | Missing alert, delayed support response |
| Updating | OTA update in progress | Interrupted update, bricked device |
| Degraded | Device works partially | User impact hidden by generic online status |
| Failed | Device cannot perform expected function | Poor diagnostics, unclear ownership |
| Retired | Device removed from active use | Data leakage, stale configuration |

## Design questions

- Who owns each state transition?
- What evidence confirms the state?
- What does support see?
- What does the user see?
- What telemetry proves the state?
- What alert fires when the state is wrong?

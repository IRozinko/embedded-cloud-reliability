# Telemetry Failure Modes

## Device-side failures

- Device does not send telemetry
- Device sends stale telemetry
- Device clock is wrong
- Device sends invalid schema
- Device sends duplicated events

## Transport failures

- Network interruption
- Message ordering mismatch
- Retry storm
- Broker/queue backpressure
- Payload truncation or serialization issue

## Cloud-side failures

- Ingestion rejects valid data
- Invalid data is accepted silently
- Data is stored but not visible in dashboards
- Alerts do not fire for missing telemetry
- Support tools show outdated state

## Operational risks

- Field failure is invisible
- Device appears healthy while user impact exists
- Rollout issue is detected too late
- Support cannot distinguish device, network and backend failure

## Controls

- Heartbeat and last-seen timestamp
- Schema validation
- Dead-letter queue
- Missing-data alerts
- Device state dashboard
- Replay and diagnostic tooling

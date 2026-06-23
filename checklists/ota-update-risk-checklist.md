# OTA Update Risk Checklist

## Pre-update

- [ ] Device compatibility is verified
- [ ] Firmware version is known
- [ ] Battery/power constraints are considered
- [ ] Network failure behavior is defined
- [ ] Update package integrity is validated

## Update process

- [ ] Partial download is handled
- [ ] Interrupted update is recoverable
- [ ] Rollback path exists
- [ ] Device remains identifiable during update
- [ ] Update progress is observable

## Post-update

- [ ] Device reports new version
- [ ] Health check confirms expected behavior
- [ ] Telemetry confirms rollout health
- [ ] Support can identify failed devices
- [ ] Rollout can be paused or rolled back

## Rollout strategy

- [ ] Canary rollout exists
- [ ] Failure threshold is defined
- [ ] Segment-based rollout is possible
- [ ] Field failures are tracked

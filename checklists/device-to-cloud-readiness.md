# Device-to-Cloud Readiness Checklist

## Device / firmware

- [ ] Device state model is documented
- [ ] Firmware version is reported
- [ ] Clock drift is handled
- [ ] Offline mode is defined
- [ ] OTA rollback path exists

## Communication

- [ ] Message format is versioned
- [ ] Retry behavior is idempotent
- [ ] Network failure is simulated
- [ ] Duplicate messages are handled

## Cloud / backend

- [ ] Ingestion path is observable
- [ ] Queue backpressure is handled
- [ ] Data validation exists
- [ ] Device identity is authenticated

## Operations

- [ ] Support can inspect device state
- [ ] Alerts map to real user/device impact
- [ ] Incident runbooks exist
- [ ] Field failure patterns are tracked

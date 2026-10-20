# Aurora Release Notes

## v2.4.0 (pending publication)

### Added
- Telemetry batching window reduced from 60s to 15s (AUR-1142)
- New /status endpoint reporting per-region latency (AUR-1130)

### Fixed
- Connection pool exhaustion under burst load (AUR-1109)
- Timezone drift in the nightly archiver (AUR-987)

### Upgrade notes
- Migration 0042 must be applied before the new /status endpoint is enabled

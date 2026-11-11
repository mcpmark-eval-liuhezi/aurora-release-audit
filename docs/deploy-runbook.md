# Aurora Deploy Runbook — v2.4.0

## Pre-flight
1. Confirm migration 0042 has been applied on all shards
2. Freeze autoscaling at a minimum of 4 instances
3. Page on-call if error-budget burn exceeds 2%

## Deploy
- aurora deploy --release v2.4.0 --strategy rolling

## Rollback
- aurora rollback --to v2.3.9
- Dashboard must return to green within 90 seconds

# recon-data (Clark Hyundai)

Data repo powering our Internal / Used Vehicle Recon tracker.

## Key idea
- `data/current/*.csv` = what the app loads (fast)
- `data/history/*` = optional snapshots + events (audit trail)

## Files
- data/current/vehicles.csv : one row per recon unit (inventory)
- data/current/tasks.csv    : recon checklist layer (detail/QC/photos/listing)
- data/current/people.csv   : code → name mapping (LB, CW, CS, etc.)
- manifests/latest.json     : tells the app which files are “current”
- config/*.json             : stage definitions + thresholds

## Privacy
This repo should NOT contain:
- Retail customer names

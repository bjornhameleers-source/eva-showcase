# Production Wall-Clock Acceptance — 300 Seconds

**Date:** 5 August 2026  
**Classification:** Acceptance  
**Result:** PASS

## Mission

This mission tested EVA’s canonical headless presence wiring for at least
300 seconds of real elapsed time.

The run used:

- the production system clock;
- the canonical runtime lifecycle;
- the normal production presence interval;
- an isolated fresh state root;
- no owner input;
- no simulated time;
- no accelerated clock;
- no cockpit or sensory I/O.

## Results

| Measure | Result |
|---|---:|
| Real elapsed time | 300.042689 seconds |
| Presence callbacks | 299 |
| Maximum active presence threads | 1 |
| Lingering presence threads after shutdown | 0 |
| Model calls | 0 |
| Background thread errors | 0 |
| Unhandled exceptions | 0 |
| Clean shutdown | PASS |
| Final presence state | STOPPED |
| Repository unchanged | PASS |

## Lifecycle

```text
STARTING
→ AWAKE
→ STOPPING
→ STOPPED

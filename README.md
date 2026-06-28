# qcp-lib-java

QCP java binding — TLB semantic delivery for 5G/6G gaming

## Features

- TLB (Time-Latency Bounded) semantic delivery
- REALTIME / CRITICAL / BATCH stream semantics
- Multi-Path (WiFi + 5G Race / Fallback)
- Recovery Policy on-demand (Fast NACK, Network Coding, ARQ)
- Zero-Copy Ring Buffer + Lock-Free queues

## Protocol

QCP 2.0:
- REALTIME: latest state wins, no recovery
- CRITICAL: bounded ARQ within deadline (Fast NACK)
- Recovery: Multi-Path > Fast NACK > Network Coding > ARQ

## License

MIT License

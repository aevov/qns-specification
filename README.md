# QNS Protocol Specification

**Quantum Name Service (QNS)** — A decentralized, quantum-secured domain system for Web 5.

## Overview

QNS resolves `.q` domains to Content-Identified Pointers (CIPs) through a globally distributed network of 200+ Points of Presence. Unlike traditional DNS, QNS provides:

- ⚡ **Instant propagation** — Seconds, not 24-48 hours
- 🔒 **Quantum-secure** — Post-quantum cryptography via ACL 3.0
- 🌐 **Censorship-resistant** — No central authority
- 💰 **Developer-friendly pricing** — From $9.99/year

## Documentation

| Document | Description |
|----------|-------------|
| [SPECIFICATION.md](SPECIFICATION.md) | Full protocol specification |
| [QNS-Protocol-Specification-v1.0.pdf](QNS-Protocol-Specification-v1.0.pdf) | PDF version for distribution |

## Quick Start

### Register a Domain

```bash
curl -X POST https://qns.cr8os.cloud/v1/register \
  -H "Content-Type: application/json" \
  -d '{"domain": "myapp.q"}'
```

### Resolve a Domain

```bash
curl https://qns.cr8os.cloud/v1/resolve/myapp.q
```

### JavaScript SDK

```javascript
import { QNS } from '@cr8os/qns-sdk';

const qns = new QNS();
const result = await qns.resolve('myapp.q');
console.log(result.cip); // QmXxxx...
```

## Pricing Tiers

Pleaase visit: http://my.quantumcloud.one for updated information.

## Browser Extension

Available for Chrome, Firefox, Edge, and Brave. Enables transparent `.q` domain resolution.

## Standards Track

QNS is pending submission to IETF for standardization as part of the Quantum Web (Web 5) initiative.

## License

This specification is released under [CC BY 4.0](LICENSE).

## Links (coming soon)

- **Cr8OS Cloud**: https://cr8os.cloud
- **QuantumCloud**: https://quantumcloud.one
- **Documentation**: https://docs.qns.cr8os.cloud

---

*© 2026 Cr8OS Cloud. All rights reserved.*

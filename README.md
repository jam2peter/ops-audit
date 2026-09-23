# JamPeter Ops Audit

JamPeter Ops Audit is the **AUDIT** module of the cross-cutting **OBSERVE**
layer in JamPeter Ops Stack.

It answers:

> Is the operational control plane coherent?

The private collector remains in the Laboratório JamPeter infrastructure
repository. This public repository is the sanitized status surface and must not
contain private source URLs, infrastructure addresses, secrets, raw logs or
internal Issue contents.

## OBSERVE

```text
OBSERVE
├── AUDIT   -> JamPeter Ops Audit
├── MONITOR -> JamPeter Ops Monitor
└── ALERT   -> JamPeter Ops Watchdog
```

Audit is distinct from Monitor:

- **Audit** checks workflows, CI, deploy/readback evidence, API capacity and
  tracked blockers.
- **Monitor** checks runtime behavior from metrics.
- **Watchdog** compares sanitized states and decides whether a transition
  warrants notification.

## Public status

Issue #1 is machine-maintained and contains the current sanitized Audit
snapshot used by the public dashboard.

Public dashboard:

https://jampeter.com.br/apps/ops-audit/

## Security

This repository is a public status bus, not the private runtime implementation.
No secret or private infrastructure detail belongs here.

## License

MIT

All infrastructure changes must be documented under `/docs`.

---

## 5. Governance Principles

1. No public exposure without explicit documentation.
2. Every service must have a defined purpose.
3. Every open port must be justified.
4. No unmanaged long-running processes.
5. No plaintext credentials stored in repository.
6. Every architectural change logged with date and reason.

---

## 6. Operating Philosophy

This node is treated as infrastructure, not a toy.

Decisions are logged.
Security is intentional.
Complexity is controlled.
Services are added deliberately.

If it cannot be explained clearly, it should not be deployed.

---

## 7. Roadmap

- Install and configure container runtime
- Define multi-agent isolation strategy
- Implement monitoring and logging
- Define backup policy
- Establish resource limits
- Formalize secret management

---

## 8. Change Control

All changes must include:

- Date
- Description
- Reason
- Security impact (if any)

See `/docs/INFRASTRUCTURE_LOG.md` for detailed history.

---

## 9. Classification

Private internal infrastructure documentation.

# AI Infrastructure Node

Private infrastructure for AI experimentation and controlled automation.

This repository documents the architecture, security model, and operational decisions behind a dedicated Ubuntu-based execution node.

---

## 1. Mission

This system exists to:

- Run AI agents
- Execute automation workflows
- Host long-running compute tasks
- Serve as an isolated experimentation environment

This is not:

- A public production server
- A personal workstation
- A general-purpose development machine

It is a hardened execution environment.

---

## 2. Architecture Summary

### Base System
- Ubuntu LTS
- Minimal installation
- Dedicated role: AI execution node

### Network Model
- Private encrypted mesh networking
- No public inbound exposure
- SSH access restricted to authenticated devices

### Access Control
- ed25519 key-based SSH authentication
- Password login disabled
- Root login disabled

### Identity Separation
Operational accounts are segregated from personal accounts to reduce risk and maintain clean boundaries.

---

## 3. Current State

| Layer | Status |
|-------|--------|
| OS Provisioning | Complete |
| Remote Access Hardening | Complete |
| Container Runtime | Not installed |
| Monitoring | Not implemented |
| Backup Strategy | Not implemented |
| Resource Governance | Not implemented |

System currently functions as a secured base compute layer.

---

## 4. Repository Structure

/docs  
 INFRASTRUCTURE_LOG.md  
 SECURITY_DECISIONS.md  
 NETWORK_MODEL.md  

/scripts  
 provisioning/  
 maintenance/  

/docker  
 compose/  
 images/  

All infrastructure changes must be documented under `/docs`.

---

## 5. Governance Principles

1. No public exposure without explicit documentation.
2. Every service must have a defined purpose.
3. Every open port must be justified.
4. No unmanaged long-running processes.
5. No plaintext credentials stored in the repository.
6. Every architectural change must be logged with date and reason.

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
- Security impact if applicable

See `/docs/INFRASTRUCTURE_LOG.md` for detailed history.

---

## 9. Classification

Private internal infrastructure documentation.

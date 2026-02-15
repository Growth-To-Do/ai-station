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

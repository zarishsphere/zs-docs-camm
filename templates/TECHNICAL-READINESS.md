# Technical Readiness Assessment

> **For:** Organisations advancing from L0 to L1
> **Purpose:** Ensure the technical prerequisites for ZarishSphere deployment are met

---

## Minimum Requirements for L1 Deployment

### Option A: Cloud Deployment (Recommended for NGOs)
- [ ] A free-tier cloud account: Oracle Cloud Free (2x ARM VMs, 24GB RAM), Google Cloud (f1-micro), or Fly.io (750 hrs/month)
- [ ] Ubuntu 22.04 or 24.04 LTS server
- [ ] Docker 29.x installed
- [ ] GitHub account for the focal point
- [ ] Domain name (can use free subdomain from Cloudflare)

### Option B: On-Premise (For facilities with servers)
- [ ] Server: minimum 4 CPUs, 8GB RAM, 100GB SSD
- [ ] Ubuntu 22.04 or 24.04 LTS
- [ ] Docker 29.x installed
- [ ] Network: accessible from health facility devices

### Option C: Raspberry Pi 5 (For offline/low-resource facilities)
- [ ] Raspberry Pi 5 (8GB RAM version)
- [ ] 256GB SD card or SSD via USB
- [ ] Ubuntu Server 24.04 LTS (ARM64)
- [ ] Power supply (stable/solar)
- [ ] Local WiFi or Ethernet for devices to connect to Pi

---

## Device Requirements for Clinical Staff

| Device | Minimum | Recommended |
|--------|---------|-------------|
| Android smartphones (CHW) | Android 10, 2GB RAM | Android 12+, 4GB RAM |
| Android tablets | Android 10, 3GB RAM | Android 12+, 4GB RAM |
| Windows computers | Windows 10, Chrome browser | Windows 11, Chrome latest |
| Linux computers | Ubuntu 20.04+, Chrome browser | Ubuntu 24.04, Chrome |

---

## Connectivity Requirements

| Scenario | Requirement |
|----------|-------------|
| Cloud-hosted ZarishSphere | Staff devices need internet to access system |
| Raspberry Pi (on-site) | Staff devices need local WiFi only; Pi syncs when available |
| Fully offline | Raspberry Pi with local SQLite; no internet required |

---

## Software Prerequisites

- [ ] Docker installed on server: `docker --version` (should show 29.x)
- [ ] GitHub account created for focal point
- [ ] Git installed: `git --version`
- [ ] Chrome browser on clinical devices (latest version)

---

## ZarishSphere Bootstrap Test

Run this on your Ubuntu server to verify it's ready:

```bash
# Test Docker is working
docker run hello-world

# Test internet access
curl -fsSL https://github.com | head -5

# Test disk space (need at least 20GB free)
df -h /

# Test RAM (need at least 4GB)
free -h
```

All tests should complete without errors before proceeding to L1 deployment.

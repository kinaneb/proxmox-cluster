# Proxmox Infrastructure Setup

This repository contains the configuration and setup for a Proxmox infrastructure with the following components:

- **Node 1**: TrueNAS providing 2TB of storage via SMB and NFS.
- **Node 2**: Virtual Machine running WireGuard for VPN access (using Docker Compose).
- **Node 3**:
  - Virtual Machine running Plex Server (using Docker Compose).
  - Virtual Machine running Home Assistant.

## Table of Contents

- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
  - [TrueNAS Setup](#truenas-setup)
  - [WireGuard Setup](#wireguard-setup)
  - [Plex Server Setup](#plex-server-setup)
  - [Home Assistant Setup](#home-assistant-setup)
- [Usage](#usage)
- [Makefile Commands](#makefile-commands)

## Architecture

![Proxmox-Cluster-Architecture](/assets/Proxmox_Cluster.jpg)

## Prerequisites

- Proxmox VE installed on all nodes.
- Debian 12 installed on all VMs.

## Setup Instructions

1. Create a VM on Node 2 with TrueNAS.
2. Install TrueNAS on VM.
3. Configure SMB and NFS shares.
4. Add the storage to the Proxmox cluster.

### WireGuard Setup

1. Create a VM on Node 2 with Debian 12.
2. Install Docker and Docker Compose.
3. Use the provided docker-compose.yml to set up

### Plex Server Setup

1. Create a VM on Node 3 with Debian 12.
2. Install Docker and Docker Compose.
3. Use the provided docker-compose.yml to set up Plex Server.

### Home Assistant Setup

1.  Create another VM on Node 3 with Debian 12.
2.  Install Home Assistant using the official installation guide.

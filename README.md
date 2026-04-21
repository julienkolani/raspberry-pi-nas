# Raspberry Pi NAS

A Network Attached Storage (NAS) system built on Raspberry Pi. The project demonstrates the full setup and configuration of a personal file server accessible over the local network, including disk mounting, Samba or similar file-sharing service configuration, and network access from multiple clients. The `screenshots/` directory contains captures of the running system interface.

## Features

- Personal NAS server running on a Raspberry Pi
- File sharing over the local network
- Accessible from multiple operating systems
- Low-power, always-on storage solution

## Tech Stack

- Raspberry Pi (ARM Linux)
- Samba (SMB/CIFS file sharing)
- Linux (storage and service configuration)

## Setup

Refer to the screenshots in the `screenshots/` directory for a visual walkthrough of the system configuration and interface.

General steps:
1. Flash a Raspberry Pi OS image to an SD card and boot the device.
2. Attach external storage and configure mount points in `/etc/fstab`.
3. Install and configure Samba:
   ```bash
   sudo apt install samba
   sudo nano /etc/samba/smb.conf
   sudo systemctl restart smbd
   ```
4. Access the share from another machine using the Raspberry Pi's local IP address.

## Project Structure

```
screenshots/    # Captures of the running NAS system interface
```

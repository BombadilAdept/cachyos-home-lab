# CachyOS Home Lab

A personal Linux home lab setup documented as part of my self-directed learning journey into IT and cybersecurity.

> **Transparency note:** This setup was built and documented with AI assistance (Claude by Anthropic). I'm an IT student learning Linux from the ground up. This repo is an honest record of what I've configured, understood, and explored, not a showcase of expert-level work.

---

## System specs

| Component | Details |
|-----------|---------|
| Distro | CachyOS (Arch-based, rolling release) |
| CPU | Intel Core i5-4690 |
| GPU | NVIDIA GeForce GTX 970 |
| RAM | 16 GB |
| Primary storage | SSD (btrfs filesystem) |
| Secondary storage | HDD (mounted manually) |

---

## What's configured

### Desktop environment
- **KDE Plasma** on **Wayland** (a modern display protocol that replaces the older X11)
- **Xwayland** for legacy app compatibility (allows older apps built for X11 to run under Wayland)

### Security & networking
- **UFW** (Uncomplicated Firewall) — basic firewall rules configured
- **DNS** set to **Quad9** (privacy-focused, malware-blocking DNS resolver)
- Standard user/root separation following Linux security practices

### Storage & backups
- Filesystem: **btrfs** (a modern Linux filesystem with built-in snapshot support)
- Snapshot tool: **Snapper** — automated system snapshots for rollback capability
- Secondary HDD mounted and configured via `/etc/fstab`

### Gaming (Linux-native setup)
- Steam installed and running under Wayland
- **ProtonGE** (a community-maintained Proton version) for Windows game compatibility
- Tested with: Deep Rock Galactic

### Other
- Printing configured under Wayland
- Browser: Firefox with uBlock Origin

---

## In progress

- [ ] Resize btrfs partition from live environment to make room for Fedora Workstation (dual-boot)
- [ ] Investigate persistent cursor glitch at cold boot
- [ ] Expand security tooling (Wireshark, log analysis)

---

## Learning context

I'm 37, working at a public library in Patagonia, Argentina, and teaching myself IT systems independently after leaving a university program. My current focus is Linux system administration and cybersecurity.

This repo is part of a broader portfolio being built alongside the **Google Cybersecurity Professional Certificate** on Coursera.

Tools and resources I'm using:
- [CachyOS](https://cachyos.org/)
- [Snapper](https://wiki.archlinux.org/title/Snapper)
- [Quad9 DNS](https://www.quad9.net/)
- [TryHackMe](https://tryhackme.com/) *(planned)*

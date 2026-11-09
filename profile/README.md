# Welcome to Conchy OS 🐚

> **An opinionated, minimal, scrolling-first Linux distribution and Desktop Environment built on Void Linux.**

Conchy OS is designed from the ground up for modern hardware, high-DPI/OLED HDR displays, and keyboard-first workflows. It blends the simplicity and raw speed of Void Linux with an integrated, cohesive desktop experience written entirely in Rust.

---

## ⚡ Core Philosophy

- **Scrolling-First (Horizontal Columns):** An infinite horizontal ribbon of columns. No clunky floating window management, no stacking clutter, just natural navigation.
- **Wayland & Rust Native:** Modern, safe, and lightning-fast. All core desktop components speak Wayland natively.
- **Void Linux Foundation:** Systemd-free, ultra-lightweight, blazing-fast boot times, and transactional package management via `xbps`.
- **Modern Hardware & HDR Out-of-the-Box:**
  - True HDR & wide color gamut (`wp_color_management_v1`, BT.2020 / scRGB) tuned for modern OLED panels.
  - Low-latency gaming via `wp_tearing_control_v1` (async page flips) and direct scanout.
  - Stutter-free rendering on Intel Xe, AMD, and Nvidia via `linux-drm-syncobj-v1` (Explicit Sync).
- **Hardened Security & Recovery by Default:**
  - Btrfs subvolumes with automated Snapper rollback snapshots.
  - LUKS2 full disk encryption + TPM2 PIN automatic unlock + Secure Boot.
  - Fast, reliable boots via Limine.

---

## 📂 Ecosystem Repositories

| Repository | Purpose | Language |
| :--- | :--- | :--- |
| [**`conchy-wm`**](https://github.com/conchy-os/conchy-wm) | The scrolling-tiling Wayland compositor (Niri fork with HDR, tearing, and explicit sync) | Rust |
| [**`smithay`**](https://github.com/conchy-os/smithay) | Upstream engine fork powering Conchy with DRM atomic colorop & connector HDR pipelines | Rust |
| [**`conchy-session`**](https://github.com/conchy-os/conchy-wm-session) | Lightweight session orchestrator & process supervisor replacing `systemd --user` on Void | Rust |
| [**`conchy-shell`**](https://github.com/conchy-os/conchy-wm-shell) | Minimalist desktop shell, status bar, OSD, and quick settings | Rust |
| [**`conchy-packages`**](https://github.com/conchy-os/conchy-wm-packages) | Official XBPS package templates and prebuilt binary repository | Shell / C |
| [**`conchy-os`**](https://github.com/conchy-os/conchy-wm-os) | Main distribution repository, live ISO builders, automated installer, and system guides | Shell / Docs |

---

*Crafted with passion for pure, distraction-free computing.*

# MouseShare Official Releases

Official multi-platform release distribution for [MouseShare](https://github.com/rijuann/pointer).

MouseShare enables seamless mouse and keyboard sharing across multiple computers over your local network with sub-millisecond latency.

---

## Downloads (v1.0.0)

### 🪟 Windows (x64)
- **[MouseShare-Setup.msi](https://github.com/rijuann/pointer-release/raw/main/MouseShare-Setup.msi)** (Standard Windows Installer)
  - **SHA-256:** `f42d2a9f0540252f401ea07ff7ed32b6c6e582868abc60f6fe78039bce42e9f8`

### 🐧 Linux (x86_64 / amd64)
- **[mouseshare_1.0.0_amd64.deb](https://github.com/rijuann/pointer-release/raw/main/mouseshare_1.0.0_amd64.deb)** (Debian / Ubuntu / Linux Mint)
  - **Install:** `sudo dpkg -i mouseshare_1.0.0_amd64.deb`
  - **SHA-256:** `8f50436998ecdaf4366159649bc41b8ffb79eb5d384fa234832d6905deedb93e`
- **[mouseshare-linux-x86_64.tar.gz](https://github.com/rijuann/pointer-release/raw/main/mouseshare-linux-x86_64.tar.gz)** (Standalone Tarball - Arch, Fedora, openSUSE)
  - **Install:** `tar -xzf mouseshare-linux-x86_64.tar.gz && cd mouseshare-linux-x86_64 && sudo ./install.sh`
  - **SHA-256:** `32c525b97fb65c0e24d5a1b99efcf2e51104b67d831cdf4edb53da4c3c6cab76`

### 🍏 macOS (Universal: Apple Silicon M1/M2/M3 + Intel)
- **[MouseShare-macOS-Universal.dmg](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.dmg)** (Drag & Drop Disk Image)
  - **Install:** Open DMG and drag `MouseShare.app` to `/Applications`
  - **SHA-256:** `5483eec47c43371428c8ff9d240f44aba97f51567c42d40ad1c4f49c41acc570`
- **[MouseShare-macOS-Universal.app.tar.gz](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.app.tar.gz)** (Portable App Bundle)
  - **SHA-256:** `04d2913bb32c1d623b38e1b8c41cf0e4088a3ede97abd4cca3b471a81819ad57`

---

## Quick Installation & Setup

### Linux uinput Permissions
MouseShare requires access to `/dev/uinput` to emulate mouse events. The installer automatically configures `/etc/udev/rules.d/99-mouseshare.rules`. Ensure your user belongs to the `input` group:
```bash
sudo usermod -a -G input $USER
```
Log out and log back in for permissions to take effect.

### macOS Accessibility Permissions
On macOS, grant Accessibility permissions to MouseShare when prompted:
`System Settings` → `Privacy & Security` → `Accessibility` → Enable `MouseShare`.

# 🚀 Samsung Exynos 9810 Custom Kernel for Android 17 (LineageOS 24.0)

<p align="center">
  <img src="https://img.shields.io/badge/Device-Samsung%20Galaxy%20Note%209%20(crownlte)-blue?style=for-the-badge&logo=samsung" alt="Device">
  <img src="https://img.shields.io/badge/Kernel-Linux%204.9.337%20LTS-orange?style=for-the-badge&logo=linux" alt="Kernel">
  <img src="https://img.shields.io/badge/Android-17%20(LineageOS%2024.0)-green?style=for-the-badge&logo=android" alt="Android">
  <img src="https://img.shields.io/badge/Root-KernelSU%20v3.3.1%20%2B%20SuSFS%20v2.3.0-red?style=for-the-badge" alt="KernelSU">
  <img src="https://img.shields.io/badge/Build-GitHub%20Actions%20CI-purple?style=for-the-badge&logo=githubactions" alt="Build">
</p>

---

## 📖 Overview

This repository hosts the **Linux 4.9.337 LTS** unified kernel source tree for **Samsung Exynos 9810** devices, tailored and optimized specifically for **LineageOS 24.0 (Android 17)**. 

It comes pre-integrated with native **KernelSU (v3.3.1)** and **SuSFS (v2.3.0)**, compiled entirely in the cloud via **GitHub Actions** using Google's official prebuilt Clang toolchain.

---

## ✨ Key Features

- 🔥 **Android 17 Ready:** Full compatibility with LineageOS 24.0 (`lineage-24.0-xxksu3-susfs2`).
- 🛡️ **Native KernelSU v3.3.1:** Integrated at the kernel level with 91 Linux 4.9 backport commits (no fragile userspace workarounds).
- 🥷 **SuSFS v2.3.0 (SuperUser Secure FileSystem):** Kernel-level hiding of root mounts and overlays, bypassing Play Integrity (`MEETS_DEVICE_INTEGRITY`) and strict banking apps out-of-the-box.
- 📞 **Samsung IMS / VoLTE & VoWiFi:** Fully functional across cellular networks.
- ⚡ **Google Clang 9.0.8 (`clang-r365631c`) + GCC 4.9 Binutils:** Compiled with Google's Android 11 release toolchain for peak stability and battery efficiency.
- ☁️ **GitHub Actions CI/CD:** Fully automated cloud build workflow with flashable artifact generation.

---

## 📱 Supported Devices

| Codename | Device Name | Chipset | Status |
| :--- | :--- | :--- | :--- |
| **`crownlte`** | Samsung Galaxy Note 9 (SM-N960F/DS/N) | Exynos 9810 | ✅ **Tested & Daily Driven** |
| **`starlte`** | Samsung Galaxy S9 (SM-G960F) | Exynos 9810 | 🔄 Compatible |
| **`star2lte`** | Samsung Galaxy S9+ (SM-G965F) | Exynos 9810 | 🔄 Compatible |

---

## 🛠️ Build Workflow

Compilation is performed automatically in the cloud via GitHub Actions.

### Trigger Build:
1. Navigate to the **[Actions Tab](https://github.com/godev777/android_kernel_samsung_exynos9810/actions)**.
2. Select **`Build Kernel Note 9`**.
3. Click **Run workflow** on the `lineage-24.0-xxksu3-susfs2` branch.
4. Once completed, download the **`Crownlte-KernelSU-Kernel`** artifact zip containing:
   - `Image-exynos9810` (arm64 zImage)
   - `dt.img` (Device Tree Blob)
   - `Image.samsung`

---

## ⚡ Quick Flash Guide

1. Extract `Crownlte-KernelSU-Kernel.zip`.
2. Repack into `boot.img` with LineageOS 24 ramdisk using `magiskboot` or custom unpacker.
3. Flash via ADB Root or Recovery:
   ```bash
   adb push boot.img /sdcard/boot.img
   adb shell "dd if=/sdcard/boot.img of=/dev/block/by-name/BOOT bs=4096 && sync"
   adb reboot
   ```
4. Install the official **[KernelSU Manager](https://github.com/tiann/KernelSU/releases)** APK.

---

## 🤝 Credits & Acknowledgements

- **[krazey90](https://github.com/krazey90)** & **[gavdoc38](https://github.com/gavdoc38)** - Exynos 9810 Android 17 bringup & IMS port
- **[tiann](https://github.com/tiann)** - KernelSU creator
- **[simonpunk](https://gitlab.com/simonpunk)** - SuSFS creator
- **[LineageOS Project](https://github.com/LineageOS)** - Open-source Android foundation
- **Google** - AOSP Clang toolchain

---

<p align="center">
  <i>Maintained with ❤️ by <b>godev777</b></i>
</p>

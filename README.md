<p align="center">
  <img src="media/banners/banner-animated.gif" alt="OmniGPU — one GPU control center built for gaming" width="100%">
</p>

<h1 align="center">OmniGPU</h1>

<p align="center">
  <strong>One gaming GPU control center for NVIDIA, AMD and Intel — driver care, profiles, capability-gated tuning, monitoring and displays.</strong>
</p>

<p align="center">
  Part of the <a href="#the-omnivex-suite">OmniVex</a> suite.
</p>

<p align="center">
  <a href="https://www.patreon.com/TheOmniGrid"><img alt="Get it on Patreon" src="https://img.shields.io/badge/Get%20it%20on-Patreon-FF424D?style=for-the-badge&logo=patreon&logoColor=white"></a>
  &nbsp;
  <a href="https://ko-fi.com/theomnigrid"><img alt="Get it on Ko-fi" src="https://img.shields.io/badge/Get%20it%20on-Ko--fi-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white"></a>
</p>

<p align="center">
  <img alt="Version 1.0.0" src="https://img.shields.io/badge/version-1.0.0-8b5cf6?style=flat-square">
  <img alt="Windows 10 and 11 x64" src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-24c8ff?style=flat-square&logo=windows&logoColor=white">
  <img alt="NVIDIA, AMD and Intel" src="https://img.shields.io/badge/GPU-NVIDIA%20%C2%B7%20AMD%20%C2%B7%20Intel-a99cff?style=flat-square">
  <img alt="Five interface languages" src="https://img.shields.io/badge/languages-EN%20%C2%B7%20DE%20%C2%B7%20ES%20%C2%B7%20FR%20%C2%B7%20RO-8b5cf6?style=flat-square">
  <img alt="No telemetry" src="https://img.shields.io/badge/telemetry-none-39e59f?style=flat-square">
  <img alt="Free donationware" src="https://img.shields.io/badge/donationware-free%20%C2%B7%20no%20ads-251e3f?style=flat-square">
</p>

<!-- Quick navigation. The accent chip introduces the product; the remaining
     chips jump to the most useful public sections and documents. -->
<p align="center">
  <a href="#one-control-center-built-around-games"><img alt="Explore OmniGPU" src="https://img.shields.io/badge/Explore%20OmniGPU-8B5CF6?style=for-the-badge"></a>
  <a href="FEATURES.md"><img alt="Features" src="https://img.shields.io/badge/Features-251E3F?style=for-the-badge"></a>
  <a href="#real-application-captures"><img alt="Screenshots" src="https://img.shields.io/badge/Screenshots-251E3F?style=for-the-badge"></a>
  <a href="COMPATIBILITY.md"><img alt="Compatibility" src="https://img.shields.io/badge/Compatibility-251E3F?style=for-the-badge"></a>
  <a href="#safety-is-part-of-the-feature-set"><img alt="Safety" src="https://img.shields.io/badge/Safety-251E3F?style=for-the-badge"></a>
  <a href="STATUS.md"><img alt="Release status" src="https://img.shields.io/badge/Status-251E3F?style=for-the-badge"></a>
  <a href="FAQ.md"><img alt="FAQ" src="https://img.shields.io/badge/FAQ-251E3F?style=for-the-badge"></a>
  <a href="CHANGELOG.md"><img alt="Changelog" src="https://img.shields.io/badge/Changelog-251E3F?style=for-the-badge"></a>
</p>

---

## One control center, built around games

OmniGPU brings the workflows normally spread across driver cleanup tools, NVIDIA profile editors, AMD tuning utilities, Windows Driver Store management and overclocking dashboards into one restrained OmniVex interface.

It detects the exact physical adapter first, then exposes only the controls reported by the installed official vendor runtime. Unsupported, ambiguous, virtual, remote and protected adapters remain unavailable for mutation instead of receiving guessed settings.

> **This is a documentation and media repository.** It intentionally contains no OmniGPU source code, application binary, installer or direct download. Use only the destinations in [Official links](LINKS.md); mirrors and repacks are unofficial.

## What OmniGPU brings together

| Area | What you get |
|---|---|
| **Driver care** | Exact-adapter discovery, reviewed Windows-serviced driver installation, known-good package vault and rollback-aware maintenance |
| **Driver reset** | A DDU-style clean-reset plan with restore point, backup, Safe Mode guidance, exact residual cleanup and restart/shutdown/manual completion |
| **Driver Store** | Online/offline package inventory, smart cleanup selection, add/install/remove/export and guarded force removal in an advanced workspace |
| **Profile Inspector** | NVIDIA DRS profiles, applications, friendly and raw values, favorites, search, purpose categories, defaults, `.nip` exchange and verified history |
| **Performance tuning** | Driver-reported NVIDIA, AMD and Intel clock, voltage, power, thermal and fan controls protected by an explicit session-only OC mode |
| **Monitoring & OSD** | Live telemetry, PresentMon FPS/1% low/frametime, graphs, CSV logging, benchmarks, screenshots and configurable in-game overlays |
| **Game automation** | Per-game performance and fan presets with apply, exit restore, interrupted-session recovery and lightweight background detection |
| **Displays & latency** | Resolution/refresh, HDR, exact-output DDC/CI brightness, standby-memory cleanup and timer-resolution controls |

The [complete feature list](FEATURES.md) documents the full surface and its capability boundaries.

## Real application captures

<p align="center">
  <img src="media/banners/omnigpu-feature-collage-1600x900.jpg" alt="OmniGPU dashboard, Profile Inspector and monitoring views" width="100%">
</p>

| Gaming dashboard | Profile Inspector |
|---|---|
| ![OmniGPU gaming dashboard](media/screenshots/omnigpu-1.0.0-home.jpg) | ![OmniGPU Profile Inspector](media/screenshots/omnigpu-1.0.0-profile-inspector.jpg) |

| Performance tuning | Live monitoring |
|---|---|
| ![OmniGPU performance tuning](media/screenshots/omnigpu-1.0.0-performance-tuning.jpg) | ![OmniGPU live monitoring](media/screenshots/omnigpu-1.0.0-monitoring.jpg) |

| Safe driver reset | Displays and HDR |
|---|---|
| ![OmniGPU safe driver reset](media/screenshots/omnigpu-1.0.0-driver-reset.jpg) | ![OmniGPU displays and HDR controls](media/screenshots/omnigpu-1.0.0-displays-hdr.jpg) |

These are real 1.0.0 application captures. Hardware-specific values and controls vary by GPU, driver, firmware, display and OEM policy.

## Safety is part of the feature set

- The normal interface runs without elevation; privileged mutations use a separate one-shot UAC broker.
- Every hardware write is bound to the selected PCI adapter, current driver and a short-lived explicit authorization.
- Driver cleanup, tuning, profile and display workflows use preview, confirmation, backup/read-back and rollback contracts.
- Unknown and unsupported states fail closed rather than falling back to generic clocks, voltages, paths or device guesses.
- OmniGPU has no automatic application updater, silent installer, advertising SDK or usage analytics service.

GPU tuning and driver removal can still cause instability, display loss, restart requirements or data loss. Keep important work backed up and use conservative settings.

## Donationware, without a paywall

OmniGPU is donationware: free to use, with no required payment, no advertisements and no paid feature tier. If it saves you time, an optional Ko-fi or Patreon contribution helps fund hardware validation, compatibility work and continued development.

<p align="center">
  <a href="https://www.patreon.com/TheOmniGrid"><img src="media/buttons/support-on-patreon.svg" height="64" alt="Support OmniGPU on Patreon"></a>
  &nbsp;&nbsp;
  <a href="https://ko-fi.com/theomnigrid"><img src="media/buttons/support-on-kofi.svg" height="64" alt="Support OmniGPU on Ko-fi"></a>
</p>

Donating does not grant source-code, redistribution, resale or trademark rights. Please send other users to the official project page instead of sharing an installer or creating a mirror. Read the [donationware policy](DONATIONWARE.md) and [public materials notice](LICENSE.md).

## Current verified state

- Product version: **1.0.0**—intentionally pinned
- Platform: Windows 10/11 x64; self-contained runtime
- Automated contracts: **360/360 passing** in Debug and Release with zero managed build warnings
- Localization: **1,836 synchronized non-empty strings** in English, Deutsch, Español, Français and Română
- Live read-only validation: NVIDIA GeForce RTX 5090 plus current NVML/NVAPI and installed PresentMon paths
- Release boundary: production Authenticode signing and the documented real-hardware write/read-back matrices remain required before the build is represented as a universally certified release candidate

See [Release status](STATUS.md), [Compatibility](COMPATIBILITY.md) and the [public roadmap](ROADMAP.md) for the honest boundary between implemented software and external certification.

## Documentation

| Read | Purpose |
|---|---|
| [Features](FEATURES.md) | Full categorized feature inventory |
| [Compatibility](COMPATIBILITY.md) | Windows, GPU, display and optional-runtime requirements |
| [FAQ](FAQ.md) | Direct answers about vendors, profiles, cleanup, tuning and updates |
| [Security](SECURITY.md) | Privilege boundary and private vulnerability reporting |
| [Privacy](PRIVACY.md) | Local data, network use and diagnostics policy |
| [Support](SUPPORT.md) | What to include in a useful report |
| [Changelog](CHANGELOG.md) | Maintained 1.0.0 development history |
| [Credits](CREDITS.md) | Independent implementations, research references and attribution |

## Independent software

OmniGPU is independent software by OmniVex. NVIDIA, AMD, Intel, Microsoft, MSI and the referenced community projects do not sponsor or endorse it. Their names identify compatible hardware, software or researched workflows only.

## The OmniVex suite

OmniGPU is one of a family of tools sharing a design language and a philosophy —
modern, fast, no telemetry:

**OmniTheme** · **OmniBlock** · **OmniCleaner** · **OmniAPO** · **OmniEQ** · **OmniPlay** · **OmniScale** · **OmniShade** · **OmniVisuals** · **OmniGPU** · **OmniWrappers**

<sub>**OmniWrappers** is four Direct3D compatibility installers — OmniDXVK, OmniDxWrapper, OmniVKD3D and OmniVoodoo2.</sub>

<p align="center">
  <strong>Tuned for framerate, mixed for headroom, sharp to the pixel.</strong><br>
  <a href="https://github.com/TheOmniGrid">Explore The OmniGrid</a> ·
  <a href="mailto:omnivex@theomnigrid.biz">omnivex@theomnigrid.biz</a>
</p>

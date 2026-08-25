# OmniGPU 1.0.0 feature list

“Supported” means the installed official driver/API reports the capability for the selected physical GPU. Unsupported or ambiguous controls stay hidden, read-only or fail closed.

## Gaming dashboard and GPU discovery

- Detects physical NVIDIA, AMD and Intel PCI display adapters without a fixed model-generation allowlist, plus conservative LISUAN inventory/reset identification.
- Shows the primary adapter, official vendor identity, driver version, Windows health, GPU load and VRAM use.
- Keeps virtual, remote, USB, unknown and protected adapters inventory-only.
- Uses vendor logos for the selected NVIDIA, AMD or Intel adapter and an OmniGPU fallback for unknown devices.
- Provides gamer-only navigation: Home, Drivers, Profile Inspector, Driver reset, Performance tuning, Monitoring, Displays, Memory & latency and Settings, with localized mouse-over descriptions for every destination.
- Keeps normal driver maintenance immediately visible while complete Windows Driver Store package management remains one click away in a clearly labeled advanced workspace.
- Groups live NVIDIA, AMD and Intel controls by gaming purpose and explains supported ranges or choices, live source and OC-mode requirements without exposing unsupported controls.
- Keeps a persistent Performance workspace switcher visible for monitoring, OSD composition, benchmark history, supported tuning, 32 manual profile slots, AMD gaming/video controls and fan curves.
- Includes four complete visual palettes, explicit reduced motion and ten complete application/setup languages.

## Driver maintenance and clean reset

- Optional startup check and manual Windows Update display-driver scan.
- Candidate binding to the selected live adapter, display class, PCI vendor/device identity and provider metadata.
- Review-before-install flow with explicit confirmation and UAC approval; never silent installation.
- Optional Windows restore point and driver-search pause with state-preserving restore.
- Vendor settings/cache backup, active display-driver removal and exact residual cleanup planning.
- Chipset, storage, platform, virtual and remote drivers are excluded from cleanup targets.
- Protected quarantine, rollback and manual recovery location when automatic recovery cannot complete.
- Durable privileged-operation journal and global mutation coordination so overlapping GPU writes are rejected and interrupted work is surfaced for recovery.
- SHA-256-verified known-good driver package vault with exact-device identity, protected pre-update capture planning and explicit restore review.
- Restart, shut down or leave the system running after cleanup, with exactly one completion mode selected.
- Captures selected-adapter driver versions before and after completed maintenance, suppresses duplicate rediscovery entries and exposes the actual transition in driver history.
- Detects Windows Safe Mode and opens Windows recovery options without silently editing the boot configuration.
- Includes current exact-name Intel `PmtChildDriver`/`IGSDSserviceDiscrete` rules and a conservative LISUAN path limited to its active display INF, `LSGPU` service and vendor registry trees.

## NVIDIA profile control

- Live NVIDIA DRS profiles, applications and settings.
- Responsive summary-first profile loading, selected-profile detail loading and recycling virtualization for very large driver databases.
- 926 friendly setting definitions plus 708 value tables with 5,519 named choices; exact raw values remain available for advanced use.
- Creates custom profiles, deletes custom profiles, edits one-application-per-line bindings and synchronizes additions/removals transactionally.
- Search and custom/predefined filters across the driver profile library.
- Collapsible groups, favorites, all/known/modified/uncatalogued views, source/override badges and separate undo-edit versus driver-default actions.
- Global-profile navigation, executable browse/drag lookup, copy setting/ID and Ctrl+F/Ctrl+R actions.
- Multi-file and drag-and-drop `.nip` import plus one-package export of all customized profiles.
- Persistent setting favorites and All/Known/Uncatalogued views.
- Curated 926-entry setting catalog with current names, groups and descriptions plus unknown-ID fallback.
- DWORD, QWORD, binary, ANSI string and Unicode string codecs.
- Keyboard-operable 32/64-bit advanced bit editor with canonical hexadecimal values.
- Transactional whole-database backup and restore.
- Automatic SHA-256-verified NVIDIA profile snapshots before every create, delete, save, import or default restore, with bounded ten-snapshot history and one-click latest restore.
- Read-only Profile Health checks for vendor mismatch, missing executable bindings, unbound custom profiles, duplicate names and duplicate custom bindings.
- Pending-change diff and linter for modified settings, risky raw overrides and application-binding issues before a NVIDIA profile save.
- Restores one setting, one profile or all NVIDIA profile defaults through the official DRS interfaces, with whole-database rollback on failure.
- Native `.nip` import/export with merge/update or exact-replace semantics.
- Exact replace removes settings and applications absent from the package only after a full backup.

## Cross-vendor profiles and game automation

- Validated `.omnigpuprofile` import/export for NVIDIA, AMD and Intel presets.
- Local Steam, Epic Games Store and GOG installed-library discovery.
- Per-game tuning/fan presets bound to the stable executable identity.
- Live process/path revalidation before apply.
- Automatic apply on launch, restore on exit and interrupted-session recovery.
- Optional automatic OSD launch.
- Per-game Compatibility Mode can independently suppress tuning, OSD, PresentMon, global hotkeys and capture for conflict-prone titles while retaining the game entry and its safe settings.
- Optional per-user Start with Windows and minimized background monitoring, without an always-elevated service.

## Monitoring, benchmarking and capture

- Vendor telemetry when available, with safe Windows fallback for unambiguous adapters.
- GPU load, VRAM, temperature, fan percentage/RPM channels, power, core/memory/SM/video clocks, NVIDIA P-state and power limit where reported.
- PresentMon FPS, 1% low, frametime, presentation path, CPU/GPU busy and wait, display latency, tearing and PSO observations when supplied by the installed runtime.
- Gaming Intelligence combines frame observations, driver-reported limits, exact-adapter DXGI video-memory budget/headroom and display state into plain-language bottleneck and compatibility guidance.
- Bounded telemetry history retains up to 30 minutes of analysis samples while rendering at most 60 timeline points to keep the interface lightweight.
- Persistent benchmark history with duration and average metrics.
- Local CSV performance logging.
- Click-through in-game OSD and global OSD hotkey.
- Lossless foreground-game PNG capture and global screenshot hotkey.
- Windows Game Bar recording shortcut and standard Windows capture library.
- Vendor-neutral Stability Lab for exact preset-bound games and benchmarks, with bounded vendor telemetry, optional PresentMon frame data and Windows GPU reset/WHEA/vendor-driver evidence.
- Game Readiness summary, conservative gaming recipes, completed-session analysis and goal-based tuning guidance without silently changing the GPU.
- Adaptive background cadence: dormant when no game presets exist, 10-second idle checks and 2-second checks while a configured game is active; duplicate telemetry ownership is suppressed during OSD, benchmarks or stability runs.
- Privacy-safe support ZIP export with deterministic redaction of user paths, account names and sensitive tokens.
- Manual signed install-over updates; OmniGPU contains no application updater, update checker or background downloader.

## Supported tuning model

- NVIDIA NVML power, clock, voltage and fixed-fan controls only when exposed by the installed runtime.
- AMD ADLX clock, voltage, power and hardware fan-curve controls with live ranges and read-back.
- AMD ADLX Variable Graphics Memory choices only when the selected adapter reports an exact supported-state list, including visible restart requirements and read-back.
- Intel IGCL clock, voltage, power and hardware fan-curve controls with live ranges and read-back.
- Vendor-default reset and prior-value rollback after partial failures.
- **Restore Everything** coordinates recovery of active tuning, fan curves, temporary performance state and per-game automation state without inventing unsupported defaults.
- No guessed ranges, undocumented mutation calls or cross-adapter writes.

## AMD gaming controls

- Anti-Lag.
- Chill with minimum/maximum FPS.
- Image Sharpening and strength.
- AFMF plus official algorithm, search, performance and Fast Motion Response modes when reported.
- Radeon Super Resolution and strength.
- Frame Rate Target Control.
- Enhanced Sync.
- FidelityFX Super Resolution Upgrade and Frame Generation Upgrade controls when reported.

## Intel gaming controls

- Low Latency.
- Frame Pacing.
- Texture Filtering Quality.
- Conservative Morphological Anti-Aliasing.
- XeSS Frame Generation override.
- Frame limit and sharpening.

## Displays and HDR

- Active Windows output discovery and exact target identity.
- Current resolution and rational refresh-rate reporting.
- Windows-advertised mode catalog and preflight-tested resolution/refresh changes.
- Read-back confirmation and automatic previous-mode restore on failure.
- Windows HDR state, switching and prior-state restoration.
- Exact-output DDC/CI hardware brightness with range normalization, read-back and rollback.

## Interface, themes and languages

- Four complete Omnivex visual palettes—Violet, Cyan, Plasma and Ember—that restyle the shell, navigation, cards, controls, titlebar, hero areas and ambient window corners.
- Readable 14–30 px hierarchy, visible keyboard focus and larger action/navigation targets.
- Restrained opacity/transform motion, interruptible interactions and Windows reduced-motion support.
- Complete English, German, Spanish, French, Romanian, Russian, Simplified Chinese, Japanese, Korean and Turkish catalogs with 1,964 synchronized non-empty application strings plus ten synchronized 63-entry setup dictionaries.
- Windows 11 x64 build 22000 or newer is required consistently by direct startup, MSI and setup; Windows 10 is unsupported.

## Deliberate boundaries

- No automatic OC scanner is claimed; safe artifact/stability validation needs a documented vendor scan contract.
- No independent video encoder or audio mixer; recording is delegated to Windows Game Bar.
- No NVIDIA temperature fan curve is claimed when the official runtime exposes only fixed fan control.
- No Eyefinity/topology mutation or undocumented color/video override path.
- Hardware-specific writes remain unavailable until the exact vendor runtime reports them and the applicable release gate is satisfied.
- The current unsigned package is not labeled RC: production signing and the version-bound NVIDIA/AMD/Intel, display, PresentMon and installer lifecycle certification matrix must pass first.

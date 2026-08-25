# OmniGPU 1.0.0 release status

The product version is intentionally pinned at **1.0.0**. Version identity and certification state are tracked separately.

## Completed

- Clean private development tree retained with the SDKs and sources needed for future work.
- One current runtime folder retained; historical packages, duplicate source snapshots and rebuildable outputs removed.
- Self-contained single-file Windows application plus separate elevated broker and AMD/Intel bridges.
- 396 automated tests pass; all ten application catalogs contain 1,964 synchronized non-empty strings and all ten setup dictionaries contain 63 synchronized entries.
- Windows 11 x64 build 22000 or newer is enforced by the app, MSI and setup bootstrapper; Windows 10 is outside supported and certified scope.
- A repeatable non-mutating RTX 5090 preflight verifies exact physical-device/driver/runtime binding, finite NVIDIA telemetry, public capability ranges and virtual-monitor exclusion without closing any write gate.
- The complete interface now uses guided navigation, progressive disclosure for advanced Driver Store work, purpose-grouped cross-vendor tuning and localized mouse-over/accessibility help without removing expert controls.
- Durable privileged-operation recovery, a verified known-good driver vault, Game Readiness and recipes, session/tuning guidance, Display Gaming Check, adaptive low-overhead monitoring, privacy-safe support bundles, automatic NVIDIA profile history and Profile Health are implemented.
- Gaming Intelligence, extended PresentMon/DXGI observations, driver before/after snapshots, per-game Compatibility Mode, pending NVIDIA profile diff/lint, Restore Everything and capability-gated AMD Variable Graphics Memory are implemented and exposed through the maintained interface.
- The current package validator confirms the app, broker, AMD bridge, Intel bridge and protected installer are all present; the release pipeline now rejects a package if either native bridge is omitted.
- Real 1440×900 application screenshots captured from the current build.
- Documentation-only GitHub package contains no binaries, installer or source code.
- Patreon/Ko-fi copy, brand assets, EULA, privacy notice, access/refund policy and third-party notices prepared.

## Required before certified public delivery

- Obtain production code-signing credentials and Authenticode-sign the app, broker and native bridges.
- Recompute and publish final SHA-256 hashes after signing.
- Run the signed package and installer/lifecycle checks on a disposable administrator-controlled Windows system.
- Complete real-hardware write/read-back certification for the vendor features advertised as writable.
- Have the EULA, refund terms, privacy notice, tax/VAT handling and local consumer-law language reviewed for the creator’s jurisdiction.

The machine-readable readiness report currently fails closed on missing production signatures, exact publisher binding and 18 named hardware/lifecycle certification gates. The files are suitable for development, presentation and pre-launch preparation, but must not be represented as a signed or universally hardware-certified release candidate until those gates pass.

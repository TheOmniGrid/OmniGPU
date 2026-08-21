# Compatibility and requirements

## Operating system

- Windows 10 or Windows 11, 64-bit.
- A normal interactive desktop session; remote/virtual display adapters remain read-only.
- Administrator approval is required only for driver, cleanup, tuning or fan operations handled by the elevated broker.
- The application is self-contained and does not require a separate .NET installation.

## Graphics hardware

| Vendor | Discovery and read-only paths | Write/tuning path |
|---|---|---|
| NVIDIA | Windows discovery, NVML telemetry and NVAPI/DRS profiles | Driver-reported NVML/NVAPI controls only |
| AMD | Windows discovery and ADLX capability probe | Driver-reported ADLX controls and fan curves only |
| Intel | Windows discovery and IGCL capability probe | Driver-reported IGCL controls and fan curves only |
| LISUAN | Conservative Windows inventory and active display-driver reset identification | No tuning contract is claimed |

There is no fixed GPU model allowlist. New GPUs can be discovered when Windows identifies them, but a writable control appears only when the official installed driver runtime supplies finite current/default/minimum/maximum/step values for that exact adapter.

## Displays

- Resolution and refresh controls use modes advertised by Windows for the exact output.
- HDR requires Windows advanced-color support on the selected output.
- Brightness requires an unambiguous physical monitor with working DDC/CI; internal panels and ambiguous monitor mappings stay read-only.

## Optional integrations

- Intel PresentMon 2.5.1-compatible installed runtime for vendor-neutral FPS, 1% low and frametime data.
- Windows Game Bar and Windows Captures enabled for gameplay recording.
- Steam, Epic Games Store or GOG local installation metadata for library discovery.

## Validation boundary for 1.0.0

- Live NVIDIA read-only paths were exercised on a GeForce RTX 5090.
- AMD and Intel native bridges compile and fail closed, but no local AMD/Intel GPU was available for real-hardware mutation/read-back certification.
- NVIDIA OC writes, driver removal/install and profile writes were not executed on the user’s production RTX 5090.
- The preserved local bundle is currently unsigned. Production Authenticode signing and signed install/lifecycle verification are required before paid distribution.

## Before downloading or publishing

Confirm the user has Windows 10/11 x64, an official current GPU driver and a physical NVIDIA, AMD or Intel GPU. Never promise that every control exists on every GPU; vendor API, firmware, driver branch, notebook policy and OEM limits decide the actual writable set.

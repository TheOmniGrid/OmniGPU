# Frequently asked questions

## Is OmniGPU open source?

No. The public repository contains documentation and media only. The application, installer and private source code are not published.

## How do I get OmniGPU?

Use a destination listed in [Official links](LINKS.md). Do not download OmniGPU from mirrors, file hosts or third-party “repack” pages.

## Is it a donation or a purchase?

It is free donationware. No payment is required, there are no ads and no feature is locked behind a paid tier. Optional Ko-fi or Patreon contributions support development and hardware validation.

## Does it support NVIDIA, AMD and Intel?

It detects all three vendors and uses official installed vendor APIs where available. The exact telemetry and tuning controls depend on GPU, driver, firmware and OEM policy. Unsupported controls stay unavailable.

## Is every MSI Afterburner feature included?

OmniGPU covers supported gaming essentials: telemetry, clocks/voltage/power, supported fan control, OSD, logging, benchmarks, screenshots, Game Bar recording and per-game automation. It does not claim an automatic OC scanner, an independent video encoder or undocumented control paths.

## Does it automatically update graphics drivers?

It can check trusted Microsoft-serviced display-driver candidates and guide a reviewed installation. Installation is never silent and requires explicit confirmation/UAC.

## Can it completely remove a graphics driver?

It provides a DDU-style clean-reset workflow with restore point, backup, driver-search protection, active driver removal, exact residual cleanup, rollback, Safe Mode guidance and restart/shutdown/manual-later completion. The implementation is independent and does not bundle DDU.

## Does it include NVIDIA Profile Inspector features?

It includes live NVIDIA DRS profile/application/settings access, 926 friendly setting definitions with 5,519 named choices, custom profile creation/deletion, exact game binding edits, typed raw/bit values, grouped favorites and all/known/modified/uncatalogued views, source states, per-setting/per-profile/all-default restore, database backup/rollback, multi-file `.nip` import and customized-profile bulk export with merge or exact-replace behavior.

## Where is my data stored?

Settings, presets, profiles, benchmarks and optional CSV logs are stored locally. Screenshots go to the user’s Pictures folder; Game Bar recordings use the Windows Captures folder. See the [privacy notice](PRIVACY.md).

## Does OmniGPU send analytics?

The 1.0.0 design contains no OmniGPU account, advertising SDK, analytics service or cloud sync. Network use is limited to selected driver/update operations through Windows or approved vendor hosts. “Telemetry” in the interface means local hardware performance sampling.

## Why is a control missing?

The installed vendor runtime did not report a safe writable contract for that exact GPU, or the applicable certification gate is not satisfied. OmniGPU fails closed instead of guessing.

## Can I share my copy with a friend?

Do not mirror, repackage, resell or upload the application. Send your friend to [Official links](LINKS.md) so they receive the current authentic package. Exported game/profile presets may be shared when they contain no proprietary application files or third-party-restricted content.

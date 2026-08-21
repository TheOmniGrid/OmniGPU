# Security policy

## Supported version

Only the current official 1.0.0 build is supported. Hashes must match the final post-signing release inventory published through an official destination.

## Private reporting

Do not open a public issue for vulnerabilities involving arbitrary code execution, privilege escalation, unsafe deletion, signature bypass, operation-plan forgery or private download exposure. Use a private GitHub security advisory after the repository is created or contact `omnivex@theomnigrid.biz`.

Include the affected version, impact, minimal reproduction and whether elevated approval was involved. Do not send unrelated personal files or secrets.

## Security model

- The main UI runs without elevation.
- Driver, cleanup and tuning mutations use a separate one-shot UAC broker.
- Plans are typed, bounded, expiring, integrity-sealed, replay-protected and bound to the selected live PCI adapter.
- Release mode requires protected installation and one trusted Authenticode signer across privileged runtime files.
- Cleanup uses exact vendor scopes, reparse-point rejection, backup/quarantine and rollback.
- Unsupported vendor operations fail closed.

The security model does not make overclocking, firmware, drivers or hardware risk-free. Keep backups and do not bypass platform protections.

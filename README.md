# TwinBuds preview downloads

Official Windows preview installers from **Studio Eclipse**.

**Default storefront preview: 2.0.6-preview.1.** All listed releases are marked **Pre-release** on GitHub. These installers are unsigned evaluation builds. Paid Pro checkout is disabled. Physical two-headphone playback and clean-Windows installation tests for the current release remain pending. This is not a production-readiness or Microsoft Store certification claim.

## Download

- [Current preview release](https://github.com/StudioEclipseHQ/twinbuds-downloads/releases/tag/2.0.6-preview.1)
- [Optional 2.0.7 preview with the independent storefront link](https://github.com/StudioEclipseHQ/twinbuds-downloads/releases/tag/2.0.7-preview.1)
- [All releases, including the archived 2.0.5 rollback](https://github.com/StudioEclipseHQ/twinbuds-downloads/releases)

Choose the asset named `TwinBuds-2.0.6-preview.1-win-x64-setup-PREVIEW-UNSIGNED.exe` for the current preview. The older 2.0.5 build is retained for controlled rollback; read its warnings before using it.

| Version | Purpose | Installer size |
| --- | --- | ---: |
| 2.0.7-preview.1 | Optional preview with the independent storefront link | 73,253,202 bytes |
| 2.0.6-preview.1 | Default storefront preview | 73,253,289 bytes |
| 2.0.5-preview.1 | Archived rollback build | 73,251,909 bytes |

## Before running

Use an x64 Windows PC. The interface requires the Microsoft Edge WebView2 Evergreen Runtime; the installer includes Microsoft’s WebView2 bootstrapper, which may need an internet connection if the runtime is missing. Clean-Windows bootstrap, installation and uninstall verification remain pending.

Close all TwinBuds versions before starting another. The current preview has separate settings, trial/licence state and startup identity from the original TwinBuds installation. It deliberately shares the original app’s audio lock, because both control Windows audio defaults; simultaneous operation is not supported. Installing another preview replaces the installed preview channel, rather than creating a separate installation for every preview version.

The 2.0.5 rollback predates separate preview settings and can use or update the original TwinBuds profile. Back up settings before a controlled rollback; do not treat 2.0.5 as an isolated test environment. It also does not accept licences from the newer dedicated online issuer.

These builds are unsigned. A matching checksum confirms that your file matches the published bytes; it does not replace a trusted publisher signature or prove safety or hardware compatibility. Do not disable Windows security protections to evaluate the app.

## Verify a download

The release’s `SHA256SUMS` lists the expected hash. In PowerShell, use the exact downloaded file path:

```powershell
Get-FileHash -LiteralPath '.\TwinBuds-2.0.6-preview.1-win-x64-setup-PREVIEW-UNSIGNED.exe' -Algorithm SHA256
```

Expected current SHA-256:

```text
CEB0B037CDDDA1BE47AFE206D1CE589E1B84F5CCFBB72DD18730F6DAC8FAC61E
```

Stop if the filename, size or hash differs. Each release’s `SHA256SUMS` identifies its installer. No source code, activation keys or private operational backups belong in this downloads repository.

## Support

Contact **studioeclipse.apps@gmail.com** with the app version, Windows version and a short description of the issue. Leave out passwords, payment details, identity documents and complete activation keys. Do not place private support information in public GitHub issues.

Audio processing runs locally on your PC. Device drivers, Bluetooth buffering, protected or exclusive playback and the selected audio route can affect results. Use comfortable volumes and try your actual devices before relying on the app. There is no promise of zero latency or compatibility with every headset.

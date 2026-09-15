# Council of Counsels — public downloads only

Token-free **install / update** packages for firms.

| | |
|---|---|
| **This repo** | Binary assets only (`coc-installer.exe`, `coc-windows-x64.zip`, digests) |
| **Product source** | **Not published here.** Private: [CouncilOfCounsels](https://github.com/MattAndTungGoToCantina/CouncilOfCounsels) |
| **License** | Issued separately via **CoCLicensing** (`license.json`). Download is **not** entitlement. |

## GitHub “Source code” links

GitHub always attaches **Source code (zip)** / **(tar.gz)** to every release. Those links **cannot be disabled**.

On this channel they archive **only this notice repo** (README / NOTICE) — **not** the Council of Counsels application source. Install from the named assets (`coc-installer.exe` or `coc-windows-x64.zip`), never from “Source code”.

## Install (Windows)

1. Prefer [latest `coc-installer.exe`](https://github.com/MattAndTungGoToCantina/CouncilOfCounsels-releases/releases/latest) (native window; fetches the package), **or** download `coc-windows-x64.zip`.
2. Verify SHA-256 against `SHA256SUMS`.
3. Run the installer (or unpack the zip and run `coc-installer.exe` beside `coc-api`).
4. Apply a signed `license.json` from your issuer (same `COC_LICENSE_HMAC_KEY` as the desk).

## Verify digests

```powershell
Get-FileHash .\coc-installer.exe -Algorithm SHA256
Get-FileHash .\coc-windows-x64.zip -Algorithm SHA256
# Compare to the matching lines in SHA256SUMS
```

## Notes

- Retrieval ONNX pins / Ollama models / media CLIs are handled by the installer path (or air-gap packs), not always bundled in the app zip.
- Report security issues privately to the org maintainers.

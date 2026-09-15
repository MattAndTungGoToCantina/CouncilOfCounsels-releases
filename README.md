# Council of Counsels — public downloads

Token-free **install / update** packages for firms.

| | |
|---|---|
| **This repo** | Public release assets (`coc-windows-x64.zip`, Linux tarball, `SHA256SUMS`) |
| **Source** | Private: [CouncilOfCounsels](https://github.com/MattAndTungGoToCantina/CouncilOfCounsels) |
| **License** | Issued separately via **CoCLicensing** (`license.json`). Download is **not** entitlement. |

## Install (Windows)

1. Download the latest `coc-windows-x64.zip` from [Releases](https://github.com/MattAndTungGoToCantina/CouncilOfCounsels-releases/releases).
2. Verify SHA-256 against `SHA256SUMS`.
3. Unpack; run `coc-api.exe` (see packaged `README-RELEASE.txt` / firm install docs).
4. Apply a signed `license.json` from your issuer (same `COC_LICENSE_HMAC_KEY` as the desk).

## Verify digests

```powershell
Get-FileHash .\coc-windows-x64.zip -Algorithm SHA256
# Compare to the matching line in SHA256SUMS
```

## Notes

- Retrieval ONNX pins / Ollama models / media CLIs are installed by the firm installer path (or air-gap packs), not always bundled in the app zip.
- Report security issues privately to the org maintainers.

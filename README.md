# SQLite DB Tools

A free Windows tool for working with SQLite databases, including encrypted (protected) databases, with PDF
documents and reports. Free of charge for any use, no license key, no registration.

| | |
|---|---|
| **Version** | 1.0.0-rc.1 (release candidate) |
| **Platform** | Windows, 64-bit |
| **Price** | Free of charge, personal or commercial |
| **Source code** | Private (this repository contains the program only) |
| **Manuals** | 10 languages: DE, EN, ES, FR, HI, IT, JA, PT, RU, ZH |
| **Interface languages** | AR, DE, ES, FR, HI, IT, JA, PT, RU, ZH (language files in `SQLite DB Tools data`) |

## Which folder do I use?

Each folder is a complete, self-contained copy of the program. Use **one** of them.

| Folder | What it contains | Choose it if |
|---|---|---|
| `Release/` | One standalone `SQLite DB Tools.exe` (build b4) | you want the simplest option |
| `Release_DLL/` | A smaller `SQLite DB Tools.exe` plus its DLLs (build b5) | you prefer shared libraries |

Keep everything in the folder together: the `.exe`, the `SQLite DB Tools data` folder, and in `Release_DLL/` also
the `.dll` files. The manuals (PDF) sit next to the program.

To get the files, use **Code > Download ZIP** on this page, or clone the repository.

## Verify your download

The program is not code-signed, so Windows SmartScreen may show a warning the first time you run it. Before
running, check that the file matches the published checksum in `SHA256SUMS.txt`.

PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 ".\Release\SQLite DB Tools.exe"
```

Compare the result with the line for that file in `SHA256SUMS.txt`. On Linux or macOS use
`sha256sum -c SHA256SUMS.txt` from the repository folder.

## Limits

The program works on databases within these limits: 255 tables, 255 columns per table and 522,003 records in all
the tables together. A database beyond them is opened read-only.

## Back up your data

Back up your databases, their attachment folders, key files and passwords. A lost password or key file makes an
encrypted database unreadable for ever, and nobody, the author included, can open it again.

## License

SQLite DB Tools is free of charge and the author keeps the copyright. In short, you may:

- use it for any purpose, on any number of computers;
- pass on copies free of charge, **only unmodified and complete**, with `LICENSE.md` and
  `THIRD-PARTY-NOTICES.md`;
- keep and use everything you create with it: the program claims nothing on your data and sends nothing anywhere.

You may not sell it, rent it, modify it, decompile it or reverse engineer it (except where the law allows it), or
remove its notices. Read the full text in [LICENSE.md](LICENSE.md). Using the program means accepting it.

## Third-party components

The program includes or links wxWidgets, SQLite, SQLite3 Multiple Ciphers, libsodium, PoDoFo and the libraries
PoDoFo needs. Each is used under its own license, listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
SQLite is a registered trademark of Hipp, Wyrick & Company, Inc.; this program is not made, endorsed or supported by
the SQLite developers.

## Support

Questions and problem reports: please open an issue in this repository.

Copyright (C) 2026 Fation Coga. All rights reserved.

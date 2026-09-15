# Check the file yourself

You don't need to do this: Budget Lock checks the file for you when you add it.
If you want to check a download yourself, compare its size and SHA-256
fingerprint with the ones for its version in [CHANGELOG.md](../CHANGELOG.md).

Version 6:

```
fe28869ce31c6e62a1e358ee0ad1974998351091884f89e067accbc74a17921a
```

It must also be exactly **501,452,480 bytes**.

## Windows (PowerShell)

```powershell
Get-FileHash .\BudgetLock-Assistant-v6.gguf -Algorithm SHA256
(Get-Item .\BudgetLock-Assistant-v6.gguf).Length
```

## macOS

```bash
shasum -a 256 BudgetLock-Assistant-v6.gguf
stat -f %z BudgetLock-Assistant-v6.gguf
```

## Linux

```bash
sha256sum BudgetLock-Assistant-v6.gguf
stat -c %s BudgetLock-Assistant-v6.gguf
```

## Android

In Budget Lock: Settings → Offline Assistant → *Check the file again*. It
takes about half a minute.

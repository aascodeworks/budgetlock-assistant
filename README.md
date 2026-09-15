<div align="center">

<img src="assets/budget-lock-icon.png" alt="Budget Lock" width="112">

# Budget Lock Assistant

**The file that runs Budget Lock's offline assistant on your own phone or PC.**

[![Release](https://img.shields.io/github/v/release/aascodeworks/budgetlock-assistant?label=assistant%20file)](https://github.com/aascodeworks/budgetlock-assistant/releases/latest)
[![Licence: Apache-2.0](https://img.shields.io/badge/licence-Apache--2.0-blue)](LICENSE)
[![Runs on llama.cpp](https://img.shields.io/badge/runs%20on-llama.cpp-555)](https://github.com/ggml-org/llama.cpp)

[<img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" height="72">](https://play.google.com/store/apps/details?id=com.budgeting365.app)

[Download page](https://budgetlock.app/model) · [Website](https://budgetlock.app) · [Privacy policy](https://budgetlock.app/privacy-policy.html)

</div>

---

## Contents

- [What it does](#what-it-does)
- [Download](#download)
- [Add it to the app](#add-it-to-the-app)
- [What stays on your device](#what-stays-on-your-device)
- [How it works](#how-it-works)
- [Space and phones](#space-and-phones)
- [About Budget Lock](#about-budget-lock)
- [More apps by AAS Codeworks](#more-apps-by-aas-codeworks)
- [Credits and licence](#credits-and-licence)
- [Contact](#contact)

This repository holds the released assistant files and their documentation. It
contains no app code.

## What it does

Type a sentence the way you would say it, and Budget Lock does the work:

| You type | Budget Lock |
|---|---|
| *spent 450 on groceries at the supermarket* | adds the expense, asking for anything it still needs, such as the account |
| *what did I spend on food last month?* | answers from your own records |

Without the file, the assistant still works in a simpler mode that understands
simple sentences only.

## Download

| Version | File | Size | Released | Works with |
|---|---|---|---|---|
| **6 (current)** | `BudgetLock-Assistant-v6.gguf` | 478 MB | 15 Sep 2026 | Budget Lock 1.7.2 or newer on Android, and Budget Lock for Windows |

**[Download version 6](https://budgetlock.app/downloads/BudgetLock-Assistant-v6.gguf)** ·
[all versions](CHANGELOG.md) ·
[check the file yourself](docs/verify-the-file.md)

SHA-256 of version 6:

```
fe28869ce31c6e62a1e358ee0ad1974998351091884f89e067accbc74a17921a
```

Please link to `https://budgetlock.app/model` or to the download address above
rather than to the release asset: the budgetlock.app address stays the same if
the file ever moves.

## Add it to the app

**On your phone, one tap:** open Budget Lock → Assistant → *Download it here*.
Budget Lock fetches the file, checks it, and can pause and resume if the
connection drops.

**Or download it yourself:**

1. Download the file on your phone. It lands in **Downloads**.
2. In Budget Lock, open **Assistant** and choose *I downloaded it from budgetlock.app*.
3. Tap **Choose the file** and pick it from Downloads.
4. Budget Lock checks that it is complete and genuine, then keeps its own copy.
   The one in Downloads can then be deleted.

**On Windows:** put the file in the app's `models` folder.

Something went wrong? See [docs/add-the-file.md](docs/add-the-file.md) for what
each message in the app means.

## What stays on your device

- The assistant runs on your device. The sentences you type are not sent anywhere.
- The file turns a sentence into one app command. It never sees your vault data.
- The app goes online for the assistant only if you choose *Download it here*,
  and only to fetch this file. That request goes to budgetlock.app, which sends
  it on to GitHub, where the file is stored.
- If you download the file in your browser instead, the app makes no request at all.

## How it works

```
 your sentence ──► assistant file (on device) ──► one command ──► Budget Lock
                                                                  runs it on your
                                                                  encrypted records
```

- The file is a small language model in GGUF format, run by
  [llama.cpp](https://github.com/ggml-org/llama.cpp) inside the app.
- Before using a file, Budget Lock checks its exact size and its SHA-256, so a
  damaged or altered file is refused and nothing is kept from it.
- Settings → Offline Assistant → *Check the file again* repeats the check at any time.

## Space and phones

- **Space:** about 1 GB free while you add it, 478 MB after.
- **Phones:** most Android phones sold in the last few years. Older or very
  basic phones may not run it; the app tells you if that is the case. Each
  reply shows how long it took.
- **Remove it any time:** Settings → Offline Assistant → *Remove the assistant
  file*. The assistant keeps working in its simpler mode.

## About Budget Lock

A personal finance app that keeps your records encrypted on your own device.

<table>
  <tr>
    <td><img src="assets/screenshots/01-dashboard.jpg" alt="Dashboard" width="200"></td>
    <td><img src="assets/screenshots/02-reports.jpg" alt="Reports" width="200"></td>
    <td><img src="assets/screenshots/03-budgets.jpg" alt="Budgets" width="200"></td>
    <td><img src="assets/screenshots/04-bills.jpg" alt="Bills and reminders" width="200"></td>
  </tr>
  <tr>
    <td><img src="assets/screenshots/05-loans.jpg" alt="Loans" width="200"></td>
    <td><img src="assets/screenshots/06-credit-cards.jpg" alt="Credit cards" width="200"></td>
    <td><img src="assets/screenshots/07-owed-to-me.jpg" alt="Money owed to you" width="200"></td>
    <td><img src="assets/screenshots/08-import-export.jpg" alt="Import and export" width="200"></td>
  </tr>
</table>

- **Accounts, budgets and bills:** every balance on one screen, budgets that warn
  you before you overspend, bills, EMIs and recurring payments.
- **Loans and cards:** interest, principal and payoff date; billed and unbilled
  card spending kept apart.
- **Goals and lending:** savings goals with a deadline, money you lent and money
  you owe.
- **Private by design:** AES-256 encryption on your device, works offline, no
  Budget Lock account to create.
- **Yours to take out:** export your data any time.
- **50 languages, 50+ currencies.**

[<img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" height="64">](https://play.google.com/store/apps/details?id=com.budgeting365.app)

## More apps by AAS Codeworks

| | App | What it is | Get it |
|---|---|---|---|
| <img src="assets/budget-lock-icon.png" width="48" alt=""> | **Budget Lock** | Encrypted budget app and expense tracker for Android | [Google Play](https://play.google.com/store/apps/details?id=com.budgeting365.app) |
| <img src="assets/budget-lock-icon.png" width="48" alt=""> | **Budget Lock for Windows** | The same budget file as your phone, on Windows 10 and 11 | [budgetlock.app/windows](https://budgetlock.app/windows.html) |
| <img src="assets/notedraft-icon.png" width="48" alt=""> | **NoteDraft — Offline Notepad** | Private offline notepad for notes, Markdown, to-do checklists and maps | [Google Play](https://play.google.com/store/apps/details?id=app.notedraft.noteall) |

## Credits and licence

The assistant file is a modified version of **Qwen3.5-0.8B** by Alibaba Cloud's
Qwen team, used under the Apache License 2.0. AAS Codeworks fine-tuned it on
Budget Lock's own sentence-to-command examples and quantised it to Q4_0 with
[llama.cpp](https://github.com/ggml-org/llama.cpp) (MIT). Full attribution is in
[NOTICE](NOTICE); the licence text is in [LICENSE](LICENSE).

The licence covers the assistant files in this repository. The Budget Lock app
is not open source and is not covered by it. Qwen is a trademark of its owner
and is named here only to credit the base model.

## Contact

- Help with the app or the file: **support@budgetlock.app**
- A problem with a download or a file that fails its check: see
  [SECURITY.md](SECURITY.md)
- Like the app? A rating on [Google Play](https://play.google.com/store/apps/details?id=com.budgeting365.app)
  helps other people find it.

<div align="center"><sub>© 2025–2026 AAS Codeworks</sub></div>

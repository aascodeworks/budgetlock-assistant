# Adding the assistant file

## On Android

**Download it here (one tap).** Assistant → *Download it here* → *Download now*.
Budget Lock fetches the file through budgetlock.app (the file itself is stored
on GitHub), checks it, and keeps it. You can pause; it resumes where it stopped.

**Download it yourself.**

1. Open https://budgetlock.app/model in your phone's browser and tap the
   download button. The file lands in Downloads.
2. In Budget Lock, open Assistant and choose *I downloaded it from budgetlock.app*.
3. Tap *Choose the file* and pick `BudgetLock-Assistant-v6.gguf`.
4. Wait while Budget Lock checks it: *Right file*, *Complete*, *Genuine*,
   then *Saving into the app*.

Where it is kept: Budget Lock's own storage, or the SD card if you choose that
in Settings → Offline Assistant.

## On Windows

Put `BudgetLock-Assistant-v6.gguf` in the app's `models` folder.

## What the messages mean

| The app says | What to do |
|---|---|
| No internet connection. Connect and try again, or download the file in your browser. | Connect to Wi-Fi or mobile data, or use *Download it yourself*. |
| The download server did not answer. Try again later, or download the file in your browser. | Try again later, or download it in your browser. |
| The download didn't finish. Only … of … arrived. Download it again. | The connection dropped. Tap download again; it continues from where it stopped. |
| Not enough space. Adding the file needs … free. | Free some space, or choose the SD card in Settings. |
| This isn't the assistant file. In Downloads, look for BudgetLock-Assistant-v6.gguf. | You picked a different file. Pick the one with that name. |
| This file is damaged or not version 6. Nothing was kept. Download it again. | The file is incomplete, altered, or an older version. Download it again. |
| The file did not pass the check. Remove it and add it again. | Settings → Offline Assistant → *Remove the assistant file*, then add it again. |

## Removing it

Settings → Offline Assistant → *Remove the assistant file*. This frees 478 MB;
the assistant keeps working in its simpler mode.

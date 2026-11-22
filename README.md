# DiskScope

**Inspect drives. Rescue hidden files before wiping. Format >32GB to FAT32 without mistakes.**  
Built for Windows 10/11 by **Gabriel**.

---

> ### 🚨 ONLY DOWNLOAD FROM THIS GITHUB REPO
> **DiskScope is ONLY released on this official GitHub page.**  
> If you found it on another website, forum, or download portal, **do not run it**—it is unofficial and may contain malware.  
> Always verify the **SHA-256 hash** below before opening `DiskScope.exe`.

---

## Why Use DiskScope?

- **Large FAT32 (>32GB) Formatting:** Bypasses Windows' 32GB FAT32 limit so you can format 64GB, 128GB, and larger USB drives or SD cards to FAT32 (tested on 128GB drives) alongside **exFAT**, **NTFS**, and **FAT**.
- **Rescues Hidden & Deleted Files Before Formatting:** Scans what's actually on your drive—including hidden folders and deleted trash items that Windows hides by default—and backs up everything to `C:\DiskScope Backups` in one click before wiping.
- **Mistake-Proof Format Lock:** Automatically blocks `C:`, boot, and system drives, and makes you type `ERASE <DRIVE>:` before anything gets wiped.
- **Real Drive & SMART Health Info:** Shows live model names, serial numbers, firmware, partition layouts, and drive health.
- **Drive Lock Checker:** Shows which background apps are holding open files on a USB drive.

---

## Known Issue
- **Direct Hardware Eject:** Checking locked files works, while ejecting directly from inside the app currently hits a Windows USB veto on some drives—will be fixed in the next update.

---

## Official SHA-256 Checksum (`DiskScope.exe` v1.0)
Open **PowerShell** and run this command:
```powershell
Get-FileHash "$env:USERPROFILE\Downloads\DiskScope.exe" -Algorithm SHA256
```
Make sure the output matches the **exact** string below:
```text
518A79230998C9186DAB4D955EF1253446268AAFD7B8AD865DED3773C3978877
```
*(If you saved `DiskScope.exe` to a different folder, replace `"$env:USERPROFILE\Downloads\DiskScope.exe"` with your file's path).*

*(Requires Windows 10/11 64-bit, .NET Framework 4.8+, and Admin rights. Clicking "More info → Run anyway" on SmartScreen is normal for independent apps without a paid signing certificate).*

---

## License
© 2026 **Gabriel**. All Rights Reserved.  
Free to download and use from this GitHub repo only. **No modifying, decompiling, or re-uploading elsewhere.** See [`LICENSE`](LICENSE).

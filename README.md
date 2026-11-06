# H-J Cafeteria ordering system: install package

For the Tri Tech administrator installing the H-J Cafeteria test server.

## Download

**[HJ-Deploy-2026-11-06.zip](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06/HJ-Deploy-2026-11-06.zip)**
(23.6 megabytes, from the [11/6/2026 release](https://github.com/OuterData/hj-cafe-deploy/releases/tag/deploy-2026-11-06))

## Then

1. Copy the zip to the server, right-click it, **Properties**, tick **Unblock** if it's there, **OK**.
2. Right-click, **Extract All...**, to `C:\HJ-Deploy-2026-11-06`.
3. Open **`INSTALL.md`** in that folder and follow it from step 2. It ends with the `/health` page,
   where every line should say OK.

To check the download is intact (optional), in PowerShell:

```
Get-FileHash .\HJ-Deploy-2026-11-06.zip
```

should print `30695038D5B1CDFB9F16AC498C1E41A7B4A7A6A7DC1ED9658541103D03E0610F`.

The package contains no passwords, keys or PINs for H-J's systems. Questions: Kevin at OuterData.

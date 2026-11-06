# H-J Cafeteria ordering system: install package

For the Tri Tech administrator installing the H-J Cafeteria test server.

## Download

**[HJ-Deploy-2026-11-06.zip](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06b/HJ-Deploy-2026-11-06.zip)**
(23.6 megabytes, from the [11/6/2026 (b) release](https://github.com/OuterData/hj-cafe-deploy/releases/tag/deploy-2026-11-06b), which adds SQL scripts for plain SSMS)

## Then

1. Copy the zip to the server, right-click it, **Properties**, tick **Unblock** if it's there, **OK**.
2. Right-click, **Extract All...**, to `C:\HJ-Deploy-2026-11-06`.
3. Open **`INSTALL.md`** in that folder and follow it from step 2. It ends with the `/health` page,
   where every line should say OK.

Database scripts for SQL Server Management Studio without SQLCMD Mode (also inside the zip):
[01-install-HJCafe-ssms.sql](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06b/01-install-HJCafe-ssms.sql),
[02-seed-test-HJCafe-ssms.sql](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06b/02-seed-test-HJCafe-ssms.sql),
[03-remove-test-data-HJCafe-ssms.sql](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06b/03-remove-test-data-HJCafe-ssms.sql),
and, if 01 was run without SQLCMD Mode,
[cleanup-failed-run-ssms.sql](https://github.com/OuterData/hj-cafe-deploy/releases/download/deploy-2026-11-06b/cleanup-failed-run-ssms.sql).

To check the download is intact (optional), in PowerShell:

```
Get-FileHash .\HJ-Deploy-2026-11-06.zip
```

should print `4A59B5374359A1B41F6B75A6A9F098AA24F3D5615F2F35AAFF71C390CD848D38`.

The package contains no passwords or keys. Questions: Kevin at OuterData.

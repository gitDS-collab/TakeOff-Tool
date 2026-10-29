[README.md](https://github.com/user-attachments/files/34121943/README.md)
# TakeOff Tool for Revit 2027

## Requirements

- Autodesk Revit 2027
- Revit must be closed during installation or removal.

## Install

1. Extract this entire ZIP to a local folder.
2. Right-click `Install-TakeOffTool.ps1` and select **Run with PowerShell**.
3. Start or restart Revit 2027. The **TakeOff Tool** ribbon tab will be available.

If PowerShell blocks the script, open PowerShell in the extracted folder and run:

```powershell
powershell -ExecutionPolicy Bypass -File .\Install-TakeOffTool.ps1
```

## Remove

Close Revit, then run `Uninstall-TakeOffTool.ps1`.

## Package contents

- `Plugin\QuantityTakeoffRevit2027.dll` — add-in assembly
- `Install-TakeOffTool.ps1` — installs the assembly and creates a user-specific Revit manifest
- `Uninstall-TakeOffTool.ps1` — removes this package from the current Windows user profile

The package does not include Autodesk Revit files or Revit API DLLs; Revit supplies those when it runs the add-in.

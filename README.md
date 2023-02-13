# ansible-role-win-appxdebloat

Role to remove appx packages in Windows

## Table of content

- [Default Variables](#default-variables)
  - [win_appxdebloat_regex_whitelist_apps](#win_appxdebloat_regex_whitelist_apps)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### win_appxdebloat_regex_whitelist_apps

List of whitelisted apps

#### Default value

```YAML
win_appxdebloat_regex_whitelist_apps:
  - .NET
  - Framework
  - Microsoft.DesktopAppInstaller
  - Microsoft.FreshPaint
  - Microsoft.HEIFImageExtension
  - Microsoft.MicrosoftStickyNotes
  - Microsoft.MSPaint
  - Microsoft.Paint3D
  - Microsoft.ScreenSketch
  - Microsoft.SecHealthUI
  - Microsoft.StorePurchaseApp
  - Microsoft.VCLibs
  - Microsoft.VP9VideoExtensions
  - Microsoft.WebMediaExtensions
  - Microsoft.WebpImageExtension
  - Microsoft.WindowsCalculator
  - Microsoft.WindowsCamera
  - Microsoft.WindowsNotepad
  - Microsoft.WindowsTerminal
  - Microsoft.WindowsSoundRecorder
  - Microsoft.WindowsStore
  - Microsoft.Windows.Photos
  - CanonicalGroupLimited.UbuntuonWindows
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888

# ansible-role-win-appxdebloat

Role to remove appx packages in Windows

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [win_appxdebloat_check_winrm](#win_appxdebloat_check_winrm)
  - [win_appxdebloat_check_winrm_retries](#win_appxdebloat_check_winrm_retries)
  - [win_appxdebloat_loop_count](#win_appxdebloat_loop_count)
  - [win_appxdebloat_post_reboot_delay](#win_appxdebloat_post_reboot_delay)
  - [win_appxdebloat_pre_reboot_delay](#win_appxdebloat_pre_reboot_delay)
  - [win_appxdebloat_reboot_after](#win_appxdebloat_reboot_after)
  - [win_appxdebloat_reboot_timeout](#win_appxdebloat_reboot_timeout)
  - [win_appxdebloat_regex_whitelist_apps](#win_appxdebloat_regex_whitelist_apps)
  - [win_appxdebloat_show_debug](#win_appxdebloat_show_debug)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.1`

## Default Variables

### win_appxdebloat_check_winrm

Wait for WinRM avaible until continue

#### Default value

```YAML
win_appxdebloat_check_winrm: false
```

### win_appxdebloat_check_winrm_retries

Number if retries to check if WinRM is available

#### Default value

```YAML
win_appxdebloat_check_winrm_retries: 20
```

### win_appxdebloat_loop_count

Number of loops to run

#### Default value

```YAML
win_appxdebloat_loop_count: 4
```

### win_appxdebloat_post_reboot_delay

Seconds to wait after the reboot command was successful before attempting to validate the system rebooted successfully.

#### Default value

```YAML
win_appxdebloat_post_reboot_delay: 30
```

### win_appxdebloat_pre_reboot_delay

Seconds to wait before reboot. Passed as a parameter to the reboot command.

#### Default value

```YAML
win_appxdebloat_pre_reboot_delay: 30
```

### win_appxdebloat_reboot_after

Set to true to reboot during loops

#### Default value

```YAML
win_appxdebloat_reboot_after: true
```

### win_appxdebloat_reboot_timeout

Maximum seconds to wait for machine to re-appear on the network and respond to a test command.

#### Default value

```YAML
win_appxdebloat_reboot_timeout: 1200
```

### win_appxdebloat_regex_whitelist_apps

List of whitelisted apps

#### Default value

```YAML
win_appxdebloat_regex_whitelist_apps:
  - .NET
  - Microsoft.549981C3F5F10
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
  - Microsoft.UI.Xaml
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

### win_appxdebloat_show_debug

Show debug information

#### Default value

```YAML
win_appxdebloat_show_debug: false
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888

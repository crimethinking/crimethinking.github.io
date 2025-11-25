# Install Windows Terminal on Windows 10 LTSC
[Thanks to a deleted GitHub user](https://github.com/microsoft/terminal/issues/3843#issuecomment-1718406341)

* Download the latest W10 preinstall kit from <https://github.com/microsoft/terminal/releases> and extract it
* Install the `Microsoft.UI.Xaml` package for your machine architecture, then the extracted `.msixbundle`
with `Add-AppxPackage <path to package>` in an admin PowerShell session
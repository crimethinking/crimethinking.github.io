# Install `winget` & Windows Terminal on Windows 10 LTSC 2021
How to install `winget` & Windows Terminal on Windows 10 LTSC 2021 (21H2 build 19044)

## `winget`
* Download `winget` and its prerequisites:
    * Use <https://store.rg-adguard.net> to generate links to App Installer dependencies.
        Paste in <https://apps.microsoft.com/detail/9nblggh4nns1> and generate links
    * Grab the necessary files:
        * `Microsoft.DesktopAppInstaller_<version>_neutral_~_8wekyb3d8bbwe.msixbundle`
        * `Microsoft.UI.Xaml.<version>_<arch>__8wekyb3d8bbwe.appx`
        * `Microsoft.VCLibs.140.00.UWPDesktop_<version>_<arch>__8wekyb3d8bbwe.appx`
        * `Microsoft.VCLibs.140.00_<version>_<arch>__8wekyb3d8bbwe.appx`
        * `Microsoft.WindowsAppRuntime.1.8_<version>_<arch>__8wekyb3d8bbwe.msix`

        !!! question "What is `8wekyb3d8bbwe`?"
            [Microsoft's publisher ID](https://learn.microsoft.com/en-us/windows/apps/desktop/modernize/package-identity-overview#package-family-name).
            [Source](https://superuser.com/a/1685558)

    * Install them with `Add-AppxPackage <path to package>` in an admin PowerShell session
    * Reboot

## Windows Terminal
Follow installing via `winget` instructions at <https://github.com/microsoft/terminal>
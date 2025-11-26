# Set Caps Lock to Ctrl
With admin PowerShell:
``` powershell
function CapsLock-To-Ctrl {
    $kbLayout = 'HKLM:\System\CurrentControlSet\Control\Keyboard Layout'
    $hexifiedBytes = "00,00,00,00,00,00,00,00,02,00,00,00,1d,00,3a,00,00,00,00,00".Split(',') | % { "0x$_" }

    if (-not (Test-Path $kbLayout)) {
        New-Item -Path $kbLayout -Force | Out-Null
    }

    Set-ItemProperty -LiteralPath $kbLayout -Name "Scancode Map" -Type Binary -Value $hexifiedBytes
}

CapsLock-To-Ctrl
```
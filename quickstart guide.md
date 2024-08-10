# GHCup
## Intro
GHCup makes it easy to install specific versions of GHC on GNU/Linux, macOS (aka Darwin), FreeBSD and Windows and can also bootstrap a fresh Haskell developer environment from scratch. 

It follows the UNIX philosophy of do one thing and do it well. Similar in scope to rustup, pyenv and jenv.

## Installation

> [!CAUTION]
> Always check system requirements before installing.

1. visit [GHCup](https://www.haskell.org/ghcup/).
2. Check system requirements before installing.
3.
+ For Windows,

open PowerShell, then type these commands and press `Enter` to execute the command.

```
Set-ExecutionPolicy Bypass -Scope Process -Force;[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; try { & ([ScriptBlock]::Create((Invoke-WebRequest https://www.haskell.org/ghcup/sh/bootstrap-haskell.ps1 -UseBasicParsing))) -Interactive -DisableCurl } catch { Write-Error $_ }
```

Take my device on Windows 11 for example. When I install GHCup, first I will see the [text on Poweshell] (https://github.com/40843245/GHCup/blob/main/example/example%20of%20install%20GHCup%20on%20Windows%2011.txt).

After installing, it will pop up a window with title `MinGW x64` and `MinGW x64` installs something from [`https://www.haskell.org/ghcup/sh/bootstrap-haskell`](https://www.haskell.org/ghcup/sh/bootstrap-haskell), then I will see the [text on MinGW x64](https://github.com/40843245/GHCup/blob/main/example/example%20of%20installing%20bootstrap-haskell%20through%20MinGW%20x64.txt)

You should see the similar outputs on Powershell if you install GHCup on Powershell on Windows.

+ For Linux, macOS, FreeBSD or Windows Subsystem 2 for Linux,

open terminal, then type these commands and press `Enter` to execute the command.

```
curl --proto '=https' --tlsv1.2 -sSf https://get-ghcup.haskell.org | sh
```

### System requirements
See [system requirements on GHCUP](https://www.haskell.org/ghcup/install/#system-requirements)

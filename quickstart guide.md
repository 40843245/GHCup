# GHCup
## Intro
GHCup makes it easy to install specific versions of GHC on GNU/Linux, macOS (aka Darwin), FreeBSD and Windows and can also bootstrap a fresh Haskell developer environment from scratch. 

It follows the UNIX philosophy of do one thing and do it well. Similar in scope to rustup, pyenv and jenv.

## Installation
1. visit [GHCup](https://www.haskell.org/ghcup/).
2.
+ If you're on Windows, open PowerShell, then type these commands. And press `Enter` to execute the command.

```
Set-ExecutionPolicy Bypass -Scope Process -Force;[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; try { & ([ScriptBlock]::Create((Invoke-WebRequest https://www.haskell.org/ghcup/sh/bootstrap-haskell.ps1 -UseBasicParsing))) -Interactive -DisableCurl } catch { Write-Error $_ }
```

Take my device for example, 

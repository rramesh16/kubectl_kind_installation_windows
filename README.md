# Installing Kubectl and Kind on Windows

## Install Chocolatey
### Requirements:
- Windows 7+ / Windows Server 2003+

### Install with cmd.exe
- Run cmd.exe as an Administrator - to avoid permission issues
- Run the following command
`@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
- Once the command is complete, check if Chocolatey is installed by typing `choco`

## Install Kubectl using Chocolatey
- Run cmd.exe or PowerShell as an Administrator
- Run the following command
`choco install kubernetes-cli`
- Check if kubectl is installed
`kubectl version --client`

## Install Kind using Chocolatey
- Run cmd.exe or PowerShell as an Administrator
- Run the following command
`choco install kind`

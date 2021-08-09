# Install Development Environment

Install Chocolatey and use chocolatey to install the development tools.

1. Open "Windows PowerShell"
2. Copy the following command and run inside "Windows PowerShell"

```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

3. Close "Windows PowerShell" and Open "Windows PowerShell" again
4. Execute the below command:

```
choco feature enable -n allowGlobalConfirmation
```

5. Make sure you are in the same folder as the file `packages.config` and execute the following command:

```
choco install packages.config
```

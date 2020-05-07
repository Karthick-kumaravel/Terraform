# Install Azure CLI on the windows.

Download the Azure msi installer.
    ``` https://aka.ms/installazurecliwindows ```
    
To install Azure cli execute the below comand.

```
cd <location of downloaded msi>
Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi 
Start-Process msiexec.exe -Wait -ArgumentList '/i  .\azure-cli-2.5.1.msi /qn /L*v log.txt'
Start-Process PowerShell.exe
```
Run the login command.

```
az login
```

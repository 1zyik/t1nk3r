icon: material/powershell

---
date:
  created: 2023-12-31
---
## Powershell Overview
Welcome to the my not so comprehensive PowerShell documentation, designed to empower users with the essential knowledge and practical insights into harnessing the power of PowerShell for various tasks. Whether you're a beginner or an advanced user, this documentation covers a wide range of topics, enjoy!

## Get list of all installed windows server optional features
```
Get-WindowsOptionalFeature -Online | where {$_.state -eq "Enabled"} | ft -Property featurename
```
!!! tip
    Since these are admin features, make sure to run this in an elevated window. <br/>
    You can also output to a file by pipeing result using below command
    ```
    | Out-File -FilePath "path\tofile.txt"
    ```

## How to kill a process
```
taskkill /f /pid <pid>
```
!!! tip
    Make sure to find the pid using Task Manager and replace `<pid>` with the unique value. 

## Set time and date to specific time zone
```
Set-TimeZone -Name "Central Standard Time"
```
!!! tip
    This is an admin feature, run in elevated window. <br>
    Use `Get-TimeZone` to know which one you are currently set to.<br>
    Use `Get-TimeZone -ListAvailable` to get all possible time zones you can apply. 

## Unzip multiple files into a single location

## Set a single service account to multiple windows services
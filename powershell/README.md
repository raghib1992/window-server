


# Execution Policy
1. AllSigned
2. RemoteSigned - Only allowed script from local host
3. Unrestricted - Nothing is blocked but it will give warning promt
4. Restricted - Permits individuala commands but not to script
5. Bypass - Nothing is blocked and no warning promts

# Secuity Features
1. Associated with notepad and not with powershell.exe
2. ExecutionPolicy Restriction
3. Required explicit path of the script
4. script signed is required
5. Add restiction that your script signed by trustworthy certificate provider

# Command Syntax
Verb-Noun
Get-Help 

## To get the list of all comannd
Get-Command

### Filter
Get-Command -Name "*Service*" 
Get-Command -Name "*Service*" | select -First 5

## Get to know detial of the any command
Get-Help <command name>
Get-Help Get-Service -Full
Get_Help Get-Service -Full -showwindow

## Get the concept of any command liko loop
Get-Help "about*"
Get-Help about_Arrays -showwindow

## Upadte help
Update-Help

## To Save help file 
Save-Help C:\powershell\help\export_help


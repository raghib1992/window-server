## To check the powershell version
```
$PSVerisonTable
```

## To check current execution policy 
```
Get-ExecutionPolicy
```

# to change execution policy
```
Set-ExecutionPolicy <execution policy name>
Set-ExecutionPolicy <execution policy name> -Force
```
## Toc check what this command will do without executing the command
```
Set-ExecutionPolicy <execution policy name> -WhatIf
```

## To get tha location of the current folder
```
Get-Location
```

## To change the location
```
Set-Location C:\dsds\ddsdsd
```

## To get current date
```
Get-Date
```

## Get the list of file and folder in current location
```
Get-ChildItem
```
## Get current folder with recursive
```
Get-CHildItem -recurse
```
## Get the list of file and folder some other path
```
Get-ChildItem -Path C:\dwd\wdwd
```

## Print on console
```
Write-Output "This is awesome"
Write_host "This is too good"
```

## To clear the console
```
Clear-Host
```

## To copy a file
Copy-Item -Path .\folder\file.txt -Destination test_folder\

## Copy everthing from source folder to destination folder
Copy-Item -Path test_folder1\* -Destination destination_folder2\ -Recurse 


## Copy everthing from source folder to destination folder (except file inside the sub folder)
Copy-Item -Path test_folder1\* -Destination destination_folder2\

## Move item from source folder to destination folder
Move-Item -Path test_folder1\sub_folder\file -Destination destination_folder2\

## ## Move item and rename from source folder to destination folder
Copy-Item -Path test_folder1\file.txt -Destination destination_folder2\imp-files.txt

## rename file
Rename-Item -Path .\test_folder1\sub_folder\file.txt -NewName New-file.txt

Rename-Item -Path .\test_folder1\sub_folder\file.txt -NewName "New file.txt"

## To delete item
Remove-Item -Path .\test-folder\file.txt
Remove-Item -Path .\test-folder\file.txt -Recurse

## Get the history of all command till now exexuted on powerdshell
Get-History

## Clear the history
Clean-History
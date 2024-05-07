# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/5e8cbad7-1d6d-4f9b-867c-9a83b03d51e4)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/6d725811-7c12-41bb-9bd5-10f5f6bcf2f2)

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/64756760-6ece-44ca-a7dc-63e7011abc48)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/cdf50ba4-ac68-4145-a80b-abe0c6488672)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/f6023194-257d-4401-8f5e-e67c48897392)

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/7e7da1cd-bddb-4a90-a2dc-f00b264d1b76)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/e3e1b89f-7999-40db-93b1-b596d0ac5589)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/SrinithiV/Windows-basic-commands-batchscript/assets/118722030/3c378815-5db2-4bf2-80b6-cfdb0f5278f2)

# RESULT:
The commands/batch files are executed successfully.



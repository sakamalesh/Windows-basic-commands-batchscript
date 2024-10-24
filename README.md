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

![alt text](image.png)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![alt text](image-1.png)
![alt text](image-2.png)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![alt text](image-3.png)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![alt text](image-4.png)

![alt text](image-5.png)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![alt text](image-6.png)

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

![alt text](image-7.png)

# RESULT:
The commands/batch files are executed successfully.


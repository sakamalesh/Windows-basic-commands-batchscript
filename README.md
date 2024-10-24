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

![image](https://github.com/user-attachments/assets/2fff3940-5dfa-489d-9bf2-0850b5a77116)

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab
![image-1](https://github.com/user-attachments/assets/7e86e82d-4f6a-4742-ba36-c0ccec7c47fa)

![image-2](https://github.com/user-attachments/assets/2a5af5be-4d0e-40e9-9fe7-6cd21d81e3ad)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image-3](https://github.com/user-attachments/assets/a9278f37-135e-4fde-bf17-f8c6c49931ad)


List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab
![image-4](https://github.com/user-attachments/assets/361c1caa-e92d-484d-9571-e637dfca5fd6)
![image-5](https://github.com/user-attachments/assets/e2733b09-03cc-4e29-a860-0a84c367ce9e)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image-6](https://github.com/user-attachments/assets/70320037-c844-4d50-8878-7bbd70b606a2)


Move the "MyLab" directory to the "Documents" folder.

![image-6](https://github.com/user-attachments/assets/70b79423-8538-4d93-ac1e-c427937aa90c)

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents


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
![image-7](https://github.com/user-attachments/assets/35125bed-8337-4d81-9901-6019b266e71d)


# RESULT:
The commands/batch files are executed successfully.


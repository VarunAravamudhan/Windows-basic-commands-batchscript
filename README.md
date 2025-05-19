![Screenshot 2025-05-15 152447](https://github.com/user-attachments/assets/6cbec5a3-aea4-4915-8d82-e02bec6b78ef)![Screenshot 2025-05-15 152437](https://github.com/user-attachments/assets/12ec73ac-c519-47ef-adde-2bf3c68f9f0c)# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware.

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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![Screenshot 2025-05-15 152331](https://github.com/user-attachments/assets/7c010365-08db-4943-9cca-ff55f4486105)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![Screenshot 2025-05-15 152341](https://github.com/user-attachments/assets/41392083-d33d-463c-82e3-4550a5cb56db)

~~~
type nul > MyFile.txt
~~~
![Screenshot 2025-05-15 152351](https://github.com/user-attachments/assets/68a91826-195d-4f12-8d36-327d6a7c33c5)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![Screenshot 2025-05-15 152402](https://github.com/user-attachments/assets/4e442df9-8183-47c0-a5b1-57517e15fcf5)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup
~~~
![Screenshot 2025-05-15 152429](https://github.com/user-attachments/assets/a5fa3f1a-9fca-4c45-b1a6-41f2d2d3b470)

~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![Screenshot 2025-05-15 152437](https://github.com/user-attachments/assets/1bf5fa61-db39-47f8-8a2c-764306ba8791)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![Screenshot 2025-05-15 152447](https://github.com/user-attachments/assets/f727f2d8-5f18-43e2-833b-cbb5c21c1d9b)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
![Screenshot 2025-05-15 152458](https://github.com/user-attachments/assets/72370142-815b-402e-9219-72036df5d588)

## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT
![Screenshot 2025-05-15 152510](https://github.com/user-attachments/assets/49da2862-a0c8-4b23-8c8c-3f22eebfddb6)


# RESULT:
The commands/batch files are executed successfully.


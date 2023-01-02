### **Step to fix USB Drive** :clipboard:

1. Hold the Windows key and press X, select PowerShell (Admin), select Yes to the pop-up. You can also use Command Prompt.

2. In the Powershell interface type `diskpart` to enter the disk partition tool.

3. Type `list disk` to see all disks listed. 

4. Select the USB drive by typing `select disk [NUMBER]`. Be careful to select the correct drive.

5. Type `clean`. An error will occur if you have the drive folder open, close the window and repeat the command if this happens.

6. Type `create partition primary`.

7. Type `format fs=ntfs quick` to format the drive (you can also choose to set `fs=fat32`).

8. Type `active`.

9. Type `assign`.

10. Type `list disk` and confirm your drive looks healthy.

11. Type `exit` to exit.

You can get visual confirmation by typing ‘disk manager’ into the windows search bar in the bottom left. Select the USB to view.

#### Mosquito :love_letter: _sethuaung@outlook.com_

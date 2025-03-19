## Problem: Use Vim,nano,to edit the editing_final_lab.txt file. Use the lab_file shell variable. Enter the visual mode of Vim. Remove the last seven characters from the first column on the first line. Preserve only the first four characters of the first column. 

### Step 1 - Create and Open the File in Nano or Vim

```
nano lab3.txt
```
or

```
vim lab3.txt
```

![image](https://github.com/user-attachments/assets/c47185cf-f441-4ee9-8254-0e4ab5f9ad1d)

### Step 2 - Use a variable to store the file

```
lab2="lab2.txt"
nano $lab2
vim $lab2
```

![image](https://github.com/user-attachments/assets/3e815a57-d9a9-4db8-aa27-7e7a0096cd9e)

### Step 3 - Entering vim in visual mode, press v to enable visual mode. use arrow keys to select text and press d to delete it

```
vim $lab2
```

![image](https://github.com/user-attachments/assets/8a44de7f-8b81-48ed-aa71-829473ed8e01)

### Step 4 - type 07x in the vim editor to remove the last seven characters from the first column on the first line

```
07x
```

### Step 5 - type 51d in the vim editor to preserve only the first four characters of first column

```
51d
```

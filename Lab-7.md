## A) Implement chown, chmod command with their options.

### Step 1 - Open Linux and create a new file using the touch command.

```
touch example_file.txt
```
![image](https://github.com/user-attachments/assets/6f04fa23-2cd8-4d2f-949e-8f0ec2c2836e)

### Step 2 - Change the ownership of the file.

```
chown username example_file.txt
```
- Replace username with the desired user's name.

![image](https://github.com/user-attachments/assets/cd60cd81-a7d7-4752-a8d7-280c6386e569)

- To change both owner and group, use:

```
chown username:groupname example_file.txt
```

### Step 3 - Verify ownership change using ls -l.

```
ls -l example_file.txt
```
- The output will show the updated owner and group of the file.

![image](https://github.com/user-attachments/assets/5eada53b-1f27-4116-bb81-7ac63390a019)

## B) Problem: Change file permissions using chmod.

### Step 1 - Create a file or directory.

```
touch another_file.txt
```
![image](https://github.com/user-attachments/assets/a7fe3ab0-098d-44b1-a6ff-d2ebb6ae13d0)

### Step 2 - Modify permissions using octal values.

```
chmod 755 another_file.txt
```
- This sets the permissions as follows:
-- Owner: Read, write, execute.
-- Group: Read, execute.
-- Others: Read, execute.

![image](https://github.com/user-attachments/assets/7b860717-2926-4ef0-8daa-7f952053a363)

### Step 3 - Verify the changes.

```
ls -l another_file.txt
```

- The output will display the file permissions as -rwxr-xr-x.

![image](https://github.com/user-attachments/assets/52dad9e9-1674-4b3d-8887-35512aca147c)

## A) Problem: Write Shell scripts to print system information

### Step 1 - Open linux and create a new file using nano editor.

```
nano <file_name.sh>
```
![image](https://github.com/user-attachments/assets/a5acd402-d2c5-4777-b5db-c1ac4b027f4f)

### Step 2 - Now fill in the contents of the script and use the 'lscpu' command for diaplaying system information.

```
#!/bin/bash

echo $(lscpu)
```

![image](https://github.com/user-attachments/assets/414395a3-eed0-40f0-a1a5-065b76650c02)

### Step 3 - Use bash command with script name to see the system info.

```
bash <file_name.sh>
```

![image](https://github.com/user-attachments/assets/c7ce6d0b-a89a-40a9-88f6-9dba8521da4b)

## B) Problem: Write Shell scripts to perform basic mathematical calculations.

### Step 1 - Open linux and create a new file using nano editor.

```
nano <file_name.sh>
```

![image](https://github.com/user-attachments/assets/68deb8a7-50c7-40ff-b54f-9a5cc39d536d)

### Step 2 - Update the contents of the file with the code below to create a calculator.

```
#!/bin/bash

echo "Enter the first number: "
read a

echo "Enter the second number: "
read b

echo "Which operator do you want to use? (Enter the corresponding number)"
echo "1. '+' (Addition)"
echo "2. '-' (Subtraction)"
echo "3. '*' (Multiplication)"
echo "4. '/' (Division)"
read op

case $op in
  1)
    result=$((a + b))
    echo "Result: $a + $b = $result"
    ;;
  2)
    result=$((a - b))
    echo "Result: $a - $b = $result"
    ;;
  3)
    result=$((a * b))
    echo "Result: $a * $b = $result"
    ;;
  4)
    result=$((a / b))
    echo "Result: $a / $b = $result";;
  *)
    echo "Invalid";;
esac
```

![image](https://github.com/user-attachments/assets/ef226750-0e20-4610-a073-e9e5f2c33e09)

### Step 3 - Now run the script using bash and start interacting.

```
bash <file_name.sh>
```
![image](https://github.com/user-attachments/assets/9bf9273c-179e-4eda-9a31-b3ab33185dd8)

## C) Problem: Use redirection command to store the output of commands.

### Step 1 - Open linux and create a new file using touch command.

```
touch <filename.txt>
```
![image](https://github.com/user-attachments/assets/af2371ed-b957-4243-a2d0-327a725819ab)

### Step 2 - Now use the redirection operator to store the contents of the command in file & use the cat command to see the contents.

```
<command> > <file_name.sh>
```

![image](https://github.com/user-attachments/assets/09cc0a76-214f-417d-b49a-5a19f5732eee)

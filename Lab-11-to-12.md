## Problem: Create the operator1 user and confirm that it exists in the system. Set the password for operator1. Create the additional operator2 and operator3 users. Set their passwords aswell. Run the usermod -c command to update the components of the operator1 user account. Remove the operator3 user from the system.

### Step 1 - Create a new user

```
sudo useradd operator1
```

![image](https://github.com/user-attachments/assets/7980063c-b8a5-40ac-bfab-d32a7d62b58d)


### Step 2 - Setting the password for operator1

```
sudo passwd operator1
```

![image](https://github.com/user-attachments/assets/21eaddd3-5b76-46c2-9769-c8cf3dea1655)

## Step 3 - Create two more users operator2 & operator3

```
sudo useradd operator2
sudo useradd operator3
```

![image](https://github.com/user-attachments/assets/f678557d-f68f-4406-8aff-ddf1a25d48b6)

### Step 4 - Setting the passwords for operator2 & operator3

```
sudo useradd operator2
sudo useradd operator3
```

![image](https://github.com/user-attachments/assets/3b423f86-44fc-49b8-967c-18d3ccb721d2)

### Step 5 - Set the comments of the user operator 1

```
sudo usermod -c "Doing lab 12" operator1
getent passwd operator1
```

![image](https://github.com/user-attachments/assets/931fc504-6979-4adf-89b1-6e5c5d255160)

### Step 6 - Remove operator 3 and view the updated users list

```
sudo userdel operator3
getent passwd
```

![image](https://github.com/user-attachments/assets/4ca4d5b3-2157-4c1c-9c4e-938304c7f762)

![image](https://github.com/user-attachments/assets/efea2198-61bd-4fd3-b83e-210030a8ee89)

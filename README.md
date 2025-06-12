# Ansible-project
Ansible project for beginners create an ansible playbook to install Apache server on slave \

Create 2 instance master and slave 
master
![image](https://github.com/user-attachments/assets/fa932233-ea8e-4ddc-8cf3-cd64779900d2)
slave
![image](https://github.com/user-attachments/assets/0f114521-f09d-4b3c-bcb8-c0e86f161562)
Ansible uses a master-slave architecture
Install Ansible on master  
![image](https://github.com/user-attachments/assets/76d97da2-5c66-41f5-982d-b462af9b59ef)
Create ssh key on master for password less authentication with slave 
![image](https://github.com/user-attachments/assets/7c808eb6-3157-4655-9b3e-b062553faec4)
Copy you master public key to slave authorized key inorder to make the password less authentication 
After create test the connection with 
ssh ububtu@ip_of_slave_instance 
if it is success you passwordless authentication with salve is done 
next step to create inventory 
![image](https://github.com/user-attachments/assets/f3afeab8-3a5c-42d9-8626-9ea1c959ca75)
![image](https://github.com/user-attachments/assets/4305b9cc-4af2-4371-8a48-34f4d58da044)
Create inventory file and try ping test first 
![image](https://github.com/user-attachments/assets/88d97d13-6d7c-4bed-8a88-1efdfa3c3dab)
Try some adhoc command with ansible 
![image](https://github.com/user-attachments/assets/fe026928-02e7-4483-ad7f-7e197ae098ae)
Lets build the Apache server to the slave 
Create first simple index file 
 file provided 
 Create the first Yamal file it include update the cache install Apache server and copy index file from master to slave 
Run the playbook 
![image](https://github.com/user-attachments/assets/bba62c63-ca67-4a46-8543-b3b94a69c417)

Open port 80 on EC2 
Access over IP  success !!!!!








# Add sudo to user with docker
1. Add user to file /etc/group (line contain sudo)
2. Add line `your_username ALL=(ALL) NOPASSWD: ALL` to file /etc/sudoers 
3. Remove password (if hashed) in file /etc/shadow

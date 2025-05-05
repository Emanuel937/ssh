# SSH: Connecting to GitHub Using SSH (MAC & Linux) - tutorial 
## What is SSH?

SSH, or Secure Shell, is a cryptographic network protocol used for secure communication over an unsecured network. It is commonly employed for remote access to command-line interfaces on Unix-like operating systems, including Linux and macOS, as well as for secure file transfer between computers. SSH generates private and public keys, and with these keys, you can connect your machine to the host securely.

## Step 1: Checking for an Existing SSH Private Key

Open your terminal and type the following command:

Run the following command in your terminal to check if you have an existing SSH public key:  
```bash
cat ~/.ssh/id_rsa.pub.
```
##
If it returns "No such file or directory," it means there is no private and public key on your system, and you need to create it.

Command to create private and public keys:
```bash
  ssh-keygen -t rsa -b 2048
```

**Note**: When prompted, you can enter a passphrase. This password will be required when uploading your files and folders to GitHub. Type Enter every time you are asked to input data.
Step 2: Viewing and Copying Your Keys

Command:

```bash

cat ~/.ssh/id_rsa.pub
```
Copy the data displayed in your terminal and go to your GitHub account.
###Step 3: 
-Adding the SSH Key to Your GitHub Account
- Click on the Settings button in your GitHub account.
- Then click on the "SSH" tab and select "New SSH key."
- Paste the SSH key that you generated.
- Save the changes.

#Now, you should be able to securely connect to GitHub using SSH.




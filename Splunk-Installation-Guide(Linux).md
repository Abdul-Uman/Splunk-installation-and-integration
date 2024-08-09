# Splunk Installation on Linux

  This guide provides step-by-step instructions for installing Splunk on a Linux system using a web browser to download the installer.

## Prerequisites

 - A Linux system with sudo privileges.
 - Internet access.

## Installation Steps

## Step 1: Download Splunk via Browser

  Visit the [Splunk download page]
  https://www.splunk.com/en_us/download.html
   
![IMG-20240809-WA0002 1](https://github.com/user-attachments/assets/8e522123-e550-43a0-b13c-6f27b6f2b1cf)

## Select the .deb package for Ubuntu/kali/Debian.
## Click the "Download" button to start the download

![Screenshot from 2024-08-09 23-56-19 1](https://github.com/user-attachments/assets/fd280122-c65c-4f57-8929-0bb076498dd6)

## Step 3: Install Splunk

After downloading the .deb file, install it using the terminal

     sudo dpkg -i ~/Downloads/splunk-*.deb

![Screenshot from 2024-08-10 00-14-34 1](https://github.com/user-attachments/assets/58efcca2-18cb-4ab7-8a1a-25dbe41c7dff)


## Step 4: Start Splunk

    /opt/splunk/bin/sudo ./splunk start

![WhatsApp Image 2024-08-10 at 00 40 21_677bc368](https://github.com/user-attachments/assets/5ca7757f-59dc-4fef-8a07-fb8be11d6196)

    
## Step 5: Select YES And Create Credeniatls for Splunk Login

![WhatsApp Image 2024-08-10 at 00 40 21_8dee72b1](https://github.com/user-attachments/assets/5c94b64b-7798-4f54-a6ab-6e4772b9aac1)

## Step 6: Access Splunk Web Interface


![WhatsApp Image 2024-08-10 at 01 05 21_8f641d52](https://github.com/user-attachments/assets/a09dc445-6d0b-4e40-bf35-4d143cfca674)


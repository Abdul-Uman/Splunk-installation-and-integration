# Splunk Universal Forwarder on Windows Guide

This guide provides step-by-step instructions for installing and configuring the Splunk Universal Forwarder on a Windows system.

## Prerequisites

- A Windows machine (Windows Server or Windows Desktop)
- Administrator access

## Step 1: Download the Universal Forwarder

1. Visit the [Splunk Universal Forwarder download page](https://www.splunk.com/en_us/download/universal-forwarder.html).
2. Select the version that matches your Windows operating system.
3. Download the installer.

![Download Univerasal Forwarder](https://github.com/user-attachments/assets/e8f88889-7435-4675-9a4f-b1f87de36df3)

## Step 2: Configure Receiving Data Port on Heavy Forwarder on which we want to Receive the logs from Windows Universal Forwarder

1. Login to Heavy Forwarder
2. Go to **Settings > Forwarding and Receiving > Configure Receving**.
3. Use **9997 Data port** and **Save it**.

![Screenshot (8)](https://github.com/user-attachments/assets/c5f9df6b-a6c4-41d7-a87d-cc8350ffd177)



## Step 3: Install the Universal Forwarder

1. Run the downloaded installer as an administrator.
2. Follow the on-screen prompts to install the Universal Forwarder.
3. During installation,

   ## Select Account and Click on Next.
   ![Screenshot (10)](https://github.com/user-attachments/assets/44f4c9da-f71e-4dfc-8fc2-8b6d7bc1eed8)

   ## Select Inputs you want to collect from Windows end point.
   
   ![Screenshot (11)](https://github.com/user-attachments/assets/c3f65332-f382-4985-9a7d-40f21d13b100)

   ## Create Credentials and Click on Next.

   ![Screenshot (12)](https://github.com/user-attachments/assets/a2325808-733b-42f0-b589-e9f2a66395aa)

   ## Specify Deployment Server Ip address or Hostname and Port No.

   ![Screenshot (13)](https://github.com/user-attachments/assets/813dca04-cf39-41db-8ca2-93dc75047087)

   ## Specify the Splunk Indexer or Heavy Forwarder to send the data.
   
   ![Screenshot (14)](https://github.com/user-attachments/assets/909dcf56-60af-46e3-96d7-e5478ee248aa)

   ## Click on Install.

   ![Screenshot (15)](https://github.com/user-attachments/assets/c010034c-6c5b-4ff0-a5be-da4545ab49aa)

   ## Finish Installation.
   
   ![Screenshot (16)](https://github.com/user-attachments/assets/855f2488-11ce-408b-8f73-10171fe0e49b)


## Step 4: Verify Data Collection.

   1.Go to Search & Reporting in Splunk Heavy Forwarder.
   
   2.Write a search Query to verify that data from the Windows Universal Forwarder machine is being 
     collected.

   ![Screenshot (17)](https://github.com/user-attachments/assets/d269bee5-97e8-4d59-9254-c0e9f21e5706)

  
## If Logs are generating it means "Integration is Successfull".








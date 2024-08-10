## Syslog Integration with Splunk on Linux (Using GUI)

This guide explains how to integrate Syslog data with Splunk on a Linux system using the Splunk Web Interface, enabling Splunk to collect and analyze logs from various network devices and services.

## Prerequisites

1.Splunk installed and running on your Linux system.

2.Access to the Splunk Web Interface.

3.Devices or services configured to send Syslog messages.

## Step 1: Log in to the Splunk Web Interface

1.Access the Splunk Web Interface.

2.Open your web browser and navigate to http://<your-splunk-server-ip>:8000.

3.Log in with your Splunk credentials.

![WhatsApp Image 2024-08-10 at 01 05 21_99b34ed6](https://github.com/user-attachments/assets/4e06bbaf-a98d-487f-a2a8-53fb274c9e77)


## Step 2: Install the Splunk Add-on for Unix and Linux via the Splunk App Browser

1.In the Splunk Web Interface, locate the **Apps menu** at the top left of the screen.

2.Click on **Find More Apps**.

3.Type **"Splunk Add-on for Unix and Linux"** into the search bar and press Enter.

![Screenshot 2024-08-10 183243](https://github.com/user-attachments/assets/3e6f7eee-6542-4a06-85d4-17cedff91414)

5.Find the Splunk Add-on for Unix and Linux in the search results.

6.Click the **Install** button next to the Splunk Add-on for Unix and Linux.

  If prompted, log in to your Splunk.com account to proceed with the installation.
  The add-on will be automatically downloaded and installed into your Splunk instance.

  
## Step 3: Add a Syslog Data Input in Splunk
    
1.Navigate to Data Inputs:

2.From the main dashboard, click on **Settings** in the upper right corner.

3.Under **Data**, click on **Data Inputs**.

![Screenshot 2024-08-10 184715](https://github.com/user-attachments/assets/7718ca9c-f3fc-4e21-a683-6df14f841e67)


## Step 4:Add a New UDP Data Input:

1.On the Data Inputs page, locate and click **UDP.**

2.On the UDP Inputs page, click New Local UDP to create a new UDP input.

![Screenshot 2024-08-10 184133](https://github.com/user-attachments/assets/3090a0c7-581d-4286-8d98-2e4894172a86)


## Step 5:Set the UDP Port:

1.Enter **514** for the UDP port (this is the standard port for Syslog messages).

2.Click **Next** to continue.

![WhatsApp Image 2024-08-10 at 18 26 06_069ab237](https://github.com/user-attachments/assets/0d1a8903-992c-4d8a-a3fd-719db6fb16be)

## Step 6:Configure Source Type:

1.In the source type configuration screen, select **linux_secure** as the source type.

2.Optionally, you can set a Hostname or Index, or you can leave these as default.

3.Click **Review** to see a summary of your settings.

![WhatsApp Image 2024-08-10 at 18 26 18_1a865196](https://github.com/user-attachments/assets/c70e1e01-75dc-4eb7-8fb4-46a3204c11e9)

## Step 7:Review and Save:

1.Review your settings on the final screen.

2.Click **Submit** to save and enable the UDP data input.

## Step 8:Test the Integration

1.Send a Test Syslog Message from a Device:

2.Ensure that a device or service on your network is sending Syslog messages to your Splunk server.

3.You can check for these messages in the Search & Reporting interface by searching for recent events.

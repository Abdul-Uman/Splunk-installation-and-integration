# WMI Integration Guide

This guide provides step-by-step instructions for integrating Windows systems with Splunk using WMI (Windows Management Instrumentation).

## Prerequisites

- Splunk installed and running
- Administrator access on the Windows machine

## Step 1: Enable WMI on Windows

1. Open the Services management console (`services.msc`).
2. Locate the `Windows Management Instrumentation` service.
3. Ensure the service is running and set to start automatically.

![1 (2)](https://github.com/user-attachments/assets/9ec44505-ffb1-4cc5-b61e-1f2bf0ecdc20)

## Step 2: Configure WMI Inputs in Splunk

1. Log in to the Splunk Web interface.
2. Go to **Settings > Data Inputs > WMI**.
3. Click **Add New** to create a new WMI input.

![Screenshot (2)](https://github.com/user-attachments/assets/5a5312d8-38ca-4063-9722-3d80f765e335)


4. Select the appropriate WMI class and configure the input settings.

![Screenshot (3)](https://github.com/user-attachments/assets/a9d3a904-bb86-4702-b068-21f2259d174c)

5. Check And Review your Configuration then Select on **Submit**.

![Screenshot (4)](https://github.com/user-attachments/assets/26fa5bd7-306b-45b3-9927-13183811fe1f)

6. Start Searching And Select **Next**.

![Screenshot (5)](https://github.com/user-attachments/assets/93acf403-b0d8-4237-9138-b8b4b718eb8e)



## Step 3: Verify Data Collection

1. Go to **Search & Reporting** in Splunk.
2. Run a search to verify that data from the Windows machine is being collected.

![Screenshot (6)](https://github.com/user-attachments/assets/498ff433-fa73-4fe3-999d-7df6fc2cff6a)

## If your Logs are generating it means "Integration is Successfull".



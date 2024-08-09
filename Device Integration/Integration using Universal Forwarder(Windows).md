# Splunk Universal Forwarder on Windows Guide

This guide provides step-by-step instructions for installing and configuring the Splunk Universal Forwarder on a Windows system.

## Prerequisites

- A Windows machine (Windows Server or Windows Desktop)
- Administrator access

## Step 1: Download the Universal Forwarder

1. Visit the [Splunk Universal Forwarder download page](https://www.splunk.com/en_us/download/universal-forwarder.html).
2. Select the version that matches your Windows operating system.
3. Download the installer.

![Download UF](screenshots/download-uf.png)

## Step 2: Install the Universal Forwarder

1. Run the downloaded installer as an administrator.
2. Follow the on-screen prompts to install the Universal Forwarder.
3. During installation, specify the Splunk Indexer or Heavy Forwarder to send the data.

![Install UF](screenshots/install-uf.png)

## Step 3: Configure Inputs on the Universal Forwarder

1. Open the Universal Forwarder configuration file (usually located in `C:\Program Files\SplunkUniversalForwarder\etc\system\local\inputs.conf`).
2. Add the paths to the log files or directories you want to monitor.

![Configure UF](screenshots/configure-uf.png)

## Step 4: Start the Universal Forwarder Service

1. Open the Services management console (`services.msc`).
2. Locate the `SplunkForwarder` service.
3. Start the service and set it to start automatically.

![Start UF Service](screenshots/start-uf-service.png)

## Step 5: Verify Data is Being Sent

1. Log in to your Splunk Indexer or Heavy Forwarder.
2. Use the Search app to verify that data from the Universal Forwarder is being received.

![Verify Data](screenshots/verify-data.png)

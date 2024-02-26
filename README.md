# Termux Setup Guide

This guide provides step-by-step instructions on how to set up certain tools and scripts using Termux on your Android device.

## Prerequisites

- Any Android device running a version supported by Termux.
- A stable internet connection.

## Installation and Setup

### Step 1: Download Termux

First, download Termux by clicking on the following link or copying it into your web browser:

[Download Termux](https://github.com/termux/termux-app/releases/download/v0.118.0/termux-app_v0.118.0+github-debug_universal.apk)

### Step 2: Initialize Termux

After installing Termux, follow the steps below to initialize the setup:

#### Initialize Installation

Copy the script below and paste it into Termux. Wait for the process to complete. If prompted to choose, always select "N" for no (default=N). After the installation is complete in Termux, close the app and reopen it before proceeding to the next step.

```
pkg update && pkg upgrade -y && pkg install dnsutils -y && pkg install -y wget screen && wget -q https://raw.githubusercontent.com/JKimDevs/termux/main/termux.sh -O termux.sh && chmod +x termux.sh && ./termux.sh l
```

### Step 3: Download Additional Scripts

After reopening Termux, execute the following commands in sequence, proceeding to the next step after each command completes successfully.

**Download IP List:**

```
wget https://raw.githubusercontent.com/JKimDevs/termux/main/ip.txt
```

**Download Domain List:**

```
wget https://raw.githubusercontent.com/JKimDevs/termux/main/domains.txt
```

### Step 4: Finalize Setup

To finalize the setup, copy and paste the script below:

```
./termux.sh
```

## Completion

Congratulations! You have successfully set up your Termux environment. For further modifications or updates, repeat the relevant steps as necessary.

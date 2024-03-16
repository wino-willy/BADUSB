# BeEF Injection Payload

## Table of Contents

- [Introduction](#introduction)
- [Payload Description](#payload-description)
- [Usage Instructions](#usage-instructions)
- [Disclaimer](#disclaimer)

## Introduction

This repository contains a payload script written in DuckyScript 1.0, intended for use with the USB Rubber Ducky, a keystroke injection tool. The script is designed to inject a payload into an Android device's Chrome browser, specifically targeting devices with Chrome as the default browser.

## Payload Description

The provided payload script is designed to open multiple tabs in the Chrome browser on the target Android device. One of these tabs is intended to lead to a specified domain or IP address, where the actual injection occurs. The idea behind this payload is to leverage the BeEF (Browser Exploitation Framework) to perform further actions on the target device.

### Script Execution Steps:

1. **Open Chrome Browser**: The script initiates by opening the Chrome browser on the target Android device.

2. **Open Multiple Tabs**: Several tabs are opened sequentially, each containing predefined URLs of popular websites like YouTube, Facebook, The New York Times, Instagram, Twitter, etc.

3. **Inject Payload**: At a specified point in the script (line 62), there is a placeholder `<link to your site>`. This is where you should replace it with the URL of your hosted site, where the actual payload or malicious content is served. The script aims to "hide" this browser tab in the background behind the other tabs, making it less noticeable to the user.

4. **Continued Tab Openings**: After injecting the payload, the script continues to open more tabs with various websites, potentially to distract the user or maintain the appearance of normal browsing activity.

## Usage Instructions

To use this payload script effectively, follow these steps:

1. **Prepare USB Rubber Ducky**: Ensure you have a USB Rubber Ducky device and that it's configured properly for use.

2. **Modify Payload Script**: Open the payload script (`beef_injection_payload.txt`) and replace `<link to your site>` on line 62 with the URL of your hosted site where the payload is hosted.

3. **Deploy Payload**: Insert the USB Rubber Ducky into the target Android device's USB port and execute the payload script. The script will run automatically, injecting the payload into the Chrome browser tabs.

## Disclaimer

This payload script is provided for educational and testing purposes only. It should only be used on devices and systems for which you have explicit authorization to perform such actions. The misuse of this script for unauthorized or malicious purposes is strictly prohibited and may violate ethical standards and legal regulations. The author of this script and the repository contributors are not responsible for any misuse or damages resulting from the use of this payload.

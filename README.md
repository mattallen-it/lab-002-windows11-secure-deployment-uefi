🖥️ Windows 11 Deployment & Recovery USB (Rufus Lab)
📌 Overview

This project documents the creation of a Windows 11 deployment and recovery USB using Rufus. It simulates how enterprise IT teams prepare bootable media to provision, recover, and secure endpoints in environments where hardware trust, security controls, and OS integrity matter.

The USB created in this lab supports:

Clean Windows 11 installations

Hardware requirement bypass (TPM, Secure Boot, RAM, CPU)

UEFI and legacy boot environments

Recovery, repair, and troubleshooting workflows

This is the same class of tooling used by help desks, MSPs, hospitals, and government contractors when reimaging or recovering machines in regulated environments.

🎯 What This Lab Demonstrates

This is not just a Windows installer. It demonstrates endpoint control — the foundation of security, identity, and enterprise IT.

Key skills shown:

Boot media creation for modern UEFI systems

OS deployment and re-provisioning

Hardware compatibility remediation

Recovery and troubleshooting access

Secure endpoint initialization

These map directly to Tier 1–2 IT, SOC, and IAM-adjacent workflows.

🛠️ Tools Used
Tool	Purpose
Rufus	Creates bootable USB media from Windows ISO
Windows 11 ISO	Operating system deployment image
UEFI Firmware	Modern secure boot environment
TPM & Secure Boot bypass	Allows recovery or installation on non-compliant systems
🧪 Lab Scenario

This lab simulates a real-world IT situation:

A Windows system must be reinstalled or recovered on hardware that may not meet Windows 11 requirements, while still maintaining control over boot and OS provisioning.

Using Rufus, the USB was configured to:

Bypass Windows 11 hardware checks

Support UEFI booting

Allow technician-level OS installation and recovery

This enables IT staff to:

Reimage failed systems

Recover from corrupted OS installs

Deploy Windows consistently across mixed hardware

🔐 Why This Matters (IAM & Security Angle)

Before users authenticate — before accounts even exist — control of the boot process determines who owns the machine.

This lab shows:

Who can boot

Who can install

Who can recover

Who controls the OS

That is the first layer of Identity and Access Management.

If you control the boot media, you control the endpoint.

📁 Repository Contents
/screenshots
 ├── 01_iso-selection.png
 ├── 02_rufus-config.png
 ├── 03_tpm-secureboot-bypass.png
 ├── 04_uefi-boot-mode.png
 ├── 05_usb-writing.png
 └── 06_successful-media.png

README.md

🧠 Skills Demonstrated

Windows deployment workflows

Boot & firmware awareness (UEFI vs Legacy)

Secure OS provisioning

Troubleshooting and recovery tooling

Enterprise-style endpoint preparation



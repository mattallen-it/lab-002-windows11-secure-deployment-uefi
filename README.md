🛡️ Windows 11 Secure Deployment & Recovery Media (Rufus)
Overview

This project documents the creation of enterprise-grade Windows 11 deployment and recovery media using Rufus and an official Microsoft ISO, validated on a modern UEFI-secured AMD platform.

The goal is to demonstrate secure endpoint provisioning, identity control, and recovery readiness — the same skills used in SOC, IAM, and government-regulated IT environments.

🎯 Objectives

Build trusted Windows 11 installation media

Bypass forced cloud identity for local account control

Enable deployment on legacy or lab hardware

Validate hardware and firmware security posture

Prepare for incident response & offline recovery

🧰 Tools Used
Tool	Purpose
Rufus 4.11	Create bootable Windows deployment media
Windows 11 25H2 ISO (x64)	Official Microsoft installation image
ASUS UEFI BIOS	Firmware-level security and boot validation
AMD Ryzen 5 7600X3D Platform	Secure, modern hardware baseline
📦 ISO Supply Chain Verification

The installation media was created using the official Microsoft ISO:

Win11_25H2_EnglishInternational_x64.iso

Architecture: x64 (Intel/AMD)

Version: Windows 11 25H2

Size: ~7.5 GB

This ensures a trusted, malware-free OS image was used.

📸 Screenshot: ISO file name and size

🛠 Rufus Deployment Configuration

Rufus was configured for modern secure systems:

Partition scheme: GPT

Target system: UEFI (non-CSM)

File system: NTFS

Image: Standard Windows Installation

This produces UEFI-bootable, enterprise-compatible installation media.

📸 Screenshot: Rufus main configuration screen

🔓 Windows Security & Identity Overrides

Rufus Windows User Experience options were used to enable enterprise-style control:

Remove TPM / Secure Boot requirement

Remove Microsoft account requirement

Enable local administrator account creation

Disable forced telemetry

This allows:

Offline deployment

Lab and air-gapped installs

Full IAM control of local accounts

📸 Screenshot: Rufus “Customize Windows Installation” options

💽 Boot Media Validation

After creation, the USB was verified to contain:

/boot  
/efi  
/sources  
setup.exe  
bootmgr.efi


This confirms the drive is fully bootable and UEFI-compliant.

📸 Screenshot: USB contents

🔐 Firmware & Hardware Trust Verification

The host system used to build this media was validated in UEFI BIOS:

Security Features Enabled

Secure Boot: Windows UEFI Mode

NX (No-Execute): Enabled

SVM (Virtualization): Enabled

PSS: Enabled

These support:

Credential Guard

Virtualization-based Security (VBS)

Exploit mitigation

Secure boot chains

📸 Screenshot: CPU configuration (NX, SVM, PSS)
📸 Screenshot: Secure Boot configuration

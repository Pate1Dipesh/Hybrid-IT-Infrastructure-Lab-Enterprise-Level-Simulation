Hybrid IT Infrastructure Simulation – Enterprise-Level Lab Environment
This repository contains the complete documentation and resources for a comprehensive 19-phase hybrid IT infrastructure simulation project. The goal of this project is to build an enterprise-level IT infrastructure that integrates modern technologies and best practices, simulating a real-world corporate environment.

Project Overview
This hybrid IT infrastructure setup integrates multiple technologies, from initial Microsoft 365 tenant deployment to device management, security configurations, and cloud integrations. The project replicates the IT infrastructure of a modern MNC, using a combination of on-premises Active Directory (AD), Microsoft Entra ID (formerly Azure AD), Intune for device management, Exchange Online, Jamf for Apple device management, and more.

Completed Phases
Phase 1: Microsoft 365 Developer Tenant Deployment

Enrollment of Microsoft 365 E5 Developer Tenant

User and group creation, service validation

Security configurations (MFA, audit logging)

Phase 2: Deployment of On-Premises Active Directory Domain Services (AD DS) & Azure AD Connect

Configured Windows Server 2022 VM with AD DS

Created and organized OUs, added users, and synchronized with Microsoft Entra ID (Azure AD Connect)

Phase 3: Microsoft Intune Integration & Windows Autopilot Provisioning

Configured Intune as the MDM authority

Enrolled Windows devices and created compliance/configuration policies

Captured hardware hashes for Autopilot and created deployment profiles

Phase 4: Exchange Online Setup & Email Infrastructure Deployment

Configured Exchange Online with user mailboxes, shared mailboxes, distribution groups

Set up mail flow rules, retention policies, anti-spam, and anti-phishing controls

Phase 5: Group Policy & Security Baselines – Hybrid Endpoint Hardening (On-Prem GPO + Intune)

Applied Group Policy Objects (GPOs) and Intune-based security baselines for devices

Configured password policies, BitLocker, Defender settings, Windows Update, and registry edits

Phase 6: Deploy osTicket on Docker (Windows Host)

Deployed the osTicket helpdesk system on Docker on Windows

Integrated with Exchange Online for ticket auto-import via IMAP

Phase 7: Enterprise Security & Mobility Stack

Integrated enterprise-level security and mobility solutions

Configured Microsoft Defender for Endpoint, hybrid file sharing with OneDrive, and Entra ID SSO for third-party apps

Phase 8: Apple Device Management with Jamf Now

Integrated Jamf Now with Apple Business Manager (ABM) for Apple device management

Configured blueprints, security policies, and deployed apps to Apple devices

Phase 9: VPN Access & Secure RDP Jump Box

Deployed WireGuard VPN server for secure remote access

Configured Windows Server 2022 Jump Box for RDP access with Multi-Factor Authentication (MFA)

Phase 10: Certificate Authority (CA) and Certificate Templates

Set up an Enterprise Root CA on Windows Server

Configured certificate templates for BitLocker, VPN, Wi-Fi, and device authentication

Configured auto-enrollment using GPO and Intune

Phase 11: Disaster Recovery Planning

Designed and implemented backup and restore strategies using on-prem and cloud-based solutions

Configured backup services, automated backups, and disaster recovery (DR) testing

Phase 12: Enterprise Wi-Fi Deployment with NPS and RADIUS

Configured Network Policy Server (NPS) for RADIUS authentication

Integrated certificate-based Wi-Fi authentication with 802.1X for secure wireless access

Phase 13: Advanced Security Configurations

Implemented advanced security measures, including BitLocker for device encryption

Applied device-based policies through Intune and GPOs to enforce security on endpoints

Phase 14: Multi-Factor Authentication (MFA) Integration

Deployed MFA for secure access to corporate resources

Configured conditional access policies to require MFA for high-risk actions

Phase 15: Device Autopilot and Imaging

Configured Windows Autopilot for automated device provisioning

Created device profiles for seamless enrollment and setup

Phase 16: Endpoint Detection and Response (EDR) with Defender for Endpoint

Full integration of Microsoft Defender for Endpoint with automated threat detection and response

Enabled device health monitoring and incident reporting

Phase 17: Hybrid Cloud Storage & File Sharing

Integrated hybrid file sharing with File Server and OneDrive for Business

Applied Known Folder Move (KFM) for automatic file redirection to OneDrive

Phase 18: Windows 365 Cloud PCs Setup

Configured and provisioned Windows 365 Cloud PCs for virtual desktop infrastructure

Enabled cloud-based desktop management for seamless user experience

Phase 19: Full IT Infrastructure Automation and Monitoring

Implemented monitoring solutions for proactive issue detection and resolution

Automated IT infrastructure provisioning and management using PowerShell and other scripts

Prerequisites
Before running or exploring this project, ensure you have the following:

A Microsoft 365 E5 Developer Tenant (free for development purposes)

Access to Microsoft Azure for Entra ID (formerly Azure AD) and other services

Windows Server 2022 or similar VM for AD DS and other server roles

Knowledge of Microsoft Intune, Group Policy, and cloud-based IT solutions

Basic understanding of IT security practices and endpoint management

Installation and Setup
Clone the repository:

bash
Copy
git clone https://github.com/your-username/hybrid-it-infrastructure-simulation.git
cd hybrid-it-infrastructure-simulation
Follow the detailed step-by-step documentation:
Each phase includes specific instructions for setup, configurations, and tools used. The documentation is organized in directories corresponding to each phase of the project.

Ensure prerequisites are met:
Some phases require access to specific cloud resources or tools. Be sure to set up Microsoft 365, Intune, and other tools as needed.

Contributions
Feel free to fork the repository, submit pull requests, or contribute improvements. If you notice any issues or have suggestions, please open an issue on GitHub.

License
This project is open-source and released under the MIT License. See the LICENSE file for more information.

Acknowledgments
Microsoft for providing cloud services like Entra ID, Exchange Online, and Intune.

Jamf for Apple device management solutions.

Docker for containerization solutions used in the project.

Community contributions and resources that have helped guide the setup process.

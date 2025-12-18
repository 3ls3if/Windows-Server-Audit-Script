# Windows-Server-Audit-Script
A comprehensive PowerShell-based security auditing tool for Windows systems that generates detailed HTML reports with security findings, risk assessments, and remediation recommendations.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Report Sections](#report-sections)
- [Configuration](#configuration)
- [Security Scoring](#security-scoring)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Windows Security Auditor is a PowerShell script that performs comprehensive security assessments of Windows systems. It analyzes system configuration, installed applications, security settings, event logs, and detects security software like EDR (Endpoint Detection and Response) and backup solutions. The tool generates an interactive HTML report with detailed findings and remediation recommendations.

## Features

### 🛡️ **Security Analysis**
- **System Information**: OS details, hardware specs, uptime, domain membership
- **Security Configuration**: Firewall status, UAC settings, SMB protocols, Windows Defender
- **User & Group Analysis**: Local users, Administrators, Remote Desktop Users
- **Network Configuration**: IP addresses, DNS, gateways, MAC addresses

### 🔍 **Threat Detection**
- **Installed Applications**: Security scoring based on vendor reputation
- **Startup Applications**: Analysis of auto-start programs with risk classification
- **Security Events**: Review of Windows Event Logs for critical events
- **EDR Detection**: Sophos and other Endpoint Detection & Response solutions
- **Backup Solution Detection**: Acronis and other backup software monitoring

### 📊 **Reporting**
- **Interactive HTML Report**: Collapsible sections, search functionality
- **Security Scoring**: Overall security score with color-coded risk levels
- **Executive Summary**: Quick overview with priority actions
- **Detailed Findings**: Severity-based findings with remediation steps
- **Statistics Dashboard**: Visual representation of security posture

### 🛠️ **Technical Features**
- **Robust Error Handling**: Continues execution even when components fail
- **Exception Management**: Comprehensive error logging and reporting
- **Domain Controller Support**: Special checks for AD environments
- **Extensible Architecture**: Easy to add new detection modules

## Installation

### Prerequisites
- **Windows PowerShell 5.1+** or **PowerShell 7+**
- **Administrator privileges** (recommended for full access)
- **Execution Policy**: Set to `RemoteSigned` or use `Bypass` for execution

### Download Options

#### Option 1: Copy Paste the Script in Powershell with Admin Privileges(Recommended)
```powershell
# Download the latest version
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/3ls3if/Windows-Server-Audit-Script/refs/heads/main/server_audit.ps1" -OutFile "SecurityAudit.ps1"




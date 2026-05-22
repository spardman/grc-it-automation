# GRC IT Automation Workflow

## Project Overview
This repository contains automation tools and PowerShell scripts designed to streamline Governance, Risk, and Compliance (GRC) processes. It automates continuous compliance monitoring, policy synchronization, and risk tracking.

## Core Features
* **Automated Policy Sync**: Synchronizes compliance policies directly via the command line.
* **Continuous Monitoring**: CI/CD workflows track compliance states automatically.
* **Data Integration**: Processes risk register updates into flat data formats (.csv).

## Automation & Scripts
### 1. Environment Setup (`ad_setup.ps1`)
This PowerShell script configures the initial environment baseline required for auditing.
* **What it does**: Provisions Active Directory department structures and forces the deployment of target audit policies.
* **How to run it**:
```powershell
.\ad_setup.ps1
```

## GitHub Actions Workflows
The project utilizes automated workflows located in `.github/workflows/`:
* **GRC Audit Workflow**: Runs on a schedule or trigger to validate system state.
* **Dependencies**: Includes automated steps to install required modules (such as `pandas` for Python data processing).

## Getting Started
1. Clone this repository:
   ```bash
   git clone https://github.com/spardman/grc-it-automation.git
   ```
2. Open PowerShell as an Administrator.
3. Run the setup script to initialize the environment.

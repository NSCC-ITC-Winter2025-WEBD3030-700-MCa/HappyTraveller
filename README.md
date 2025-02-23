# Hugo Installation Guide

This document provides clear and concise steps to install Hugo on both Windows and macOS.

## Prerequisites
- **Hugo** (`hugo_extended`) from [GitHub Releases](https://github.com/gohugoio/hugo/releases)
  - *Recommended:* Latest version or at least version X.X.X
- **Visual Studio Code** or another code editor
- **Command-line interface** (Command Prompt, PowerShell, or Terminal)
- Basic knowledge of command-line operations

---

## Installation on Windows

### 1. Using ZIP File:
- Navigate to `C:\Program Files` and create a folder named `Hugo`.
- Inside `Hugo`, create a `bin` folder.
- Download the latest `hugo_extended` version for Windows (.zip file).
- Extract the downloaded file and move the contents to `C:\Program Files\Hugo\bin`.
- Set Environment Variables:
    - Open **Start Menu** > **Environment Variables** > **Edit the system environment variables**.
    - Click **Environment Variables** > **System Variables** > **Path** > **Edit**.
    - Click **New** and add `C:\Program Files\Hugo\bin`.

### 2. Using Chocolatey:
- Open PowerShell as Administrator:
    ```bash
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = 
    [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
    ```
- Install Hugo:
    ```bash
    choco install hugo -y
    ```

### 3. Verify Installation:
```bash
hugo version

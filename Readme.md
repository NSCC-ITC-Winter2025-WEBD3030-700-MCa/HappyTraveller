# Hugo Installation for Windows
This document provides step-by-step instructions to set up Hugo on a Windows, and Mac machine and prepare your project for contribution by the GitHub community.

## Prerequisites

Before installing Hugo, ensure you have the following:

- **Hugo** (`hugo_extended`) downloaded from the [GitHub Releases](https://github.com/gohugoio/hugo/releases) page  
  - *Recommended:* Latest version or at least version X.X.X (if applicable)  
- **Visual Studio Code** (or any code editor of your choice)  
- **Command-line interface** (e.g., Command Prompt, PowerShell)  
- **Basic understanding of command-line operations**  


Always use the hugo_extended version for advanced features and better compatibility.
Ensure your contributions follow the project guidelines and coding standards.



***Below is the instruction to install Hugo for Windows***

1. Go to Windows PowerShell in Administration view

2. Run: choco --version (To check for chocolaty.)

If chocolaty is installed, navigate to the location of the cloned folder, then run:

3. choco install hugo-extended
4. hugo verison (If Hugo is correctly installed, you should see the version information.)
5. hugo server
6. Then navigate to the localhost's port.
EX: http://localhost:1313


If chocolaty is not installed run:

1. Set-ExecutionPolicy Bypass -Scope Process -Force
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.SecurityProtocolType]::Tls12;
iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

This will allow you to download choclaty with elevated privilages. These are needed for properly running the site.

Afterwards, check the installation suceeced by running:
2. choco --version
3. Navigate to the location of the cloned folder, and run the following commands.
4. choco install hugo-extended
5. hugo verison (If Hugo is correctly installed, you should see the version information.)
6. hugo server
7. Then navigate to the localhost's port.
EX: http://localhost:1313



***Below is the instruction to install Hugo in MacOS***
1. Install Homebrew (If Not Installed)

Hugo is best installed using Homebrew. If you don’t have Homebrew installed, run this command in the terminal:

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

2. Install Hugo

Once Homebrew is installed, use the following command to install Hugo:

brew install hugo

3. Verify Installation

Check if Hugo is installed correctly by running:

hugo version

This should output the installed Hugo version, confirming a successful installation.
Alternative Installation: Download Binary

If you prefer not to use Homebrew, you can manually download Hugo:

Go to the official Hugo Releases page.

Download the macOS binary (hugo_extended_x.x.x_macOS-universal.tar.gz).

Extract the archive and move the hugo binary to /usr/local/bin:

tar -xvzf hugo_extended_x.x.x_macOS-universal.tar.gz


mv hugo /usr/local/bin/

Verify installation using:

hugo version



Another way:
Step 1: Open PowerShell as Administrator

    Press Win + X

    Click Windows Terminal (Admin) or PowerShell (Admin)

    Run the following command to install Chocolatey (if not installed already):

    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

    Restart your terminal after installation.

Step 2: Install Hugo

Once Chocolatey is installed, run the following command:

choco install hugo -y

Step 3: Verify Installation

After installation, check the installed Hugo version:

hugo version

✅ If successful, you will see output like:

hugo v0.142.0-xxxxxx windows/amd64 BuildDate=xxxx
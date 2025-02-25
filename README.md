
# Happy Traveller
 
## Overview
Your ultimate destination for planning unforgettable journeys and discovering the world's hidden gems. Whether you're a seasoned explorer or a first-time traveler, we’re here to make your adventures seamless, exciting, and memorable.

 
## Features
- Travel Guides: Expertly curated guides to help you explore destinations like a local.
- Trip Planning Tools: Easily organize your itinerary, book accommodations, and find the best deals.
- Inspiration: Stunning photos, travel stories, and tips to fuel your wanderlust.
- Community: Connect with fellow travelers, share experiences, and get personalized recommendations.

## Hugo Installation for Windows

## Prerequisites

Before installing Hugo, ensure you have the following:

- **Hugo** (`hugo_extended`) downloaded from the [GitHub Releases](https://github.com/gohugoio/hugo/releases) page  
  - *Recommended:* Latest version or at least version X.X.X (if applicable)  
- **Visual Studio Code** (or any code editor of your choice)  
- **Command-line interface** (e.g., Command Prompt, PowerShell)  
- **Basic understangitding of command-line operations**  

## Installation Instructions

### 1. Create Directory Structure:
- Navigate to the root directory (`C:\Program Files`).
- Create a folder named `Hugo` (with a capital H).
- Inside the `Hugo` folder, create another folder named `bin`.

### 2. Download Hugo:
- Visit the [Hugo GitHub Releases Page](https://github.com/gohugoio/hugo/releases).
- Locate the latest release and download the `hugo_extended` version for Windows.
- Ensure you select the appropriate file ending with `.zip`.

### 3. Extract Hugo Files:
- Extract the contents of the downloaded zip file.
- Copy the extracted files into the `bin` folder created earlier (`C:\Program Files\Hugoin`).

### 4. Set Environment Variables:
- Open the Start Menu and search for **Environment Variables**.
- Select **Edit the system environment variables**.
- Click the **Environment Variables** button.
- Under **System Variables**, find and select the **Path** variable, then click **Edit**.
- Click **New** and add the path to the `bin` folder (`C:\Program Files\Hugoin`).
- Click **OK** to close all dialog boxes.

### 5. Verify Installation:
- Open **Command Prompt** (`cmd`).
- Type the following command and press Enter:
  ```bash
  hugo version
  ```
- If Hugo is correctly installed, you should see the version information.

### 6. Run the Application:
- Open the cloned folder in **VS Code** and to run the web application, press the following command:
  ```bash
  hugo server
  ```

## Important Notes
- Always use the `hugo_extended` version for advanced features and better compatibility.
- Ensure your contributions follow the project guidelines and coding standards.

---

## Hugo Installation for macOS

### 1. Install Homebrew (If Not Installed)
Hugo is best installed using Homebrew. If you don’t have Homebrew installed, run this command in the terminal:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 2. Install Hugo
Once Homebrew is installed, use the following command to install Hugo:
```bash
brew install hugo
```

### 3. Verify Installation
Check if Hugo is installed correctly by running:
```bash
hugo version
```
This should output the installed Hugo version, confirming a successful installation.

### Alternative Installation: Download Binary

If you prefer not to use Homebrew, you can manually download Hugo:

- Go to the official [Hugo Releases page](https://github.com/gohugoio/hugo/releases).
- Download the macOS binary (`hugo_extended_x.x.x_macOS-universal.tar.gz`).
- Extract the archive and move the Hugo binary to `/usr/local/bin`:
  ```bash
  tar -xvzf hugo_extended_x.x.x_macOS-universal.tar.gz
  mv hugo /usr/local/bin/
  ```

Verify installation using:
```bash
hugo version
```

-run using 
hugo server 

## Hugo installation for Linux-based operating systems:
### 1. Install repository package
**Alpine:** `doas apk add --no-cache --repository=https://dl-cdn.alpinelinux.org/alpine/edge/community hugo`

**Arch:** `sudo pacman -S hugo`

**Debian:** `sudo apt install hugo`

**Fedora:** `sudo dnf install hugo`

*For more information, visit the [Hugo Linux Installation page](https://gohugo.io/installation/linux/)*

Verify installation using `hugo version`

-run using `hugo server` 

### Contributing
Fork the repository.
Create a new branch (feature-branch)
Commit your changes.
Push to your branch and submit a pull request.
 
## Live Site
Visit the live website here: [HappyTraveller](https://happytraveller2.onrender.com/)

### Licence
Copyright 2025



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

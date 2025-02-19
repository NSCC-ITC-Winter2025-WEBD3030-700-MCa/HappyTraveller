# Hugo Installation for Windows
This document provides step-by-step instructions to set up Hugo on a Windows machine and prepare your project for contribution by the GitHub community.

## Prerequisites

Before installing Hugo, ensure you have the following:

- **Hugo** (`hugo_extended`) downloaded from the [GitHub Releases](https://github.com/gohugoio/hugo/releases) page  
  - *Recommended:* Latest version or at least version X.X.X (if applicable)  
- **Visual Studio Code** (or any code editor of your choice)  
- **Command-line interface** (e.g., Command Prompt, PowerShell)  
- **Basic understanding of command-line operations**  


Installation Instructions
1.Create Directory Structure:
Navigate to the root directory (C:\Program Files).
Create a folder named Hugo (with a capital H).
Inside the Hugo folder, create another folder named  bin.
Download Hugo:
Visit the Hugo GitHub Releases Page.
Locate the latest release and download the hugo_extended version for Windows.
Ensure you select the appropriate file ending with .zip.
Extract Hugo Files:
Extract the contents of the downloaded zip file.
Copy the extracted files into the bin folder created earlier (C:\Program Files\Hugo\bin).
Set Environment Variables:
Open Start Menu and search for Environment Variables.
Select Edit the system environment variables.
Click the Environment Variables button.
Under System Variables, find and select the Path variable, then click Edit.
Click New and add the path to the bin folder (C:\Program Files\Hugo\bin).
Click OK to close all dialog boxes.
Verify Installation:
Open Command Prompt (cmd).
Type the following command and press Enter:
    
hugo version

If Hugo is correctly installed, you should see the version information.

Open the cloned folder in VS Code and To run the web application press following command 

hugo server
 
Important Notes
Always use the hugo_extended version for advanced features and better compatibility.
Ensure your contributions follow the project guidelines and coding standards.


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

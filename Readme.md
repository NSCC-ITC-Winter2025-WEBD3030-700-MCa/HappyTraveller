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

1. **Create Directory Structure:**  
   - Navigate to `C:\Program Files` and create a folder named `Hugo`.
   - Inside `Hugo`, create a `bin` folder.

2. **Download Hugo:**  
   - Visit [Hugo GitHub Releases](https://github.com/gohugoio/hugo/releases).
   - Download the latest `hugo_extended` version for Windows (.zip file).

3. **Extract and Move Files:**  
   - Extract the downloaded zip file.
   - Copy the extracted files into `C:\Program Files\Hugo\bin`.

4. **Set Environment Variables:**  
   - Open **Start Menu** > Search **Environment Variables** > Select **Edit the system environment variables**.
   - Click **Environment Variables** > Under **System Variables**, select **Path** > Click **Edit**.
   - Click **New** and add `C:\Program Files\Hugo\bin` > Click **OK** to save.

5. **Verify Installation:**  
   - Open **Command Prompt** and run:
     ```bash
     hugo version
     ```
   - You should see the Hugo version information.

6. **Start Hugo Server:**  
   - Open the cloned project folder in **VS Code**.
   - Run the following command to start the server:
     ```bash
     hugo server
     ```

---

## Installation on macOS

1. **Install Homebrew (If Not Installed):**  
   Run the following command in Terminal:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Hugo:**  
   ```bash
   brew install hugo
   ```

3. **Verify Installation:**  
   ```bash
   hugo version
   ```
   - You should see the Hugo version information.

4. **Alternative Installation (Without Homebrew):**  
   - Download `hugo_extended_x.x.x_macOS-universal.tar.gz` from [Hugo Releases](https://github.com/gohugoio/hugo/releases).
   - Extract and move the binary:
     ```bash
     tar -xvzf hugo_extended_x.x.x_macOS-universal.tar.gz
     mv hugo /usr/local/bin/
     ```
   - Verify installation:
     ```bash
     hugo version
     ```

---

## Important Notes
- Always use the `hugo_extended` version for advanced features and compatibility.
- Follow project guidelines and coding standards when contributing.


# Hugo Installation
## Windows 10/11
Prerequisites:
- **Hugo** (`hugo_extended`) downloaded from the [GitHub Releases](https://github.com/gohugoio/hugo/releases) page  
    - *Recommended:* Latest version or at least version X.X.X (if applicable)  
- **Visual Studio Code** (or any code editor of your choice)  
- **Command-line interface** (e.g., Command Prompt, PowerShell)  
- **Basic understanding of command-line operations**  
Installation Instructions:
1. Create Directory Structure:
    - Navigate to the root directory (`C:\Program Files`).
    - Create a folder named `Hugo`.
    - Inside the `Hugo` folder, create another folder named `bin`.
2. Download Hugo:
    - Visit the [Hugo](https://github.com/gohugoio/hugo) GitHub Releases Page.
    - Locate the latest release and download the `hugo_extended` version for Windows 10/11.
3. Extract Hugo Files:
    - Extract the contents of the downloaded `.zip` file.
    - Copy the extracted files into the `bin` folder (`C:\Program Files\Hugo\bin`).
4. Set Environment Variables:
    - Open Start Menu and search for Environment Variables.
    - Select Edit the system environment variables.
    - Click the Environment Variables button.
    - Under System Variables, find and select the Path variable, then click Edit.
    - Click New and add the path to the bin folder (`C:\Program Files\Hugo\bin`).
    - Click OK to close all dialog boxes.
5. Verify Installation:
    - Open Command Prompt (cmd).
    - run `hugo version` to view the version of Hugo you have installed.
6. Run web application:
    - from the root of the cloned repository, run `hugo server`
## MacOS
### Homebrew:
- Install Homebrew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- Install Hugo: `brew install hugo`
- Verify Installation: `hugo version`
    - This should output the installed Hugo version, confirming a successful installation.
### Binary
If you prefer not to use Homebrew, you can manually download Hugo:
- Go to the official [Hugo Releases](https://github.com/gohugoio/hugo) page.
- Download the macOS binary (`hugo_extended_x.x.x_macOS-universal.tar.gz`).
- Extract the archive and move the hugo binary to `/usr/local/bin`:
    - `tar -xvzf hugo_extended_x.x.x_macOS-universal.tar.gz`
    - `mv hugo /usr/local/bin/`
- Verify installation using:
    - `hugo version`
## Important Notes
- Always use the `hugo_extended` version for advanced features and better compatibility.
- Ensure your contributions follow the project guidelines and coding standards. All commits should follow [conventional commits](https://www.conventionalcommits.org) standards.
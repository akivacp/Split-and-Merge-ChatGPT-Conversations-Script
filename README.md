# Unified Split and Merge ChatGPT Conversations Script

This PowerShell script helps you split and merge large ChatGPT conversation files exported from your ChatGPT account. It provides an easy way to manage and organize JSON-based conversation data, especially when dealing with large exports.

## Features:
- **File Selection**: Use a Windows file picker dialog to choose your ChatGPT conversation file for processing.
- **Automatic Directory Creation**: Automatically creates a "split" directory to store split conversation files.
- **Installation of `jq`**: Checks if the `jq` tool is installed on your system and prompts you to install it if it's missing. The script does not force installation and allows you to install `jq` manually if you prefer.
- **Split Functionality**: Supports splitting large JSON files into smaller, more manageable pieces based on the content.
- **Multiverse Viewer Integration**: Once you've split your JSON into individual conversation files, you can use the **[Multiverse Viewer](https://github.com/akivacp/chatgpt-json-tree-viewer)** to navigate and explore the conversation data visually.

## Prerequisites:
- **Windows Operating System** (or Windows Subsystem for Linux - WSL if you're using Linux)
- **PowerShell** (pre-installed on Windows)

### Dependencies:
- **`jq`**: A command-line tool used for processing JSON files. The script checks if it's installed, and if not, it provides the option to install it via `winget`.

## Installation:
1. **Clone this repository**:
    ```bash
    git clone https://github.com/yourusername/ChatGPT-Conversations-Split-Merge.git
    ```

2. **Install `jq` manually**:
   - If you do not have `jq` installed on your system, you can install it manually by following these instructions:
     - Visit the [official jq website](https://stedolan.github.io/jq/download/) for installation instructions.
     - Alternatively, on Windows, you can install `jq` using `winget` (Windows Package Manager):
       ```bash
       winget install jqlang.jq
       ```

   **Note**: The script will check for `jq` installation and prompt you to install it automatically, but it will not force the installation.

## Usage:

1. **Run the script**: 
   After cloning the repository and ensuring that `jq` is installed, you can run the PowerShell script:
   ```bash
   .\unified_splitAndMergeChatGPT-Conversations-Public.ps1

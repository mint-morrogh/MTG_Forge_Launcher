# Forge Updater

A Python-based Forge Updater designed for Windows machines, packaged as an executable using PyInstaller. This utility simplifies the process of backing up, downloading, and extracting the latest Forge SNAPSHOT updates directly into your local Forge directory.
## Features

- **Automated Forge Update Process**: Fetches, downloads, and extracts the latest Forge updates with a single click.
- **Automatic Backup**: Backs up existing files in a designated `Backup` folder before updating.
- **Integrated Extractors**: Contains built in extraction tools for both .bz2 and .tar files.
- **Error Handling**: Errors and safety measures to ensure the tool is run in the proper directory and the proper files are downloaded and extracted.

## Installation

Just simply download the forge_updater.exe file

## Usage

1. Ensure the `Forge_updater.exe` is located within your Forge directory. (Your folder that contains 'forge.exe' , 'forge.cmd' , 'forge.sh' and the rest of your Forge files.)
2. Run the executable from within your Forge Directory to open the updater GUI.
3. Click the **Update Forge** button to start the update process.
4. Once the update is complete, you will see a confirmation message.

### Environment

- **Paths**: The updater dynamically uses the path of the executable for icons and resources when frozen as an executable.


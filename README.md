# Forge Updater

A Python-based Forge Updater and Installer designed for Windows machines, packaged as an executable using PyInstaller. This utility simplifies the process of backing up, downloading, and extracting the latest Forge SNAPSHOT updates directly into your local Forge directory.
## Features

- **Automated Forge Update Process**: Fetches, downloads, and extracts the latest Forge version. This also creates a backup of your old version automatically.
- **Automated Forge Fresh Install Process**: Fetches, downloads, and extracts the latest Forge version.
- **Integrated Extractors**: Contains built in extraction tools for both .bz2 and .tar files.
- **Error Handling**: Errors and safety measures to ensure the tool is run in the proper directory, the proper files are downloaded and extracted, and prevents the user from fresh installing Forge if forge files are found in the root directory. 

## Installation

Just simply download the forge_updater.exe file

## Usage

1. Ensure the `Forge_updater.exe` is located within your Forge directory. (Your folder that contains 'forge.exe' , 'forge.cmd' , 'forge.sh' and the rest of your Forge files.)
2. Run the executable from within your Forge Directory to open the updater GUI.
3. Click the **Update Forge** button to start the update process and create a backup, or click the **Install Forge** button to fresh install with the latest version.
4. Once the update or install is complete, you will see a confirmation message prompting you to close the window.

### Environment

- **Paths**: The updater dynamically uses the path of the executable for icons and resources when frozen as an executable.


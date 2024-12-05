# Forge Updater

A Python-based Forge Updater and Installer designed for Windows machines, packaged as an executable using PyInstaller. This utility simplifies the process of backing up, downloading, and extracting the latest Forge SNAPSHOT and RELEASE updates directly into your local Forge directory.
## Features

- **Automated Forge Update Process**: Fetches, downloads, and extracts the latest Forge versions. This also creates a backup of your old versions automatically.
- **Integrated Extractors**: Contains built in extraction tools for both .bz2 and .tar files.
- **Error Handling**: Errors and safety measures to ensure the tool is run in the proper directory, the proper files are downloaded and extracted, and prevents the user from fresh installing Forge if forge files are found in the root directory. 

## Installation

Just simply download the forge_updater.exe file.

## Usage

1. Ensure the `Forge_updater.exe` is located within your Forge SNAPSHOT directory. (Your folder that contains 'forge.exe' , 'forge.cmd' , 'forge.sh' and the rest of your Forge files.) if this is a fresh install, place this in its own folder where you would like Forge to be installed.
2. Run the executable from within your Forge Directory to open the updater GUI.
3. Click the **Update Forge** button to start the update process for both SNAPSHOT and RELEASE version, and create a backup. If this is a fresh install, click the **Install Forge** button.
4. Once the update or install is complete, you will see a confirmation message prompting you to close the window, please wait until this message appears as these files can take some time depending on your network speed.

### Environment

- **Paths**: The updater dynamically uses the path of the executable for icons and resources when frozen as an executable. No need to point to any paths!


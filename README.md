# Forge Launcher

EDIT: Used to be "Forge Updater" but now it includes a Launcher so I've decided to rename the repo.

A Python-based Forge Updater, Installer, and Launcher designed for Windows machines, packaged as an executable using PyInstaller. This utility simplifies the process of backing up, downloading, launching, and extracting the latest Forge SNAPSHOT and RELEASE updates directly into your local Forge directory.

## Features

- **Automated Forge Update Process**: Fetches, downloads, and extracts the latest Forge versions. This also creates a backup of your old versions automatically.
- **Integrated Extractors**: Contains built-in extraction tools for both `.bz2` and `.tar` files.
- **Error Handling**: Includes safety measures to ensure the tool is run in the proper directory, the proper files are downloaded and extracted, and prevents the user from fresh installing Forge if forge files are found in the root directory.
- **Java Version Handler**: Added a Java version check on launch to make sure the user has a compatible version installed, and if not, will easily fetch the correct version.
- **Dynamic Memory Allocation**: The heap memory (up to 50% of available RAM or capped at 32GB) is allocated to the Java process only for the game runtime. If the game requires more memory within that limit, Java will adjust the heap size dynamically during the runtime.
- **Game-Specific Additions**: Any runtime configuration provided via the `-D` options (like reflection accessibility, encoding, or module permissions) is applied to the game process as long as it’s running.
- **External Dependencies Management**: If your game needs additional system resources (e.g., graphics, I/O), those will be managed by the game and Java process while it’s running. When the game is closed, all memory and resources are released.
- **GUI Exit Behavior**: The launcher GUI now exits immediately after launching the game, ensuring no redundant processes linger in the background.

## Installation

Simply download the `forge_updater.exe` file.


## Usage for Updating

1. Ensure the `forge_updater.exe` is located within your Forge SNAPSHOT directory (the folder containing `forge.exe`, `forge.cmd`, `forge.sh`, and the rest of your Forge files). For a fresh install, place this in a new folder where you want Forge to be installed.
2. Run the executable from within your Forge directory to open the updater GUI.
3. If "Java Version is Unsupported" is shown in the bottom right of the GUI, click on that message and the launcher will download Java 17 for you, simply run that Java 17 installer and then restart the Launcher. 
4. Click the **Update Forge** button to start the update process for both SNAPSHOT and RELEASE versions and create a backup. For a fresh install, click the **Install Forge** button.
5. Once the update or install is complete, a confirmation message will prompt you to close the window. Please wait for this message as the process may take time depending on your network speed.


## Usage for Launching (After Updating)

1. Ensure the `forge_updater.exe` is located within your Forge SNAPSHOT directory (the folder containing `forge.exe`, `forge.cmd`, `forge.sh`, and the rest of your Forge files).
2. `Launch Snapshot` or `Launch Release` will launch the game using an imbedded bash script with better memory allocation for newer systems.


### Environment

- **Paths**: The updater dynamically uses the path of the executable for icons and resources when frozen as an executable. There is no need to manually configure paths!

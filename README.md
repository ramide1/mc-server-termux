# Minecraft Server on Termux
This script allows you to easily set up and run a Minecraft server on your Android device using Termux. It supports Paper, Purpur, DivineMC, Fabric, Folia, Vanilla and Spigot server types, and automates the installation of Java, downloading the server files, and configuring the server.
# Features
Automatic Java Installation: Installs the correct version of Java (OpenJDK 21) for your server.
Storage Permissions: Requests and sets up storage permissions for Termux.
Customizable Server Directory: Lets you choose where to store your Minecraft server files.
RAM Allocation: Allows you to specify how much RAM to allocate to the server.
Server Type Selection: Supports Paper, Purpur, and Fabric server types.
Automatic EULA Acceptance: Automatically accepts the Minecraft EULA.
Easy-to-Use Command: Creates a mcserver command to start your server with a single command.
# Requirements
Termux: Make sure you have Termux installed on your Android device.
Internet Connection: The script requires an active internet connection to download dependencies and server files.
# Installation
To set up your Minecraft server, simply run the following command in Termux:
```bash
curl -s -o ~/x https://raw.githubusercontent.com/ramide1/mc-server-termux/main/install && . ~/x
```
This command will:
Download the installation script.
Execute the script to set up your Minecraft server.
# Usage
After running the installation script, follow the on-screen instructions to:
Choose a directory for your server.
Select the amount of RAM to allocate.
Pick the server type (Paper, Purpur, or Fabric).
Specify the Minecraft version.
Once the setup is complete, you can start your server at any time by typing:
```bash
mcserver
```
# Customization
RAM Allocation: You can change the allocated RAM by editing the mcserver script located at $PREFIX/bin/mcserver.
Server Directory: The server files are stored in the directory you specified during setup (e.g., ~/storage/shared/your_directory_name).
# Troubleshooting
Java Installation Issues: If Java fails to install, ensure your Termux environment is up to date by running pkg update && pkg upgrade.
Storage Permissions: If storage permissions are not granted, the script will exit. Make sure to allow Termux access to your device's storage.
Server Download Issues: If the server fails to download, check your internet connection and ensure the specified Minecraft version is valid.
# Notes
This script is designed for Termux and may not work on other environments.
The mcserver command is created for convenience and can be overwritten if the script is run multiple times.
# Support
If you encounter any issues or have suggestions for improvement, feel free to open an issue on the GitHub repository.

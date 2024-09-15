# linux-commands

## Update software
To update Visual Studio Code (VS Code) to the latest version on your Ubuntu system, you can follow these steps:

   #### Method 1: Using the Command Line

   1. **Open the Terminal**: You can do this by pressing `Ctrl + Alt + T` or searching for "Terminal" in your applications menu.

   2. **Check for updates**: Run the following commands to ensure your package list is up to date:
   ```bash
   sudo apt update
   ```

   3. **Upgrade VS Code**: If you installed VS Code via the official Microsoft repository, you can upgrade it with:
   ```bash
   sudo apt upgrade code
   ```

   #### Method 2: Re-download and Install

   If you didn't install VS Code via the repository or prefer a fresh installation:

   1. **Download the latest .deb package** from the [official VS Code website](https://code.visualstudio.com/Download).

   2. **Navigate to your downloads folder** (or wherever you saved the .deb file):
   ```bash
   cd ~/Downloads
   ```

   3. **Install or update VS Code** using `dpkg`:
   ```bash
   sudo dpkg -i code_*.deb
   ```

   4. If there are missing dependencies, run:
   ```bash
   sudo apt --fix-broken install
   ```

   #### Method 3: Using the Snap Package

   If you installed VS Code via Snap, you can update it with:

1. **Run the following command** to update the Snap package:
   ```bash
   sudo snap refresh code
   ```

After updating, you can verify the version by opening VS Code and checking the version under **Help > About**.

# Create folder
To create a folder with a name containing a space (like "adjacency matrix"), you need to wrap the folder name in quotes. Here's the correct command:

```bash
mkdir "adjacency matrix"
```

Alternatively, you can escape the space with a backslash:

```bash
mkdir adjacency\ matrix
```

This will create a single folder named "adjacency matrix."

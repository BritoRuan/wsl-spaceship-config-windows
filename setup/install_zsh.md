## Installation Steps

**Zsh** (Z shell) is a powerful alternative to the default Linux shell, Bash. Zsh offers features like autocompletion of commands, customizable prompts, and plugin integration.

Follow the steps below to install Zsh on your WSL system.

### 1. Update Repository

Before installing any package, it's recommended to update the repository list to ensure you're getting the latest versions of the packages.

```powershell
sudo apt update
```

### 2. Install Zsh

After updating the repositories, install Zsh with the following command:

```powershell
sudo apt install zsh -y
```

The `-y` flag automatically confirms the installation.

### 3. Set Zsh as Default Shell (Optional)

If you want Zsh to be your default shell instead of Bash, run the following command. This will change your login shell to Zsh.

```powershell
chsh -s $(which zsh)
```

After running this command, log out and log back in. Zsh will start automatically.

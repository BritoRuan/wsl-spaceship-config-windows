# Installing Oh My Zsh on WSL

**Oh My Zsh** is a framework for managing Zsh configurations, which makes it easier to customize and extend your shell with themes and plugins. It enhances the Zsh experience with many built-in features.

Follow the steps below to install **Oh My Zsh** on your WSL system.

## 🚀 Installation Steps

### 1️⃣ **Install Dependencies**

Before installing **Oh My Zsh**, you need to ensure that either **curl** or **wget** is installed, as it will use one of these to download the installation script.

To install **curl**, run:

```powershell
sudo apt install curl -y
```

Or, if you prefer to use wget:

```powershell
sudo apt install wget -y
```

### 2️⃣ **Install Oh My Zsh**

Now that the dependencies are installed, run the following command to download and install Oh My Zsh:

Using curl:

```powershell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Using wget:

```powershell
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

### 3️⃣ **Close and Reopen the Terminal**

After installation, your terminal will automatically restart, and Oh My Zsh will be loaded. If it doesn’t, simply close and reopen your terminal.

Now Oh My Zsh will be installed, and you can enjoy the enhanced Zsh experience with ready-to-use themes and plugins.

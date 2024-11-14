# How to Install WSL on Windows

## Prerequisites

- You must be running Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11 to use the commands below.
- If you are on an older version, please refer to the manual installation guide.

## 🚀 WSL Installation Steps

### 1️⃣ **Open PowerShell or Command Prompt as Administrator**

- Right-click the PowerShell or Command Prompt icon and select "Run as Administrator".

### 2️⃣ **Run the Command to Install WSL**

Run the following command in PowerShell or Command Prompt:

```powershell
wsl --install
```

This command will enable the necessary features to run WSL and install the default Ubuntu Linux distribution. The system will ask you to restart your computer after the installation.

### 3️⃣ **Change the Default Distribution**

By default, Ubuntu will be installed. If you prefer to install another distribution, use the following command:

```powershell
wsl --install -d <Distribution Name>
```

Replace `<Distribution Name>` with the name of the distribution you wish to install (e.g., `Debian`, `Kali`).

To see a list of available distributions, run:

```powershell
wsl --list --online
```

### 4️⃣ **Configure Linux User and Password**

After restarting your computer, when you start the Linux distribution, you will be prompted to create a username and password for the newly installed distribution.

### 5️⃣ **Check WSL Version**

To check the version of WSL that is being run, use the command:

```powershell
wsl -l -v
```

### 6️⃣ **Change WSL Version (Optional)**

New installations of distributions will be set to WSL 2 by default. If you want to change the version of an installed distribution, use the following command:

```powershell
wsl --set-version <Distribution Name> <Version>
```

Replace `<Distribution Name>` with the name of the distribution (e.g., `Ubuntu-20.04`) and `<Version>` with `1` or `2`.

### 7️⃣ **Install Windows Terminal (Recommended)**

For a better experience, install the Windows Terminal. It supports multiple tabs and panes, allowing you to switch between different Linux distributions and other command lines.

### 8️⃣ **Access the Linux Distribution**

You can access your Linux distribution in several ways:

In the Start menu, type the name of the distribution, such as `Ubuntu`.

In PowerShell or Command Prompt, run `wsl` or `wsl -d <Distribution Name>`.

### Additional Tips

To list installed distributions and check the WSL version, use:

```powershell
wsl -l -v
```

- To change the default distribution, use:

```powershell
wsl --set-default <Distribution Name>
```

For more details, refer to [the official WSL documentation](https://docs.microsoft.com/en-us/windows/wsl/).

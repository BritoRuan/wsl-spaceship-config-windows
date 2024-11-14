# Installing the Spaceship Theme on Oh My Zsh

**Spaceship** is a highly customizable and informative theme for **Zsh**, perfect for those who want a visually appealing and informative terminal experience. It displays various useful information, such as the Git repository status, Python environment, machine information, and much more.

Follow the steps below to install the **Spaceship theme** on your **Oh My Zsh** terminal.

## 🚀 Installation Steps

### 1️⃣ **Clone the Theme Repository**

To install the **Spaceship** theme, use the following command to clone the repository directly into the **Oh My Zsh** themes directory with the `--depth=1` option:

```powershell
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
```

### 2️⃣ **Create the Symlink for the Theme**

Now, create a symlink from the spaceship.zsh-theme file to the custom themes directory of Oh My Zsh:

```powershell
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

### 3️⃣ **Edit the .zshrc File**

Next, you will need to edit the Zsh configuration file, `~/.zshrc`, to set the theme to Spaceship.

- Using nano (primary option):

To edit the `~/.zshrc` file directly in the terminal, use the nano editor:

```powershell
nano ~/.zshrc
```

In the `~/.zshrc` file, look for the line that defines the theme and change its value to spaceship. The line should look like this:

```powershell
ZSH_THEME="spaceship"
```

- Using VS Code (optional option):

```powershell
code ~/.zshrc
```

If VS Code is properly set up on your system, this command will open the file directly in the editor.

### 4️⃣ **Apply the Configuration**

After saving and closing the `~/.zshrc` file, apply the changes by running the following command:

```powershell
source ~/.zshrc
```

### 5️⃣ **Customize the Theme (Optional)**

The Spaceship theme is highly customizable. You can adjust various configuration options in the `~/.zshrc` file to change the behavior and appearance of the theme. For more information on customization, refer to [the official Spaceship documentation](https://github.com/spaceship-prompt/spaceship-prompt#configuration).

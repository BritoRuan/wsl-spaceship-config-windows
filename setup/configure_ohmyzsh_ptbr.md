# Instalação do **Oh My Zsh** no WSL

O **Oh My Zsh** é um framework de gerenciamento para o Zsh, que facilita a personalização e a extensão do shell com temas e plugins. Ele melhora a experiência do Zsh, oferecendo diversos recursos prontos para uso.

Siga as etapas abaixo para instalar o **Oh My Zsh** no seu sistema **WSL**.

## 🚀 Etapas de Instalação

### 1️⃣ **Instalar Dependências**

Antes de instalar o **Oh My Zsh**, é necessário garantir que o **curl** ou o **wget** esteja instalado, pois ele usará um desses para baixar o script de instalação.

- Para instalar o **curl**, execute:

```powershell
sudo apt install curl -y
```

### 2️⃣ **Instalar o Oh My Zsh**

Agora que as dependências estão instaladas, execute o seguinte comando para baixar e instalar o Oh My Zsh:

Usando curl:

```powershell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Usando wget:

```powershell
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

### 3️⃣ **Fechar e Reabrir o Terminal**

Após a instalação, o terminal será reiniciado automaticamente e o Oh My Zsh será carregado. Caso contrário, basta fechar e abrir o terminal novamente.

Agora o Oh My Zsh estará instalado e você poderá aproveitar a experiência personalizada do Zsh, com temas e plugins prontos para uso.

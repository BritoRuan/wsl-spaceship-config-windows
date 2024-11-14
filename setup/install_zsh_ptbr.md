# Instalação do Zsh no WSL

O **Zsh** (Z shell) é uma alternativa poderosa ao shell padrão do Linux, o Bash. O Zsh oferece recursos como autocompletar comandos, personalização de prompts e integração com plugins.

Siga as etapas abaixo para instalar o Zsh no seu sistema WSL.

## Etapas de Instalação

### 1. Atualizar o Repositório

Antes de instalar qualquer pacote, é sempre recomendável atualizar a lista de repositórios para garantir que você obtenha a versão mais recente dos pacotes.

```powershell
sudo apt update
```

### 2. Instalar o Zsh

Após atualizar os repositórios, instale o Zsh com o seguinte comando:

```powershell
sudo apt install zsh -y
```

O `-y` é utilizado para confirmar automaticamente a instalação.

### 3. Definir o Zsh como Shell Padrão (Opcional)

Se você deseja que o Zsh seja o shell padrão em vez do Bash, execute o comando abaixo. Isso fará com que o Zsh seja utilizado como shell de login.

```powershell
chsh -s $(which zsh)
```

Após executar este comando, saia da sessão atual e entre novamente. O Zsh será iniciado automaticamente.

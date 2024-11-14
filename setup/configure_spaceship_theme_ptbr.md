# Instalando o Tema Spaceship no Oh My Zsh

O **Spaceship** é um tema altamente personalizável e informativo para o **Zsh**, ideal para quem deseja uma experiência visualmente agradável e informativa no terminal. Ele exibe várias informações úteis, como o estado do repositório Git, o ambiente Python, informações sobre a máquina e muito mais.

Siga as etapas abaixo para instalar o **tema Spaceship** no seu terminal **Oh My Zsh**.

## 🚀 Etapas de Instalação

### 1️⃣ **Clonar o Repositório do Tema**

Para instalar o tema **Spaceship**, use o seguinte comando para clonar o repositório diretamente no diretório de temas do **Oh My Zsh** com a opção `--depth=1`:

```powershell
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
```

### 2️⃣ **Criar o Symlink para o Tema**

Agora, crie um symlink do arquivo spaceship.zsh-theme para o diretório de temas personalizados do Oh My Zsh:

```powershell
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

### 3️⃣ **Editar o Arquivo .zshrc**

Agora, você precisará editar o arquivo de configuração do Zsh, o `~/.zshrc`, para definir o tema como Spaceship.

- Usando o nano (opção principal):

Para editar o arquivo `~/.zshrc` diretamente no terminal, use o editor nano:

```powershell
nano ~/.zshrc
```

No arquivo `~/.zshrc`, procure pela linha que define o tema e altere o valor para spaceship. A linha deve ser modificada da seguinte maneira:

```powershell
ZSH_THEME="spaceship"
```

- Usando o VS Code (opção opcional):

Se preferir editar o arquivo `~/.zshrc` usando o VS Code, use o seguinte comando:

```powershell
code ~/.zshrc
```

Se o VS Code estiver corretamente configurado no seu sistema, esse comando abrirá o arquivo diretamente no editor.

### 4️⃣ **Aplicar as Configurações**

Depois de salvar e fechar o arquivo `~/.zshrc`, aplique as mudanças executando o seguinte comando:

```powershell
source ~/.zshrc
```

### 5️⃣ **Personalizar o Tema (Opcional)**

O Spaceship é altamente personalizável. Você pode ajustar várias opções de configuração no arquivo `~/.zshrc` para alterar o comportamento e a aparência do tema. Para mais informações sobre personalização, acesse a [documentação oficial do Spaceship](https://github.com/spaceship-prompt/spaceship-prompt#configuration).

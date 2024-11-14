# Guia de Instalação do WSL no Windows

## Pré-requisitos

- O Windows 10 versão 2004 ou superior (Build 19041 ou superior) ou o Windows 11 são necessários para usar os comandos abaixo.
- Se você estiver utilizando versões mais antigas, consulte a página de instalação manual.

## 🚀 Passos para Instalar o WSL

### 1️⃣ **Abra o PowerShell ou o Prompt de Comando do Windows como Administrador**

- Clique com o botão direito do mouse no ícone do PowerShell ou Prompt de Comando e selecione "Executar como administrador".

### 2️⃣ **Execute o Comando para Instalar o WSL**

Execute o seguinte comando no PowerShell ou Prompt de Comando:

```powershell
wsl --install
```

Esse comando habilitará os recursos necessários para executar o WSL e instalará a distribuição Ubuntu do Linux. O sistema pedirá para reiniciar o computador após a instalação.

### 3️⃣ **Alterar a Distribuição Padrão**

Por padrão, o Ubuntu será instalado. Se preferir instalar outra distribuição, use o seguinte comando:

```powershell
wsl --install -d <Nome da Distribuição>
```

Substitua `<Nome da Distribuição>` pelo nome da distribuição desejada (exemplo: `Debian`, `Kali`).

Para ver uma lista de distribuições disponíveis, execute:

```powershell
wsl --list --online
```

### 4️⃣ **Configurar Usuário e Senha no Linux**

Após reiniciar o computador, ao iniciar a distribuição do Linux, será solicitado que você crie um usuário e senha para a distribuição recém-instalada.

### 5️⃣ **Verificar a Versão do WSL**

Para verificar a versão do WSL que está sendo executada, execute o comando:

```powershell
wsl -l -v
```

### 6️⃣ **Alterar a Versão do WSL (Opcional)**

As novas instalações de distribuições serão definidas como WSL 2 por padrão. Se quiser mudar a versão de uma distribuição instalada, execute o comando:

```powershell
wsl --set-version <Nome da Distribuição> <Versão>
```

Substitua `<Nome da Distribuição>` pelo nome da distribuição (exemplo: `Ubuntu-20.04`) e `<Versão>` por `1` ou `2`.

### 7️⃣ **Instalar o Terminal do Windows (Recomendado)**

Para uma melhor experiência, instale o **Terminal do Windows**. Ele suporta várias guias e painéis, permitindo que você alterne entre várias distribuições do Linux e outras linhas de comando.

### 8️⃣ **Acessar a Distribuição do Linux**

Você pode acessar sua distribuição do Linux de várias maneiras:

- No menu Iniciar, digite o nome da distribuição, como `Ubuntu`.
- No PowerShell ou Prompt de Comando, execute `wsl` ou `wsl -d <Nome da Distribuição>`.

### Dicas Adicionais

- Para listar as distribuições instaladas e verificar a versão do WSL, use:

```powershell
wsl -l -v
```

- Para mudar a distribuição padrão, use:

```powershell
wsl --set-default <Nome da Distribuição>
```

Para mais detalhes, consulte a [documentação oficial do WSL](https://learn.microsoft.com/pt-br/windows/wsl/install).

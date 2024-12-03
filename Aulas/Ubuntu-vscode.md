# Instalando o VS Code no Ubuntu 24.04 LTS

Para instalar o Visual Studio Code no Ubuntu 24.04 LTS, siga os passos abaixo:

## Passo 0: Instalar Drives Do Virtual Box no UBUNTU 

```bash
sudo apt install bzip2 tar
```

0.1: Clique em Despositivos, Inserir imagem de CD dos adicionais de Convidado

0.2 Clique no Simbolo de CD que apareceu na barra de tarefas, e execute.

## Passo 1: Abrir o Terminal
Abra um terminal usando as teclas `CTRL + ALT + T`.

## Passo 2: Atualizar a Base de Pacotes
Atualize a base de pacotes com o seguinte comando:
```bash
sudo apt update
sudo apt upgrade
sudo apt full-upgrade
sudo apt dist-upgrade
sudo apt autoremove
sudo apt autoclean
sudo apt clean
```

 ## Passo 3: Instalar Pacotes Necessários
Instale alguns pacotes necessários com o seguinte comando:
```bash
sudo apt install wget gpg apt-transport-https
```

## Passo 4: Baixar e Importar as Chaves GPG da Microsoft
Para garantir que os pacotes do Visual Studio Code sejam genuínos, baixe e importe as chaves GPG assinadas pela Microsoft com os comandos:
```bash
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
```

## Passo 5: Adicionar o Repositório do Visual Studio Code
Adicione o repositório oficial do Visual Studio Code ao sistema para garantir atualizações automáticas:
```bash
echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list > /dev/null
```

## Passo 6: Atualizar a Lista de Pacotes
Antes de prosseguir com a instalação, atualize a lista de pacotes:
```bash
sudo snap install --classic code
```

## Passo 7: Instalando e Configurando as Principais Extensões Microsoft Visual Studio Code VSCode

#Instalação das Extensões Básicas do VSCode
Portuguese (Brazil) Language Pack for Visual Studio Code
  Sem necessidade de configuração)
#Code Runner atalho Ctrl + Alt + N

# Instalando o VS Code no Ubuntu 24.04 LTS

Para instalar o Visual Studio Code no Ubuntu 24.04 LTS, siga os passos abaixo:

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
sudo apt install software-properties-common apt-transport-https wget -y
```

## Passo 4: Baixar e Importar as Chaves GPG da Microsoft
Para garantir que os pacotes do Visual Studio Code sejam genuínos, baixe e importe as chaves GPG assinadas pela Microsoft com os comandos:
```bash
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
```

## Passo 5: Adicionar o Repositório do Visual Studio Code
Adicione o repositório oficial do Visual Studio Code ao sistema para garantir atualizações automáticas:
```bash
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```

## Passo 6: Instalando o VSCODE
Comando para Baixar o vscode:
```bash
sudo apt install code
```

## Passo 7: Instalando e Configurando as Principais Extensões Microsoft Visual Studio Code VSCode

### Portuguese (Brazil) Language Pack for Visual Studio Code
  (Sem necessidade de configuração)
### Code Runner
  (Sem necessidade de configuração)

## Passo 8: Faça um comando Simples para executar com o Code Runner dentro do VSCODE com o atalho Ctrl + Alt + N

```bash
let nome = "seunome"
let idade = "suaidade"
console.log(nome, idade)
```
Substitua "seunome" para o seu nome e "suaidade" para sua idade

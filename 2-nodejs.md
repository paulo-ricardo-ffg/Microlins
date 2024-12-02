# Instalando o Node.js no Ubuntu usando o APT

Este método usa o gerenciador de pacotes APT para instalar o Node.js a partir dos repositórios padrão do Ubuntu. É uma maneira simples e que integra bem com o gerenciamento de pacotes do seu sistema.

## 1. Atualizar o Índice de Pacotes
Antes de instalar novos softwares, é uma boa prática atualizar o índice de pacotes para garantir que você obtenha as versões mais recentes disponíveis.
```bash
sudo apt update
sudo apt upgrade
sudo apt full-upgrade
sudo apt dist-upgrade
sudo apt autoremove
sudo apt autoclean
sudo apt clean
```
## 2. Instale o Node.js
Instale o Node.js diretamente usando o APT.
```bash
sudo apt install nodejs
```
Este comando instala o Node.js junto com as dependências necessárias.

## 3. Verifique a instalação
Confirme que o Node.js foi instalado com sucesso verificando a versão instalada.
```bash
node -v
```
Este comando exibe a versão do Node.js instalada.

## 4. Instale o NPM
O npm (Node Package Manager) não está incluído no pacote padrão do Node.js disponível nos repositórios do Ubuntu. Instale-o separadamente.
```bash
sudo apt install npm
```
O npm é essencial para gerenciar pacotes e dependências do Node.js.


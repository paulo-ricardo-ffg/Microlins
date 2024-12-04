# Aula Introdutória: Instalação do Ubuntu em uma Máquina Virtual

Neste guia, você aprenderá como criar uma máquina virtual usando o Oracle VirtualBox e instalar o Ubuntu.

---

## 1. Ativando a Virtualização (VT-x) no BIOS

Antes de começar, você precisa garantir que a virtualização esteja ativada no seu computador:

1. **Reinicie o computador** e, ao iniciar, pressione a tecla **F12** (ou a tecla indicada pelo fabricante, como **Del**, **Esc**, ou **F2**).
2. **Entre na BIOS**. Navegue até a aba **Avançado** ou **Configurações**.
3. **Procure pela opção VT-x** ou **Intel Virtualization Technology** e altere para **ENABLE**.
4. **Salve as alterações** (geralmente pressionando **F10**) e reinicie o computador.

---

## 2. Baixando e Instalando o Oracle VirtualBox

### 2.1. Baixando o VirtualBox

1. Acesse o site oficial do VirtualBox: [VirtualBox](https://www.virtualbox.org/).
2. Clique em **Download** e selecione a versão para o seu sistema operacional (por exemplo, **Windows Hosts** para sistemas Windows).

### 2.2. Instalando o VirtualBox

1. Abra o arquivo de instalação que você baixou.
2. Siga as instruções na tela:
   - Clique em **Next**.
   - Aceite os termos da licença.
   - Continue clicando em **Next** até chegar à opção **Install**.
   - Clique em **Yes** quando solicitado.
   - Finalize clicando em **Finish**.

---

## 3. Baixando a ISO do Ubuntu

### 3.1. Acessando o site oficial

1. Vá para o site oficial do Ubuntu: [Baixar Ubuntu](https://ubuntu.com/download/desktop).
2. Escolha a versão desejada e clique em **Download**.

---

## 4. Configurando a Máquina Virtual no VirtualBox

### 4.1. Criando a Máquina Virtual

1. Abra o **Oracle VirtualBox**.
2. Clique em **Novo** para criar uma nova máquina virtual.
3. Preencha as informações:
   - **Nome**: Ubuntu (ou outro nome que preferir).
   - **Tipo**: Linux.
   - **Versão**: Ubuntu (64-bit).
4. Clique em **Avançar**.

### 4.2. Configurando o Hardware

1. **Memória RAM**: Altere para **2048 MB** (2 GB) ou mais, dependendo da capacidade do seu computador.
2. **Processador**: Altere para **2 núcleos** ou mais (se disponível).
3. Clique em **Avançar**.

### 4.3. Criando o Disco Rígido Virtual

1. Escolha **Criar disco rígido virtual agora**.
2. Selecione:
   - **Tipo do disco**: VDI (VirtualBox Disk Image).
   - **Modo de armazenamento**: Dinamicamente alocado.
   - **Tamanho**: 25 GB ou mais (dependendo do espaço disponível no seu computador).
3. Clique em **Criar**.

### 4.4. Configurando Mouse e teclado Bi-direcional

1. Clique com o botão direito na maquina virtual criada
2. Configurações
3. Geral/Avançado
4. Area de Transferencia Compartilhada, Selecione Bi-direcional
5. Arrastar e soltar, Selecione Bi-direcional
---

## 5. Iniciando a Instalação do Ubuntu

1. Na lista de máquinas virtuais do VirtualBox, selecione a máquina virtual que você criou (Ubuntu).
2. Clique em **Iniciar**.
3. Quando solicitado, selecione o arquivo **ISO do Ubuntu** que você baixou.
4. A instalação do Ubuntu começará. Siga as etapas de instalação:
   - Selecione o idioma, fuso horário, e outras configurações.
   - Quando perguntar sobre o tipo de instalação, escolha **Instalar Ubuntu**.

---

## 6. Atualização

1. Apos a instalação do Ubuntu faça a realização das atualizações atravez do terminal que pode ser acessado apertando CTRL + ALT + T
```bash
 sudo apt update && sudo apt upgrade -y && sudo apt full-upgrade -y && sudo apt dist-upgrade -y && sudo apt autoremove -y && sudo apt autoclean && sudo apt clean
```
2. Instale os Drivers do Virtual Box

2.1. Clique em Dispositivos, Inserir Imagem de CD dos Adicionais para Convidado, Clique duas vezes no Disco que agora aparece na barra de tarefas, Abra o terminal e digite 
```bash
sudo apt install bzip2 tar
```

2.2 Clique em Executar Disco

---

## Atalho importante:

- Para **liberar o mouse** da máquina virtual, pressione **Ctrl + Alt**.

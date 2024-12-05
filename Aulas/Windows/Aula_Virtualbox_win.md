# Aula Introdutória: Instalação do Windows 10 em uma Máquina Virtual

Neste guia, você aprenderá a configurar uma máquina virtual usando o **Oracle VirtualBox** e instalar o **Windows 10**. 

---

## **1. Ativando a Virtualização (VT-x) no BIOS**

1. Reinicie o computador e pressione **F12** (ou outra tecla indicada, como `Del`, `Esc` ou `F2`, dependendo do fabricante).
2. No menu da BIOS, vá até a aba **Avançado**.
3. Procure pela opção **VT-x** (ou **Intel Virtualization Technology**) e altere para **ENABLE**.
4. Salve as alterações (normalmente pressionando **F10**) e reinicie o computador.

---

## **2. Baixando e Instalando o Oracle VirtualBox**

### **2.1. Baixando o VirtualBox**
1. Acesse o site oficial: [VirtualBox](https://www.virtualbox.org/).
2. Clique em **Download**.
3. Escolha a opção **Windows Hosts**

### **2.2. Instalando o VirtualBox**
1. Abra o arquivo baixado.
2. Siga os passos da instalação:
   - Clique em **Next**.
   - Aceite os termos da licença (**I Accept the Terms in the License Agreement**) e clique em **Next** até chegar na opção **Install**.
   - Clique em **Yes** quando solicitado e finalize clicando em **Finish**.

---

## **3. Baixando a ISO do Windows 10**

### **3.1. Acessando o site oficial**
1. Acesse: [Baixar Windows 10](https://www.microsoft.com/pt-br/software-download/windows10).
2. Na seção **Criar mídia de instalação do Windows 10**, clique em **Baixar agora**.

### **3.2. Criando a ISO**
1. Abra o arquivo baixado e clique em **Sim** para iniciar.
2. Aceite os termos de uso e clique em **Avançar**.
3. Na janela **O que você deseja fazer?**, escolha a opção **Criar mídia de instalação (pen drive, DVD ou arquivo ISO)** e clique em **Avançar**.
4. Confirme que a opção **Usar as opções recomendadas para este computador** está marcada e clique em **Avançar**.
5. Na janela **Escolha a mídia a ser usada**, selecione **Arquivo ISO** e clique em **Avançar**.
6. Escolha onde salvar o arquivo e aguarde o download ser concluído.

---

## **4. Configurando a Máquina Virtual**

### **4.1. Criando a Máquina Virtual**
1. Abra o **Oracle VirtualBox**.
2. Clique em **Novo**.
3. Preencha as informações:
   - **Nome:** *Win 10 Microlins* .
   - **Imagem ISO:** Selecione o arquivo ISO baixado anteriormente.
   - Marque a opção **Pular Instalação Desassistida**.

### **4.2. Configurando o Hardware**
1. **Memória RAM:** Defina como **4096 MB (4 GB)**.
2. **Núcleos do Processador:** Altere para **4 núcleos** (se disponível).

### **4.3. Criando o Disco Rígido Virtual**
1. Escolha a opção **Criar disco rígido virtual agora**.
2. Selecione:
   - **Tipo do disco:** VDI (VirtualBox Disk Image).
   - **Modo de armazenamento:** Dinamicamente alocado.
   - **Tamanho:** **50 GB**.
3. Clique em **Criar** para finalizar.

---

## **5. Iniciando a Máquina Virtual**
1. Na lista de máquinas virtuais, clique na que você criou.
2. Clique em **Iniciar**.
3. O instalador do Windows será carregado. Siga as etapas de instalação.
4. Apos a Instalação do Windows deverá ser realizado a instalação dos Drives de Convidados do Virtualbox, Para isso Clique Dispositivos , Inserir Imagem de CD dos Adicionais para Convidado e no Gerenciador de Arquivos do Windows execute o Disco.
---

## **6. Conclusão**
Após finalizar a instalação do Windows, sua máquina virtual estará pronta para uso! O sistema operacional rodará de forma isolada, sem interferir na sua máquina física. Você pode experimentar configurações e aplicativos com segurança.

> **Atalho importante:** Para liberar o mouse da máquina virtual, pressione **Ctrl + Alt**.


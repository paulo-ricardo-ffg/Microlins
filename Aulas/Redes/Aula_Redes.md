# AULA DE REDES

## Introdução a conceitos básicos de rede

**Redes:** Dispositivos conectados que conseguem transmitir dados e recursos um para o outro.

### Rede LAN
Rede Local, a mesma usada em sua casa ou em escolas, consiste em dispositivos que transmitem dados entre si localmente.

### Rede WAN
Rede de longa distância que conecta diversas redes locais (LANs) e outros sistemas, como servidores, permitindo a transmissão de dados a grandes distâncias, consiste em dispositivos que transmitem dados a longa distância.

## Conceitos

### Host Name (Nome do Host)
Refere-se ao nome da sua máquina na rede.

### IP (Endereço IP)
Comparável ao "CPF" da máquina, é um número que identifica sua máquina dentro da rede. Pode ser alterado manualmente.

### MAC Address
Similar ao "RG", é um número único que identifica a placa de rede do seu computador, não podendo ser alterado.

### TCP/IP (Protocolo de Controle de Transmissão/Protocolo de Internet)
É um protocolo que permite configurar as propriedades de rede, como o endereço IP, IP público e gateway.

### Gateway (Roteador)
O gateway (roteador) funciona como uma porta de entrada e saída de dados, permitindo a comunicação entre redes, como a rede local (LAN) e a internet (WAN). O gateway possui um IP próprio na rede local, e o IP público atribuído pelo provedor de internet. O IP público é aquele que é usado para acessar um site.

### DNS
Converte o nome que o usuário digita no navegador em um IP para se comunicar com o site. Alguns DNS bloqueiam certos sites.

### ICMP (Protocolo de Mensagens de Controle da Internet)
Facilita a comunicação entre computadores na rede, permitindo a realização de diagnósticos básicos e testes, como saber se está ocorrendo perda de informações na rede.

## Comandos Básicos para Teste em Redes

- **`ipconfig /all`**  
  Mostra todas as configurações de rede do computador.

- **`hostname`**  
  Exibe o nome da máquina.

- **`net view`**  
  Exibe os computadores conectados à rede.

- **`net send`**  
  Envia uma mensagem para um computador específico na rede. Para isso, o serviço "mensagem" precisa estar ativado.

- **`tracert [nomedosite.com]`**  
  Mostra a rota que o computador faz até chegar ao site indicado.

- **`ping [nomedosite.com]`**  
  Testa a conectividade do seu desktop até o site informado.

## Mão na massa

Baixe o [VirtualBox](https://www.virtualbox.org/)
e com o auxilio do professor Baixe a [ISO do Windows XP](https://drive.google.com/file/d/1MomeTvtlHJhn48us-nhfQ4lJ7GrWMwH8/view?usp=sharing)


Como Alterar o Hostname Windows XP

```
pressionando Win + Pause/Break
Vá para a Aba "Nome do Computador":

Quando a janela Propriedades do Sistema abrir, clique na aba Nome do Computador.
```
![HOSTNAMEIMAGEM](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM1.png?raw=true)


Como Compartilhar uma Pasta na Rede

```
Clique com o Botão direito na pasta desejada e selecione Propriedades
Apos isso clique em Compartilhamento
Marque a Opção Compartilhar esta Pasta na Rede
```

![COMPARTILHAMENTOPASTA](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM3.png?raw=true)
```
Observação: Para o compartilhamento funcionar corretamente, o computador precisa ter um endereço IP fixo, configurado nas propriedades do protocolo IPv4 (TCP/IP).
```
![image](https://github.com/user-attachments/assets/ea4a73ce-3b82-4fb1-932a-c734a6ec320a)

Mapeamento de Pastas na Rede:

```
Em Outro Computador na Rede Clique com o botão direito na pasta compartilhada e selecione Mapear Unidade.
```
![MAPEAMENTOPASTA](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM4.png?raw=true)

```
Escolha uma letra para a unidade mapeada.
```
![LETRAUNIDADE](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM5.png?raw=true)

```
Agora, essa pasta aparecerá em "Meu Computador" como uma "Unidade de Rede", com a letra que você escolheu.
```
![LOCALMAPEAMENTO](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM6.png?raw=true)

Compartilhamento de Pasta Oculta:
```
Para criar uma pasta compartilhada secreta, adicione o símbolo "$" no final do nome da pasta
Exemplo:segredo$.
```
![PASTASECRETA](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM7.png?raw=true)

```
Somente quem souber o caminho completo poderá acessar essa pasta.
Exemplo: \\192.168.1.10\segredo$.
```
![CAMINHOSECRETA](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM8.png?raw=true)

Compartilhamento de Impressoras na Rede:
```
O processo é o mesmo do compartilhamento de pastas. A impressora será visível e acessível para outros computadores na rede.
```

Area de Trabalho Remoto
```
Acesso Remoto (MSTSC):
Pressione Win + Pause.
Clique em Remoto e Clique em ''Permita que usuários se conectem remotamente ao computador''
```
![REMOTO](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM9.png?raw=true)

```
Depois, abra o MSTSC
Digite o IP da máquina que deseja acessar
Insira o nome de usuário e senha
Pronto! Agora você está conectado ao computador remoto.
```
![ACESSOREMOTO](https://github.com/paulo-ricardo-ffg/senac-aulas/blob/main/imagens/IMAGEM10.png?raw=true)


Desafio Para Mostrar que Aprendeu

```
Instale um novo Windows XP na Maquina Virtual (se for clonar, troque o MAC Address).
Configure o Hostname como "PCTime".
Defina o IP como 192.168.1.30.
Teste o ping para os IPs 192.168.1.10 e 192.168.1.20.
Compartilhe a pasta TIME com permissão de leitura.
Compartilhe a pasta RIVAL com permissão de leitura e gravação.
Mapeie a pasta TIME como unidade T: e RIVAL como R:.
Crie um compartilhamento oculto chamado JOGO.
Compartilhe uma impressora Epson no PCTime e acesse-a de outro computador na rede.
Envie uma mensagem com net send para todos na rede com a frase: "REDES!!!".
Esses passos irão garantir que você esteja pronto para configurar redes e realizar testes básicos no Windows XP!
```

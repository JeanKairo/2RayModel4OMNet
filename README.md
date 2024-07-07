# Manual de Instalação do OMNeT++

Este guia fornece instruções passo a passo para a instalação do OMNeT++ em diferentes sistemas operacionais, bem como orientações para importar um projeto e integrá-lo ao INet.

## Instalação do OMNeT++

### Passo 1: Baixar o OMNeT++

1. Acesse o site oficial do OMNeT++ em [https://omnetpp.org/download/](https://omnetpp.org/download/).
2. Faça o download da versão mais recente e extraia o conteúdo para uma pasta de sua escolha.

### Passo 2: Instalação por Sistema Operacional

#### Linux e macOS

Abra o terminal na pasta extraída e execute os seguintes comandos:

```bash
$ source setenv
$ ./configure
$ make
```

#### Windows

Inicie o terminal MinGW (mingwenv.cmd) na pasta extraída e execute os seguintes comandos:

```bash
$ ./configure
$ make
```

Certifique-se de ter iniciado o terminal usando o arquivo `mingwenv.cmd`.

### Passo 3: Executar o OMNeT++

1. No arquivo OMNeT++ Shell (versão), execute o seguinte comando:

```bash
$ omnetpp
```

Aguarde até que o simulador seja aberto.

2. Aceite a instalação sugerida do INet pela plataforma.

## Importação do Projeto

### Passo 1: Clonar o Repositório

1. Faça um clone deste repositório para sua máquina.

### Passo 2: Importar o Projeto no OMNeT++

1. Com o OMNeT++ aberto, vá em **File > Open Project from File System...** e encontre o diretório do arquivo clone.

### Passo 3: Integrar ao INet 

1. No File Explorer do OMNeT++, clique com o botão direito na pasta do projeto.
2. Selecione **Properties > Project References**.
3. Marque a opção referente ao INet instalado.

### Passo 4: Habilitar vizualização 3D 

1. Nos aquivos configure.user e configure.user.dist, na pasta de instalação do OMNet, habilite o OSG:

WITH_OSG=yes
WITH_OSGEARTH=yes

2. Ao executar o OMNet, na pasta do inet aperte com o botão direito, vá em **properties>OMNet++>Project Features** e habilte o Visualization OSG (3D) e o Visualization OSG (3D) showcases.


### Passo 5: Atualizar Imports e Renomear Módulos

Certifique-se de atualizar os imports do projeto para a versão do INet utilizada. Além disso, renomeie os módulos conforme necessário para garantir a compatibilidade com a versão específica do INet.

Agora, você concluiu a instalação do OMNeT++, a importação do projeto e a integração com o INet. Explore as funcionalidades do simulador e faça as adaptações necessárias em seu projeto.

Para mais informações, consulte a [documentação oficial do OMNeT++](https://omnetpp.org/documentation/).


no README acima 

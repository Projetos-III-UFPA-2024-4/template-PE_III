# Template LaTeX de Projetos De Engenharia III 

Este repositório contém um documento LaTeX que serve de base para os relatórios de componente EC01027 - PROJETOS DE ENGENHARIA III da FCT na UFA. Neste README há um pequeno guia de como clonar esse template, compilar e fazer suas alterações.

Com o template clonado e com suas alterações realizadas o projeto pode ser _upado_ em um repositório de escolha da equipe para ser desenvolvido colaborativamente por todos integrantes, dessa forma, servindo de alternativa ao tradicional _Overleaf_ que recentemente impôs limites às contas gratuitas como limite de colaboradores e tempo de compilação de projeto.

Esta abordagem possui mais requisitos e uma curva de aprendizado maior porém bastante útil para projetos futuros.

## Dependências

Certifique-se de ter as seguintes dependências instaladas no seu sistema:

- [TeX Live](https://www.tug.org/texlive/) (incluindo LuaLaTeX)
- [Biber](https://sourceforge.net/projects/biblatex-biber/)
- [Visual Studio Code](https://code.visualstudio.com/) (opcional, mas recomendado)
- [Extensão LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) para Visual Studio Code (opcional, mas recomendado)
- [Git](https://git-scm.com/)

## Instalação

Este processo de tutorial foi feito integralmente no linux Ubuntu 22.04 LTS, sendo o recomendado porém abaixo segue um tutorial para windows também, talvez um pouco mais passível de inconsistências.

Caso surja alguma dúvida ou sugestão de melhoria, [abra uma _issue_ neste repositório](https://github.com/Projetos-III-UFPA-2024-4/template-PE_III/issues/new).  

### Linux 🐧

1. **Instale o Git**: pelo [site](https://git-scm.com/) ou pela linha de comando:
   ```sh
   sudo apt update
   sudo apt install git
    ```


2. **Instale o TeX Live**: Isso vai demorar um pouco por ser um pacote grande e podendo "travar" o terminal quando chegar numa parte específica do log que não lembro, se travar aperte o `enter`  
   ```sh
   sudo apt install texlive-full
    ```



3. **Instale o Biber**:
   ```sh
   sudo apt install biber
    ```

4. **Instale o Visual Studio Code**: Siga as instruções no [site oficial do Visual Studio Code](https://code.visualstudio.com/).

5. **Instale a extensão LaTeX Workshop**: Abra o Visual Studio Code e instale a extensão LaTeX Workshop a partir do Marketplace.

### Windows 🪟

1. **Instale o TeX Live**: Baixe e instale o TeX Live a partir do [site oficial](https://www.tug.org/texlive/windows.html).

2. **Instale o Biber**: Baixe e instale o Biber a partir do [site oficial](https://sourceforge.net/projects/biblatex-biber/).

3. **Instale o Visual Studio Code**: Siga as instruções no [site oficial do Visual Studio Code](https://code.visualstudio.com/).

4. **Instale a extensão LaTeX Workshop**: Abra o Visual Studio Code e instale a extensão LaTeX Workshop a partir do Marketplace.

## Compilação

### Usando o Visual Studio Code

No VS code abra o terminal no diretório que desejar (Atalho `Ctrl+J`) e:

1. **Clone o repositório**:
   ```sh
   git clone <URL-do-repositorio>
   cd <nome-do-repositorio>
   ```

2. **Abra o projeto no Visual Studio Code**: 

3. **Compile o documento:**: Pressione `Ctrl+Shift+B`

## Estrutura do Projeto
```sh
<template-PE_III>/
├── .vscode/                    # Diretório contendo configurações específicas do Visual Studio Code.       
│   └── tasks.json              # Arquivo de configuração de tarefas para automatizar a compilação do projeto LaTeX.
├── sections/                   # Diretório contendo os arquivos das seções do documento.
│   ├── 01-identificacao.tex    # Arquivo LaTeX para a seção de identificação.
│   ├── 02-introducao.tex       # Arquivo LaTeX para a seção de introducao
│   └── 03-plano.tex            # Arquivo LaTeX para a seção de plano.
├── figures/                    # Diretório para armazenar figuras usadas no documento
│   └── ...
├── main.tex                    # Arquivo principal do documento LaTeX, que inclui todas as seções e configurações do documento.
└── README.md                   # Arquivo de documentação do projeto, contendo instruções de instalação, compilação e contribuição.
├── referencias.bib             # Arquivo bib onde são armazenadas as referências. 
└── defs.tex                    # Arquivo contendo definições e configurações personalizadas para o documento LaTeX, como pacotes, cores, fontes, formatação de seções, cabeçalhos e rodapés.
   ```



---
published: true
layout: post
categories: latex overleaf
title: Como começar no LaTeX
---
Olá pessoal, neste _post_ vou falar sobre como dá os primeiros passos para gerar documentos em LaTeX de maneira fácil e descomplicada, principalmente para quem não tem afinidade com programação. Apresentarei ferramentas e modos de usar templates que podem lhe ajudar muito na introdução ao LaTeX.

| ![](https://miro.medium.com/max/1280/1*jZ6-zthg418clkertSnk8w.png) | 
|:------------:| 
| |

## Mas afinal, o que é LaTeX

**LaTeX** (pronuncia-se LAY-tek ou LAH-tek) é uma ferramenta usada para gerar documentos com aparência profissional. É baseado na idéia **WYSIWYM** (_what you see is what you mean_ - o que você vê é o que você quer dizer) que significa que você precisa focar apenas no conteúdo que deseja descrever, e não preocupar-se com elementos como formatação, espaçamento e símbolos da página fora do lugar.

O LaTeX é usado largamente pelo mundo para escrita científica, principalmente para gerar livros e artigos. Devido ao grande número de bibliotecas disponíveis (criadas principalmente por outros amantes de LaTeX), as possibilidades são infinitas na criação de documentos científicos bem formatados e com aparência respeitável.

## E como começar?

Embora o LaTeX tenha o objetivo de facilitar a geração de documentos, a sua instalação nem sempre é das mais agradáveis, e a instalação de bibliotecas, pacotes de linguagens e outros _features_ pode ser uma tarefa árdua para usuários comuns.

Neste _post_ recomendo o uso de editores LaTeX online, espécies de google docs para LaTeX. Entre esses, destaco o que usei por muitos anos, o [ShareLaTeX](http://sharelatex.com/), uma plataforma de código aberto que integra um ambiente de compilação LaTeX e online, permitindo que o usuário não se preocupe com instalação de ferramentas, editores ou bibliotecas para gerar seus documentos. Há algum tempo atrás, no entanto, esta foi integrado ao [Overleaf](http://overleaf.com/) em apenas uma plataforma, que é a recomendada aqui.

> (...) esta foi integrado ao [Overleaf](http://overleaf.com/) em apenas uma plataforma, que é a recomendada aqui.

Para começar no **Overleaf**, crie um usuário usando seu email, conta do google ou do orcid [Overleaf register](https://www.overleaf.com/register). Após a criação do usuário, clique na aba _templates_ na barra superior para pesquisar templates LaTeX para facilitar o começo da sua jornada, conforme Figura 1. Nesta etapa você pode pesquisar os templates mais diversos como _journals_ conhecidos do IEEE, slides de universidades, modelos de carta, etc.

> Após a criação do usuário, clique na aba _templates_ na barra superior para pesquisar templates LaTeX para facilitar o começo da sua jornada

| ![Template search](https://user-images.githubusercontent.com/1641686/71539654-e8805d00-2915-11ea-9dc0-96a404b176e5.png) | 
|:------------:| 
| Figura 1 - Busca de _templates_ do Overleaf |

Neste caso vamos fazer uma busca simples: `Curriculum Vitae`. Após selecionar algum dos resultados da busca você verá uma tela com uma pequena prévia do modelo do documento, conforme a Figura 2. Para abri-lo na sua conta pessoal do Overleaf, clique em **Open as Template**, que criará uma cópia na sua área de trabalho do Overleaf, para começar a edição.

| ![Template opening](https://user-images.githubusercontent.com/1641686/71539691-7ceabf80-2916-11ea-9471-7619ed5e1488.png) | 
|:------------:| 
| Figura 2 - Clona o _template_ para área de trabalho do usuário |

Após isso, o projeto será aberto. Em geral haverá apenas um arquivo `.tex` (chamado TeX), que é o código principal do documento e onde normalmente será escrito o código.

## E o código, como funciona?

Um documento TeX é composto de duas partes que serão discutidas a seguir:

* **Preâmbulo**: contém parâmetros gerais de organização e formatação do documento;
* **Corpo**: contém todo o texto, seus ambientes e estruturas.

### Preâmbulo do código

Cada código LaTeX começa com uma preâmbulo, delimitado por uma função predefinida chamada `\documentclass[opções]{classe}`, que define o tipo de classe de documento que pode ter diversos tipos de formato como:

* artigo (`article`): classe para textos pequenos como artigos, resumos e relatórios que seguem a estrutura de seções (`\section` e `\subsection`);
* slides (`beamer`): classe para geração de _slides_;
* poster (`sciposter`): classe para criação de _banners_;
* livro (`book`): classe para livros com estruturas de capítulos (`\chapter`).

Uma lista mais completa de classes disponíveis pode ser encontrada em [[1]](https://ctan.org/topic/class){:target="_blank"}. Algumas opções também podem ser editadas nesse mesmo comando tais como tamanho da fonte (12pt), tamanho do papel (`a4paper`), formato da página (`onecolumn` ou `twocolumn`), entre outros. O comando abaixo, por exemplo, gera um documento do tipo artigo, com fonte padrão tamanho 12pt, em papel a4 e de impressão nos 2 lados da folha (`twosided`).

'''latex
\documentclass[12pt, a4paper, twoside]{article}
'''

Logo abaixo são declaradas, opcionalmente, eventuais bibliotecas usadas no código através do comando `\usepackage[opções]{biblioteca}`. Estas bibliotecas podem ser das mais diversas e podem servir para mudar cores no texto, inserir imagens, inserir fórmulas matemáticas, desenhos, mudar a linguagem e codificação, entre outros.

Um exemplo pode ser visto na Figura 3, utilizando um dos resultados da busca por `Curriculum Vitae`. O resultado pode ser visto no Overleaf toda vez que você clicar no `Ctrl + Enter` ou `Ctrl + S`.

| ![Seleção_102](https://user-images.githubusercontent.com/1641686/71540449-49616280-2921-11ea-9c64-26c433c26948.png) | 
|:------------:| 
| Figura 3 - Prêambulo de um documento LaTeX |

### Iniciando o documento

Cada documento é inicializado oficialmente após o uso das _tags_ `\begin{document}` e `\end{document}`. Tudo que vem antes de `\begin{document}` é chamado de preâmbulo e tudo que vem após `\end{document}` é descartado. Dentro desta tag é colocado os elementos textuais como as seções (`\section{Introdução}`), subseções (`\subsection{Subseção}`) e demais elementos. Um exemplo de criação de projeto e escrita básica pode ser visto no _gif_ da Figura 4.

| ![out](https://user-images.githubusercontent.com/1641686/71540738-fee1e500-2924-11ea-801a-68769a541287.gif) | ![Seleção_104](https://user-images.githubusercontent.com/1641686/71540877-b297a480-2926-11ea-9ae5-0b962bfb0146.png) |
|:----------------------------:|:----------------------------:|
||	Figura 4 - Criando um projeto LaTeX e escrevendo texto	 |



## Referências

[1] [https://ctan.org/topic/class](https://ctan.org/topic/class)

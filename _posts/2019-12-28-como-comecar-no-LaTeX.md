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

Após isso, o projeto será aberto. Em geral haverá apenas um arquivo `.tex`, que é o código principal do documento e onde normalmente será escrito o código.

## E o código, como funciona?

Cada código LaTeX começa com uma preâmbulo, delimitado por uma função predefinida chamada `\documentclass[opções]{classe}`, que define o tipo de classe de documento que pode ter diversos tipos de formato como artigo (`article`), slides (`beamer`), artigo do IEEE (`IEEEtran`), livro (`book`), etc. Uma lista mais completa de classes disponíveis pode ser encontrada em [[1]](https://ctan.org/topic/class){:target="_blank"}. 

## Referências

[1] [https://ctan.org/topic/class](https://ctan.org/topic/class)

Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.

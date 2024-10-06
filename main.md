---
title: Título
subtitle: Subtítulo
author: "Nome do Autor"
date: \today
thanks: Email do autor
paper: a4
numbersections: true
autoEqnLabels: true
header-includes: |
  \RequirePackage[outer=25mm,inner=35mm,vmargin=20mm,includehead,includefoot,headheight=15pt]{geometry}
  \usepackage[portuguese]{babel}
  \usepackage{indentfirst}
  \usepackage{amsmath}
  \usepackage{setspace}
  \usepackage{emptypage}
  \onehalfspacing
  \setlength{\parindent}{1.25cm}
  \setlength{\parskip}{6pt}
  \newcommand{\newpara}
  {
      \vskip 6pt
  }
  \usepackage{hyperref, bookmark} 
  \hypersetup{pdfborder=0 0 0}
  \usepackage{titlesec}
  \titlelabel{\thetitle.\quad}
  \usepackage{lipsum}
  \usepackage{float}
  \let\origfigure\figure
  \let\endorigfigure\endfigure
  \renewenvironment{figure}[1][2]{
  \expandafter\origfigure\expandafter[H]
  }{
  \endorigfigure}
---

# Introdução {#sec:header1}

\lipsum{1-2}

## Objetivos {#sec:header2}

\lipsum[3]

---

# Desenvolvimento {#sec:header3}

Aqui podemos fazer o desenvolvimento do documento, utilizando listas:

+ Primeiro ponto.
+ Segundo ponto.
  + Ponto dentro do ponto.
+ Terceiro ponto.

Uma equação:
$$
  \int_{-\infty}^{+\infty} \phi(t) \cdot \phi(t-to) \cdot dt
$$ {#eq:eq1}

Se quisermos adicionar uma imagem:

![Exemplo](assets/exemplo.png){#fig:fig1}

Podemos referenciar seções, figuras, equações, etc., da seguinte forma.
Por exemplo, na [@sec:header1] temos a introdução. Na [@fig:fig1] temos uma figura de exemplo. Na [@eq:eq1] temos uma equação de exemplo.

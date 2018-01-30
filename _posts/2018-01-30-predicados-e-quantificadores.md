---
layout: post
title: Evoluindo com a lógica de predicados
description: "Na série anterior de postagens, abordamos os conceitos básicos sobre a lógica proposicional, porém esta não é capaz de expressar de forma correta o significado das proposições, tanto em matemática quanto em linguagem natural. Para que seja possível expressar um vasto grupo de proposições daremos início ao estudo da chamada lógica de predicados."
tags: [matemática discreta]
image:
  feature: /posts/2018-01-30-evoluindo.png
comments: true
share: true
---

**Nota:** Neste post daremos início ao estudo da chamada lógica de predicados. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

Confira os posts da série sobre lógica proposicional:

* <a href="/algebra-das-proposicoes">Algebra das proposições</a>
* <a href="/implicacao-e-equivalencia">Implicação e equivalência lógica</a>
* <a href="/tautologia-contraticao-e-contingencia">Tautologia, contradição e contingência</a>
* <a href="/operacoes-logicas-fundamentais">Operações lógicas fundamentais</a>
* <a href="/logica-matematica-e-computacional-primeiros-passos">Lógica matemática e computacional, primeiros passos!</a>

---

Na série anterior de postagens, abordamos os conceitos básicos sobre a lógica proposicional, porém esta não é capaz de expressar de forma correta o significado das proposições, tanto em matemática quanto em linguagem natural.

#### Exemplo

É de conhecimento que:

* *Todas as séries produzidas pela Netflix são consideradas ótimas pela crítica.*

Através das regras estabelecidas pela lógica proposicional não é possível determinar se a afirmação abaixo é verdadeira ou falsa.

* *Stranger Things é considerada ótima pela crítica.*

Em que *Stranger Things* é uma das séries produzidas pela Netflix.

De maneira semelhante, não podemos concluir a partir da afirmação:

* *Punho de Ferro está sendo bombardeada pelos críticos.*

Em que *Punho de Ferro* é uma das séries produzidas pela Netflix, para determinar que é verdade que:

* *Existe uma série produzida pela Netflix que está sendo bombardeada pelos críticos.*

Para que seja possível expressar esse e um vasto grupo de proposições daremos início ao estudo da chamada lógica de predicados.

## Predicados

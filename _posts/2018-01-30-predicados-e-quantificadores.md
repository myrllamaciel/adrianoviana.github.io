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

* `Todas as séries produzidas pela Netflix são consideradas ótimas pela crítica.`

Através das regras estabelecidas pela lógica proposicional não é possível determinar se a afirmação abaixo é verdadeira ou falsa.

* `Stranger Things é considerada ótima pela crítica.`

Em que *Stranger Things* é uma das séries produzidas pela Netflix.

De maneira semelhante, não podemos concluir a partir da afirmação:

* `Punho de Ferro está sendo bombardeada pelos críticos.`

Em que *Punho de Ferro* é uma das séries produzidas pela Netflix, para determinar que é verdade que:

* `Existe uma série produzida pela Netflix que está sendo bombardeada pelos críticos.`

Para que seja possível expressar esse e um vasto grupo de proposições daremos início ao estudo da chamada lógica de predicados.

## Predicados

É comum encontrarmos na matemática e em programas de computador expressões no formato das sentenças abaixo:

* `z = y + x`
* `A série y é considerada ótima pela crítica.`
* `A série x está sendo bombardeada pelos críticos.`

Essas expressões não assumem valores de `verdade` ou `falsidade` enquanto os valores das variáveis não são especificados. Notamos que cada sentença é composta por duas partes. A primeira é chamada de __sujeito da declaração__ e a segunda de __predicado__.

* `A série x` (sujeito)
* `está sendo bombardeada pelos críticos.` (predicado)

Ou seja, um predicado é uma __propriedade__ que o sujeito da declaração pode ter.

#### Representação

Podemos representar a declaração `A série x está sendo bombardeada pelos críticos` por:

* `P(x)`, em que `P` indica o predicado `está sendo bombardeada pelos críticos` e `x` é a variável.

Uma vez que o valor é atribuído a variável `x`, a declaração `P(x)` __torna-se uma proposição__ e dessa forma terá um valor de `Verdade` ou `Falsidade`.

#### Exemplo

* Seja `P(x)` a declaração `x > 5`. Qual o valor-verdade de `P(4)` e `P(6)`?
  * Obtemos a proposição `P(4)` substituindo `x = 4` na declaração `x > 5`. Então, `P(4)`, que é a proposição `4 > 5`, é falsa.
  * Obtemos a proposição `P(6)` substituindo `x = 6` na declaração `x > 5`. Então, `P(6)`, que é a proposição `6 > 5`, é verdadeira.

## Quantificadores

## Conclusão

Este foi um post sobre as propriedades e equivalências das operações lógicas fundamentais, conhecimentos que serão de total importância quando tratarmos da validade de argumentos, regras de inferência e dedução lógica. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos.

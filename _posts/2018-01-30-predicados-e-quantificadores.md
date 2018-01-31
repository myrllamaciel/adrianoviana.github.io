---
layout: post
title: Evoluindo com a lógica de predicados
description: "Na série anterior de postagens, abordamos os conceitos básicos sobre a lógica proposicional, porém esta não é capaz de expressar de forma correta o significado das proposições, tanto em matemática quanto em linguagem natural. Para que seja possível expressar um vasto grupo de proposições daremos início ao estudo da chamada lógica de predicados."
tags: [matemática discreta,lógica matemática]
image:
  feature: /posts/2018-01-31-predicados-quantificadores.png
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

Na série anterior de postagens, abordamos os conceitos básicos sobre a lógica proposicional, porém esta não é capaz de expressar, de forma correta, o significado das proposições, tanto em matemática quanto em linguagem natural.

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

Essas expressões, chamadas de __funções proposionais__, não assumem valores de `verdade` ou `falsidade` enquanto os valores das variáveis não são especificados. Notamos que cada sentença é composta por duas partes. A primeira é chamada de __sujeito da declaração__ e a segunda de __predicado__.

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

Existe uma maneira importante, chamada de quantificação, para criar proposições a partir de funções proposicionais.

**Quantificação:** É a maneira de dizer que um predicado é verdadeiro para um conjunto de elementos.
{: .notice}

Visto esse conceito, vamos nos ater a dois tipos de quantificação:

* __Universal__ - Nesta modalidade, um predicado é verdadeiro para todos os elementos em consideração.
* __Existencial__ - Aqui, existe um ou mais elementos para os quais o predicado é verdadeiro.

#### Quantificador Universal (`∀`)

`P(x)` é válida para todos os valores de `x` do domínio.

* `∀xP(x)`
  * A notação acima indica a quantificação universal de `P(x)`.
  * `∀xP(x)` é chamado de quantificador universal.
  * Lê-se `∀xP(x)` como *"para todo x P(x)"*.

**Nota:** Um elemento para o qual `P(x)` é falsa é chamado de contra-exemplo para `∀xP(x)`
{: .notice}

##### Exemplo

* Seja `P(x)` a função proposicional `x + 3 > x`.
* Qual o valor-verdade da quantificação `∀xP(x)`, no domínio dos números reais?

Como `P(x)` é verdadeira para todo número real `x`, `∀xP(x)` é __verdadeira__.

#### Quantificador Existencial (`∃`)

Existe um elemento `x` no domínio tal que `P(x)`.

* `∃xP(x)`
  * A notação acima indica a quantificação existencial de `P(x)`.
  * `∃xP(x)` é chamado de quantificador existencial.
  * Lê-se `∃xP(x)` como *"existe um x tal que P(x)"* ou *"existe pelo menos um x tal que P(x)"*.

**Nota:** No lugar da palavra *Existe*, podemos também expressar a quantificação existencial de muitas outras formas, tais como *para algum*, *para pelo menos um*, etc.
{: .notice}

##### Exemplo

* Seja `P(x)` a função proposicional `x > 2`.
* Qual o valor-verdade da quantificação `∃xP(x)`, no domínio dos números reais?

Como `P(x)` é verdadeira para alguns dos números reais, como `x = 4` por exemplo, `∃xP(x)` é __verdadeira__.

## Resumo

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">Quantificação</th>
			<th style="text-align:center;">verdadeira</th>
			<th style="text-align:right;">falsa</th>
		</tr>
	</thead>
	<tbody>
		<tr >
			<td style="text-align:left;">`∀xP(x)`</td>
			<td style="text-align:center;">`P(x)` é verdadeira para todo `x`</td>
			<td style="text-align:right;">existe um `x` tal que `P(x)` é falsa</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">`∃xP(x)`</td>
			<td style="text-align:center;">Existe um `x` tal que `P(x)` é verdadeira</td>
			<td style="text-align:right;">`P(x)` é falsa para todo `x`</td>
		</tr>
	</tbody>
</table>

## Conclusão

Este foi um post sobre os conceitos básicos da lógica de predicados. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos e colegas de turma.

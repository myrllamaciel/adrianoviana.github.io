---
layout: post
title: Lógica matemática e computacional, primeiros passos!
description: "Este é um post introdutório sobre lógica matemática e computacional, o mesmo abrange conceitos básicos que ajudarão a dar inicio aos nossos estudos."
tags: [lógica matemática]
image:
  feature: /posts/2015-02-20-artificial-brain.jpg
comments: true
share: true
---


**Nota:** Este é um post introdutório sobre lógica matemática e computacional, o mesmo abrange conceitos básicos que ajudarão a dar inicio aos nossos estudos. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

Confira os demais posts desta série:

* <a href="/implicacao-e-equivalencia">Implicação e equivalência lógica</a>
* <a href="/tautologia-contraticao-e-contingencia">Tautologia, contradição e contingência</a>
* <a href="/operacoes-logicas-fundamentais">Operações lógicas fundamentais</a>

---


## Proposição

Quando falamos em lógica matemática, a primeira coisa que devemos ter em mente é o conceito de proposição. Segundo ALENCAR, Edgar Filho: Proposição é todo conjunto de __palavras ou símbolos__ que exprimem um pensamento de __sentido completo__.

Destaco duas partes desse conceito que julgo serem as principais: a primeira é o fato de termos a possibilidade de formar proposições tanto com letras (pertencentes a  algum alfabeto) compondo assim, palavras quanto formarmos proposições com símbolos formando expressões matemáticas, etc.  A segunda é o fato de que, para ser proposição, a sentença deve possuir sentido completo, ou seja, a mesma deve sempre afirmar fatos.

Outra característica importante das proposições é que elas são expressadas através de orações declarativas e nunca exclamativas ou interrogativas e por serem orações, devem possuir sujeito e predicado.  Agora vejamos alguns exemplos:

{% highlight yaml %}
São proposições:
  A Espanha é um país da Europa.
  O uniforme do Corinthians é alvinegro.
  5 < 25
  Lógica matemática é a melhor disciplina do curso de sistemas de informação.

Não são proposições:
  Pedro Álvares Cabral descobriu o Brasil?
  2 + 3 / 5
  Saia da minha frente!
  2x + 3 = 5
{% endhighlight %}

## Axiomas

Quando tomamos como verdade uma sentença ou proposição que não pode ser provada ou demonstrada temos um axioma. A lógica matemática é regida por dois princípios (axiomas) básicos:

* Princípio da __não contradição__ - uma proposição não pode ser verdadeira e falsa ao mesmo tempo.
* Princípio do __terceiro excluído__ - toda proposição ou é verdadeira ou é falsa, isto é, verifica-se sempre um desses casos e nunca um terceiro.

## Valores Lógicos

A partir dos axiomas que regem a lógica matemática, podemos dizer que as proposições possuem um, e um só, valor lógico, este nunca deve assumir outra forma que não seja a de __Verdade (V)__ para proposições verdadeiras ou __Falsidade (F)__ para proposições falsas. Vejamos um exemplo considerando as duas proposições abaixo:

1.  O planeta Terra gira em torno do Sol
2.  São Luís é a capital do estado de Mato Grosso

O valor lógico da proposição `1` é a __Verdade (V)__ e o valor lógico da proposição `2` é a __Falsidade (F)__.

## Classificação

Existem dois tipos de classificação para uma proposição, esta pode ser simples (atômica) caso não possua nenhuma outra proposição como parte integrante de si mesmo, ou composta (molecular) caso seja formada pela combinação de duas ou mais proposições, sejam estas simples ou também compostas. 

É comum representarmos as proposições simples com letras minúsculas `p, q, r`, etc. Enquanto que as proposições compostas representamos com letras maiúsculas `P, Q, R`, etc.Vejamos alguns exemplos:

### Proposições simples

* p : Daniel é animado
* q : Henrique fuma cigarro
* r : Edísio come muito

### Proposições compostas

* P : Daniel é animado e Henrique fuma cigarro 
* Q : Daniel é animado ou Henrique fuma cigarro
* R : Se Edísio come muito, então Daniel é animado

> Proposições compostas também costumam ser chamadas de formulas proposicionais.

## Conectivos

Note que nos exemplos acima precisamos de algumas palavras especiais para formar as proposições compostas a partir das proposições simples, estas são chamadas de conectivos. Abaixo listo alguns dos conectivos mais usuais da lógica matemática:

`"e", "ou", "não", "se.. então..", "..se e somente se.."`

## Tabela-verdade

Analisando novamente os princípios básicos da lógica matemática, notamos que o valor lógico para uma proposição simples sempre terá duas possibilidades, ou seja,  a proposição pode assumir o valor de Verdade (V) ou de Falsidade (F). Já no que diz respeito a proposições compostas, o estabelecimento de seu valor lógico depende dos valores lógicos de suas proposições simples componentes. 

A tabela-verdade é o dispositivo utilizado para estabelecer esses possíveis valores lógicos da proposição composta, os mesmos correspondem a todas as possíveis combinações dos valores lógicos das proposições simples componentes. Veja o exemplo de uma tabela-verdade para uma proposição composta de duas proposições simples `p e q`:

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;"></th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
</table>

> OBS: Falaremos especificamente da construção de tabelas-verdade em outro post.

## Notação

Para finalizar, mostro abaixo como é feita a notação para denotar o valor lógico de uma proposição simples:

V(p) = V, caso o valor lógico da proposição seja a Verdade.

V(p) = F, caso o valor lógico da proposição seja a falsidade.

Para proposições compostas deve-se usar as letras maiúsculas como já foi mostrado, nesse caso ficaria: V(P).

## Considerações Gerais

Este foi um post introdutório sobre os conceitos básicos da lógica matemática e computacional, nos próximos falaremos sobre operações lógicas e construção de tabelas-verdade. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem compartilhe com seus amigos. 

Por hoje é só moçada, abraço!

## Slides

<script async class="speakerdeck-embed" data-id="6fa6db4b6e1440e2a836d0a309d05d9a" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>



---
layout: post
title: Tautologias, contradições e contingências
description: "Existem algumas proposições compostas, chamadas de tautologias, cujo valor lógico é sempre a verdade. O oposto também ocorre: certas proposições compostas, chamadas de contradições, cujo o valor lógico é sempre a falsidade. Caso a proposição composta não seja tautologia e nem contradição é chamada de contingência."
tags: [lógica matemática]
image:
  feature: /posts/2016-01-03-tautologia-contradicao-contingencia.png
comments: true
share: true
---

**Nota:** Neste post conheceremos as classificação das proposições compostas de acordo com seus respectivos valores lógicos. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

<div markdown="0"><a href="https://speakerd.s3.amazonaws.com/presentations/883d0ce342684229897810f1c778c637/Aula04-logicaMatematica.pdf" class="btn">Baixar apresentação</a></div>

---

Existem algumas proposições compostas, chamadas de tautologias, cujo valor lógico é sempre a verdade. O oposto também ocorre: certas proposições compostas, chamadas de contradições, cujo o valor lógico é sempre a falsidade. Caso a proposição composta não seja tautologia e nem contradição é chamada de contingência.

## Tautologia

Também chamada de __proposição tautológica__ ou __proposição logicamente verdadeira__, tautologia é toda proposição composta `P(p, q, etc.)` cujo valor lógico é sempre a Verdade, quaisquer que sejam os valores lógicos das proposições simples que a compõe `(p, q, etc.)`.

### Exemplos

A proposição composta `p ∨ ~p` __é tautologia__, pois para qualquer valor de `p` (Verdade ou Falsidade) seu valor lógico é a Verdade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">p &or; ~p</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

A proposição composta `p ∨ ~(p ∧ q)` __é tautologia__, pois para quaisquer valores de `p` e `q` seu valor lógico é a Verdade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;">~(p &and; q)</th>
			<th style="text-align:right;">p &or; ~(p &and; q)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

A proposição composta `p ∧ r → ~q ∨ r` __é tautologia__, pois para quaisquer valores lógicos de `p`, `q` e `r` seu valor lógico é a Verdade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">p &and; r</th>
			<th style="text-align:right;">~q &or; r</th>
			<th style="text-align:right;">p ∧ r → ~q ∨ r</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">6</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

## Contradição

Também chamada de __proposição contraválida__ ou __proposição logicamente falsa__, contradição é toda proposição composta `P(p, q, etc.)` cujo valor lógico é sempre a Falsidade, quaisquer que sejam os valores lógicos das proposições simples que a compõe `(p, q, etc.)`.

### Exemplos

A proposição composta `p ∧ ~p` __é contradição__, pois para qualquer valor de `p` (Verdade ou Falsidade) seu valor lógico é a Falsidade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">p &and; ~p</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
</table>

A proposição composta `~(p ∨ ~(p ∧ q))` __é contradição__, pois para quaisquer valores de `p` e `q` seu valor lógico é a Falsidade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;">~(p &and; q)</th>
			<th style="text-align:right;">p &or; ~(p &and; q)</th>
			<th style="text-align:right;">~(p &or; ~(p &and; q))</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
</table>

A proposição composta `~(p ∧ r → ~q ∨ r)` __é contradição__, pois para quaisquer valores lógicos de `p`, `q` e `r` seu valor lógico é a Falsidade como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">p &and; r</th>
			<th style="text-align:right;">~q &or; r</th>
			<th style="text-align:right;">p ∧ r → ~q ∨ r</th>
			<th style="text-align:right;">~(p ∧ r → ~q ∨ r)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">6</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
</table>

## Fique Atento

Observe que como uma tautologia é sempre Verdadeira, sua negação sempre assumirá o valor lógico da Falsidade, resultando assim em uma contradição.

##Contingência

Também chamada de __proposição contingente__ ou __proposição indeterminada__, contingência é toda proposição composta `P(p, q, etc.)` cujo valor lógico pode ser a Falsidade ou a Verdade, dependendo dos valores lógicos das proposições simples que a compõe `(p, q, etc.)`, ou seja, é toda proposição composta que não é tautologia e nem contradição.


### Exemplos

A proposição composta `p → ~p` __é contingência__, pois seu valor lógico ora é a Falsidade e ora é a Verdade dependendo do valor lógico da proposição simples `p` como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">p → ~p</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

A proposição composta `p ∨ q` __é contingência__, pois seu valor lógico ora é a Falsidade e ora é a Verdade dependendo dos valores lógicos da proposições simples `p` e `q` como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &or; q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#FF0000;">F</td>
		</tr>
	</tbody>
</table>

## Conclusão

Este foi um post sobre tautologias, contradições e contingências, importantes conceitos para prosseguirmos no estudo da lógica matemática e computacional. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos. 

Por hoje é só moçada, abraço!

## Slides

<script async class="speakerdeck-embed" data-id="883d0ce342684229897810f1c778c637" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>




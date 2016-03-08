---
layout: post
title: Implicação e equivalência lógica
description: "Uma proposição `P(p, q, r, ...)` implica logicamente ou apenas implica uma proposição `Q(p, q, r, ...)` se `Q(p, q, r, ...)` __é verdadeira todas as vezes que__ `P(p, q, r, ...)` __for verdadeira__."
tags: [lógica matemática]
image:
  feature: /posts/2016-03-07-implicacao-e-equivalencia.png
comments: true
share: true
---

**Nota:** Neste post conheceremos os conceitos de implicação e equivalência lógica. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

Confira os demais posts desta série:

* <a href="/tautologia-contraticao-e-contingencia">Tautologia, contradição e contingência</a>
* <a href="/operacoes-logicas-fundamentais">Operações lógicas fundamentais</a>
* <a href="/logica-matematica-e-computacional-primeiros-passos">Lógica matemática e computacional, primeiros passos!</a>

---

## Implicação Lógica (&#8658;)

Uma proposição `P(p, q, r, ...)` __implica logicamente__ ou apenas implica uma proposição `Q(p, q, r, ...)` se `Q(p, q, r, ...)` __é verdadeira todas as vezes que__ `P(p, q, r, ...)` __for verdadeira__.

### Notação

`P(p, q, r, ...)` &#8658; `Q(p, q, r, ...)`

### Exemplos

A proposição composta `p ∧ q` __implica logicamente__ nas proposições `p ∨ q` e `p ↔ q`, pois `p ∧ q` é verdadeira somente na primeira linha e, nesta linha, as proposições `p ∨ q` e `p ↔ q` também são verdadeiras como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;">p &or; q</th>
			<th style="text-align:right;">p &#8596; q</th>
		</tr>
	</thead>
	<tbody>
		<tr style="background-color:#fefb02;">
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
</table>

A proposição composta `p ↔ q` __implica logicamente__ nas proposições `p → q` e `q → p`, pois `p ↔ q` é verdadeira somente na primeira e última linha e, nestas linhas, as proposições `p → q` e `q → p` também são verdadeiras como demonstrado por sua tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p ↔ q</th>
			<th style="text-align:right;">p → q</th>
			<th style="text-align:right;">q → p</th>
		</tr>
	</thead>
	<tbody>
		<tr style="background-color:#fefb02;">
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr style="background-color:#fefb02;">
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
</table>   

### Tautologias e implicações lógicas

A proposição `P(p, q, r,...)` __implica__ a proposição `Q(p, q,r,...)`, isto é, `P(p, q, r,...)` &#8658; `Q(p, q, r,...)` __se e somente se__ a condicional `P(p, q, r,...)` → `Q(p, q, r,...)` é __tautologia__. 

A proposição composta `p ↔ q` __implica logicamente__ na proposição `p → q`, logo aS condicional `(p ↔ q) → (p → q)` é __tautologia__ conforme demonstrado pela tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p ↔ q</th>
			<th style="text-align:right;">p → q</th>
			<th style="text-align:right;">(p ↔ q) → (p → q)</th>
		</tr>
	</thead>
	<tbody>
		<tr >
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
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
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>   

### Propriedades

A implicação lógica possui duas importantes propriedades:

* Reflexiva (__R__)
	* `P(p, q, r,...)` &#8658; `P(p, q, r,...)`
* Transitiva (__T__)
	* Se `P(p, q, r,...)` &#8658; `Q(p, q, r,...)` e `Q(p, q, r,...)` &#8658; `R(p, q, r,...)` então `P(p, q, r,...)` &#8658; `R(p, q, r,...)`

## Equivalência Lógica (&#8660;)

Uma proposição `P(p, q, r, ...)` é __logicamente equivalente__ ou apenas equivalente a uma proposição `Q(p, q, r, ...)` se se as tabelas-verdade destas duas proposições forem idênticas.

### Notação

`P(p, q, r, ...)` &#8660; `Q(p, q, r, ...)`

### Exemplos

A proposição composta `p → p ∧ q` é __logicamente equivalente__ a proposição `p → q`, pois `p → q` e `p → p ∧ q` possuem a mesma tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;">p → p ∧ q</th>
			<th style="text-align:right;">p → q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;background-color:#fefb02;">F</td>
			<td style="text-align:right;background-color:#fefb02;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
</table>

A proposição composta `p → q` é __logicamente equivalente__ a proposição `~p ∨ q`, pois `~p ∨ q` e `p → q` possuem a mesma tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">p → q</th>
			<th style="text-align:right;">~p ∨ q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;background-color:#fefb02;">F</td>
			<td style="text-align:right;background-color:#fefb02;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
			<td style="text-align:right;background-color:#fefb02;">V</td>
		</tr>
	</tbody>
</table>


### Tautologias e equivalências lógicas

A proposição `P(p, q, r,...)` é __equivalente__ a proposição `Q(p, q,r,...)`, isto é, `P(p, q, r,...)` &#8660; `Q(p, q, r,...)` __se e somente se__ a bicondicional `P(p, q, r,...)` ↔ `Q(p, q, r,...)` é __tautologia__. 

A proposição composta `p → p ∧ q` é __equivalente__ a proposição `p → q`, logo a bicondicional `(p → p ∧ q) ↔ (p → q)` é __tautologia__ conforme demonstrado pela tabela-verdade.

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;">p → p ∧ q</th>
			<th style="text-align:right;">p → q</th>
			<th style="text-align:right;">(p → p ∧ q) ↔ (p → q)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
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
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
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
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>  

### Propriedades

A implicação lógica possui três importantes propriedades:

* Reflexiva (__R__)
	* `P(p, q, r,...)` &#8660; `P(p, q, r,...)`
* Transitiva (__T__)
	* Se `P(p, q, r,...)` &#8660; `Q(p, q, r,...)` e `Q(p, q, r,...)` &#8660; `R(p, q, r,...)` então `P(p, q, r,...)` &#8660; `R(p, q, r,...)`
* Simétrica (__S__)
	* Se `P(p, q, r,...)` &#8660; `Q(p, q, r,...)`  então `Q(p, q, r,...)` &#8660; `P(p, q, r,...)`

## Conclusão

Este foi um post sobre implicação e equivalência lógica, importantes conceitos para prosseguirmos no estudo da lógica matemática e computacional. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos. 

Por hoje é só moçada, abraço!

## Slides

<script async class="speakerdeck-embed" data-id="08c59043e45a449fa761e103125f61ba" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>




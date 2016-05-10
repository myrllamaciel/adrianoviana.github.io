---
layout: post
title: Ganhando superpoderes com as propriedades das operações lógicas fundamentais
description: "Da mesma forma que na matemática básica, onde estudamos operações algébricas com números reais e complexos, na álgebra das proposições estudaremos operações e suas respectivas propriedades envolvendo nossas queridas proposições."
tags: [lógica matemática]
image:
  feature: /posts/2016-05-10-superpoderes.png
comments: true
share: true
---

**Nota:** Neste post conheceremos as propriedades e equivalências das operações lógicas fundamentais. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

Confira os demais posts desta série:

* <a href="/implicacao-e-equivalencia">Implicação e equivalência lógica</a>
* <a href="/tautologia-contraticao-e-contingencia">Tautologia, contradição e contingência</a>
* <a href="/operacoes-logicas-fundamentais">Operações lógicas fundamentais</a>
* <a href="/logica-matematica-e-computacional-primeiros-passos">Lógica matemática e computacional, primeiros passos!</a>

---

Da mesma forma que na matemática básica, onde estudamos operações algébricas com números reais e complexos, na álgebra das proposições estudaremos operações e suas respectivas propriedades envolvendo nossas queridas proposições.

## Idempotência 

Seja `p` uma proposição simples qualquer, temos:

* `p ∧ p` &#8660; `p`
* `p ∨ p` &#8660; `p`

Para ficar mais claro, vejamos os exemplos acima em linguagem natural:

* *Bruce Wayne gosta de rock `e` Bruce Wayne gosta de rock &#8660; Bruce Wayne gosta de rock*
* *Bruce Wayne gosta de rock `ou` Bruce Wayne gosta de rock &#8660; Bruce Wayne gosta de rock*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;color:#0000FF;">p</th>
			<th style="text-align:right;color:#0000FF;">p &and; p</th>
			<th style="text-align:right;color:#0000FF;">p &or; p</th>
		</tr>
	</thead>
	<tbody>
		<tr >
			<td style="text-align:left;">1</td>
			<td style="text-align:center;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Como pode ser visto através da tabela-verdade, o valor lógico de uma conjunção ou disjunção (inclusiva) de uma proposição `p` qualquer, com ela mesma, equivale ao valor lógico da mesma proposição de forma isolada.

## Comutação 

Sejam `p` e `q` proposições simples quaisquer, temos:

* `p ∧ q` &#8660; `q ∧ p`
* `p ∨ q` &#8660; `q ∨ p`

Em linguagem natural:

* *Bruce Wayne gosta de rock `e` Clark Kent gosta de pop &#8660; Clark Kent gosta de pop `e` Bruce Wayne gosta de rock*
* *Bruce Wayne gosta de rock `ou` Clark Kent gosta de pop &#8660; Clark Kent gosta de pop `ou` Bruce Wayne gosta de rock*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &and; q</th>
			<th style="text-align:right;color:#0000FF;">q &and; p</th>
			<th style="text-align:right;color:#00FF00;">p &or; q</th>
			<th style="text-align:right;color:#00FF00;">q &or; p</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#00FF00;">V</td>
			<td style="text-align:right;color:#00FF00;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#00FF00;">V</td>
			<td style="text-align:right;color:#00FF00;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#00FF00;">V</td>
			<td style="text-align:right;color:#00FF00;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#00FF00;">F</td>
			<td style="text-align:right;color:#00FF00;">F</td>
		</tr>
	</tbody>
</table>

Como pode ser visto através da tabela-verdade, o valor lógico de uma conjunção ou disjunção (inclusiva) de duas proposições `p` e `q` quaisquer, é independente quanto a ordem dos fatores.

## Associação 

Sejam `p`, `q` e `r` proposições simples quaisquer, temos:

#### Na conjunção

* `(p ∧ q) ∧ r` &#8660; `p ∧ (q ∧ r)`

Em linguagem natural:

* *Bruce Wayne gosta de rock `e` Clark Kent gosta de pop `e` Lex Luthor gosta de música clássica &#8660; Clark Kent gosta de pop `e` Lex Luthor gosta de música clássica `e` Bruce Wayne gosta de rock*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">p ∧ q</th>
			<th style="text-align:right;">q ∧ r</th>
			<th style="text-align:right;color:#0000FF;">(p ∧ q) ∧ r</th>
			<th style="text-align:right;color:#0000FF;">p ∧ (q ∧ r)</th>
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
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

#### Na disjunção

* `(p ∨ q) ∨ r` &#8660; `p ∨ (q ∨ r)`

Em linguagem natural:

* *Bruce Wayne gosta de rock `ou` Clark Kent gosta de pop `ou` Lex Luthor gosta de música clássica &#8660; Clark Kent gosta de pop `ou` Lex Luthor gosta de música clássica `ou` Bruce Wayne gosta de rock*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">p ∨ q</th>
			<th style="text-align:right;">q ∨ r</th>
			<th style="text-align:right;color:#0000FF;">(p ∨ q) ∨ r</th>
			<th style="text-align:right;color:#0000FF;">p ∨ (q ∨ r)</th>
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
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">6</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Como pode ser visto através das tabelas-verdade, o valor lógico de várias conjunções ou disjunções (inclusivas) é independente quanto a ordem das operações.

## Identidade

Seja `p` proposição simples e sejam `t` e `c` tautologia e contradição respectivamente, temos:

#### Na conjunção

* `p ∧ t` &#8660; `p`
* `p ∧ c` &#8660; `c`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">t</th>
			<th style="text-align:right;">c</th>
			<th style="text-align:right;">p ∧ t</th>
			<th style="text-align:right;">p ∧ c</th>
		</tr>
	</thead>
	<tbody>
		<tr >
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
</table>

Através da tabela-verdade podemos observar que o valor lógico da composta `p ∧ t` vai depender exclusivamente do valor lógico da proposição simples `p`, caso a mesma seja verdadeira, a composta assumirá o valor da Verdade, da mesma forma que, se `p` for Falsa, a composta também irá assumir o valor lógico da Falsidade. Já a composta `p ∧ c` sempre terá o valor lógico da Falsidade independentemente do valor da proposição `p`.

#### Na disjunção

* `p ∨ t` &#8660; `t`
* `p ∨ c` &#8660; `p`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">t</th>
			<th style="text-align:right;">c</th>
			<th style="text-align:right;">p ∨ t</th>
			<th style="text-align:right;">p ∨ c</th>
		</tr>
	</thead>
	<tbody>
		<tr >
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
		</tr>
	</tbody>
</table>

Através da tabela-verdade podemos observar que o valor lógico da composta `p ∨ c` vai depender exclusivamente do valor lógico da proposição simples `p`, caso a mesma seja verdadeira, a composta assumirá o valor da Verdade, da mesma forma que, se `p` for Falsa, a composta também irá assumir o valor lógico da Falsidade. Já a composta `p ∨ t` sempre terá o valor lógico da Verdade independentemente do valor da proposição `p`.

## Distribuição

Sejam `p`, `q` e `r` proposições simples quaisquer, temos:

#### Na conjunção

* `p ∧ (q ∨ r)` &#8660; `(p ∧ q) ∨ (p ∧ r)`

Em linguagem natural:

* *Bruce Wayne gosta de rock `e` Clark Kent gosta de pop `ou` música clássica &#8660; Bruce Wayne gosta de rock `e` Clark Kent gosta de pop `ou` Bruce Wayne gosta de rock `e` Clark Kent gosta de música clássica*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">p ∧ q</th>
			<th style="text-align:right;">q ∨ r</th>
			<th style="text-align:right;">p ∧ r</th>
			<th style="text-align:right;color:#0000FF;">p ∧ (q ∨ r)</th>
			<th style="text-align:right;color:#0000FF;">(p ∧ q) ∨ (p ∧ r)</th>
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
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">6</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

#### Na disjunção

* `p ∨ (q ∧ r)` &#8660; `(p ∨ q) ∧ (p ∨ r)`

Em linguagem natural:

* *Bruce Wayne gosta de rock `ou` Clark Kent gosta de pop `e` música clássica &#8660; Bruce Wayne gosta de rock `ou` Clark Kent gosta de pop `e` Bruce Wayne gosta de rock `ou` Clark Kent gosta de música clássica*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">r</th>
			<th style="text-align:right;">p ∨ q</th>
			<th style="text-align:right;">q ∧ r</th>
			<th style="text-align:right;">p ∨ r</th>
			<th style="text-align:right;color:#0000FF;">p ∨ (q ∧ r)</th>
			<th style="text-align:right;color:#0000FF;">(p ∨ q) ∧ (p ∨ r)</th>
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
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">5</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">6</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">7</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">8</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

## Absorção

Sejam `p` e `q` proposições simples, temos:

#### Na conjunção

* `p ∧ (p ∨ q)` &#8660; `p`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;color:#0000FF;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &or; q</th>
			<th style="text-align:right;color:#0000FF;">p ∧ (p ∨ q)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;color:#0000FF;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;color:#0000FF;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;color:#0000FF;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;color:#0000FF;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

#### Na disjunção

* `p ∨ (p ∧ q)` &#8660; `p`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;color:#0000FF;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;color:#0000FF;">p ∨ (p ∧ q)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;color:#0000FF;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;color:#0000FF;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;color:#0000FF;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;color:#0000FF;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Através das tabelas-verdade podemos comprovar que não há necessidade de aplicar a propriedade distributiva quando a proposição se repete no primeiro e segundo termo.

## Lei de Morgan

Sejam `p` e `q` proposições simples, temos:

#### Na conjunção

* `~(p ∧ q)` &#8660; `~p ∨ ~q`

Em linguagem natural:

* *Não é verdade que Bruce Wayne gosta de rock `e` Clark Kent gosta de pop &#8660; Bruce Wayne não gosta de rock `ou` Clark Kent não gosta de pop*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">p &and; q</th>
			<th style="text-align:right;color:#0000FF;">~(p &and; q)</th>
			<th style="text-align:right;color:#0000FF;">~p &or; ~q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

#### Na disjunção

* `~(p ∨ q)` &#8660; `~p ∧ ~q`

Em linguagem natural:

* *Não é verdade que Bruce Wayne gosta de rock `ou` Clark Kent gosta de pop &#8660; Bruce Wayne não gosta de rock `e` Clark Kent não gosta de pop*

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">p &or; q</th>
			<th style="text-align:right;color:#0000FF;">~(p &or; q)</th>
			<th style="text-align:right;color:#0000FF;">~p &and; ~q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

Podemos perceber que essa importante lei é bem simples de ser aplicada, basta negarmos as duas proposições e trocar o conectivo (o que era conjunção vira disjução e vice-versa).

## Equivalências importantes

Todas as propriedades e leis apresentadas até aqui somente são aplicadas para os conectivos da disjunção (inclusiva) e conjunção. Porém, vimos que também podemos formar proposições compostas através dos conectivos: condicional, bicondicional e disjunção exclusiva. Devemos representar as proposições compostas formadas por esses conectivos através de suas respectivas equivalências.

#### Condicional

Sejam `p` e `q` proposições simples, temos:

* `p → q` &#8660; `~p ∨ q`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;color:#0000FF;">p → q</th>
			<th style="text-align:right;color:#0000FF;">~p &or; q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>


#### Bicondicional

Sejam `p` e `q` proposições simples, temos:

* `p ↔ q` &#8660; `(~p ∧ ~q) ∨ (q ∧ p)`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">~p &and; ~q</th>
			<th style="text-align:right;">q &and; p</th>
			<th style="text-align:right;color:#0000FF;">p ↔ q</th>
			<th style="text-align:right;color:#0000FF;">(~p ∧ ~q) ∨ (q ∧ p)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

#### Disjunção exclusiva

Sejam `p` e `q` proposições simples, temos:

* `p ⊻ q` &#8660; `(p ∧ ~q) ∨ (~p ∧ q)`

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;">~p</th>
			<th style="text-align:right;">~q</th>
			<th style="text-align:right;">p &and; ~q</th>
			<th style="text-align:right;">~p &and; q</th>
			<th style="text-align:right;color:#0000FF;">p ⊻ q</th>
			<th style="text-align:right;color:#0000FF;">(p ∧ ~q) ∨ (~p ∧ q)</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">V</td>
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
			<td style="text-align:right;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Importante notar que a disjunção exclusiva pode ser obtida através da negação de um bicondicional e vice-versa.

## Conclusão

Este foi um post sobre as propriedades e equivalências das operações lógicas fundamentais, conhecimentos que serão de total importância quando tratarmos da validade de argumentos, regras de inferência e dedução lógica. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos. 

Por hoje é só moçada, abraço!

## Slides

<script async class="speakerdeck-embed" data-id="b9fa0ccaa83b4b8fb33435489f90ac09" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>




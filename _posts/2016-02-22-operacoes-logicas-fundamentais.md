---
layout: post
title: Operações lógicas fundamentais
description: "Proposições simples podem ser combinadas através de conectivos lógicos resultando em proposições compostas, denominamos essas combinações de operações lógicas, as mesmas obedecem a regras estabelecidas pelo cálculo proposicional. Conheceremos agora as operações fundamentais."
tags: [lógica matemática]
image:
  feature: /posts/2016-02-22-operacoes-logicas-dogs.png
comments: true
share: true
---


**Nota:** Neste post conheceremos as operações lógicas fundamentais e construiremos as tabelas-verdade correspondentes. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

<div markdown="0"><a href="https://speakerdeck.com/adrianoviana/logica-matematica-e-computacional-tabela-verdade" class="btn">Baixar apresentação</a></div>

---

## Recapitulando

Proposições simples podem ser combinadas através de conectivos lógicos resultando em proposições compostas (caso não esteja familiarizado com os conceitos básicos da lógica <a href="http://www.adrianoviana.com.br/logica-matematica-e-computacional-primeiros-passos/" >clique aqui</a>), denominamos essas combinações de __operações lógicas__, as mesmas obedecem a regras estabelecidas pelo cálculo proposicional. Conheceremos agora as operações fundamentais.

### Negação (~)

Denominamos __negação de uma proposição__ `p` a proposição representada por `não p`, cujo valor lógico é a __Verdade (V)__ quando `p` __é falsa__ e a __falsidade (F)__ quando `p` __é verdadeira__, ou seja, `não p` tem o valor lógico oposto de `p`. Simbolicamente, a negação da proposição `p` é representada através da notação `~p` ou `¬p`. Assim, obtemos a seguinte tabela-verdade:

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left;">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;color:#0000FF;">~p</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">2</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

Em linguagem natural a negação pode ser obtida através do advérbio `não`, basta colocá-lo antes do verbo. Vejamos alguns exemplos:

{% highlight html %}
Exemplo 1:
	p: Winterfell será atacada ao amanhecer
	~p: Winterfell não será atacada ao amanhecer
Exemplo 2:
	p: Os lannisters assumiram o trono de ferro
	~p: Os lannisters não assumiram o trono de ferro
{% endhighlight %}

Também é possível obter negação através de algumas expressões especiais como:

{% highlight html %}
Exemplo 1:
	p: Daenerys está perdida
	~p: Não é verdade que Daenerys está perdida
Exemplo 2:
	p: O inverno está chegando
	~p: É falso que o inverno está chegando
{% endhighlight %}

### Conjunção (&and;)

Chamamos __conjunção de duas proposições__ `p` e `q` a proposição representada por `p e q`, cujo valor lógico é a __Verdade (V)__ quando `p` e `q` forem amabas __verdade__ e a __falsidade (F)__ nos outros possíveis casos. Simbolicamente, a conjunção das proposições `p` e `q` é representada através da notação `p ^ q`. Assim, obtemos a seguinte tabela-verdade:

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &and; q</th>
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
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Em linguagem natural a conjunção pode ser obtida através da adição do conectivo `e` entre as duas proposições componentes. Vejamos alguns exemplos:

{% highlight html %}
Exemplo 1:
	p: John Snow não sabe de nada
	q: Winterfell será atacada ao amanhecer
	p ^ q: John Snow não sabe de nada e Winterfell será atacada ao amanhecer 
Exemplo 2:
	p: Daenerys está perdida
	q: Os lannisters assumiram o trono de ferro
	p ^ q: Daenerys está perdida e os lannisters assumiram o trono de ferro
{% endhighlight %}

### Disjunção Inclusiva (&or;)

Chamamos __disjunção de duas proposições__ `p` e `q` a proposição representada por `p ou q`, cujo valor lógico é a __Verdade (V)__ quando ao menos uma das proposições `p` e `q` forem __verdade__ e a __falsidade (F)__ quando as proposições `p` e `q` forem ambas falsas. Simbolicamente, a disjunção das proposições `p` e `q` é representada através da notação `p v q`. Assim, obtemos a seguinte tabela-verdade:

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &or; q</th>
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
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

Em linguagem natural a disjunção pode ser obtida através da adição do conectivo `ou` entre as duas proposições componentes. Vejamos alguns exemplos:

{% highlight html %}
Exemplo 1:
	p: John Snow não sabe de nada
	q: Winterfell será atacada ao amanhecer
	p ^ q: John Snow não sabe de nada ou Winterfell será atacada ao amanhecer 
Exemplo 2:
	p: Daenerys está perdida
	q: Os lannisters assumiram o trono de ferro
	p ^ q: Daenerys está perdida ou os lannisters assumiram o trono de ferro
{% endhighlight %}

### Disjunção Exclusiva (&#8891;)

Em linguagem natural a palavra `ou` possui dois sentidos. Partindo dessa afirmação vamos considerar duas proposições compostas `P` e `Q` :

{% highlight html %}
	P: John Snow juntou-se a patrulha da noite ou salvou seu povo dos white walkers
	Q: O pai biológico de John Snow é da família Stark ou da família Targaryen 
{% endhighlight %}

Na proposição `P` ao menos uma das proposições componentes `p: John Snow juntou-se a patrulha da noite` e `q: John Snow salvou seu povo dos white walkers` é verdadeira, podendo ser as duas verdadeiras: `P: John Snow juntou-se a patrulha da noite e salvou seu povo dos white walkers`. Porém, na proposição `Q`, uma e somente uma das proposições componentes pode ser verdadeira, pois não pode ocorrer a verdade nas duas ao mesmo tempo: `Q: O pai biológico de John Snow é da família Stark e da família Targaryen`. 

Chamamos o `ou` na proposição `P` de __disjunção inclusiva__ e o `ou` na proposição `Q` de __disjunção exclusiva__. Dessa forma chamamos __disjunção exlusiva de duas proposições__ `p` e `q` a proposição representada por `p ou exlusivo q`, cujo valor lógico é a __Verdade (V)__ quando ao menos uma das proposições `p` e `q` forem __verdade__ e a __falsidade (F)__ quando as proposições `p` e `q` forem ambas falsas ou ambas verdadeiras. Simbolicamente, a disjunção exclusiva das proposições `p` e `q` é representada através da notação p &#8891; q. Assim, obtemos a seguinte tabela-verdade:

<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &#8891; q</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="text-align:left;">1</td>
			<td style="text-align:center;">V</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
</table>

### Condicional (&#8594;)

Chamamos __proposição condicional__ a proposição representada por `se p então q` onde `p` é chamado de antecedente e `q` de consequente, cujo valor lógico é a __Falsidade (F)__ quando `p` é __verdadeira__ e `q` é __falsa__ e a __Verdade (V)__ nos demais casos, ou seja, `p` é condição suficiente para `q` e `q` é condição necessária para `p`. Simbolicamente, a proposição condicional é representada através da notação p &#8594; q. Assim, obtemos a seguinte tabela-verdade:


<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &#8594; q</th>
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
			<td style="text-align:right;color:#0000FF;">F</td>
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
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

Em linguagem natural a proposição condicional pode ser obtida através da adição dos conectivos `se..então` entre as duas proposições componentes. Vejamos alguns exemplos:

{% highlight html %}
Exemplo 1:
	p: John Snow não sabe de nada
	q: Winterfell será atacada ao amanhecer
	p → q: Se John Snow não sabe de nada então Winterfell será atacada ao amanhecer 
Exemplo 2:
	p: Daenerys está perdida
	q: Os lannisters assumiram o trono de ferro
	p → q: Se Daenerys está perdida então os lannisters assumiram o trono de ferro
{% endhighlight %}

**Nota:** Uma proposição condicional não afirma que o consequente se deduz a partir do antecedente.
{: .notice}

### Bicondicional (&#8596;)

Chamamos __proposição bicondicional__ a proposição representada por `p se e somente se q`, cujo valor lógico é a __Verdade (V)__ quando `p` e `q` possuirem valores lógicos iguais e a __falsidade (F)__ caso contrário, ou seja, `p` é condição necessária e suficiente para `q` e `q` é condição necessária e suficiente para `p`.. Simbolicamente, a proposição bicondicional é representada através da notação p &#8596; q. Assim, obtemos a seguinte tabela-verdade:


<table rules="groups" width="100%">
	<thead>
		<tr>
			<th style="text-align:left; ">linha</th>
			<th style="text-align:center;">p</th>
			<th style="text-align:right;">q</th>
			<th style="text-align:right;color:#0000FF;">p &#8596; q</th>
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
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">3</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">V</td>
			<td style="text-align:right;color:#0000FF;">F</td>
		</tr>
	</tbody>
	<tbody>
		<tr>
			<td style="text-align:left;">4</td>
			<td style="text-align:center;">F</td>
			<td style="text-align:right;">F</td>
			<td style="text-align:right;color:#0000FF;">V</td>
		</tr>
	</tbody>
</table>

Em linguagem natural a proposição condicional pode ser obtida através da adição da expressão `se e somente se` entre as duas proposições componentes. Vejamos alguns exemplos:

{% highlight html %}
Exemplo 1:
	p: John Snow não sabe de nada
	q: Winterfell será atacada ao amanhecer
	p → q: John Snow não sabe de nada se e somente se Winterfell será atacada ao amanhecer 
Exemplo 2:
	p: Daenerys está perdida
	q: Os lannisters assumiram o trono de ferro
	p → q: Daenerys está perdida se e somente se os lannisters assumiram o trono de ferro
{% endhighlight %}


## Conclusão

Este foi um post sobre as operações lógicas fundamentais, nos próximos falaremos sobre construções de tabelas-verdade mais complexas. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos. 

Por hoje é só moçada, Abraço!
---
layout: post
title: A pesquisa operacional e a arte da modelagem
description: "A modelagem de um problema nos leva a uma compreensão mais profunda do mesmo, tornando possível identificar seus elementos internos, suas interações com o ambiente externo, as informações necessárias e os possíveis resultados."
tags: [pesquisa operacional]
image:
  feature: /posts/2016-02-23-queue-theory-model.png
comments: true
share: true
---

**Nota:** Neste post conheceremos as abordagens e as fases da Pesquisa Operacional assim como daremos início aos estudos do processo de modelagem. Caso queira acrescentar algo, sinta-se livre para ajudar a melhorá-lo.
{: .notice}

<div markdown="0"><a href="https://speakerdeck.com/adrianoviana/a-arte-da-modelagem" target="_blank" class="btn">Baixar apresentação</a></div>

---

## Abordagens da Pesquisa Operacional

Como vimos <a href="http://www.adrianoviana.com.br/pesquisa-operacional-primeiros-passos/">aqui</a>, desde seu surgimento, a pesquisa operacional vem propondo métodos para auxiliar o processo de tomada de decisão. Para chegar a esse propósito se utiliza principalmente da construção de modelos. No que diz respeito a gestão empresarial a pesquisa operacional pode ser vista por duas abordagens complementares:

### Abordagem Clássica

Neste tipo de abordagem, o objetivo principal é a busca pela solução ótima, ou seja, após a identificação do problema e o levantamento das informações necessárias, são aplicadas técnicas de modelagem e resolução desses modelos visando à obtenção da melhor solução possível como pode ser visto através da figura:

<figure>
	<img src="/images/posts/2016-02-23-classic-focuse-or.png"  />
	<figcaption>Abordagem clássica de problemas de Pesquisa Operacional</figcaption>
</figure>


### Abordagem Atual

A abordagem clássica foi e ainda é bastante útil no campo da administração, porém o alto rigor matemático e a pouca flexibilidade dos modelos frustrava os administradores por produzirem respostas apenas para perguntas padronizadas. 

A abordagem atual surgiu para complementar a clássica. Neste tipo de abordagem, a modelagem de um problema leva a uma compreensão mais profunda do mesmo, tornando possível identificar seus elementos internos, suas interações com o ambiente externo, as informações necessárias e os possíveis resultados, ou seja, os administradores conseguem uma maior compreensão do problema como mostrado na figura:

<figure>
	<img src="/images/posts/2016-02-23-current-focuse-or.png"  />
	<figcaption>Abordagem atual de problemas de Pesquisa Operacional</figcaption>
</figure>

## A arte modelagem

Fica evidente, nas duas abordagens, que o processo de modelagem e solução do problema é a parte mais importante quando se trata de um estudo de Pesquisa Operacional. 

Um modelo pode ser visto como uma __simplificação de um sistema__, este por sua vez, pode já existir ou estar em fase de concepção.  No primeiro caso, o modelo irá servir como instrumento de análise e compreensão do comportamento do sistema existente fornecendo ações para aprimora-lo. No segundo caso, o modelo serve para estruturar o futuro sistema.

<figure>
	<img src="/images/posts/2016-02-23-abstracao-modelo.png"  />
	<figcaption>Níveis de abstração no desenvolvimento do modelo (retirado de TAHA, H. A. 2008)</figcaption>
</figure>

A figura acima mostra os níveis de abstração que constituem o desenvolvimento de um modelo em Pesquisa Operacional. O __mundo real considerado__ é uma abstração da situação real, evidenciando apenas as __variáveis dominantes__ que controlam o comportamento do sistema real. Por fim, o __modelo__ representa de maneira tratável as __funções matemáticas__ que constituem o comportamento do mundo real considerado.

### Exemplo (empresa de fabricação de utensílios domésticos)

Considere uma empresa de fabricação de utensílios domésticos, as matérias-primas necessárias são solicitadas dos próprios estoques da empresa ou comprada de fornecedores externos. No momento que o lote de produção é finalizado, o setor de vendas cuida da distribuição do produto. 

Uma questão interessante para analisarmos nesta empresa é a determinação do tamanho de um lote de produção, vejamos como um modelo pode representar esta situação.

O sistema como um todo possui diversas variáveis que podem o modificar diretamente:

* Capacidade de produção
* Estoque disponível de matérias-primas
* Previsão de vendas
* Etc.

Para o primeiro nível de abstração (mundo real considerado) devemos definir suas fronteiras. Dessa forma, chegamos a duas variáveis dominantes:

* Taxa de produção
* Taxa de consumo

A determinação da taxa de produção envolve variáveis como capacidade de produção e estoque disponível de matérias-primas. A taxa de consumo é determinada pelas variáveis associadas ao departamento de vendas (previsão, etc.). Portanto, a simplificação do mundo real para o mundo real considerado é obtida através do agrupamento de diversas variáveis do mundo real em uma única variável do mundo real considerado.

O próximo nível de abstração (modelo) se torna muito mais simples a partir do mundo real considerado. A partir das duas variáveis identificadas (Taxa de consumo e produção) podem-se estabelecer medições de excesso ou escassez de estoque. O modelo abstraído pode então ser construído para minimizar o custo total do estoque balanceando os custos conflitantes de excesso e escassez de estoque.

### Exemplo (problemas de congestionamento)

Agora vamos analisar duas situações: o desempenho de uma secretária e uma estação de passageiros de trem. Na primeira situação, a secretária pode estar sobrecarregada por várias razões, como por exemplo, o excesso de solicitações do chefe, problema de saúde, etc. Na segunda situação, as variáveis causadoras de problemas são outras, por exemplo, a programação de horário de vendas, a disposição dos guichês, etc.

Para o primeiro nível de abstração (mundo real considerado) definimos as fronteiras do problema chegando a duas variáveis controladoras:

* Número de clientes que chegam ao poto de atendimento por unidade de tempo
* Número de atendimentos que o posto de serviço pode fornecer por unidade de tempo

O próximo nível de abstração (modelo) pode ser representado como um modelo de filas:

<figure>
	<img src="/images/posts/2016-02-23-modelo-filas.png"  />
	<figcaption>Representação do modelo de filas</figcaption>
</figure>

Na situação da secretária, as ordens do chefe são as __chegadas__ ocasionando uma __fila de serviços__, a própria secretária é representada pela estação de __atendimento__ e assim que a mesma conclui a tarefa, gera a __saída__ que representa os serviços prontos.

Na situação da estação de passageiros, as chegadas de passageiros são as __chegadas__ ocasionando uma __fila de passageiros__, a própria estação é representada pela estação de __atendimento__, assim que a mesma atende o passageiro, acontece o __embarque__.

## Fases de estudo

è complicado estabelecer diretrizes exatas para um estudo de Pesquisa Operacional, pois o mesmo envolve uma série de ações complementares entre sí como mostrado anteriormente. Porém, qualquer estudo possui as seguintes etapas principais:

* Definição do problema
* Construção do Modelo
* Solução do Modelo
* Validação do Modelo
* Implementação dos resultados

### Definição do problema

Nesta fase, toda a equipe deve participar afim de estabelecer o escopo do problema, fazer todo o levantamento das informações necessárias para a construção e solução do modelo e fazer a descrição exata dos objetivos do estudo.

### Construção do modelo

Aqui a equipe de pesquisa operacional estabelece os níveis de abstração necessários para representar o sistema real com base nas informações levantadas na fase de definição do problema.

### Solução do modelo

Nesta fase são utilizados os algoritmos e formalismos matemáticos correspondentes ao modelo construído, assim como a utilização de ferramentas computacionais.


### Validação do modelo

Aqui acontece a verificação se a solução fornecida é viável de ser aplicada no sistema real através de uma previsão do comportamento do mesmo.

### Implementação dos resultados

A partir de um modelo solucionado e validado, pode-se retirar os níveis de abstração e aplicar a solução no sistema real. São definidas as regras operacionais e possivelmente, eventuais correções no modelo.

### Resumindo

1. Entenda o problema
2. Modele
3. Teste
4. Implemente para toda a organização

## Conclusão

O processo de tomada de decisão de um executivo pode ser desenvolvido em __ambientes especialmente construídos (a arte da modelagem)__ tornando possível a tomada de __decisão com qualidade__. Se você tem alguma dúvida, crítica ou sugestão, não esqueça de deixar seu comentário abaixo. Se gostou dessa postagem não esqueça de compartilhar com seus amigos. 

Por hoje é só moçada, abraço!

## Slides

<script async class="speakerdeck-embed" data-id="315809f8baeb4d9286aafe79bf07180f" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>




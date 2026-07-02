# Miniguia de Estudos com NotebookLM

## Caderno Temático: Teorias dos Fãs sobre *Jogos Vorazes*

## Contexto

Este projeto foi desenvolvido como parte do desafio da DIO sobre o uso do **NotebookLM** como ferramenta de aprendizagem ativa.

Como tema de estudo, escolhi investigar **teorias criadas pela comunidade de fãs da série *Jogos Vorazes***, utilizando como única fonte de conhecimento todos os livros da saga escritos por Suzanne Collins.

O objetivo não foi descobrir novas teorias, mas verificar até que ponto um modelo de linguagem consegue recuperar informações presentes nas obras, conectar acontecimentos distribuídos entre diferentes livros e analisar hipóteses elaboradas pelos leitores.

---

# Objetivos

Os principais objetivos deste estudo foram:

* Utilizar o NotebookLM como ferramenta de análise literária baseada exclusivamente nos livros da saga.
* Investigar teorias populares da comunidade de fãs.
* Verificar quais teorias possuem evidências textuais e quais dependem apenas de interpretação.
* Avaliar a capacidade do modelo em recuperar informações espalhadas entre diferentes volumes.
* Observar as limitações da IA ao interpretar aspectos subjetivos da narrativa, como emoções, simbolismos e narradores pouco confiáveis.

---

# Fontes

Foram utilizados como base de conhecimento os cinco livros da saga.

* *Jogos Vorazes*
* *Em Chamas*
* *A Esperança*
* *A Cantiga dos Pássaros e das Serpentes*
* *Amanhecer na Colheita*

Todos os livros foram adicionados ao NotebookLM para que as respostas fossem fundamentadas exclusivamente no conteúdo das obras.

---

# Engenharia de Prompts e Cicatrizes

O NotebookLM foi utilizado para investigar teorias populares da comunidade de fãs. Em vez de realizar perguntas isoladas, os prompts foram refinados progressivamente para aprofundar a análise e avaliar as limitações do modelo.

## Objetivo do experimento

Verificar se o NotebookLM consegue:

* recuperar informações distribuídas entre diferentes livros;
* conectar acontecimentos cronologicamente;
* diferenciar fatos explícitos de interpretações;
* analisar teorias criadas pelos fãs;
* interpretar sentimentos e motivações dos personagens.

---

## Experimento 1 — O triângulo amoroso

A primeira sequência de perguntas investigou os sentimentos de Katniss.

### Prompt inicial

> Katniss já gostou romanticamente de Gale?

O modelo recuperou acontecimentos de toda a saga e concluiu que Katniss desenvolveu sentimentos românticos por Gale ao longo da história.

Em seguida, os prompts foram refinados:

* Quando Katniss começou a gostar romanticamente de Peeta?
* Ela gostou de Peeta e Gale ao mesmo tempo?

### Resultado

O NotebookLM conseguiu reconstruir corretamente a evolução do relacionamento entre Katniss, Gale e Peeta, utilizando acontecimentos distribuídos entre os livros.

### Cicatriz

Apesar de recuperar corretamente os eventos, o modelo interpreta os pensamentos narrados por Katniss como fatos objetivos. Como ela frequentemente não compreende os próprios sentimentos, o NotebookLM apresenta dificuldade em interpretar o subtexto emocional da personagem.

---

## Experimento 2 — Avaliação de teorias dos fãs

### Prompt

> Nos 74º Jogos Vorazes, Foxface morre após comer amoras venenosas. Alguns fãs acreditam que ela escolheu morrer de forma indolor. Essa teoria faz sentido?

### Resultado

O modelo apresentou argumentos favoráveis e contrários, citou acontecimentos relevantes da narrativa e concluiu que a teoria é plausível, mas que os livros indicam com mais força que Foxface foi enganada pela falta de conhecimento de Peeta sobre plantas.

### Cicatriz

O NotebookLM consegue analisar teorias utilizando evidências textuais, porém evita confirmar interpretações que não possuem confirmação explícita nas obras.

---

## Experimento 3 — Cronologia e plausibilidade

### Prompt

> Fãs acreditam que Alma Coin possa ser neta de Lucy Gray. Levando em consideração a diferença de idade, faz sentido?

Após a resposta, foi realizado um refinamento:

> A teoria de ela ser filha faria mais sentido cronológico?

### Resultado

O NotebookLM calculou corretamente a diferença de idade entre as personagens e concluiu que, caso existisse parentesco direto, a hipótese de Coin ser filha de Lucy Gray seria cronologicamente mais plausível do que ser sua neta.

### Cicatriz

O NotebookLM consegue verificar se uma teoria é cronologicamente possível, mas não diferencia claramente uma hipótese plausível de uma hipótese sustentada pelo texto. Em alguns momentos, uma conclusão lógica pode parecer mais forte do que realmente é dentro da narrativa.

---

## Experimento 4 — Mistérios sem resposta oficial

### Prompts

* O que aconteceu com Lucy Gray no final do livro?
* Você acha que ela sobreviveu ou morreu?

### Resultado

O NotebookLM reuniu evidências que sustentam tanto a hipótese de sobrevivência quanto a de morte, respeitando a ambiguidade deixada propositalmente pela autora.

### Cicatriz

Quando não existe resposta oficial, o modelo evita assumir uma posição definitiva e prefere apresentar todas as interpretações compatíveis com o texto.

---

## Experimento 5 — Interpretação psicológica

### Prompts

* Snow amava Lucy Gray de verdade?
* Lucy Gray amava Snow de verdade?

### Resultado

O NotebookLM reuniu passagens sobre afeto, possessividade, manipulação, confiança e traição para construir uma análise consistente da relação entre os personagens.

### Cicatriz

Embora consiga reunir evidências relevantes, o modelo evita conclusões categóricas sobre estados emocionais quando eles dependem de interpretação do leitor.

---

# Miniguia de Estudo

## Resumo

A saga *Jogos Vorazes* utiliza frequentemente narradores limitados e finais abertos, permitindo múltiplas interpretações dos acontecimentos.

Esse aspecto faz surgir inúmeras teorias elaboradas pelos fãs, principalmente sobre:

* o triângulo amoroso entre Katniss, Peeta e Gale;
* o destino de Lucy Gray;
* o passado de Coriolanus Snow;
* possíveis relações familiares entre personagens;
* acontecimentos deixados em aberto pela autora.

O NotebookLM demonstrou excelente capacidade de recuperar informações distribuídas entre diferentes livros e utilizá-las para responder perguntas complexas. Entretanto, interpretações que dependem de subtexto, emoções implícitas e simbolismos continuam representando um desafio para o modelo.

---

# Glossário

**Subtexto**

Informações implícitas que não são afirmadas diretamente pelo texto.

**Teoria de fã**

Hipótese criada pelos leitores para explicar acontecimentos não confirmados oficialmente.

**Evidência textual**

Trecho do livro utilizado para justificar uma interpretação.

**Inferência**

Conclusão construída a partir de diferentes evidências presentes na narrativa.

**Narrador não confiável**

Narrador cuja percepção dos acontecimentos pode ser limitada ou influenciada por seus próprios sentimentos. Katniss é um exemplo desse tipo de narrador.

**Recuperação de contexto**

Capacidade do modelo de localizar informações relevantes dentro das fontes fornecidas.

---

# Prompts reutilizáveis

Os seguintes prompts podem ser utilizados para analisar outras obras literárias utilizando o NotebookLM:

* Quais evidências dos livros apoiam essa teoria?
* Existem passagens que contradizem essa hipótese?
* Diferencie fatos confirmados de interpretações dos leitores.
* Construa uma linha do tempo dos acontecimentos relacionados a esse personagem.
* Cite todos os trechos relevantes para responder essa pergunta.
* Analise essa teoria utilizando apenas informações presentes nas fontes.
* Existe alguma inconsistência cronológica nessa hipótese?
* Quais são os argumentos favoráveis e contrários para essa interpretação?
* Há elementos de subtexto que influenciam essa conclusão?
* Essa resposta depende de fatos explícitos ou de interpretação?

---

# Conclusão

O NotebookLM demonstrou excelente desempenho na recuperação de informações e na construção de respostas fundamentadas exclusivamente nas fontes fornecidas.

Os melhores resultados foram obtidos quando os prompts solicitavam evidências específicas, comparações entre acontecimentos e diferenciação entre fatos e interpretações.

Por outro lado, observou-se que modelos de linguagem ainda apresentam limitações na interpretação de aspectos subjetivos da narrativa. Personagens como Katniss, que frequentemente não compreendem plenamente seus próprios sentimentos, representam um desafio para a IA, que tende a interpretar suas falas como verdades objetivas.

A experiência mostrou que o NotebookLM é uma ferramenta extremamente útil para estudos, revisão de conteúdo e análise de obras literárias, mas que a interpretação crítica do leitor continua sendo indispensável em discussões que envolvem ambiguidades e subtexto.

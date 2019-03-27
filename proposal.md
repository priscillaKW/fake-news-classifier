# Nanodegree - Engenheiro de Machine Learning
## Proposta de projeto final
Priscilla Koch Wagner  
20 de março de 2019

### Histórico do assunto

A disseminação de notícias falsas (fake news em inglês), tem o poder de interferir em diversos setores da sociedade, como política, saúde, segurança, etc. Podem também prejudicar empresas, celebridades, políticos e até pessoas comuns. Qualquer tipo de fake news pode induzir pessoas à erros e ter consequências sérias. Atualmente, por conta da fácil disseminação de informações em redes sociais, as fake news ficaram mais populares. Por isso,  a identificação e punição de autores de fake news se tornou uma grande necessidade para autoridades em todo o mundo. Nessa competição para estudantes, disponível na plataforma Kaggle, é disponibilizado um conjunto de notícias com o objetivo de classificar quais são confiáveis e quais não são.  

Como irei iniciar um projeto que envolve NLP no meu trabalho, esse desafio é ótimo para testar e aperfeiçoar meus conhecimentos na área. Além disso, tenho me interessado pessoalmente em pesquisar como a disseminação de fake news tem interferido em assuntos importantes e alterando rumo de sociedades ao redor do mundo.


### Descrição do problema

O objetivo desse desafio é auxiliar na classificação de notícias confiáveis e não confiáveis através de algoritmos de Machine Learning. Os algoritmos que serão utilizados serão comparados entre si a fim de determinar qual possui maior acurácia para resolver o problema descrito acima. A solução poderá ser comparada com os primeiros vencedores da competição do Kaggle.


### Conjuntos de dados e entradas

O conjunto de dados foi obtido a partir da competição para estudantes disponível no Kaggle. A competição, bem como o conjunto de dados pode ser acessado através do link: https://www.kaggle.com/c/fake-news/data.

O conjunto de dados consiste de notícias obtidas durante o último período eleitoral dos Estados Unidos. As notícias foram previamente divididas em conjunto de treinamento e de teste sendo que existem 20.800 notícias no conjunto de treinamento e 5.200 notícias no conjunto de teste. Cada notícia tem como atributos: um id, o título, o autor e o próprio conteúdo (pode estar inclompleto), e foram classificadas como confiáveis e não confiáveis (rótulo). 


### Descrição da solução

Dado que o problema envolve análise de texto, a solução utilizará técnicas de NLP (Natural Language Processing). A solução utilizará algoritmos de aprendizagem supervisionada, dado que o conjunto de dados é rotulado. Os algoritmos que serão analisados para encontrar a melhor solução, serão: AdaBoost, RandomForest e Regressão Logística. A análise da solução será feita utilizando métricas padrão de análise de algoritmos supervisinados como: acurácia, precision, recall, f1-score. 


### Modelo de referência (benchmark)
_(aproximadamente 1-2 parágrafos)_

Até o 7 do leaderboard público.

Nesta seção, forneça os detalhes de um modelo ou resultado de referência que esteja relacionado ao assunto, definição do problema e solução proposta. Idealmente, o resultado ou modelo de referência contextualiza os métodos existentes ou informações conhecidas sobre o assunto e problema propostos, que podem então ser objetivamente comparados à solução. Descreva detalhadamente como o resultado ou modelo de referência é mensurável (pode ser medido por alguma métrica e claramente observado).


### Métricas de avaliação

A principal métrica para avaliação será a acurácia (quanto maior, melhor), pois foi a métrica escolhida para avaliação da competição do kaggle. Os 2 melhores resultados apresentados no leaderboard público da competição do kaggle, utilizados como benchmark, possuem uma acurácia de 0.98. Como o objetivo no kaggle é ganhar na pontuação com pequenas mudanças no placar, vamos nos concentrar em obter um modelo com, no mínimo, 0.9 de acurácia, o que me colocaria na posição 8 do placar.
A acurácia é calculada pela equação abaixo:

$$
accuracy = \frac{correct predictions}{correct predictions + incorrect predictions}
$$

Além da acurácia, outras métricas serão consideradas: precision (quantas notícias preditas como confiáveis são realmente confiáveis), recall(quantas notícias confiáveis foram preditas como confiáveis) e f1-score (média harmônica entre precision e recall).


### Design do projeto
_(aprox. 1 página)_

Nesta seção final, sintetize um fluxo de trabalho teórico para obtenção de uma solução para o problema em questão. Discuta detalhadamente quais estratégias você considera utilizar, quais análises de dados podem ser necessárias de antemão e quais algoritmos serão considerados na sua implementação. O fluxo de trabalho e discussão propostos devem estar alinhados com as seções anteriores. Adicionalmente, você poderá incluir pequenas visualizações, pseudocódigo ou diagramas para auxiliar na descrição do design do projeto, mas não é obrigatório. A discussão deve seguir claramente o fluxo de trabalho proposto para o projeto de conclusão.

-----------

**Antes de enviar sua proposta, pergunte-se. . .**

- A proposta que você escreveu segue uma estrutura bem organizada, similar ao modelo de projeto?
- Todas as seções (em especial, **Descrição da solução** e **Design do projeto**) estão escritas de uma forma clara, concisa e específica? Existe algum termo ou frase ambígua que precise de esclarecimento?
- O público-alvo de seu projeto será capaz de entender sua proposta?
- Você revisou sua proposta de projeto adequadamente, de forma a minimizar a quantidade de erros gramaticais e ortográficos?
- Todos os recursos usados neste projeto foram corretamente citados e referenciados?




http://qwone.com/~jason/20Newsgroups/
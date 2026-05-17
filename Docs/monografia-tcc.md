# CENTRO ESTADUAL DE EDUCAÇÃO TECNOLÓGICA PAULA SOUZA
# Faculdade de Tecnologia Baixada Santista – Rubens Lara
# Curso Superior de Tecnologia em Sistemas para Internet

**Diego de Oliveira Ferreira**
**Kauê de Oliveira Martins**

## PomoHistória

Santos, SP
2026

---

**Diego de Oliveira Ferreira**
**Kauê de Oliveira Martins**

### PomoHistória

Trabalho de Conclusão de Curso apresentado à Faculdade de Tecnologia Rubens Lara, como exigência para a obtenção do Título de Tecnólogo em Sistemas para Internet.

**Orientador:** Prof.

Santos, SP
2026

---

## RESUMO

No contexto da preparação para o vestibular, muitos estudantes encontram dificuldades para manter a regularidade dos estudos, administrar o tempo de forma eficiente e sustentar a atenção por longos períodos, sobretudo diante das distrações frequentes do meio digital. Entre as estratégias utilizadas para enfrentar esse problema, destaca-se a Técnica Pomodoro, que organiza o estudo em intervalos de concentração alternados com pausas, favorecendo maior foco e melhor aproveitamento das tarefas. Considerando esse cenário, este projeto propõe o desenvolvimento do PomoHistória, uma aplicação web voltada ao estudo de História para vestibulandos. A proposta consiste em reunir, em um mesmo ambiente, organização do tempo, acompanhamento do desempenho e estímulos visuais de progresso, de modo a tornar a experiência de aprendizagem mais envolvente. Para isso, o sistema contará com temporizador inspirado na técnica Pomodoro, questionários sobre conteúdos históricos, cadastro e armazenamento do progresso do usuário, além de um personagem virtual que evolui conforme o estudante avança em seus estudos. O projeto também prevê regras de progressão baseadas no desempenho obtido nas atividades, exigindo aproveitamento mínimo para continuidade, bem como mecanismos que desencorajam a interrupção dos ciclos de estudo. Com isso, espera-se oferecer uma ferramenta de apoio capaz de contribuir para a disciplina, a constância e o engajamento do vestibulando, associando produtividade e motivação em uma proposta digital aplicada ao ensino de História.

**Palavras-chaves:** Método Pomodoro. História. Estudo.

---

## ABSTRACT

In the context of preparing for university entrance exams, many students face difficulties in maintaining regular study habits, managing their time efficiently, and sustaining attention for long periods, especially in the face of frequent distractions in the digital environment. Among the strategies used to address this issue, the Pomodoro Technique stands out, as it organizes study sessions into intervals of concentration alternated with breaks, promoting greater focus and better use of study tasks. Considering this scenario, this project proposes the development of PomoHistória, a web application aimed at supporting History studies for students preparing for university entrance exams. The proposal consists of bringing together, in a single environment, time organization, performance monitoring, and visual progress stimuli, in order to make the learning experience more engaging. To achieve this, the system will include a timer inspired by the Pomodoro Technique, quizzes on historical content, user registration and progress storage, as well as a virtual character that evolves as the student advances in their studies. The project also includes progression rules based on the performance achieved in the activities, requiring a minimum level of achievement for continuation, as well as mechanisms that discourage the interruption of study cycles. Thus, it is expected to provide a support tool capable of contributing to the student's discipline, consistency, and engagement, associating productivity and motivation in a digital proposal applied to the teaching of History.

**Keywords:** Pomodoro Technique. History. Study.

---

## LISTA DE ABREVIATURAS E SIGLAS

Abreviatura ou sigla 01 – Título	01

---

## LISTA DE ILUSTRAÇÕES

Ilustração  01 – Título	01

---

## LISTA DE TABELAS

TABELA 01 - IMPACTOS DO METODO POMODORO – 11

---

## SUMÁRIO

1. INTRODUÇÃO – 9
   - 1.1 OBJETIVO – 10
     - 1.1.1 OBJETIVO GERAL – 10
     - 1.1.2 OBJETIVOS ESPECÍFICOS – 10
   - 1.2 ESTADO DA ARTE – 11
     - Fundamentação Teórica da Técnica Pomodoro – 11
     - Aplicações e Eficácia no Ensino – 11
     - Impactos do Método Pomodoro – 11
     - Gamificação e Engajamento – 12
     - Análise de Mercado e Lacunas – 12
2. DESENVOLVIMENTO – 12
   - 2.1 ANÁLISE DO SISTEMA – 12
     - 2.1.1 ANÁLISE DE REQUISITOS – 13
     - 2.1.2 DIAGRAMA DE CASO DE USO – 13
     - 2.1.3 FLUXO DE EVENTOS – 13
   - 2.2 BANCO DE DADOS – 13
   - 2.3 CAMADA DE NEGÓCIO – 14
   - 2.4 CAMADA DE APRESENTAÇÃO – 14
3. RESULTADO – 15
REFERÊNCIAS BIBLIOGRÁFICAS – 16
ANEXO A – 17

---

## 1. INTRODUÇÃO

No cenário educacional contemporâneo, a preparação para exames vestibulares exige dos estudantes não apenas a absorção de grande volume de conteúdo, mas também disciplina e gerenciamento eficiente do tempo. A dificuldade em manter a concentração por longos períodos e organizar as sessões de estudo de maneira produtiva constitui um dos principais desafios enfrentados por vestibulandos, especialmente diante da crescente quantidade de distrações presentes no ambiente digital.

Nesse contexto, destaca-se a Técnica Pomodoro, desenvolvida por Francesco Cirillo no final da década de 1980 e amplamente difundida a partir dos anos 1990. Trata-se de um método de gerenciamento de tempo que propõe a divisão do trabalho em intervalos curtos e focados, tradicionalmente de 25 minutos, intercalados por pausas breves. Segundo Cirillo (2018), a técnica visa reduzir a ansiedade relacionada ao tempo e aumentar a concentração ao minimizar interrupções, mostrando-se particularmente adequada a atividades que exigem atenção sustentada, como o estudo para vestibulares.

O presente trabalho insere-se nesse cenário ao propor o desenvolvimento de um sistema web denominado PomoHistória, que integra a Técnica Pomodoro a conteúdos de História Geral e História do Brasil direcionados a vestibulandos. A delimitação do projeto concentra-se na criação de uma ferramenta que, além de estruturar o tempo de estudo por meio de ciclos pomodoro, incorpora um sistema de questionários progressivos — nos quais o usuário somente avança para o próximo tema ao atingir 70% de aproveitamento — e um personagem virtual cuja evolução visual acompanha o progresso do estudante pelos períodos históricos. Tal abordagem busca combinar produtividade, avaliação contínua e elementos lúdicos para enriquecer a experiência de aprendizagem.

Observa-se, no entanto, que embora a Técnica Pomodoro seja amplamente empregada, sua aplicação isolada não garante a efetividade do aprendizado, uma vez que o estudante permanece responsável pela seleção e assimilação autônoma dos conteúdos. Diante disso, o problema central que orienta este projeto pode ser formulado da seguinte maneira: como conciliar o gerenciamento do tempo de estudo, por meio da Técnica Pomodoro, com mecanismos estruturados de avaliação e engajamento que favoreçam a retenção de conteúdo histórico por vestibulandos?

### 1.1 OBJETIVO

Considerando os desafios enfrentados por vestibulandos na gestão do tempo e na manutenção do foco em conteúdo densos de História, este item apresenta as metas fundamentais do projeto PomoHistória. O objetivo geral e os objetivos específicos aqui delineados servem como guia para a resolução da problemática apresentada, estabelecendo os critérios técnicos e pedagógicos para o desenvolvimento da aplicação.

#### 1.1.1 OBJETIVO GERAL

O intuito do projeto é desenvolver uma aplicação web que utilize o método Pomodoro de estudo, com o uso de um personagem virtual para acompanhar o progresso do usuário, ajudando-o a manter o foco e consistência nos estudos, junto de uma recompensa visual.

O site contará com um sistema de questionário voltado a conteúdos de história de vestibulares, ajudando nos estudos dos vestibulandos. O personagem virtual irá progredir conforme o vestibulando avança em seus estudos e isso se dá com a mudança visual do personagem.

#### 1.1.2 OBJETIVOS ESPECÍFICOS

1. Projetar e implementar uma interface responsiva e intuitiva, garantindo acessibilidade e usabilidade em diferentes dispositivos.
2. Implementar um sistema temporizador baseado na técnica Pomodoro, permitindo o gerenciamento dos ciclos de estudo.
3. Desenvolver um personagem virtual, cuja evolução visual esteja diretamente vinculada ao progresso do usuário nos módulos de história, oferecendo feedback lúdico e motivacional.
4. Estabelecer um sistema de penalidades, a fim de desestimular o abandono ou a não conclusão dos ciclos de estudo, promovendo a disciplina.
5. Criar um sistema de avaliação de conhecimento, por meio de questionários, para mensurar as habilidades adquiridas pelo usuário durante os períodos de estudo.
6. Implementar um sistema de autenticação e armazenamento de dados, permitindo que o usuário mantenha seu histórico de progresso de forma personalizada.

### 1.2 ESTADO DA ARTE

#### Fundamentação Teórica da Técnica Pomodoro

A Técnica Pomodoro, criada por Francesco Cirillo no final da década de 1980, baseia-se na alternância entre blocos de trabalho focado e breves intervalos de descanso. A premissa central é que a segmentação temporal auxilia no gerenciamento da carga cognitiva, facilitando a codificação da informação no cérebro e prevenindo a exaustão mental. Cirillo estabeleceu que o "pomodoro" é uma unidade indivisível: se houver interrupção, o ciclo deve ser reiniciado, treinando a mente para ignorar distrações.

#### Aplicações e Eficácia no Ensino

Pesquisas recentes indicam que o método é altamente eficaz no ambiente educacional. Uma revisão de 32 estudos envolvendo 5.270 participantes demonstrou que 88% das aplicações obtiveram resultados positivos, com uma redução média de 20% na fadiga mental e melhora na motivação do aluno. No ensino de disciplinas densas, como Biologia e História, a técnica atua como um andaime metacognitivo que ajuda o estudante a gerenciar sua autonomia e fixar termos complexos.

#### Impactos do Método Pomodoro

| Atributo Avaliado         | Impacto Médio Identificado |
|---------------------------|----------------------------|
| Fadiga Mental             | Redução de ~20%            |
| Foco Autorrelatado        | Aumento de 15% a 25%       |
| Eficiência de Aprendizagem | Incremento de 12%          |

#### Gamificação e Engajamento

A gamificação integra elementos de jogos em contextos sérios para disparar a liberação de dopamina, mantendo o foco sustentado. Ao associar o ciclo Pomodoro a recompensas visuais, como o crescimento de árvores (aplicativo Forest) ou a evolução de civilizações (Age of Pomodoro), o sistema capitaliza sobre a motivação extrínseca para sedimentar hábitos de estudo. O sistema PomoHistória alinha-se a essa tendência ao vincular a evolução de um personagem virtual ao progresso curricular, preenchendo uma lacuna de mercado onde a maioria das ferramentas é "vazia" de conteúdo didático específico.

#### Análise de Mercado e Lacunas

O mapeamento de softwares atuais revela ferramentas robustas como Focus To-Do e Reclaim.ai, que focam em automação e produtividade geral. No entanto, raras aplicações integram o cronômetro diretamente a um banco de conteúdos curriculares verticalizados para exames como o vestibular. O PomoHistória posiciona-se como uma resposta a essa lacuna, unindo a mecânica de tempo, a diversão da gamificação e a necessidade acadêmica de preparação em História.

---

## 2. DESENVOLVIMENTO

Nesse capítulo será abordado as fases do desenvolvimento do sistema proposto. Para tanto, esse capítulo será subdividido nos seguintes itens; análise do sistema, a estrutura do Banco de Dados, as ferramentas utilizadas para o desenvolvimento do front-end e as principais rotinas implementadas no back-end.

### 2.1 ANÁLISE DO SISTEMA

Entre vários mecanismos de análise disponível para o desenvolvimento de um sistema, foi feita a escolha pela Unified Modeling Language (UML) por ser uma linguagem de modelagem, isto é, uma forma de especificar um sistema de maneira visual (procurar uma citação).

#### 2.1.1 ANÁLISE DE REQUISITOS

Nesta fase ocorre a captura das intenções e as necessidades dos usuários a ser desenvolvido através dos requisitos funcionais (RF) que nesse caso serão:

[RF01] [RF0x] ...

#### 2.1.2 DIAGRAMA DE CASO DE USO

Com os requisitos funcionais estabelecidos, o próximo passo é a criação do diagrama de caso de uso que tem como finalidade a representação gráfica e semântica da interação do usuário e o sistema, bla bla bla...

O diagrama de caso de uso desse sistema pode ser visualizado no Apêndice A.

#### 2.1.3 FLUXO DE EVENTOS

O fluxo de eventos tem por intenção caracterizar o início e o término do caso de uso, estabelecer a interação dos atores no processo em descrição, gerando assim um fluxo principal e um fluxo alternativo do comportamento de cada caso de uso do sistema, bla bla bla...

A descrição dos fluxos de eventos desse sistema pode ser consultada no Apêndice B.

### 2.2 BANCO DE DADOS

Aqui a intenção é mostrar a modelagem dos dados, através de suas tabelas e também apresentar o MER (Modelo Entidade Relacionamento).

### 2.3 CAMADA DE NEGÓCIO

Nesse tópico se comenta parte do código que for relevante para o desenvolvimento em questão, fazendo as respectivas considerações.

### 2.4 CAMADA DE APRESENTAÇÃO

Aqui são apresentadas as telas principais e quais as características técnicas do seu desenvolvimento e seu respectivo comentário.

---

## 3. RESULTADO

Deve ser mostrado os resultados dos testes de desenvolvimento e os testes finais do sistema junto ao usuário.

Finalizando com uma conclusão, isto é, comprovando se os objetivos firmados no cap.1 foram atingidos e se não foram o que aconteceu para inviabilizar a proposta inicial.

---

## REFERÊNCIAS BIBLIOGRÁFICAS

CIRILLO, Francesco. **A Técnica Pomodoro**. Tradução de Camilla Werner. Rio de Janeiro: Sextante, 2018. Título original: The Pomodoro Technique.

MÜLLER NETO, Marcos Antônio. Aplicabilidade do Método Pomodoro no Ensino Médio nas aulas de Ciências Biológicas. **Revista Científica Multidisciplinar Núcleo do Conhecimento**, 2023. Disponível em: https://revistaft.com.br/aplicabilidade-do-metodo-pomodoro-no-ensino-medio-nas-aulas-de-ciencias-biologicas/. Acesso em: 08 abr. 2026.

SCOPING Review on the Pomodoro Technique (PT) in education. **PMC - PubMed Central**, 2023. Disponível em: https://pmc.ncbi.nlm.nih.gov/articles/PMC12532815/. Acesso em: 08 abr. 2026.

SHIKUDO. **Age of Pomodoro: Focus timer**. 2026. Disponível em: https://play.google.com/store/apps/details?id=com.shikudo.focus.civilization.google. Acesso em: 08 abr. 2026.

---

## ANEXO A

## OBSERVAÇÃO IMPORTANTE...

**ANEXO** – é todo e qualquer documento que alicerça as necessidades do usuário, sendo isso, fornecido pelo mesmo.

**APÊNDICE** – é todo e qualquer documento que fora concebido no desenvolvimento do sistema que dá uma abrangência maior para a sua compreensão.
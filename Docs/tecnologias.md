# **PomoHistória**

- **Equipe:** Diego Ferreira e Kauê de Oliveira
- **Público-alvo:** Jovens e estudantes de 16 a 19 anos que estão se preparando para o vestibular.
- **Tipo de aplicação:** Aplicação web.
- **Plataforma(s):** Web.
- **Domínio:** Educação e Produtividade
- **Previsão de entrega:** 27/06/2026

## **Visão geral**

> O PomoHistória é uma aplicação web voltada ao estudo de História para vestibulandos, que integra a organização do tempo através da Técnica Pomodoro com estímulos visuais de progresso e gamificação.

## **Problema**

> Muitos estudantes encontram dificuldades em manter a regularidade dos estudos, administrar o tempo de forma eficiente e sustentar a atenção diante das distrações digitais. Isso gera ansiedade e prejudica a absorção do grande volume de conteúdo exigido nos vestibulares.

## **Solução proposta**

> A plataforma oferece um ambiente que reúne um temporizador Pomodoro, questionários de conteúdos históricos e um personagem virtual que evolui conforme o estudante avança nos módulos. O sistema utiliza recompensas visuais e regras de progressão para tornar a aprendizagem mais envolvente e disciplinada.

## **Funcionalidades**

- **Temporizador inspirado na técnica Pomodoro** para gerenciamento dos ciclos de foco e pausa.
- **Sistema de questionários progressivos**, exigindo aproveitamento mínimo de 70% para avançar entre os temas históricos.
- **Personagem virtual com evolução visual** vinculada ao progresso nos estudos do usuário.
- Sistema de **autenticação e armazenamento de dados** para manutenção do histórico de progresso personalizado.
- **Mecanismos de penalidade** para desestimular a interrupção dos ciclos de estudo, promovendo a constância.
- Interface responsiva e intuitiva para uso em diferentes dispositivos.

## **Diferencial / Concorrência**

> Embora existam ferramentas de produtividade robustas como o *Focus To-Do* ou o *Forest*, raras aplicações integram o cronômetro diretamente a um banco de conteúdos curriculares específicos para o vestibular. O PomoHistória diferencia-se ao unir a mecânica de tempo e a gamificação à necessidade acadêmica real de preparação em História Geral e do Brasil.

## **Inovação / Criatividade**

> O projeto inova ao utilizar a gamificação (evolução de personagem e civilizações) como um "andaime" para disparar a motivação do aluno. Além disso, preenche uma lacuna de mercado ao oferecer uma ferramenta de produtividade que não é "vazia" de conteúdo didático.

## **Escopo do projeto**

### **Essencial (MVP – obrigatório)**

- Sistema de cadastro e login de usuários.
- Temporizador Pomodoro funcional.
- Banco de questões de História com sistema de correção automática.

### **Importante (se houver tempo)**

- Desenvolvimento visual das fases de evolução do personagem virtual.
- Implementação da regra de aproveitamento mínimo (70%) para progressão de módulos.

### **Opcional (baixa prioridade)**

- Sistema de ranking entre usuários ou integração com outras disciplinas.

## **Planejamento (simplificado)**

| Etapa | Descrição | Prazo |
|-------|-----------|-------|
| 1 | Definição do projeto | 08/04/2026 |
| 2 | Desenvolvimento inicial | 19/04/2026 |
| 3 | Integração | 05/2026 |
| 4 | Testes | 05/2026 |
| 5 | Entrega final | 06/2026 |

## **Tecnologias**

O PomoHistória utiliza um conjunto de tecnologias modernas para garantir desempenho, escalabilidade e facilidade de manutenção. O front-end é desenvolvido com **React**, responsável pela interface visual e interação com o usuário. O back-end é implementado em **Java** com o framework **Spring Boot**, que expõe uma API REST para processar as regras de negócio e gerenciar a persistência dos dados. O banco de dados escolhido foi o **PostgreSQL**, que armazena informações de usuários, progressão nos módulos, histórico de estudos e questões. Para o versionamento de código, utiliza-se **Git** e **GitHub**, enquanto o acompanhamento do projeto é feito com **Trello**.

## **Estrutura da aplicação**

A aplicação será organizada em três camadas principais:

- **Front-end (React)** – Responsável pela interface do usuário, incluindo o temporizador Pomodoro, a exibição do personagem virtual, os questionários e o painel de progresso. O front-end consome a API REST fornecida pelo back-end e comunica-se exclusivamente via requisições HTTP.

- **Back-end (Spring Boot com Java)** – Contém as regras de negócio: cálculo de aproveitamento nos questionários, evolução do personagem, aplicação das penalidades, autenticação e gerenciamento de sessões. Expõe endpoints RESTful para o front-end. Utiliza o ecossistema Spring (Spring Data JPA, Spring Security, Spring Web) para acelerar o desenvolvimento.

- **Banco de dados (PostgreSQL)** – Persiste os dados de usuários (credenciais, progresso por módulo, histórico de ciclos Pomodoro, pontuações e fase atual do personagem). As consultas e atualizações são realizadas pelo back-end por meio do Spring Data JPA (Hibernate).

A comunicação entre as partes ocorre via JSON sobre HTTPS. O front-end realiza chamadas assíncronas para os endpoints do back-end, que valida os dados, aplica a lógica de negócio e retorna respostas estruturadas.

## **Tecnologias utilizadas**

| Categoria | Tecnologia | Função no Projeto |
|-----------|------------|-------------------|
| Front-end | React | Construção da interface interativa, componentes reutilizáveis e gerenciamento de estado. |
| Back-end | Java com Spring Boot | Implementação da API REST, regras de negócio, autenticação e integração com o banco. |
| Banco de dados | PostgreSQL | Armazenamento persistente de usuários, progressão, questões e resultados. |
| API/Integração | REST + JSON | Comunicação padronizada entre front-end e back-end. |
| Versionamento | Git e GitHub | Controle de versões, colaboração entre os membros e hospedagem do repositório. |
| Gerenciamento de projeto | Trello | Organização de tarefas, acompanhamento do cronograma e gestão do backlog. |

## **Justificativa técnica**

- **React** – Permite criar interfaces dinâmicas e responsivas com alta performance, além de possuir vasto ecossistema de bibliotecas para gerenciamento de estado (ex.: Redux, Context API) e roteamento, adequado para uma aplicação web interativa.

- **Java com Spring Boot** – Spring Boot é o framework mais consolidado no ecossistema Java para construção de APIs REST e microsserviços. Oferece produtividade elevada (autoconfiguração, starters), segurança robusta via Spring Security (JWT, OAuth2), e integração nativa com PostgreSQL através do Spring Data JPA. A equipe possui familiaridade com Java, e a vasta documentação e comunidade garantem suporte para os desafios previstos.

- **PostgreSQL** – Sistema gerenciador de banco de dados relacional confiável, com suporte a transações ACID e recursos avançados como chaves estrangeiras, constraints e índices. A equipe já possui experiência prévia com essa tecnologia, o que reduz riscos e acelera o desenvolvimento.

- **Git e GitHub** – Controle de versão distribuído essencial para trabalho colaborativo, com recursos de pull requests, code review e rastreamento de issues. O GitHub atua como repositório remoto central.

- **Trello** – Ferramenta visual e de baixa complexidade para gerenciamento de tarefas, ideal para pequenas equipes. Permite criar quadros com listas (To Do, Doing, Done) e prazos, facilitando o acompanhamento diário do andamento do projeto.

## **Integração entre sistemas**

A integração ocorre da seguinte forma:

- O front-end em React acessa o back-end através de chamadas HTTP para os endpoints da API REST construída com Spring Boot. Exemplo: `GET /api/modulos`, `POST /api/questoes/responder`, `GET /api/usuario/progresso`.

- As APIs serão desenvolvidas seguindo os princípios RESTful, utilizando verbos HTTP (GET, POST, PUT, DELETE) e códigos de status apropriados. A autenticação será baseada em **JWT (JSON Web Token)**: o usuário faz login, o back-end retorna um token, e o front-end o envia no cabeçalho `Authorization` para requisições protegidas.

- O formato de troca de dados será **JSON**, leve e nativamente suportado tanto pelo JavaScript (front-end) quanto pelo Java (com bibliotecas como Jackson, já inclusa no Spring Boot).

- Os testes de integração serão realizados em duas etapas:

  1. Testes manuais com o auxílio de ferramentas como Postman ou Insomnia para validar cada endpoint antes da integração com o front-end.
  2. Testes automatizados com JUnit e MockMvc no back-end (Spring Boot Test) e, no front-end, com React Testing Library + Jest, simulando chamadas à API.

## **Organização do desenvolvimento**

A equipe utilizará as seguintes práticas e ferramentas:

- **Git e GitHub:**
  - Repositório único para o projeto, com branch principal `main` (ou `master`) protegida.
  - Uso de branches por funcionalidade (`feature/autenticacao`, `feature/pomodoro-timer`, etc.) e branches de correção (`hotfix/...`).
  - Commits semânticos e mensagens claras. Pull requests obrigatórios para mesclagem, com revisão pelo outro membro da equipe.

- **Divisão de tarefas:**
  - Diego fica responsável pelo back-end (Spring Boot, banco de dados, API, segurança JWT).
  - Kauê fica responsável pelo front-end (React, componentes, consumo da API e gamificação visual).
  - Ambos colaboram na definição dos contratos da API, testes e implantação.

- **Controle de versões:** Versionamento semântico e tags no GitHub para cada release.

- **Ferramenta de acompanhamento:** Trello com três quadros principais:
  - **Backlog** (funcionalidades pendentes, ordenadas por prioridade – MVP, importante, opcional).
  - **Em andamento** (tarefas sendo executadas).
  - **Concluído** (tarefas finalizadas e testadas).
  - São adicionados checklists, prazos e etiquetas (ex.: "front-end", "back-end", "banco de dados").

## **Desafios técnicos esperados**

A equipe prevê os seguintes desafios técnicos:

- **Integração contínua entre front-end e back-end** – Garantir que as requisições e respostas estejam sempre alinhadas com o contrato da API, especialmente durante alterações simultâneas nos dois lados.

- **Configuração da autenticação JWT com Spring Security** – Implementar o fluxo seguro de login, renovação de token e proteção de rotas no front-end e back-end exige conhecimento do filtro de requisições, gerenciamento de UserDetailsService e exposição correta dos endpoints públicos/privados.

- **Implementação correta da gamificação** – A evolução visual do personagem vinculada ao progresso (nota mínima de 70% para avançar, penalidades por interrupção) exige lógica de estado consistente e persistente no banco de dados, além de transações bem definidas para evitar inconsistências.

- **Gerenciamento de tempo real** – Embora o Pomodoro não exija comunicação em tempo real com o servidor (o temporizador roda no front-end), é necessário sincronizar o estado do ciclo com o back-end para evitar perda de progresso ao recarregar a página. Isso exigirá uma estratégia de salvamento periódico ou ao final de cada ciclo.

- **Desempenho e responsividade** – Garantir que a interface funcione bem em diferentes dispositivos (desktop, tablet, mobile) e com conexões de internet variadas, otimizando o carregamento dos questionários e das imagens do personagem.

- **Estruturação da arquitetura do back-end** – Organizar adequadamente as camadas (controller, service, repository), utilizar DTOs para não expor entidades diretamente, e aplicar injeção de dependência de forma correta para manter o código testável e de fácil manutenção.

## **Referências**

- React – Biblioteca JavaScript para interfaces de usuário. Disponível em: [https://react.dev](https://react.dev)
- Spring Boot – Framework para desenvolvimento de aplicações Java empresariais. Disponível em: [https://spring.io/projects/spring-boot](https://spring.io/projects/spring-boot)
- Spring Security – Módulo para autenticação e autorização. Disponível em: [https://spring.io/projects/spring-security](https://spring.io/projects/spring-security)
- PostgreSQL – Sistema de banco de dados relacional open source. Disponível em: [https://www.postgresql.org](https://www.postgresql.org)
- GitHub – Plataforma de hospedagem de código e versionamento Git. Disponível em: [https://github.com](https://github.com)
- Trello – Ferramenta de gerenciamento de projetos baseada em quadros. Disponível em: [https://trello.com](https://trello.com)
- JSON Web Tokens (JWT) – Padrão para autenticação stateless. Disponível em: [https://jwt.io](https://jwt.io)
- Hibernate / Spring Data JPA – Camada de persistência para Java. Disponível em: [https://spring.io/projects/spring-data-jpa](https://spring.io/projects/spring-data-jpa)
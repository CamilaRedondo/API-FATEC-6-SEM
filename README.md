<div align="center">
  <h1>API 6º SEMESTRE</h1>
</div>

<div align="center">
  <h2>Projeto de IA Generativa</h2>
</div>

##### <p align="center">Projeto Integrador</p>
<div align="center"> <img src="/readme/Logo.png" alt="Equipe bytech"/></div>

##### <p align="center">  Empresa parceira - Dom Rock </p>

<div align="center">
  
 [Proposta do projeto](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#proposta) • [Backlog](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#backlog) • [Tecnologias](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#tecnologias) • [Entregas](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#entregas) • [Documentação](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#documentacao) • [Equipe](https://https://github.com/CamilaRedondo/API-FATEC-6-SEM#equipe)
 
</div>

<div name="proposta"></div>

# :dart: Proposta do projeto

<p align="left"> A proposta visa o desenvolvimento de um chatbot inteligente baseado em IA generativa que será capaz de analisar uma vasta base de depoimentos de clientes da B2W. Esse sistema usará a técnica RAG (Retrieval Augmented Generation) para buscar respostas diretamente da base de dados vetorizada, proporcionando insights rápidos e precisos. O chatbot auxiliará equipes de marketing na personalização de campanhas e estratégias publicitárias, identificando tendências e áreas de melhoria a partir de comentários reais dos clientes. Dessa forma, ele ajudará a ajustar estratégias rapidamente e sugerir novos segmentos, otimizando a eficácia das campanhas de marketing.</p>

## 📖 Requisitos funcionais
+ RF1 - Análise de produtos: Identificação do chatbot sobre padrões e características dos produtos apontadas pelas opiniões analisadas.
  + Usabilidade:
    + Pergunta: Me fala caracteristicas do Iphone 8
    + Resposta: * Tela de 5,5 polegadas * Processador iOS 11 * Opções de estoque: 64GB * Suporte a 4G e Wi-Fi * Camera traseira de 12MP * Cor disponível: dourado (no caso do iPhone 8 Plus) e cinza espacial.
+ RF2 - Recomendação de produtos entre clientes (percepção dos clientes): Sugestões de produtos baseadas nas recomendações dos clientes.
  + Usabilidade:
    + Pergunta: Me indique smartphones
    + Resposta:  1. Smartphone Samsung Galaxy J5 Prime, 2. Smartphone Samsung Galaxy J5 Prime, 3. Smartphone LG G6
+ RF3 - Análise de satisfação do cliente por produto: Avaliação do nível de contentamento por produto.
  + Usabilidade:
    + Pergunta: Me fale a satisfação de todas as reviews do produto Smartphone Samsung Galaxy J5
    + Resposta: A satisfação dos clientes com o produto Smartphone Samsung Galaxy J5 é baixa. Das 4 reviews fornecidas, 3 delas são negativas e 1 é positiva. A review com nota 1 menciona problemas com a tela do produto, que começou a piscar alguns minutos após o uso.
+ RF4 - Ideia para campanhas: Criação de ideias para marketing com base em feedbacks
  + Usabilidade:
    + Pergunta: Como podemos usar os feedbacks dos clientes para criar uma nova campanha de marketing?"
    + Resposta: Excelente pergunta! A partir dos feedbacks dos clientes, podemos identificar alguns pontos que podem ser utilizados para criar uma nova campanha de marketing: 1. Transparência: O cliente menciona que valoriza a transparência da empresa. Podemos criar uma campanha que destaque a transparência da nossa empresa, mostrando como trabalhamos para ser ...
+ RF5 - Comparação de experiência de compra: Análise comparativa de compras entre diferentes perfis consumidores.
  + Usabilidade:
    + Pergunta: Me de comparação de experiencia de compra sobre o seguinte produto: Smartphone Motorola Moto G5 Plus
    + Resposta: Existem quatro reviews para o produto Motorola Moto G5 Plus: A primeira review com um rating de 5 estrelas menciona que o smartphone é rápido, preciso, com boa bateria e design agradável. O reviewer também destaca que o produto tem um espaço de armazenamento adequado e funções intuitivas. A segunda review com um rating de 1 estrela menciona que o smartphone parou de funcionar após apenas 3 meses de uso, após uma atualização de software. O reviewer também criticou a Motorola por não ter resolvido o problema e negar as motivações da paralisação. A terceira review com um rating de 2 estrelas menciona que o reviewer comprou o produto e a entrega foi rápida, mas a transportadora não movimentou o produto após 15 dias e emitiu uma nota fiscal. A quarta review com um rating de 5 estrelas menciona que o smartphone atendeu às expectativas do reviewer, com câmeras excelentes e uma bateria que carrega rapidamente.

## 🔖 Requisitos não funcionais
+ RNF1 - BD Vetorial ChromaDB
+ RNF2 - Modelos LLM de uso público do Huggingface
+ RNF3 - Framework Langchain
+ RNF4 - Vídeo-tutorial: Criação de um vídeo-tutorial para auxiliar usuários sem experiencia prévia.

</br>
</br>

<div name="backlog"></div> 

 # :bulb: Backlog


| Rank | Prioridade | User Story | Estimativa | Sprint | Requisito do Parceiro | Cenários |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | Alta | Desenvolvimento do RAG/ChromaDB<br>Como um usuário final, gostaria de fazer perguntas e receber respostas sobre as análises de produtos em linguagem natural.| 20 | 1 | RF1-RF2, RNF1-RNF2-RNF3 | Cenário 1: O usuário final faz uma pergunta sobre a qualidade de um produto específico.O chatbot utiliza a base de dados vetorial para encontrar depoimentos relevantes e responde de forma clara e objetiva, utilizando linguagem natural.<br> Cenário 2: O usuário final pergunta sobre a comparação entre dois produtos. O chatbot consulta os comentários da base, organiza os dados e fornece uma resposta resumida e compreensível.  |
| 2 | Alta | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente.| 12 | 1 | RF1-RF2,  RNF1-RNF2-RNF3 | Cenário 1: O analista de marketing pergunta sobre o nível de satisfação dos clientes para um produto específico. O chatbot acessa a base de dados da B2W e retorna uma análise com base nos depoimentos.<br> Cenário 2: O analista de marketing pergunta sobre o nível de satisfação dos clientes para um produto específico. O chatbot acessa a base de dados e não encontra o produto em especifico no contexto fornecido, o próprio informa isso.|
| 3 | Alta | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre padrões de compra.| 12 | 1 | RF1-RF2,  RNF1-RNF2-RNF3 | Cenário 1: O analista de marketing pergunta sobre o padrão de compra de clientes para um produto específico. O chatbot acessa a base de dados da B2W e retorna uma análise com base nos depoimentos.<br> Cenário 2: O analista de marketing pergunta sobre o sobre o padrão de compra de clientes para um produto específico. O chatbot acessa a base de dados e não encontra o produto em especifico no contexto fornecido, o próprio informa isso. |
| 4 | Media | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre menções a produtos específicos.| 12 | 1 | RF1-RF2,  RNF1-RNF2-RNF3  | Cenário 1: O analista de marketing pergunta sobre menções a produtos específicos. O chatbot acessa a base de dados da B2W e retorna uma análise com base nos depoimentos.<br> Cenário 2: O analista de marketing pergunta sobre menções a produtos específicos. O chatbot acessa a base de dados e não encontra o produto em especifico no contexto fornecido, o próprio informa isso. |
| 5 | Média | Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente, para que eu possa focar nas métricas mais relevantes para campanhas de marketing | 12 | 2 | RF3-RF4,  RNF1-RNF2-RNF3  | Cenário 1: O analista de marketing pergunta sobre a satisfação dos clientes em relação a um produto recém-lançado. O chatbot acessa a base de dados e retorna um resumo da análise de sentimento.<br>Cenário 2: O analista de marketing pergunta sobre a satisfação dos clientes em relação a um produto recém-lançado. O chatbot não encontra o produto na base de dados e retorna um resumo do acontecimento.|
| 6 | Média | Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de  recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing | 15 | 2 | RF3-RF4,  RNF1-RNF2-RNF3  | Cenário 1: O analista de marketing pergunta sobre a recorrencia de compras em relação a um produto recém-lançado. O chatbot acessa a base de dados e retorna um resumo da análise de sentimento.<br>Cenário 2: O analista de marketing pergunta sobre a recorrencia de compras a um produto recém-lançado. O chatbot não encontra o produto na base de dados e retorna um resumo do acontecimento. |
| 7 | Baixa | Análise de Sentimento em Reviews de Produtos<br>Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. | 15 | 2 |RF3-RF4,  RNF1-RNF2-RNF3  | O analista de marketing pede uma análise de sentimento para as reviews de um produto. O chatbot retorna que a maioria das avaliações é positiva, indicando alto índice de satisfação.<br>Cenário 2: O analista de marketing pergunta sobre o sentimento das reviews dos clientes. O chatbot não encontra o produto na base de dados e retorna um resumo do acontecimento. |
| 8 | Baixa | Comparação de Experiência de Compra por Perfil de Cliente<br>Como um analista de marketing, eu quero interagir com o chatbot e fazer perguntas sobre a experiência de compra de clientes específicos (idade, gênero, região), para que eu possa obter insights personalizados para campanhas direcionadas. | 15 | 2 | RF3-RF4,  RNF1-RNF2-RNF3 | Cenário 1: O analista de marketing pergunta sobre a experiência de Compra por Perfil de Cliente. O chatbot acessa a base de dados e retorna um resumo da análise.<br>Cenário 2: O analista de marketing pergunta sobre a experiência de Compra por Perfil de Cliente. O chatbot não encontra o produto na base de dados e retorna um resumo do acontecimento. |
| 9 | Baixa | Tutorial para Novos Usuários<br>Como um usuário final não técnico, eu quero interagir com um tutorial, para que eu possa aprender a utilizar o chatbot e todas as suas funcionalidades de forma rápida e eficiente.| 4 | 3 | RNF4 | Cenário 1: O Analista de marketing assiste o vídeo e aprende a utilizar a aplicação <br> Cenário 2: O Analista de marketing assiste o vídeo e descobre funcionaliades que ele não sabia anteriormente. |

</br>
</br>

<div name="entregas"></div> 

# 📌 Sprints

<h3><strong>Sprint 1:</strong></h3>
  <details>

## :dart: MVP
  <h4>Nessa sprint, focamos em entregar a integração do chatbot com a base de dados da B2W, garantindo a consulta de informações sobre satisfação do cliente.</h4>

## :dart: DoR
+ 1 - Objetivo e solução definidos claramente: O escopo e os objetivos do projeto devem ser claros, incluindo a definição das funcionalidades principais do chatbot;
+ 2 - Dados/colunas definidos: As colunas e atributos relevantes nos dados (e.g., ID de produto, review, sentimento, categoria, perfil do cliente) devem estar mapeados e prontos para serem utilizados na criação dos embeddings e no treinamento de modelos;
+ 3 - Ambiente configurado: Todos os ambientes devem estar configurados com as dependências necessárias;
+ 4 - Critérios de Aceitação Especificados: Cada funcionalidade deve ter critérios de aceitação claros;


## 🔎 Sprint Backlog
  | Rank | Tarefa | Status | Tag | Estimativa de Horas |
  |:-:|:-:|:-:|:-:|:-:|
  | 1 | Configuração dos repositórios Git. | Concluído | Ambiente de desenvolvimento | 5 |
  | 2 | Design inicial do frontend no Figma. | Concluído | Front-end | 8 |
  | 3 | Seleção inicial de modelos de IA. | Concluído | IA | 8 |
  | 4 | Integração básica com LangChain. | Concluído | IA | 8 |
  | 5 | Implementar retrievers simples para consultas básicas. | Concluído | IA | 15 |
  | 6 | Testes iniciais de integração entre modelos de IA e base de dados vetorial. | Concluído | IA/Banco de dados | 15 |
  | 7 | Criar pipeline de leitura de dados CSV (reviews da B2W). | Concluído | IA | 15 |
  | 8 | Conversão dos dados CSV para o formato necessário (IA e banco de dados vetorial). | Concluído | IA/Banco de dados | 10 |
  | 9 | Utilização de embeddings a partir dos dados da B2W. | Concluído | IA | 12 |
  | 10 | Armazenamento de embeddings no banco de vetores (ChromaDB). | Concluído | Banco de Dados | 10 |
  | 10 | Implementar pipeline fim a fim para processar os dados e gerar output final. | Concluído | IA/Banco de dados | 25 |
</br>
</br>

## 📌 Critérios de Aceitação 

| Rank | User Story | Critério de Aceitação |
|:-:|:-:|:-:|
|1|Desenvolvimento do RAG/ChromaDB Como um usuário final, gostaria de fazer perguntas e receber respostas sobre as análises de produtos em linguagem natural.| - O chatbot deve responder perguntas em linguagem natural com base nos dados armazenados na ChromaDB. </br> - O chatbot deve utilizar o modelo RAG para garantir que as respostas sejam o mais precisas e contextualizadas.|
|2|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente. | - O chatbot deve ser integrado à base de dados da B2W. </br> - O chatbot deve consultar e retornar informações sobre satisfação do cliente. | 
|3|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre padrões de compra. | - O chatbot deve ser capaz de acessar dados sobre padrões de compra e fornecer respostas relevantes com base nos dados de compra de clientes. |



</br>
</br>

## ✅ Entrega

<h4 align="center">Recomendação de produtos entre clientes.</h4>

<p align="center">
    <img src="/readme/usabilidade_sprint_1.gif"/>
    <br>
    <a href="https://youtu.be/JtSUlmFG2dQ">Link para uma melhor resolução</a>
</p>

   <br>
  </details>
<h3><strong>Sprint 2:</strong></h3>
<details>

## :dart: MVP
<h4>Nessa sprint, focamos em entregar melhorias com relação a comunicação ao chat, além de criar uma interface.</h4>

## :dart: DoR
+ 1 - User Stories Detalhadas: As US definidas devem estar refinadas, com critérios de aceitação específicos para guiar o desenvolvimento e os testes.
+ 2 - Dados Estruturados e Filtrados por Segmento: Os dados de clientes devem estar prontos permitir a comparação de experiências de compra.
+ 3 - Ambiente de Testes Configurado: O ambiente de desenvolvimento e teste deve estar configurado com todos os datasets e modelos integrados.
+ 4 - Integração da Interface com as Novas Funcionalidades: O mockup da interface Vue.JS deve estar preparada para receber e alinhada com as necessidades do cliente, além de estar pronta para ser desenvolvida.

## 🔎 Sprint Backlog
  | Rank | Tarefa | Status | Tag | Estimativa de Horas |
  |:-:|:-:|:-:|:-:|:-:|
  | 1 | Retirar vector store de tempo de execução e resolver problema de memória | Concluído | IA | 20 |
  | 2 | Aprimorar o PLN, a técnica de 'chunking' e 'embedding' | Concluído | IA | 20 |
  | 3 | Integrar o frontend com a IA | Concluído | Frontend-IA | 20 |
  | 4 | Realizar o retriver invoke e bloquear perguntas que não tenha haver com o dataset.| Concluído | IA | 12 |
  | 5 | Criar os endpoints para conectar a IA com o frontend envolve definir a comunicação entre o chatbot de IA generativa e a interface do usuário.| Concluído | Frontend-IA | 15 |
  | 6 | Criação do layout do frontend | Concluído | Front-end | 18 |
</br>
</br>

## 📌 Critérios de Aceitação 

| Rank | User Story | Critério de Aceitação |
|:-:|:-:|:-:|
|4|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre menções a produtos específicos. | - O chatbot deve permitir a consulta de menções a produtos específicos e apresentar informações organizadas. |
|5|Análise de Satisfação do Cliente e Recorrência de Compra Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente e recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing. | - O chatbot deve fornecer a taxa de recorrência de compra e a média de satisfação do cliente. </br> - O chatbot deve segmentar os clientes com base na frequência de compra e nível de satisfação. |
|6|Análise de Sentimento em Reviews de Produtos Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. | - O chatbot deve classificar reviews de produtos em sentimentos (positivo, neutro, negativo) e fornecer um resumo baseado nas análises predominantes. |

</br>
</br>

## ✅ Entrega

<h4 align="center">Análise de produtos: Identificação do chatbot sobre padrões e características</h4>

<p align="center">
    <img src="/readme/usabilidade_sprint_2_rf1.gif"/>
    <br>
    <a href="https://youtu.be/ACrOamonwGQ">Link para uma melhor resolução</a>
</p>
</br>

<h4 align="center">Análise de satisfação do cliente por produto: Avaliação do nível de contentamento por produto.</h4>

<p align="center">
    <img src="/readme/usabilidade_sprint_2_rf3.gif"/>
    <br>
    <a href="https://youtu.be/vi4vMpG3HIo">Link para uma melhor resolução</a>
</p>
</br>
</details>

<h3><strong>Sprint 3:</strong></h3>
<details>

## :dart: MVP
<h4>Para a 3ª sprint, nosso foco foi implementar testes múltiplos modelos de IA e realizar a engenharia de prompts, garantindo respostas precisas e eficientes para o chatbot. Também avançamos na comparação entre os modelos, identificando o mais adequado, e realizamos a refatoração e otimização do código para melhor desempenho.</h4>

## :dart: DoR
+ 1 - User Stories Detalhadas: As User Stories para a sprint devem estar bem definidas e detalhadas, com critérios de aceitação específicos.
+ 2 - Definição dos Modelos de IA: Os modelos de IA selecionados devem estar definidos.
+ 3 - Integração dos Prompts com o ChromaDB: Os prompts devem estar preparados e ajustados para interação otimizada com o banco ChromaDB, alinhados para extrair informações precisas e fornecer respostas adequadas ao usuário.
+ 4 - Ambiente de Testes Configurado e Validado: Todo o ambiente de desenvolvimento deve estar configurado com acesso aos datasets, modelos e ferramentas de monitoramento.
+ 5 - Base para o Vídeo Tutorial Organizada: A estrutura do vídeo tutorial devem estar definidos, cobrindo as principais funcionalidades do chatbot.


## 🔎 Sprint Backlog
  | Rank | Tarefa | Status | Tag | Estimativa de Horas |
  |:-:|:-:|:-:|:-:|:-:|
  | 1 | Implementar diferentes modelos de IA. | Concluido | IA | 20 |
  | 2 | Engenharia de Prompts. | Concluido | IA | 20 |
  | 3 | Comparar resultados dos modelos. | Concluido | IA | 20 |
  | 4 | Refatoração e otimização. | Em progresso | Concluido | 12 |
  | 5 | Testes finais e entrega do produto.| Concluido | Testes | 15 |
  | 5 | Criação do video tutorial.| Concluido | Usabilidade | 15 |
  

</br>
</br>

## 📌 Critérios de Aceitação 

| Rank | User Story | Critério de Aceitação |
|:-:|:-:|:-:|
|7|Análise de Satisfação do Cliente e Recorrência de Compra Como um analista de marketing, eu quero interagir com o chatbot para obter dados de recorrência de compra, para que eu possa identificar padrões e otimizar campanhas de marketing. | - O chatbot deve apresentar dados sobre a frequência de compra dos clientes. </br> - O chatbot deve fornecer informações sobre os clientes que realizam compras repetidas. |
|8| Comparação de Experiência de Compra por Perfil de Cliente<br>Como um analista de marketing, eu quero interagir com o chatbot e fazer perguntas sobre a experiência de compra de clientes específicos (idade, gênero, região), para que eu possa obter insights personalizados para campanhas direcionadas. | - O chatbot deve gerar respostas diferenciadas com base nos filtros, destacando insights relevantes para cada perfil de cliente (ex: preferências de compra por faixa etária e região).|
|9| Tutorial para Novos Usuários<br>Como um usuário final não técnico, eu quero interagir com um tutorial, para que eu possa aprender a utilizar o chatbot e todas as suas funcionalidades de forma rápida e eficiente.| - O tutorial deve cobrir as funcionalidades principais do chatbot, como iniciar uma conversa, consultar informações, e executar comandos básicos. <br> - O tutorial deve ter boa qualidade de áudio e vídeo, garantindo que os usuários possam compreender claramente as instruções e o conteúdo apresentado. |

</br>
</br>

## ✅ Entrega

<h4 align="center">Ideia para campanhas: Criação de ideias para marketing com base em feedbacks</h4>
<p align="center">
    <img src="/readme/usabilidade_sprint_3_rf4.gif"/>
    <br>
    <a href="https://youtu.be/pfvrSn_8XUs">Link para uma melhor resolução</a>
</p>
</br>

<h4 align="center">Comparação de experiência de compra: Análise comparativa de compras entre diferentes perfis consumidores</h4>
<p align="center">
    <img src="/readme/usabilidade_sprint_3_rf5.gif"/>
    <br>
    <a href="https://youtu.be/JM9tgYW5css">Link para uma melhor resolução</a>
</p>
</br>

</details>
</br>
</br>

<div name="tecnologias"></div> 

# 🛠️ Tecnologias

As seguintes ferramentas, linguagens e tecnologias foram utilizadas na execução do projeto:
+ Vue.js;
+ Python;
+ Langchain;
+ ChromaDB.
</br>
</br>

<div name="equipe"></div> 

# 🎓 Equipe

<table align="center">
  <tr>
    <th><b>Nome</b></th>
    <th><b>Função</b></th>
    <th><b>Github</b></th>
    <th><b>Linked-In</b></th>
  </tr>
    <tr>
      <td>Gustavo Marques</td>
      <td>Product Owner</td>
      <td><a href="https://github.com/gusta7597">Github</a></td>
      <td><a href="https://www.linkedin.com/in/gustavo-marques-lima-695b331a2/">Linked-In</a></td>
    </tr>
    <tr>
      <td>Camila Redondo</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/CamilaRedondo">Github</a></td>
      <td><a href="https://www.linkedin.com/in/camila-silveira-redondo-7941631ab/">Linked-In</a></td>
    </tr>
    <tr>
      <td>João Henrique</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/JoaoHenrique7">Github</a></td>
      <td><a href="https://www.linkedin.com/in/jo%C3%A3o-henrique-trist%C3%A3o-b63385207/">Linked-In</a></td>
    </tr>
    <tr>
      <td>Thalles Torres</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/thallestorres">Github</a></td>
      <td><a href="https://www.linkedin.com/in/thalles-torres-83449a285">Linked-In</a></td>
    </tr>
    <tr>
      <td>Douglas José Ferreira de Queiroz</td>
      <td>Dsenvolvedor</td>
      <td><a href="https://github.com/douglaswe">Github</a></td>
      <td><a href="">Linked-In</a></td>
    </tr>
    <tr>
      <td>Henrique Neto</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/henriqFerreira">Github</a></td>
      <td><a href="https://www.linkedin.com/in/henriquepfneto/">Linked-In</a></td>
    </tr>
    <tr>
      <td>Yago Pereira</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/YagoPSilva">Github</a></td>
      <td><a href="https://www.linkedin.com/in/yago-pereira21/">Linked-In</a></td>
    </tr>
</table>

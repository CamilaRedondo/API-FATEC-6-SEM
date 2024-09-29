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
+ RF1 - Respostas em Linguagem Natural sobre Análises de Produtos: O chatbot deve permitir que a equipe de marketing faça perguntas sobre análises de produtos e receba respostas em linguagem natural;
+ RF2 - Acesso a Informações sobre Satisfação do Cliente: O chatbot deve permitir que a equipe consulte dados de satisfação do cliente extraídos dos reviews da B2W para avaliar o desempenho de produtos;
+ RF3 - Acesso a Padrões de Compra: O chatbot deve fornecer informações sobre padrões de compra dos clientes, permitindo que a equipe identifique comportamentos de compra relevantes para campanhas;
+ RF4 - Acesso a Menções de Produtos Específicos: O chatbot deve buscar menções específicas a produtos nas reviews dos clientes, para que a equipe possa analisar a percepção pública sobre produtos-chave;
+ RF5 - Análise de Satisfação e Recorrência de Compra: O chatbot deve realizar análises de satisfação do cliente e recorrência de compra, fornecendo insights sobre métricas cruciais para decisões de marketing;
+ RF6 - Análise de Sentimento de Reviews: O chatbot deve ser capaz de analisar o sentimento (positivo, neutro, negativo) das reviews de produtos, ajudando a ajustar campanhas de acordo com o feedback emocional dos clientes;
+ RF7 - Comparação de Experiência de Compra por Perfil de Cliente: O chatbot deve permitir a comparação de experiências de compra com base em perfis de clientes (idade, gênero, região), para personalizar campanhas;
+ RF8 - Recomendações Automáticas de Produtos: O chatbot deve fornecer recomendações automáticas de produtos com base na satisfação e recorrência de compra, para otimizar campanhas publicitárias;
+ RF9 - Classificação e Priorização de Produtos: O chatbot deve classificar e priorizar produtos com base em reviews e métricas de satisfação, permitindo à equipe de marketing focar nos produtos com maior potencial de sucesso.

## 🔖 Requisitos não funcionais
+ RNF1 - Interface Intuitiva e de Fácil Uso: O chatbot deve possuir uma interface simples e intuitiva, de modo que mesmo usuários sem conhecimento técnico possam utilizá-lo de maneira eficiente e sem dificuldades;
+ RNF2 - Desempenho e Tempo de Resposta: O sistema deve ser capaz de processar e responder às perguntas dos usuários de maneira fluida;
+ RNF3 - Qualidade das respostas: O sistema deve ser capaz de oferecer respostas que correspondam corretamente as suas respectivas perguntas;
+ RNF4 - Vídeo Tutorial para Novos Usuários: Deve ser criado um vídeo tutorial que demonstre o uso do chatbot, visando auxiliar usuários sem experiência tecnológica no uso das funcionalidades. 
</br>
</br>

<div name="backlog"></div> 

 # :bulb: Backlog


| Rank | Prioridade | User Story | Estimativa | Sprint | Requisito do Parceiro |
|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | Alta | Desenvolvimento do RAG/ChromaDB<br>Como um usuário final, gostaira de fazer perguntas e receber respostas sobre as análises de produtos em linguagem natural.|| 1 | RF1, RNF2-RNF3 |
| 2 | Alta | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente.|| 1 | RF2, RNF2-RNF3 |
| 3 | Alta | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre padrões de compra.|| 1 | RF3, RNF2-RNF3 |
| 4 | Alta | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre menções a produtos específicos.|| 1 | RF4, RNF2-RNF3 |
| 5 | Alta | Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente, para que eu possa focar nas métricas mais relevantes para campanhas de marketing || 1 | RF5, RNF2-RNF3 |
| 6 | Alta | Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de  recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing || 1 | RF5, RNF2-RNF3 |
| 7 | Alta | Análise de Sentimento em Reviews de Produtos<br>Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. || 1 | RF6, RNF2-RNF3 |
| 8 | Média | Comparação de Experiência de Compra por Perfil de Cliente<br>Como um analista de marketing, eu quero interagir com o chatbot e fazer perguntas sobre a experiência de compra de clientes específicos (idade, gênero, região), para que eu possa obter insights personalizados para campanhas direcionadas. || 2 | RF7, RNF2-RNF3 |
| 9 | Média | Recomendações Baseadas em Satisfação e Recorrência<br>Como um analista de marketing, eu quero interagir com o chatbot para receber recomendações automáticas de produtos com alto índice de satisfação e recorrência de compra, para que eu possa otimizar minhas campanhas publicitárias. || 2 | RF8, RNF2-RNF3 |
| 10 | Média | Classificação e Priorização de Produtos para Marketing<br>Como um analista de marketing, eu quero interagir com o chatbot para visualizar uma classificação clara dos produtos (muito bom, bom, neutro, ruim) com base em reviews e métricas de satisfação, para que eu possa priorizar os produtos para campanhas publicitárias. || 2 | RF9, RNF2-RNF3 |
| 11 | Baixa | Usabilidade<br>Como um usuário final, eu quero interagir com uma interface intuitiva, para que eu possa acessar facilmente todas as funcionalidades do chatbot || 2 | RNF1 |
| 12 | Baixa |  Tutorial para Novos Usuários<br>Como um usuário final não técnico, eu quero interagir com um tutorial, para que eu possa aprender a utilizar o chatbot e todas as suas funcionalidades de forma rápida e eficiente.|| 3 | RNF4 |

</br>
</br>

<div name="entregas"></div> 

# 📌 Sprints

<h3><strong>Sprint 1:</strong></h3>
  <details>

## :dart: MVP
<div name="backlog">
  <h4>Nessa sprint, focamos em entregar a integração do chatbot com a base de dados da B2W, garantindo a consulta de informações sobre satisfação do cliente.</h4>
</div> 

## 🔎 Sprint Backlog
  | Rank | Tarefa | Status | User Story relacionada |
  |:-:|:-:|:-:|:-:|
  | 1    | Configuração dos repositórios Git. |     Concluído     | Todas as US da Sprint 1 |
  | 2    | Design inicial do frontend no Figma. |     Concluído     | US11 |
  | 3    | Seleção inicial de modelos de IA. |     Concluído      | US1 |
  | 4    | Integração básica com LangChain. |     Concluído      | US1 |
  | 5    | Implementar retrievers simples para consultas básicas. |     Concluído      | US1 |
  | 6    | Testes iniciais de integração entre modelos de IA e base de dados vetorial. |     Concluído      | US1 |
  | 7    | Criar pipeline de leitura de dados CSV (reviews da B2W). |     Concluído      | US2, US3, US4 |
  | 8    | Conversão dos dados CSV para o formato necessário (IA e banco de dados vetorial). |     Concluído      | US1 |
  | 9    | Utilização de embeddings a partir dos dados da B2W. |     Concluído      | US2, US3, US4, US5, US6, US7 |
  | 10    | Armazenamento de embeddings no banco de vetores (ChromaDB). |     Concluído      | US1 |
  | 10    | Implementar pipeline fim a fim para processar os dados e gerar output final. |     Concluído      | Todas as US da Sprint 1 |
</br>
</br>

## 📌 Critérios de Aceitação 

| Rank | User Story | Critério de Aceitação |
|:-:|:-:|:-:|
|1|Desenvolvimento do RAG/ChromaDB Como um usuário final, gostaria de fazer perguntas e receber respostas sobre as análises de produtos em linguagem natural.| - O chatbot deve responder perguntas em linguagem natural com base nos dados armazenados na ChromaDB. </br> - O chatbot deve utilizar o modelo RAG para garantir que as respostas sejam o mais precisas e contextualizadas.|
|2|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente. | - O chatbot deve ser integrado à base de dados da B2W. </br> - O chatbot deve consultar e retornar informações sobre satisfação do cliente. | 
|3|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre padrões de compra. | - O chatbot deve ser capaz de acessar dados sobre padrões de compra e fornecer respostas relevantes com base nos dados de compra de clientes. |
|4|Integração com a Base de Dados da B2W Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre menções a produtos específicos. | - O chatbot deve permitir a consulta de menções a produtos específicos e apresentar informações organizadas. |
|5|Análise de Satisfação do Cliente e Recorrência de Compra Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente e recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing. | - O chatbot deve fornecer a taxa de recorrência de compra e a média de satisfação do cliente. </br> - O chatbot deve segmentar os clientes com base na frequência de compra e nível de satisfação. |
|6|Análise de Sentimento em Reviews de Produtos Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. | - O chatbot deve classificar reviews de produtos em sentimentos (positivo, neutro, negativo) e fornecer um resumo baseado nas análises predominantes. |
|7|Análise de Satisfação do Cliente e Recorrência de Compra Como um analista de marketing, eu quero interagir com o chatbot para obter dados de recorrência de compra, para que eu possa identificar padrões e otimizar campanhas de marketing. | - O chatbot deve apresentar dados sobre a frequência de compra dos clientes. </br> - O chatbot deve fornecer informações sobre os clientes que realizam compras repetidas. |

</br>
</br>

## ✅ Entrega

  </details>
<h3><strong>Sprint 2:</strong></h3>
<h3><strong>Sprint 3:</strong></h3>
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
      <td><a href="">Github</a></td>
      <td><a href="www.linkedin.com/in/thalles-torres-83449a285">Linked-In</a></td>
    </tr>
    <tr>
      <td>Douglas José Ferreira de Queiroz</td>
      <td>Dsenvolvedor</td>
      <td><a href="">Github</a></td>
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

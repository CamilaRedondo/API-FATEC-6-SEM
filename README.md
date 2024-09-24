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
+ RF1 - Pipeline de Processamento de Dados para Banco de Vetor: Desenvolver o pipeline necessário para preparar, processar e armazenar os dados dos depoimentos de clientes de forma vetorizada;
+ RF2 - Agente para Engenharia de Prompt em LLM: Criar um agente que otimiza a formulação de prompts para garantir que o modelo de linguagem (LLM) gere respostas relevantes, personalizadas e de alta qualidade;
+ RF3 - Interface de Chatbot Integrado com LLM: Desenvolver uma interface amigável que conecta o agente LLM ao usuário final, permitindo que as equipes de marketing interajam diretamente com o chatbot;
+ RF4 - Funcionalidades de Análise de Sentimento e Segmentação: Melhorar a capacidade do chatbot para fornecer insights ainda mais úteis para a equipe de marketing, como análise automática de sentimentos e segmentação de usuários com base em padrões de feedback.

## 🔖 Requisitos não funcionais
+ RNF1 - Escalabilidade e Desempenho: Garantir que o sistema seja capaz de processar grandes volumes de dados e responda rapidamente às solicitações do chatbot, mantendo a experiência do usuário fluida e eficiente;
+ RNF2 - Disponibilidade de documentação para usabilidade: Garantir a disponibilidade de um 'Manual do Usuário' e um vídeo demostrando o uso do sistema.
</br>
</br>

<div name="backlog"></div> 

 # :bulb: Backlog


| Rank | Prioridade | User Story                                                                                                                                                      | Estimativa | Sprint | Requisito do Parceiro |
|:----:|:----------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------:|:------:|:---------------------:|
| 1    | Alta       | Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente, padrões de compra e menções a produtos específicos.|          | 1      | RF1                |
| 2    | Alta       | Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente e recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing |          |    1    |      RF2              |
| 3    | Alta       | Análise de Sentimento em Reviews de Produtos<br>Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. |          | 1      |      RF2                   |
| 4    | Média      | Comparação de Experiência de Compra por Perfil de Cliente<br>Como um analista de marketing, eu quero interagir com o chatbot e fazer perguntas sobre a experiência de compra de clientes específicos (idade, gênero, região), para que eu possa obter insights personalizados para campanhas direcionadas. |            | 2      | RF1 - RF2                   |
| 5    | Média      | Recomendações Baseadas em Satisfação e Recorrência<br>Como um analista de marketing, eu quero interagir com o chatbot para receber recomendações automáticas de produtos com alto índice de satisfação e recorrência de compra, para que eu possa otimizar minhas campanhas publicitárias. |            | 2      | RF1 - RF2                   |
| 6    | Média      | Classificação e Priorização de Produtos para Marketing<br>Como um analista de marketing, eu quero interagir com o chatbot para visualizar uma classificação clara dos produtos (muito bom, bom, neutro, ruim) com base em reviews e métricas de satisfação, para que eu possa priorizar os produtos para campanhas publicitárias. |            | 2      | RF1 - RF2                   |
| 7    | Baixa      | Usabilidade<br>Como um usuário final, eu quero interagir com uma interface intuitiva, para que eu possa acessar facilmente todas as funcionalidades do chatbot                                                                                                                            |            |   2     |          RF3            |
| 8    | Baixa      |  Tutorial para Novos Usuários<br>Como um usuário final não técnico, eu quero interagir com um tutorial, para que eu possa aprender a utilizar o chatbot e todas as suas funcionalidades de forma rápida e eficiente.                                                                                                                            |            |   3     |          RNF1            |

</br>
</br>

<div name="entregas"></div> 

# 📌 Sprints

<h3><strong>Sprint 1:</strong></h3>
  <details>

## 🔎 Sprint Backlog
  | Rank | Tarefa | Status |
  |:-:|:-:|:-:|
  | 1    | Configuração dos repositórios Git. |     Concluído     |
  | 2    | Design inicial do frontend no Figma. |     Concluído     |    
  | 3    | Seleção inicial de modelos de IA. |     Concluído      |
  | 4    | Integração básica com LangChain. |     Concluído      |
  | 5    | Implementar retrievers simples para consultas básicas. |     Concluído      |
  | 6    | Testes iniciais de integração entre modelos de IA e base de dados vetorial. |     Concluído      |
  | 7    | Criar pipeline de leitura de dados CSV (reviews da B2W). |     Concluído      |
  | 8    | Conversão dos dados CSV para o formato necessário (IA e banco de dados vetorial). |     Concluído      |
  | 9    | Utilização de embeddings a partir dos dados da B2W. |     Concluído      |
  | 10    | Armazenamento de embeddings no banco de vetores (ChromaDB). |     Concluído      |
  | 10    | Implementar pipeline fim a fim para processar os dados e gerar output final. |     Concluído      |
</br>
</br>

## :dart: MVP
<div name="backlog">
  <h4>Nessa sprint, focamos em entregar a integração do chatbot com a base de dados da B2W, garantindo a consulta de informações sobre satisfação do cliente.</h4>
</div> 


## 📌 Critérios de Aceitação 

| Rank | User Story | Critério de Aceitação |
|:-:|:-:|:-:|
|1|Integração com a Base de Dados da B2W<br>Como um analista de marketing, eu quero interagir com um chatbot que tenha acesso à base de dados da B2W, para que eu possa consultar informações sobre satisfação do cliente, padrões de compra e menções a produtos específicos.| - O chatbot deve ser integrado à base de dados da B2W e garantir o acesso seguro via credenciais de autenticação.<br>- O chatbot deve consultar e retornar informações sobre satisfação do cliente, padrões de compra e menções a produtos específicos.|
|2|Análise de Satisfação do Cliente e Recorrência de Compra<br>Como um analista de marketing, eu quero interagir com o chatbot criado para obter dados de satisfação do cliente e recorrência de compra, para que eu possa focar nas métricas mais relevantes para campanhas de marketing. | - O chatbot deve fornecer a taxa de recorrência de compra e a média de satisfação do cliente.<br>- O chatbot deve segmentar os clientes com base na frequência de compra e nível de satisfação. |    
|3|Análise de Sentimento em Reviews de Produtos<br>Como um analista de marketing, eu quero interagir com o chatbot para que ele analise o sentimento das reviews dos clientes (positivo, neutro, negativo) sobre produtos específicos, para que eu possa ajustar minhas campanhas conforme o sentimento predominante. | - O chatbot deve classificar reviews de produtos em sentimentos (positivo, neutro, negativo).<br>- O chatbot deve fornecer um relatório com a porcentagem de cada sentimento associado a um produto. |

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

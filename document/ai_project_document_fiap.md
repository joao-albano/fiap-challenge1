
<img src="../assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=30% height=30%>

# AI Project Document - Módulo 1 - FIAP

## Nome do Grupo

#### Nomes dos integrantes do grupo
- Gabriella Serni Ponzetta – RM 566296
- João Francisco Maciel Albano – RM 565985
- Fernando Ricardo – RM 566501
- João Pedro Abreu dos Santos – RM 563261
- Gabriel Schuler Barros – RM 564934

## Sumário

[1. Introdução](#c1)  
[2. Visão Geral do Projeto](#c2)  
[3. Desenvolvimento do Projeto](#c3)  
[4. Resultados e Avaliações](#c4)  
[5. Conclusões e Trabalhos Futuros](#c5)  
[6. Referências](#c6)  
[Anexos](#c7)

<br>

# <a name="c1"></a>1. Introdução

## 1.1. Escopo do Projeto

### 1.1.1. Contexto da Inteligência Artificial

O projeto de manutenção preditiva se insere no contexto da aplicação de Inteligência Artificial no setor industrial, com foco na indústria 4.0. A IA tem papel estratégico para aumentar a eficiência operacional, reduzindo paradas não planejadas por meio de análise preditiva. Com abrangência global, a aplicação de IA na manutenção de ativos industriais representa um dos segmentos mais promissores da transformação digital industrial.

### 1.1.2. Descrição da Solução Desenvolvida

Desenvolvemos uma solução digital que coleta dados em tempo real de sensores de máquinas industriais (reais ou simulados), armazena esses dados em um banco PostgreSQL (RDS/AWS), executa previsões com TensorFlow, gera insights com o modelo GPT da OpenAI e emite notificações via WhatsApp utilizando a Evolution API. A solução conta ainda com uma interface web acessível via React para visualização dos dados, permitindo uma gestão eficiente e preventiva das operações industriais.

# <a name="c2"></a>2. Visão Geral do Projeto

## 2.1. Objetivos do Projeto

O principal objetivo é desenvolver uma aplicação de IA capaz de prever falhas em máquinas industriais, evitando paralisações inesperadas por meio de insights baseados em dados operacionais coletados em tempo real.

## 2.2. Público-Alvo

Empresas do setor industrial que buscam reduzir custos com manutenção corretiva, aumentar a disponibilidade dos seus ativos e implantar soluções digitais integradas à Internet das Coisas.

## 2.3. Metodologia

A metodologia adotada se baseia em etapas práticas: definição do escopo, simulação e/ou captura de dados, criação de modelo preditivo com TensorFlow, integração com backend FastAPI, geração de insights com OpenAI GPT, testes e visualização em frontend React.

# <a name="c3"></a>3. Desenvolvimento do Projeto

## 3.1. Tecnologias Utilizadas

- Python (FastAPI)
- TensorFlow
- OpenAI GPT API
- PostgreSQL (AWS RDS)
- AWS IoT Core, Lambda, EC2
- React + Vite + Tailwind
- Evolution API (WhatsApp)

## 3.2. Modelagem e Algoritmos

Foi utilizado um modelo de regressão preditiva com TensorFlow para calcular o tempo restante de vida útil (RUL) dos equipamentos. Esse modelo retorna uma probabilidade de falha que alimenta o pipeline de notificações e geração de insights.

## 3.3. Treinamento e Teste

Os dados foram simulados com base em padrões reais da indústria. O modelo foi avaliado utilizando métricas de MSE (erro quadrático médio) e RMSE, além de validações cruzadas. O backend periodicamente envia os dados para o modelo, que retorna ao backend para nova análise e geração de resposta.

# <a name="c4"></a>4. Resultados e Avaliações

## 4.1. Análise dos Resultados

Os resultados esperados foram atingidos: o modelo identificou com precisão padrões de degradação e a integração com GPT gerou feedbacks explicativos, facilmente interpretáveis no painel de controle.

## 4.2. Feedback dos Usuários

Usuários-teste relataram que a visualização por insights (ao invés de dados brutos) melhorou a tomada de decisão e aumentou a confiança na adoção da solução no ambiente fabril.

# <a name="c5"></a>5. Conclusões e Trabalhos Futuros

A solução atingiu com êxito os objetivos definidos. Entre os pontos fortes estão: modularidade da arquitetura, clareza visual no dashboard e acurácia dos alertas. Como melhorias futuras, pretende-se incluir uma camada de aprendizado contínuo e expandir o número de sensores monitorados por máquina.

# <a name="c6"></a>6. Referências

- https://www.fiap.com.br  
- https://www.tensorflow.org  
- https://platform.openai.com  
- https://aws.amazon.com  
- https://doc.evolution-api.com/v1/pt/get-started/introduction

# <a name="c7"></a>Anexos

## Diagramas e Estrutura Arquitetural

![TPBFZjD03CRlynHMJt1OYGiN3cWBNH0IIALPn05ny6RSTDIPySXsTlaZ7WPns2VW2V9Y9DssYLesjt6-Rtx-FBvKGx4sHHTfRM0C4fgDWGz2jGNEJhSX5nHCaDcJKe7dpoP5mRmzAzQS2cVALjdtI31SXRc9D97e1ZtVXTp06gEISrWR2rGXjH4zo_xyITlkjmHshc2znOPWzXeJUWHFC2](https://github.com/user-attachments/assets/6cdb3460-4fa5-4f15-a894-1d2e7e22bfc1)

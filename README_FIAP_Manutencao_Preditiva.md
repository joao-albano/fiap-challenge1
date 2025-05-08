
# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Sistema de Manutenção Preditiva com IoT e IA

## Nome do grupo

## 👨‍🎓 Integrantes: 
- Nome do integrante 1
- Nome do integrante 2
- Nome do integrante 3
- Nome do integrante 4

## 👩‍🏫 Professores:
### Tutor(a) 
- Nome do Tutor
### Coordenador(a)
- Nome do Coordenador

---

## 📜 Descrição

Indústrias que dependem de equipamentos para produção enfrentam prejuízos operacionais e financeiros significativos com falhas inesperadas. O sistema desenvolvido prevê falhas usando sensores (reais ou simulados), análise preditiva com TensorFlow, geração de insights via GPT da OpenAI e notificações via WhatsApp com a Evolution API. O frontend exibe dados e insights em tempo real, com acesso autenticado.

---

## 🧠 Tecnologias Utilizadas

- Python (FastAPI) - Backend
- React + Vite + Tailwind - Frontend
- TensorFlow - IA preditiva
- OpenAI GPT - Geração de insights
- PostgreSQL (AWS RDS) - Armazenamento
- AWS IoT Core, Lambda, EC2 - Integração IoT e IA
- Evolution API - Notificação por WhatsApp

---

## 🏗️ Arquitetura da Solução

```mermaid
graph TD
    A[Simulated Industrial Machine] -->|MQTT| B[AWS IoT Core]
    B --> C[AWS Lambda]
    C --> D[FastAPI Backend]
    D -->|Armazena| E[PostgreSQL - RDS]
    D -->|Envia| F[Modelo TensorFlow]
    F -->|Retorna resultado| D
    D -->|Consulta GPT| G[OpenAI GPT]
    G -->|Insight| D
    D -->|Grava no BD e envia alerta| E
    D -->|Notifica| H[Evolution API - WhatsApp]
    I[Usuário (Frontend React)] -->|Consulta| D
```

---

## 📁 Estrutura de Pastas

- **.github**: Configurações do GitHub
- **assets**: Imagens do projeto
- **config**: Arquivos de configuração
- **document**: Documentos e entregáveis
- **scripts**: Scripts auxiliares
- **src**: Código-fonte completo
- **README.md**: Este documento

---

## 🚀 Como Executar o Projeto

1. Clonar o repositório
2. Configurar variáveis de ambiente (OpenAI, Evolution API, AWS)
3. Instalar dependências com `pip install -r requirements.txt` e `npm install` no frontend
4. Rodar backend: `uvicorn main:app --reload`
5. Rodar frontend: `npm run dev`

---

## 📆 Roadmap de Desenvolvimento

| Semana | Atividade |
|--------|-----------|
| 1 | Setup AWS IoT + simulação Cloud9 |
| 2 | Backend FastAPI + Lambda |
| 3 | Modelo TensorFlow com dados simulados |
| 4 | Integração GPT + Evolution API |
| 5 | Frontend com dashboard React |
| 6 | Integração e testes do sistema |

---

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>

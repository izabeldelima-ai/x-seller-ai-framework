![n8n](https://img.shields.io/badge/n8n-FF6D5B?style=flat-square&logo=n8n&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

# X-Seller | AI Conversational Architecture & Workflow Orchestration

## 📝 Descrição Técnica
Desenvolvimento de uma arquitetura de **IA Conversacional** e **Orquestração de Workflows** para otimização de resposta em tempo real e automação de funil de vendas. A solução resolve a latência de atendimento humano através de agentes inteligentes com persistência de contexto, transformando a interação passiva em uma jornada ativa de conversão.




## 🛠️ Stack Tecnológica
* **Orquestrador:** n8n (Workflow Automation & Event-Driven Logic)
* **LLM (Large Language Model):** OpenAI GPT-4o
* **Gerenciamento de Estado e Memória:**
    * **Short-term Memory:** Redis (para respostas rápidas e baixa latência)
    * **Long-term Memory:** PostgreSQL / Supabase (para histórico contextual e RAG)
* **Banco de Dados & Persistência:** Supabase (PostgreSQL)
* **Interface de Comunicação:** Evolution API (WhatsApp Integration)
* **CRM & Visualização de Pipeline:** Trello API (Sincronização de dados em tempo real)
* **Protocolo de Entrada:** Webhooks (Event-Driven Architecture)



## 🏗️ Destaques de Engenharia (Key Achievements)

### 1. Arquitetura Event-Driven
Implementação de gatilhos via **Webhooks** para processamento assíncrono de mensagens, garantindo que o sistema escale sem perda de pacotes de dados durante picos de demanda.

### 2. Context Persistence (Dual-Layer Memory)
Estruturação de memória em duas camadas (**Redis/Postgres**) para garantir que o agente de IA mantenha a coerência em conversas longas. O sistema é capaz de retomar interações após hiatos temporais, consultando o histórico via **RAG (Retrieval-Augmented Generation)**.

### 3. Data Synchronization & CRM Orchestration
Automação do fluxo de dados entre a interface de chat e o CRM, eliminando o *data entry* manual. A arquitetura garante a integridade dos dados desde o primeiro contato até a movimentação do card de fechamento.

### 4. Fallback & Guardrails
Implementação de lógica de controle no Supabase para gestão de logs, prevenção de mensagens duplicadas e mecanismos de **Guardrails** para evitar loops de automação ou respostas fora do escopo de negócio.



## 📊 Arquitetura e Visualização
> **Nota de Propriedade Intelectual:** O código-fonte (JSON workflows) e endpoints de API são privados por questões de segurança e confidencialidade comercial. Esta documentação visa detalhar a arquitetura, a lógica de engenharia aplicada e os resultados alcançados.

*(Falta: Inserir aqui um print do fluxo n8n com as notas explicativas visíveis)*

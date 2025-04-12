# LangGraphExampleAgent 🌐

Este projeto cria um agente inteligente capaz de buscar informações atualizadas na web usando o modelo **Gemini 2.0 Flash** integrado à **Tavily Search API**.

O agente é implementado usando a arquitetura **ReAct** via **LangGraph**, permitindo raciocinar sobre perguntas recebidas e executar ações externas, como buscas online, para construir respostas mais completas.

---

## 🛠️ Tecnologias Utilizadas

- [Python 3.12+](https://www.python.org/)
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain Core](https://github.com/langchain-ai/langchain)
- [LangChain Google Generative AI (Gemini)](https://github.com/langchain-ai/langchain/tree/main/libs/langchain-google-genai)
- [LangChain Community Tools (Tavily)](https://github.com/langchain-ai/langchain/tree/main/libs/langchain-community)
- [Tavily Search API](https://app.tavily.com/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)

---
![image](https://github.com/user-attachments/assets/3a0cc284-7fbf-4c87-81c8-a700c3a9bfe2)
---
## 📦 Estrutura do Projeto

```
LangGraphExampleAgent/
├── .env.example     # Exemplo de configuração de variáveis de ambiente
├── README.md        # Documentação do projeto
├── langgraph_example.py         # Código principal do agente LangGraph (ReAct Agent)
├── requirements.txt # (opcional) Arquivo com dependências do projeto
└── langgraph.json   # Arquivo de Configuração LangGraph
```

---

## ⚙️ Configuração e Instalação

1. **Clone o repositório:**

```bash
git clone https://github.com/profmoisesomena/LangGraphExampleAgent.git
cd LangGraphExampleAgent
```

2. **Crie e ative um ambiente virtual:**

```bash
python3.12 -m venv .venv
source .venv/bin/activate  # Linux / MacOS
# ou
.venv\Scripts\activate      # Windows
```

3. **Instale as dependências necessárias:**

```bash
pip install -U langgraph langchain-core langchain-google-genai langchain-community tavily-python python-dotenv
pip install -U "langgraph-cli[inmem]"
```

*(Dica: Você pode também criar um `requirements.txt` com essas bibliotecas para facilitar a instalação.)*

4. **Configure as variáveis de ambiente:**

Crie um arquivo `.env` baseado no exemplo `.env.example`:

```bash
cp .env.example .env
```

Edite o arquivo `.env` preenchendo com suas chaves de API:

```env
GEMINI_API_KEY=your_gemini_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here
```

---

## 🚀 Como Rodar o Agente

Após configurar tudo, para iniciar o ambiente de desenvolvimento do LangGraph:

```bash
langgraph dev
```

Isso abrirá um ambiente interativo para testar o agente!

---

## 💑 Sobre o `langgraph.json`

O arquivo `langgraph.json` pode ser utilizado para configurar e gerenciar múltiplos agentes, rotas e parâmetros de execução no seu projeto LangGraph.


---

## 🤝 Contribuindo

Contribuições são muito bem-vindas!

- Encontrou um problema? Abra uma [issue](https://github.com/profmoisesomena/LangGraphExampleAgent/issues).
- Quer melhorar o agente? Envie um pull request!

Sugestões, melhorias e correções pertinentes são bem vindas. 🚀

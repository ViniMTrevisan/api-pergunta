# 🤖 Ollama Chatbot com Flask

Este projeto é um aplicativo de chat simples e moderno que usa uma interface web para se comunicar com um servidor **Ollama** local. O backend em Python com Flask atua como uma ponte, enviando suas perguntas para o Ollama e recebendo as respostas de modelos de linguagem grandes.

## ✨ Funcionalidades

- **Interface de Usuário Responsiva:** Um front-end limpo e responsivo, estilizado com **Tailwind CSS**.
- **Backend Robusto:** Um servidor **Flask** que gerencia a comunicação entre o front-end e a API do Ollama.
- **Integração com Ollama:** Conecta-se a um servidor Ollama local para gerar respostas usando modelos como o Mistral.
- **Comunicação Assíncrona:** Usa a API `fetch` para interagir com o backend sem recarregar a página.

## 🚀 Tecnologias Utilizadas

- **Frontend:** HTML, JavaScript, Tailwind CSS
- **Backend:** Python, Flask, Flask-CORS, `requests`
- **AI:** Ollama

## 📦 Pré-requisitos

Para executar este projeto, você precisará ter o seguinte instalado:

- **Python 3.8+** e `pip`.
- **Ollama:** Instale e execute o Ollama em sua máquina. O modelo **Mistral** é o padrão para este projeto. Você pode baixá-lo com o comando `ollama run mistral`.

## ⚙️ Como Começar

Siga estes passos para configurar e executar a aplicação:

1.  **Salve os arquivos:** Certifique-se de que o código HTML (`index.html`) e o script Python (`ollama_api.py`) estejam na mesma pasta.

2.  **Crie e ative um ambiente virtual** (recomendado):
    ```bash
    python3 -m venv venv
    # No macOS/Linux
    source venv/bin/activate
    # No Windows
    .\venv\Scripts\activate
    ```

3.  **Instale as dependências do Python:**
    Com o ambiente virtual ativado, execute:
    ```bash
    pip install Flask flask-cors requests
    ```

4.  **Inicie o servidor Flask:**
    Abra seu terminal na pasta do projeto e execute:
    ```bash
    python3 ollama_api.py
    ```
    O servidor da API estará rodando em `http://127.0.0.1:5000`.

5.  **Inicie o Ollama:**
    Em um terminal separado, certifique-se de que o servidor Ollama está em execução. Se ainda não tiver o modelo `mistral`, baixe-o e inicie-o com:
    ```bash
    ollama run mistral
    ```

6.  **Abra o Frontend:**
    Abra o arquivo `index.html` diretamente em seu navegador. A interface se conectará automaticamente ao servidor Flask em execução.

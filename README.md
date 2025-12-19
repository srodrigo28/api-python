# API com Python e FastAPI

Uma API de exemplo construída com Python e FastAPI para demonstrar as operações básicas de CRUD (Create, Read, Update, Delete).

## ✨ Funcionalidades

-   Criação de itens
-   Leitura de itens
-   Atualização de itens
-   Exclusão de itens

## 🚀 Tecnologias Utilizadas

-   [Python 3.10+](https://www.python.org/)
-   [FastAPI](https://fastapi.tiangolo.com/)
-   [Uvicorn](https://www.uvicorn.org/)

## 📋 Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com), [Python](https://www.python.org/). 
Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/).

## ⚙️ Instalação

1. Clone o repositório:
   ```bash
   git clone <URL_DO_SEU_REPOSITORIO>
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd python-api
   ```

3. Crie um ambiente virtual:
   ```bash
   python -m venv venv
   ```

4. Ative o ambiente virtual:
   - **Windows:**
     ```bash
     .\venv\Scripts\activate
     ```
   - **Linux/Mac:**
     ```bash
     source venv/bin/activate
     ```

5. Instale as dependências (crie um arquivo `requirements.txt` com `fastapi` e `uvicorn`):
   ```bash
   pip install -r requirements.txt
   ```

## ▶️ Executando a Aplicação

Para iniciar o servidor, execute o comando:

```bash
uvicorn main:app --reload
```

O servidor estará disponível em `http://127.0.0.1:8000`. A documentação interativa (Swagger UI) pode ser acessada em `http://127.0.0.1:8000/docs`.

## 📝 Endpoints da API

A seguir estão os exemplos de endpoints que você pode implementar.

### **GET** `/items`
Retorna uma lista de todos os itens.

### **GET** `/items/{item_id}`
Retorna um item específico pelo seu ID.

### **POST** `/items`
Cria um novo item. Você precisa enviar os dados do item no corpo da requisição.
- **Corpo da Requisição (Exemplo):**
  ```json
  {
    "name": "Meu Item",
    "description": "Uma descrição para o meu item.",
    "price": 19.99,
    "is_offer": false
  }
  ```

### **PATCH** `/items/{item_id}`
Atualiza parcialmente um item existente.
- **Corpo da Requisição (Exemplo):**
  ```json
  {
    "price": 25.50
  }
  ```

### **DELETE** `/items/{item_id}`
Deleta um item pelo seu ID.

---

Feito com ❤️ por [Seu Nome](https://github.com/seu-usuario)
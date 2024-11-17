### README.md  

# Trabalho Final Américo  
Este é um projeto completo que integra um backend desenvolvido com **Node.js** e **Supabase** e um frontend simples com JavaScript puro. O objetivo principal é gerenciar produtos, permitindo a criação, leitura, atualização e exclusão (CRUD) de itens.

---

## 🚀 Funcionalidades  

### Backend  
1. **API RESTful** desenvolvida com **Express.js**.  
2. Integração com o banco de dados usando **Supabase**.  
3. Rotas para gerenciar produtos:  
   - `GET /products`: Lista todos os produtos.  
   - `GET /products/:id`: Obtém detalhes de um produto específico.  
   - `POST /products`: Cria um novo produto.  
   - `PUT /products/:id`: Atualiza um produto existente.  
   - `DELETE /products/:id`: Remove um produto pelo ID.  
4. Logs de requisições gerenciados por **Morgan**.  
5. Suporte ao **CORS**, permitindo integração com qualquer origem.  
6. Middleware para parsing de requisições JSON e formulários com **Body-Parser**.  

---

### Frontend  
1. Interface simples em HTML/CSS/JS que consome a API.  
2. Funcionalidades:  
   - Listagem de produtos.  
   - Criação de novos produtos via formulário.  
   - Atualização de produtos com modal dinâmico.  
   - Exclusão de produtos diretamente pela interface.  
3. Integração direta com a API do backend.  

---

## 📂 Estrutura do Projeto  

```
trabalho-final-americo
│
├── backend
│   ├── index.js       # Código principal do servidor
│   ├── package.json   # Dependências e scripts do backend
│
├── frontend
│   ├── index.html     # Interface principal
│   ├── style.css      # Estilização
│   ├── script.js      # Lógica do frontend
│
└── README.md          # Documentação do projeto
```

---

## 🛠️ Tecnologias Utilizadas  

### Backend:  
- **Node.js**: Ambiente de execução do JavaScript no servidor.  
- **Express.js**: Framework web para criação das rotas e APIs.  
- **Supabase**: Gerenciamento de banco de dados e autenticação.  
- **Morgan**: Logging de requisições HTTP.  
- **Body-Parser**: Manipulação de requisições JSON e form-data.  
- **CORS**: Controle de políticas de acesso entre domínios.  

### Frontend:  
- **HTML5**: Estrutura da interface.  
- **CSS3**: Estilização.  
- **JavaScript (ES6+)**: Consumo da API e manipulação da DOM.  

---

## 🔧 Pré-requisitos  

- Node.js 18+ instalado.  
- Navegador web atualizado.  
- Banco de dados configurado no Supabase com a tabela `products`.  

### Estrutura da tabela `products`:  

| **Coluna**   | **Tipo** | **Descrição**               |  
|--------------|----------|-----------------------------|  
| id           | Integer  | Identificador único (PK).  |  
| name         | String   | Nome do produto.           |  
| description  | String   | Descrição do produto.      |  
| price        | Decimal  | Preço do produto.          |  

---

## 🚀 Iniciando o Projeto  

### 1. Clonar o repositório  
```bash
git clone <url-do-repositorio>
cd trabalho-final-americo
```

### 2. Configurar o Backend  
```bash
cd backend
npm install
node index.js
```

### 3. Rodar o Frontend  
Abra o arquivo `index.html` no navegador ou utilize uma extensão de servidor estático (como a Live Server no VSCode).  

---

## 🌐 Rotas Disponíveis  

- **`GET /products`**: Retorna todos os produtos.  
- **`GET /products/:id`**: Retorna os detalhes de um produto pelo ID.  
- **`POST /products`**: Cria um novo produto (requisição JSON).  
- **`PUT /products/:id`**: Atualiza um produto existente (requisição JSON).  
- **`DELETE /products/:id`**: Remove um produto pelo ID.  

---

## 🔑 Variáveis Sensíveis  
As chaves de conexão com o Supabase devem ser mantidas em segurança. Recomenda-se o uso de variáveis de ambiente em um arquivo `.env`.

---

## 🖥️ Demonstração  

### Backend em execução:  
```bash
> Ready on http://localhost:3000
```

### Frontend:  
1. Interface de listagem:  
   - Mostra todos os produtos.  
2. Formulário para adicionar produtos.  
3. Modal para editar produtos.  
4. Botão para excluir diretamente na tabela.  

---

## 🛡️ Licença  

Este projeto é distribuído sob a licença MIT.  

--- 

Caso tenha dúvidas ou sugestões, sinta-se à vontade para entrar em contato! 🎉  
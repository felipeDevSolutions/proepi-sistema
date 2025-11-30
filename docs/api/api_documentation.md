---

### 4. Documentação da API: `docs/api/api_documentation.md`

```markdown
# Documentação da API REST

URL Base: `http://localhost:3001/api`

## Autenticação

### Login
*   **Endpoint:** `POST /auth/login`
*   **Body:** `{ "email": "admin@...", "password": "..." }`
*   **Retorno:** `{ "auth": true, "token": "eyJhb..." }`

---

## Produtos (Requer Header: `Authorization: Bearer <token>`)

### Listar Todos
*   **Endpoint:** `GET /products`
*   **Retorno:** Array de objetos Produto.

### Criar Produto
*   **Endpoint:** `POST /products`
*   **Body:** 
    ```json
    {
      "name": "Capacete",
      "description": "Classe B",
      "photoUrl": "data:image/png;base64..."
    }
    ```

### Deletar Produto
*   **Endpoint:** `DELETE /products/:id`

---

## Movimentações (Requer Token)

### Registrar Entrada/Saída
*   **Endpoint:** `POST /movements`
*   **Body:**
    ```json
    {
      "productId": "ID_DO_PRODUTO",
      "type": "IN" (ou "OUT"),
      "quantity": 10
    }
    ```
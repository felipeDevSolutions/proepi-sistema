# ProEPI - Sistema de Gestão de Estoque de EPIs

![Badge Status](https://img.shields.io/badge/STATUS-CONCLUÍDO-brightgreen)
![Badge Stack](https://img.shields.io/badge/STACK-React%20%7C%20Node.js%20%7C%20Firebase-blue)

O **ProEPI** é um sistema SaaS (Software as a Service) desenvolvido para modernizar e simplificar o controle de estoque de Equipamentos de Proteção Individual (EPIs). O projeto visa substituir planilhas manuais propensas a erros por uma interface visual intuitiva, focada na agilidade do setor de Segurança do Trabalho (SESMT).

---

## 🎯 Objetivo
Resolver a desorganização no controle de EPIs em canteiros de obras e indústrias, centralizando entradas e saídas de estoque em um sistema web simples, que não exige o cadastro complexo de colaboradores para realizar baixas, focando puramente na gestão quantitativa e visual dos itens.

---

## 🚀 Funcionalidades Implementadas

*   **Autenticação Segura:** Login administrativo com JWT (JSON Web Token).
*   **Catálogo Visual:** Listagem de EPIs com fotos, descrição e indicadores visuais de estoque baixo.
*   **Gestão de Produtos:** Cadastro e exclusão de itens (CRUD).
*   **Controle de Estoque:** Registro de Entradas e Saídas com atualização em tempo real.
*   **Busca Inteligente:** Filtro instantâneo por nome do EPI.
*   **Dashboard Interativo:** Interface responsiva com design moderno (Glassmorphism/Blueprint).

---

## 🛠 Tecnologias Utilizadas

### Frontend
*   **React.js (v18):** Biblioteca para construção da interface (SPA).
*   **CSS3 Moderno:** Variáveis CSS, Flexbox, Grid Layout e Design Responsivo.
*   **Axios:** Cliente HTTP para comunicação com a API.

### Backend
*   **Node.js & Express:** Servidor de aplicação e API RESTful.
*   **JWT & Bcrypt:** Segurança, criptografia de senhas e controle de sessões.
*   **Arquitetura em Camadas:** Separação clara entre Controllers, Services e Configuração.

### Banco de Dados & Infraestrutura
*   **Firebase Firestore:** Banco de dados NoSQL para alta performance e flexibilidade.
*   **Firebase Storage:** Armazenamento de imagens (via Base64 para este MVP).




⚙️ Instruções de Instalação e Execução

Pré-requisitos
Node.js (v18 ou superior)
Conta no Firebase (Google Cloud)

1. Configuração do Backend
code
Bash
# Entre na pasta do backend
cd backend

# Instale as dependências
npm install

# Configuração de Ambiente (.env)
# Crie um arquivo .env na raiz do backend com:
# PORT=3001
# JWT_SECRET=sua_chave_secreta_aqui

# Configuração do Firebase
# Coloque seu arquivo 'serviceAccountKey.json' baixado do Firebase em:
# backend/src/config/serviceAccountKey.json

# Inicie o servidor
npm run dev

2. Configuração do Frontend
code
Bash
# Em outro terminal, entre na pasta web
cd frontend/web

# Instale as dependências
npm install

# Inicie a aplicação
npm start
O sistema estará acessível em: http://localhost:3000


---

🔐 Acesso ao Sistema (Ambiente de Teste)

Para fins de avaliação acadêmica e testes locais:
URL Local: http://localhost:3000
Usuário Admin: admin@proepi.com
Senha: 123
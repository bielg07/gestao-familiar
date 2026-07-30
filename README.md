# 👨‍👩‍👧 FamilyHub

O **FamilyHub** é uma plataforma web desenvolvida para auxiliar famílias na organização do dia a dia. O sistema permite gerenciar membros da família, acompanhar atividades e visualizar informações em um dashboard simples e intuitivo.

## 📸 Demonstração

> Adicione aqui prints do sistema.

| Landing Page | Dashboard |
|--------------|-----------|
| *(Imagem)* | *(Imagem)* |

---

# ✨ Funcionalidades

- 🔐 Sistema de Login e Cadastro
- 👨‍👩‍👧 Gerenciamento de membros da família
- 📅 Cadastro e controle de atividades
- 📊 Dashboard com informações do sistema
- 🔒 Autenticação de usuários
- 💾 Integração com banco de dados MySQL

---

# 🛠️ Tecnologias Utilizadas

### Front-end
- HTML5
- CSS3
- JavaScript

### Back-end
- PHP 8+

### Banco de Dados
- MySQL

---

# 📂 Estrutura do Projeto

```
FamilyHub/
│
├── frontend/
│   ├── index.html
│   ├── landing.html
│   ├── login.html
│   ├── script.js
│   └── style.css
│
├── backend/
│   ├── api/
│   │   ├── auth.php
│   │   ├── dashboard.php
│   │   ├── membros.php
│   │   └── atividades.php
│   │
│   ├── config/
│   │   └── db.php
│   │
│   ├── middleware/
│   │   └── auth.php
│   │
│   ├── index.php
│   └── .htaccess
│
├── database.sql
├── adicionar_prioridade.sql
└── README.md
```

---

# ⚙️ Como Executar

## 1. Clone o repositório

```bash
git clone https://github.com/SEU-USUARIO/FamilyHub.git
```

---

## 2. Configure o banco de dados

Crie um banco MySQL e importe o arquivo:

```
database.sql
```

Caso utilize a funcionalidade de prioridades, execute também:

```
adicionar_prioridade.sql
```

---

## 3. Configure a conexão

Edite:

```
backend/config/db.php
```

Configure as credenciais do seu banco.

Exemplo:

```php
define('DB_HOST', 'localhost');
define('DB_NAME', 'familyflow');
define('DB_USER', 'root');
define('DB_PASS', '');
```

---

## 4. Coloque o projeto no servidor

Caso utilize XAMPP:

```
htdocs/
    FamilyHub/
```

Depois acesse:

```
http://localhost/FamilyHub/frontend/landing.html
```

---

# 📌 Rotas da API

## Autenticação

| Método | Endpoint |
|---------|----------|
| POST | /auth/login |
| POST | /auth/cadastro |
| POST | /auth/logout |
| GET | /auth/me |

---

## Membros

| Método | Endpoint |
|---------|----------|
| GET | /membros |
| POST | /membros |
| PUT | /membros |
| DELETE | /membros |

---

## Atividades

| Método | Endpoint |
|---------|----------|
| GET | /atividades |
| POST | /atividades |
| PUT | /atividades |
| DELETE | /atividades |

---

# 🔒 Segurança

- Autenticação por token
- Middleware de autenticação
- Separação entre Front-end e Back-end
- Organização em API REST

---

# 🚀 Melhorias Futuras

- Notificações
- Calendário compartilhado
- Upload de fotos
- Aplicativo mobile
- Integração com Google Calendar
- Sistema de lembretes
- Perfis com diferentes permissões

---

# 👨‍💻 Autor

Desenvolvido por **Gabriel Gomes**.

Caso tenha sugestões ou encontre algum problema, fique à vontade para abrir uma **Issue** ou enviar um **Pull Request**.

---

# 📄 Licença

Este projeto foi desenvolvido para fins acadêmicos e de estudo.

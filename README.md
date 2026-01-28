# 📝 Flask Auth – Sistema de Autenticação  
### Aplicação simples para gerenciamento de usuários e autenticação

Este projeto foi desenvolvido com **Flask**, com foco em reforçar conhecimentos sobre autenticação, CRUD de usuários, gerenciamento de perfil e boas práticas de backend.

---

## 🚀 Funcionalidades Principais

- 🆕 Cadastro de usuários  
- 🔐 Login com verificação de credenciais  
- 👤 Página de perfil  
- ✏️ Atualização de informações do usuário  
- 🚪 Logout  
- 🛢️ Banco de dados com SQLAlchemy  
- 🧱 Migrações com Flask-Migrate  

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**  
- **Flask**  
- **Flask SQLAlchemy**  
- **Flask Migrate**  
- **Werkzeug Security**  
- **SQLite**  
- **Dotenv**  

---

## ⚙️ Como Rodar o Projeto Localmente

### 📦 1. Clone o repositório

git clone https://github.com/gabrieleMarciano/sample-flask-auth  
cd sample-flask-auth

### 📦 2. Crie e ative o ambiente virtual

python -m venv venv  
source venv/bin/activate   # Linux/Mac  
venv\Scripts\activate      # Windows

### 📜 3. Instale as dependências

pip install -r requirements.txt

### 🔑 4. Configure o arquivo .env

FLASK_APP=app.py  
FLASK_DEBUG=True  
SECRET_KEY=sua_chave_secreta

### 🗄️ 5. Inicialize o banco de dados

flask db init  
flask db migrate  
flask db upgrade

### 🚀 6. Execute a aplicação

flask run

A aplicação rodará em:  
http://127.0.0.1:5000

---

## 🔐 Fluxo de Autenticação

1. Usuário realiza cadastro  
2. Senha é armazenada com hash seguro  
3. Login valida credenciais e gera sessão  
4. Usuário autenticado acessa e edita o perfil  
5. Logout encerra a sessão com segurança  

---

## 🧱 Endpoints Principais  
*(caso adicione uma versão API mais tarde)*

- **POST /register** → Criar usuário  
- **POST /login** → Autenticar usuário  
- **GET /profile** → Ver perfil  
- **PUT /profile** → Atualizar dados  
- **GET /logout** → Encerrar sessão  

---

## 🧠 Aprendizados Reforçados

- Estruturação de aplicação Flask  
- Modelagem e migração de banco de dados  
- Hashing seguro de senhas  
- Organização modular de rotas  
- Gerenciamento de sessão  
- Uso de templates com Jinja2  
- Boas práticas de backend  

---

## 🧱 Estrutura do Projeto

/
├── app.py                 # Arquivo principal Flask  
├── models.py              # Modelos de usuário  
├── routes/                # Rotas da aplicação  
│   ├── auth.py  
│   └── profile.py  
├── templates/             # Páginas HTML (Jinja2)  
├── static/                # CSS, imagens, etc.  
├── requirements.txt       # Dependências  
├── .env                   # Variáveis de ambiente  
└── README.md              # Documentação  

---

## 🔮 Possíveis Melhorias

- Recuperação de senha  
- Confirmação de email  
- Testes automatizados  
- Blueprints mais avançados  
- Integração com APIs externas  

---

## 📜 Licença

Projeto aberto para estudo e evolução contínua.  
Sinta-se à vontade para contribuir! 💜


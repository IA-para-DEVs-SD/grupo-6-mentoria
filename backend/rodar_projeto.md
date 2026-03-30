# Como rodar o projeto — Backend

## Pré-requisitos

| Ferramenta | Versão mínima | Como verificar | Download |
|---|---|---|---|
| Python | **3.12** | `python3 --version` | [python.org](https://www.python.org/downloads/) |
| pip | qualquer recente | `pip --version` | já vem com o Python |
| Git | qualquer | `git --version` | [git-scm.com](https://git-scm.com/) |

> **Atenção:** Python 3.12 é obrigatório. Versões anteriores (3.10, 3.11) não são suportadas.

---

## Credenciais necessárias (obtenha antes de começar)

Você vai precisar de 3 chaves antes de rodar o projeto:

### 1. GEMINI_API_KEY
1. Acesse [Google AI Studio](https://aistudio.google.com)
2. Clique em **"Get API key"** → **"Create API key"**
3. Copie a chave gerada

### 2. GOOGLE_CLIENT_ID e GOOGLE_CLIENT_SECRET (OAuth)
1. Acesse [Google Cloud Console](https://console.cloud.google.com)
2. Crie um projeto (ou selecione um existente)
3. Vá em **APIs & Services → Credentials**
4. Clique em **"+ Create Credentials" → "OAuth 2.0 Client IDs"**
5. Tipo: **Web application**
6. Em **Authorized redirect URIs**, adicione: `http://localhost:8000/auth/google/callback`
7. Copie o **Client ID** e o **Client Secret**

### 3. JWT_SECRET
- Qualquer string longa e aleatória. Exemplo: `minha-chave-super-secreta-123`

---

## Primeira vez

```bash
# 1. Entre na pasta do backend
cd backend

# 2. Criar o ambiente virtual
python3 -m venv .venv

# 3. Ativar o ambiente virtual
# Linux/macOS:
source .venv/bin/activate
# Windows:
.venv\Scripts\activate

# 4. Instalar dependências
pip install -r requirements.txt

# 5. Criar o arquivo de configuração
cp .env.example .env
```

Abra o arquivo `.env` e preencha com suas credenciais:

```env
DATABASE_URL=sqlite:///./mentoria.db
REDIS_URL=redis://localhost:6379
GOOGLE_CLIENT_ID=cole-seu-client-id-aqui
GOOGLE_CLIENT_SECRET=cole-seu-client-secret-aqui
GOOGLE_REDIRECT_URI=http://localhost:8000/auth/google/callback
JWT_SECRET=cole-uma-string-longa-e-aleatoria-aqui
GEMINI_API_KEY=cole-sua-chave-gemini-aqui
```

```bash
# 6. Criar as tabelas no banco de dados
alembic upgrade head

# 7. Subir o servidor
uvicorn src.main:app --reload
```

---

## Próximas vezes

```bash
# Ativar o ambiente virtual (sempre necessário)
source .venv/bin/activate   # Linux/macOS
# .venv\Scripts\activate    # Windows

# Subir o servidor
uvicorn src.main:app --reload
```

---

## Acessar

| Interface | URL |
|---|---|
| Swagger UI (documentação interativa) | http://127.0.0.1:8000/docs |
| ReDoc (documentação alternativa) | http://127.0.0.1:8000/redoc |
| Login Google | http://127.0.0.1:8000/auth/google/login |

---

## Rodar os testes

```bash
# Com o ambiente virtual ativado:
pytest tests/ -v

# Com relatório de cobertura:
pytest tests/ --cov=src --cov-report=term-missing
```

---

## Problemas comuns

**`ModuleNotFoundError`** — ambiente virtual não está ativado. Rode `source .venv/bin/activate`.

**`alembic: command not found`** — ambiente virtual não está ativado.

**Erro de autenticação Google** — verifique se o `GOOGLE_REDIRECT_URI` no `.env` é exatamente `http://localhost:8000/auth/google/callback` e se essa URI está cadastrada no Google Cloud Console.

**`GEMINI_API_KEY` inválida** — verifique se copiou a chave corretamente sem espaços extras.

---

## Documentação do projeto

| Documento | Descrição |
|---|---|
| [PRD — Requisitos do Produto](docs/PRD.md) | User stories, critérios de aceite e requisitos não-funcionais |
| [Arquitetura do Backend](docs/ARCHITECTURE.md) | Modelo de dados, endpoints, agentes IA e infraestrutura |

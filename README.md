# 🎯 Mentoria.IA

> Plataforma de mentoria de carreira impulsionada por inteligência artificial. Analisa seu perfil profissional, identifica gaps de competência e gera planos de desenvolvimento personalizados com ações concretas para alcançar seus objetivos.

---

## 📚 Documentação

| Documento | Descrição |
|---|---|
| [PRD — Requisitos do Produto](backend/docs/PRD.md) | User stories, critérios de aceite, casos de uso e requisitos não-funcionais |
| [Arquitetura do Backend](backend/docs/ARCHITECTURE.md) | Modelo de dados, endpoints, agentes IA e infraestrutura Docker |
| [Arquitetura do Frontend](frontend/docs/ARCHITECTURE.md) | Stack, estrutura de pastas, rotas, stores e fluxo do usuário |

---

## 🛠️ Tecnologias

Para detalhes completos com versões, consulte a seção Stack de cada módulo:

- [Stack do Backend](backend/docs/ARCHITECTURE.md#stack)
- [Stack do Frontend](frontend/docs/ARCHITECTURE.md#stack)
| Camada | Tecnologia | Versão mínima |
|---|---|---|
| Frontend | Vue.js 3 + PrimeVue 4 + Tailwind CSS 4 | — |
| State | Pinia | — |
| Build | Vite 7 + TypeScript 5.9 | Node.js **20.19** ou **22.12+** |
| Backend | FastAPI | Python **3.12** |
| ORM | SQLAlchemy + Alembic | — |
| Banco de Dados | SQLite | — |
| LLM | Google Gemini 2.5 Flash via PydanticAI | — |
| Autenticação | Google OAuth 2.0 + JWT | — |
| Infra | Docker Compose | Docker **24+** |

---

## 🚀 Como rodar

### Opção 1 — Docker Compose (recomendado, mais simples)

- [Docker](https://docs.docker.com/get-docker/) e [Docker Compose](https://docs.docker.com/compose/install/)
- Chave de API do [Google Gemini](https://aistudio.google.com/api-keys)
- Credenciais OAuth do Google (para autenticação)

### Configuração

1. Clone o repositório:
**Pré-requisitos:**
- [Docker Desktop](https://docs.docker.com/get-docker/) instalado e rodando
- Chaves de API (veja seção abaixo)

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/mentoria-ia.git
cd mentoria-ia

# 2. Crie o arquivo de configuração
cp backend/.env.example backend/.env
```

Abra `backend/.env` e preencha:

```env
GEMINI_API_KEY=sua-chave-gemini
DATABASE_URL=sqlite:///./mentoria.db
JWT_SECRET=qualquer-string-longa-e-aleatoria
GOOGLE_CLIENT_ID=seu-client-id
GOOGLE_CLIENT_SECRET=seu-client-secret
GOOGLE_REDIRECT_URI=http://localhost:8000/auth/google/callback
```

```bash
# 3. Suba os serviços
docker compose up --build
```

4. Na primeira execução, crie a estrutura do banco de dados:

```bash
docker compose exec backend alembic upgrade head
```

5. Acesse a aplicação:

| Serviço | URL |
|---|---|
| Frontend | http://localhost:5173 |
| Backend API | http://localhost:8000 |
| Swagger UI | http://localhost:8000/docs |

---

### Opção 2 — Sem Docker (desenvolvimento local)

Veja os guias detalhados com passo a passo completo:

- **Backend:** [backend/rodar_projeto.md](backend/rodar_projeto.md) — Python 3.12 obrigatório
- **Frontend:** [frontend/rodar_projeto.md](frontend/rodar_projeto.md) — Node.js 20.19+ ou 22.12+

---

## 🔑 Obtendo as credenciais

### GEMINI_API_KEY
1. Acesse [Google AI Studio](https://aistudio.google.com)
2. Clique em **"Get API key"** → **"Create API key"**

### GOOGLE_CLIENT_ID e GOOGLE_CLIENT_SECRET
1. Acesse [Google Cloud Console](https://console.cloud.google.com)
2. Vá em **APIs & Services → Credentials**
3. Crie um **OAuth 2.0 Client ID** do tipo **Web application**
4. Adicione `http://localhost:8000/auth/google/callback` como URI de redirecionamento autorizado

### JWT_SECRET
Qualquer string longa e aleatória. Exemplo: `minha-chave-super-secreta-2024`

---

## 👥 Integrantes do Grupo

| Nome | Papel |
|---|---|
| Willian Silvano Maira | 🎵 Bardo |
| Taiane Baldin | 🛡️ Paladina |
| Murilo Henrique da Silva Pires | 🔮 Mago |
| Murilo Barcelos Corrêa | 🔮 Mago |
| Paulo Sérgio Nunes Gonçalves | 🔮 Mago |

---

## 📄 Licença

MIT

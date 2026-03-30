# 🎯 Mentoria.IA

> Plataforma de mentoria de carreira impulsionada por inteligência artificial. Analisa seu perfil profissional, identifica gaps de competência e gera planos de desenvolvimento personalizados com ações concretas para alcançar seus objetivos.

---

## 📚 Sumário de Documentações

| Documento | Descrição |
|---|---|
| [Requisitos do Produto (PRD)](backend/docs/PRD.md) | User stories, critérios de aceite, casos de uso e requisitos não-funcionais |
| [Arquitetura do Backend](backend/docs/ARCHITECTURE.md) | Arquitetura completa: modelo de dados, endpoints, agentes IA, infraestrutura Docker |
| [Arquitetura do Frontend](frontend/docs/ARCHITECTURE.md) | Stack, estrutura de pastas, rotas, stores, fluxo do usuário |
---

## 🛠️ Tecnologias Utilizadas

Para detalhes completos com versões, consulte a seção Stack de cada módulo:

- [Stack do Backend](backend/docs/ARCHITECTURE.md#stack)
- [Stack do Frontend](frontend/docs/ARCHITECTURE.md#stack)

---

## 🚀 Instruções de Instalação e Uso

### Pré-requisitos

- [Docker](https://docs.docker.com/get-docker/) e [Docker Compose](https://docs.docker.com/compose/install/)
- Chave de API do [Google Gemini](https://aistudio.google.com/api-keys)
- Credenciais OAuth do Google (para autenticação)

### Configuração

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/mentoria-ia.git
cd mentoria-ia
```

2. Copie o arquivo de variáveis de ambiente e preencha com suas credenciais:

```bash
cp backend/.env.example backend/.env
```

```env
GEMINI_API_KEY=sua-chave-gemini
DATABASE_URL=sqlite:///./mentoria.db
JWT_SECRET=sua-chave-secreta
GOOGLE_CLIENT_ID=seu-client-id
GOOGLE_CLIENT_SECRET=seu-client-secret
GOOGLE_REDIRECT_URI=http://localhost:8000/auth/google/callback
```

3. Suba os serviços:

```bash
docker compose up -d
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
| Documentação da API | http://localhost:8000/docs |

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

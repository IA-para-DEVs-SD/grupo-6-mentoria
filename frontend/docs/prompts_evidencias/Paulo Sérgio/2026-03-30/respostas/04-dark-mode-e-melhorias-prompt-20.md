[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

---

# Resposta da IA — Prompt 20
### Dark Mode, Accordion de Perfil, Favicon e Infra

> Access to XMLHttpRequest at 'http://localhost:8000/profile' from origin 'http://localhost:5173' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested res...

---

**Passo 1** — `execute_bash`

> O CORS aparece porque o backend está crashando (500) antes de enviar os headers CORS. Vou ver o erro real:

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && docker compose logs --tail 40 backen`

**Passo 2** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && docker compose logs --tail 80 backen`

**Passo 3** — `execute_bash`

> O banco SQLite está como read-only. O arquivo foi criado pelo root (dentro do container) e o processo não consegue escrever:

- 🖥️ `ls -la /home/paulo/dev/work/grupo-6-mentoria/backend/mentoria.db`

**Passo 4** — `execute_bash`

> Permissão `644` com owner `root` — o processo no container não consegue escrever. Vou corrigir:

- 🖥️ `sudo chmod 666 /home/paulo/dev/work/grupo-6-mentoria/backend/mentoria.db`

**Passo 5** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && docker compose restart backend 2>&1`

---

[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

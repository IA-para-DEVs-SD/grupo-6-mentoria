[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

---

# Resposta da IA — Prompt 4
### Dark Mode, Accordion de Perfil, Favicon e Infra

> pode reverter e abra o documento em um novo terminal com glow pra mim

---

**Passo 1** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git diff --name-only`

**Passo 2** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git checkout -- frontend/src/ fronte`

**Passo 3** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git diff --name-only`

**Passo 4** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git status --short`

**Passo 5** — `execute_bash`

> O `useTheme.ts` antigo ficou como untracked. Vou remover ele também já que vai ser recriado pela tarefa nova:

- 🖥️ `rm /home/paulo/dev/work/grupo-6-mentoria/frontend/src/composables/useTheme.ts`

**Passo 6** — `execute_bash`

- 🖥️ `which glow 2>/dev/null || echo "NOT_FOUND"`

**Passo 7** — `execute_bash`

- 🖥️ `setsid gnome-terminal -- bash -c "glow /home/paulo/dev/work/grupo-6-mentoria/fro`

---

[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

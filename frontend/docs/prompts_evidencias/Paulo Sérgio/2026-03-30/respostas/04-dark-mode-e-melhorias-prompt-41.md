[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

---

# Resposta da IA — Prompt 41
### Dark Mode, Accordion de Perfil, Favicon e Infra

> o componente todo tem que ter o background igual ao desse elemento <div class="bg-white dark:bg-slate-800 rounded-2xl border border-gray-200 dark:border-slate-700 p-5 space-y-4"><h3 class="font-bold t...

---

**Passo 1** — `fs_write`

> Entendi — o accordion precisa ter o mesmo visual de card que o GapsList: `bg-white dark:bg-slate-800 rounded-2xl border border-gray-200 dark:border-slate-700 p-5`. Vou envolver o accordion num wrapper com essas classes e garantir que o PrimeVue accordion fique transparente:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ProfileAccordion.vue`

**Passo 2** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ProfileAccordion.vue`

**Passo 3** — `fs_write`

> Agora forçar o accordion inteiro (header, content, panel) transparente pra herdar do wrapper:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/assets/main.css`

**Passo 4** — `fs_write`

> Preciso que funcione nos dois modos, não só dark:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/assets/main.css`

**Passo 5** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && docker compose build --no-cache fron`

---

[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

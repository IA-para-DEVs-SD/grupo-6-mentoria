[← Voltar aos prompts](../02-features-core.md)

---

# Resposta da IA — Prompt 7
### Features Core — Login até Novo Plano (Tarefas 1-6)

> Execute a tarefa 6 conforme docs/tarefas/6-novo-plano.md.
Tarefas 0-5 concluídas — todo o fluxo funcional: login, onboarding, geração, detalhes e Home com lista de planos.

---

**Passo 1** — `fs_read`

**Passo 2** — `fs_read`

> Let me check the current state of the files I need to modify:

**Passo 3** — `fs_write`

> The changes needed are minimal. Looking at the current code:
> 
> 1. `OnboardingPage.vue` already pre-fills from `profileStore.profile` (line: `profileStore.profile ? JSON.parse(JSON.stringify(profileStore.profile)) : ...`). It just needs the `isNewPlan` detection for the button label.
> 2. `HomePage.vue` just needs `?mode=new-plan` added to the navigation.
> 3. `useOnboarding.ts` and `profileStore.ts` don't need changes — they already work correctly.
> 
> Two small edits:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/HomePage.vue`

**Passo 4** — `fs_write`

> Now update OnboardingPage to detect the mode and change the button label + ensure profile is loaded for pre-fill:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/OnboardingPage.vue`

**Passo 5** — `fs_write`

> Now update the button label:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/OnboardingPage.vue`

**Passo 6** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend && npm run build 2>&1`

---

[← Voltar aos prompts](../02-features-core.md)

[← Voltar aos prompts](../02-features-core.md)

---

# Resposta da IA — Prompt 1
### Features Core — Login até Novo Plano (Tarefas 1-6)

> Execute a tarefa 1 conforme docs/tarefas/1-login.md. 
A tarefa 0 já foi concluída — o projeto está em frontend/ com scaffold, stores, services mock, router e páginas placeholder.

---

**Passo 1** — `fs_read`

> Let me start by reading the task file and understanding the current state of the project.

**Passo 2** — `fs_read`

> Now let me read all the existing files I need to modify:

**Passo 3** — `fs_read`

> Good, I have a clear picture. Let me also check the existing components/auth directory and the package.json for installed deps:

**Passo 4** — `fs_write`

> Now I have everything I need. Let me implement the task. Here's the plan:
> 
> 1. Create `GoogleLoginButton.vue` component
> 2. Update `authService.ts` (mock with dicebear avatar)
> 3. Update `authStore.ts` (login with profile check, localStorage persistence)
> 4. Update `LoginPage.vue` (full layout with logo, subtitle, loading state)
> 5. Update `DefaultLayout.vue` (header with logo + logout icon)
> 6. Update `router/index.ts` (guard already looks good, minor tweak)
> 
> Let's go:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/auth/GoogleLoginButton.vue`

**Passo 5** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/services/authService.ts`

**Passo 6** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/stores/authStore.ts`

**Passo 7** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/LoginPage.vue`

**Passo 8** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/layouts/DefaultLayout.vue`

**Passo 9** — `fs_write`

> The router guard already looks correct from the scaffold. Let me just make sure the guard uses `to.path` consistently (it currently mixes `to.name` and that's fine, but let me align with the task spec which uses `to.path`):

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/router/index.ts`

**Passo 10** — `execute_bash`

> Now let's verify the build passes:

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend && npm run build 2>&1`

**Passo 11** — `fs_read`

> Build passed cleanly (type-check + vite build). Let me do a quick sanity check on the final state of all modified files:

---

[← Voltar aos prompts](../02-features-core.md)

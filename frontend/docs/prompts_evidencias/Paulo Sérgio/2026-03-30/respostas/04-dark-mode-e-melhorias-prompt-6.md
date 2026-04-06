[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

---

# Resposta da IA — Prompt 6
### Dark Mode, Accordion de Perfil, Favicon e Infra

> pode implementar

---

**Passo 1** — `fs_read`

> Vou seguir a tarefa 14 na ordem definida.
> 
> **Passo 1/6 — main.ts (darkModeSelector → `.dark`)**

**Passo 2** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/main.ts`

**Passo 3** — `fs_write`

> **Passo 2/6 — main.css (@custom-variant)**

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/assets/main.css`

**Passo 4** — `fs_write`

> **Passo 3/6 — composables/useTheme.ts**

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/composables/useTheme.ts`

**Passo 5** — `fs_read`

> **Passo 4/6 — DefaultLayout.vue (toggle + dark classes)**

**Passo 6** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/layouts/DefaultLayout.vue`

**Passo 7** — `fs_read`

> **Passo 5/6 — Variantes dark em todos os componentes**

**Passo 8** — `fs_write`

> Agora vou aplicar as variantes dark em todas as pages:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/LoginPage.vue`

**Passo 9** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/HomePage.vue`

**Passo 10** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/OnboardingPage.vue`

**Passo 11** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/LoadingAIPage.vue`

**Passo 12** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/AuthCallbackPage.vue`

**Passo 13** — `fs_read`

> Agora os componentes home, plan, onboarding e auth:

**Passo 14** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/home/PlanCard.vue`

**Passo 15** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/home/EmptyState.vue`

**Passo 16** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/auth/GoogleLoginButton.vue`

**Passo 17** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/auth/GoogleLoginButton.vue`

**Passo 18** — `fs_read`

> Agora os componentes plan:

**Passo 19** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/PlanHeader.vue`

**Passo 20** — `fs_write`

> ProgressCard já é escuro (bg-indigo-600), mas vou ajustar pro dark mode ficar mais sutil:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ProgressCard.vue`

**Passo 21** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/GapsList.vue`

**Passo 22** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ActionItem.vue`

**Passo 23** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ActionItem.vue`

**Passo 24** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ActionItem.vue`

**Passo 25** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/plan/ActionTimeline.vue`

**Passo 26** — `fs_read`

> Agora os componentes de onboarding:

**Passo 27** — `fs_write`

> Vou aplicar dark em todos os onboarding de uma vez:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepTrajetoria.vue`

**Passo 28** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding && s`

**Passo 29** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepFormacao.vue`

**Passo 30** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepHabilidades.vue`

**Passo 31** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepHabilidades.vue`

**Passo 32** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepHabilidades.vue`

**Passo 33** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepObjetivo.vue`

**Passo 34** — `fs_write`

> Agora o StepRevisao:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 35** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 36** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 37** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 38** — `execute_bash`

> **Passo 6/6 — Build para validar**

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && docker run --rm -v "$(pwd)/frontend:`

**Passo 39** — `execute_bash`

> Build limpo. Vou verificar o resumo final:

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git diff --stat`

---

[← Voltar aos prompts](../04-dark-mode-e-melhorias.md)

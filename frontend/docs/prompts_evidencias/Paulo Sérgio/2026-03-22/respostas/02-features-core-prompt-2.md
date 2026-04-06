[← Voltar aos prompts](../02-features-core.md)

---

# Resposta da IA — Prompt 2
### Features Core — Login até Novo Plano (Tarefas 1-6)

> Execute a tarefa 2 conforme docs/tarefas/2-onboarding.md.
As tarefas 0 e 1 estão concluídas — login funcional, router com guard, stores e services base criados.

---

**Passo 1** — `fs_read`

> Let me start by reading the task file and understanding the current state.

**Passo 2** — `fs_read`

> Now let me check the current state of the files I need to modify/understand:

**Passo 3** — `fs_read`

> Let me also check the MVP for reference on the onboarding visual style:

**Passo 4** — `fs_read`

> Let me see the MVP onboarding section more closely for visual reference:

**Passo 5** — `fs_write`

> Good, I have full context. Now let me implement everything. I'll create the files in order:
> 
> 1. `composables/useOnboarding.ts`
> 2. `profileStore.ts` (update with `hasProfile`)
> 3. `StepTrajetoria.vue`
> 4. `StepFormacao.vue`
> 5. `StepHabilidades.vue`
> 6. `StepObjetivo.vue`
> 7. `StepRevisao.vue`
> 8. `OnboardingPage.vue`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/composables/useOnboarding.ts`

**Passo 6** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/stores/profileStore.ts`

**Passo 7** — `fs_write`

> Now the step components. Starting with StepTrajetoria:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepTrajetoria.vue`

**Passo 8** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepFormacao.vue`

**Passo 9** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepHabilidades.vue`

**Passo 10** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepObjetivo.vue`

**Passo 11** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 12** — `fs_write`

> Now the main OnboardingPage:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/pages/OnboardingPage.vue`

**Passo 13** — `execute_bash`

> Now let's build and check for errors:

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend && npm run build 2>&1`

**Passo 14** — `fs_write`

> Several TS issues to fix. The main problems:
> 
> 1. DatePicker expects `Date` objects, not strings — need to use `Date | null` in the reactive data
> 2. The `senioridade` and `objetivo` types don't allow empty string for initial state
> 3. The `SENIORIDADES` readonly array can't be assigned to mutable `any[]`
> 4. Step navigation types
> 
> Let me fix these. The types in `profile.ts` use `string` for dates, but PrimeVue DatePicker needs `Date`. I need to handle this at the component level. Let me update the 

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/types/profile.ts`

**Passo 15** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/types/index.ts`

**Passo 16** — `fs_write`

> Now fix the composable to work with null instead of empty string:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/composables/useOnboarding.ts`

**Passo 17** — `fs_write`

> Now fix StepTrajetoria — use mutable array for SENIORIDADES and Date types:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepTrajetoria.vue`

**Passo 18** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepFormacao.vue`

**Passo 19** — `fs_write`

> Now fix StepObjetivo to use the updated type:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepObjetivo.vue`

**Passo 20** — `fs_write`

> Fix StepRevisao to handle Date objects:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/components/onboarding/StepRevisao.vue`

**Passo 21** — `fs_write`

> Now I need to update the profileService to handle Date serialization/deserialization since localStorage stores JSON (which doesn't support Date objects natively):

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/services/profileService.ts`

**Passo 22** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend && npm run build 2>&1`

**Passo 23** — `fs_write`

> The STEPS array indexing can return undefined. Quick fix:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/frontend/src/composables/useOnboarding.ts`

**Passo 24** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria/frontend && npm run build 2>&1`

---

[← Voltar aos prompts](../02-features-core.md)

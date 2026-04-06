[← Voltar aos prompts](../06-criacao-estudo-ia.md)

---

# Resposta da IA — Prompt 12
### Criação do Estudo de Uso de IA (Meta-documentação)

> o link nao funcionou pro arquivo docs/tarefas/0-fundacao.md. tem q ser o caminho completo eu imagino

---

**Passo 1** — `execute_bash`

> O prompt da tarefa 0 usa o caminho `docs/tarefas/0-fundacao.md` sem o prefixo `docs/tarefas/` — ele diz `"Execute a tarefa 0: docs/tarefas/0-fundacao.md"`. Deixa eu verificar:

- 🖥️ `grep "fundacao" /home/paulo/dev/work/grupo-6-mentoria/docs/historico-ia/2026-03-`

**Passo 2** — `execute_bash`

> O link está correto no arquivo gerado. O problema é que o MarkText (flatpak) pode não abrir links externos no browser. Deixa eu testar se o link funciona no GitHub — o caminho `frontend/docs/tarefas/0-fundacao.md` existe na branch `main`?

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git show main:frontend/docs/tarefas/`

**Passo 3** — `execute_bash`

> O arquivo existe na `main` e o link está correto: `https://github.com/IA-para-DEVs-SD/grupo-6-mentoria/blob/main/frontend/docs/tarefas/0-fundacao.md`
> 
> O problema é o MarkText — ele não abre links externos clicando. Esses links vão funcionar quando o professor abrir no GitHub (que é onde ele vai ver). Quer testar abrindo direto no browser?

- 🖥️ `xdg-open "https://github.com/IA-para-DEVs-SD/grupo-6-mentoria/blob/main/frontend`

---

[← Voltar aos prompts](../06-criacao-estudo-ia.md)

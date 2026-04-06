[← Voltar aos prompts](../06-criacao-estudo-ia.md)

---

# Resposta da IA — Prompt 3
### Criação do Estudo de Uso de IA (Meta-documentação)

> quero que crie um .md que detalhe isso, meu professor quer um relatorio do uso de IA nesse projeto. Quero que crie de uma forma que de para ver exemplos reais, com links para exemplos reais dos prompt...

---

**Passo 1** — `thinking`

**Passo 2** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git log --oneline --all --decorate 2`

**Passo 3** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git remote get-url origin 2>/dev/nul`

**Passo 4** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git log --oneline --all | grep -i "p`

**Passo 5** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git log --format="%H %s" --author="$`

**Passo 6** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && ls docs/tarefas/ 2>/dev/null; echo "`

**Passo 7** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git show 4be5c2f --stat | tail -5; e`

**Passo 8** — `execute_bash`

- 🖥️ `# Extract specific real prompts from conversations for evidence
sqlite3 /home/pa`

**Passo 9** — `execute_bash`

- 🖥️ `# Extract real prompts from conversation 4 (dark mode + features)
sqlite3 /home/`

**Passo 10** — `execute_bash`

- 🖥️ `# Extract prompts from conversation 5 (evaluation)
sqlite3 /home/paulo/.local/sh`

**Passo 11** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git show 4be5c2f --stat | head -60`

**Passo 12** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && ls docs/prompts_evidencias.md 2>/dev`

**Passo 13** — `fs_write`

> Agora tenho tudo que preciso. Vou criar o relatório.

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/docs/relatorio-uso-ia.md`

**Passo 14** — `thinking`

---

[← Voltar aos prompts](../06-criacao-estudo-ia.md)

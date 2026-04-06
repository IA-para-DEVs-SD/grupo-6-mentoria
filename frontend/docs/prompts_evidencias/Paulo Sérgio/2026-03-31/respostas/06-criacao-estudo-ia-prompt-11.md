[← Voltar aos prompts](../06-criacao-estudo-ia.md)

---

# Resposta da IA — Prompt 11
### Criação do Estudo de Uso de IA (Meta-documentação)

> docs/tarefas/1-login.md. esses .md mencionados no prompt a gente já tem armazenados ne. daria pra colocar link neles também pra o prof ver eles

---

**Passo 1** — `execute_bash`

- 🖥️ `find /home/paulo/dev/work/grupo-6-mentoria -path "*/docs/tarefas/*.md" -o -path `

**Passo 2** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && git log --all --oneline -- frontend/`

**Passo 3** — `fs_write`

> Estão no repo. Vou atualizar o script pra transformar referências a `docs/tarefas/*.md` em links pro GitHub automaticamente:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/scripts/gerar_historico_ia.py`

**Passo 4** — `fs_write`

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/scripts/gerar_historico_ia.py`

**Passo 5** — `fs_write`

> Agora aplico o `linkify` nos prompts:

- 📄 `/home/paulo/dev/work/grupo-6-mentoria/scripts/gerar_historico_ia.py`

**Passo 6** — `execute_bash`

- 🖥️ `cd /home/paulo/dev/work/grupo-6-mentoria && python3 scripts/gerar_historico_ia.p`

**Passo 7** — `execute_bash`

- 🖥️ `grep -n "docs/tarefas" /home/paulo/dev/work/grupo-6-mentoria/docs/historico-ia/2`

**Passo 8** — `execute_bash`

- 🖥️ `flatpak run com.github.marktext.marktext /home/paulo/dev/work/grupo-6-mentoria/d`

---

[← Voltar aos prompts](../06-criacao-estudo-ia.md)

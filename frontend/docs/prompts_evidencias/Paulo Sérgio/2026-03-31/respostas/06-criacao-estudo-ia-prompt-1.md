[← Voltar aos prompts](../06-criacao-estudo-ia.md)

---

# Resposta da IA — Prompt 1
### Criação do Estudo de Uso de IA (Meta-documentação)

> voce conhece esse banco de dados? /home/paulo/.local/share/kiro-cli/data.sqlite3

---

**Passo 1** — `execute_bash`

> Vou dar uma olhada nesse banco de dados para você.

- 🖥️ `file /home/paulo/.local/share/kiro-cli/data.sqlite3 && sqlite3 /home/paulo/.loca`

**Passo 2** — `execute_bash`

- 🖥️ `sqlite3 /home/paulo/.local/share/kiro-cli/data.sqlite3 ".schema"`

**Passo 3** — `execute_bash`

- 🖥️ `sqlite3 /home/paulo/.local/share/kiro-cli/data.sqlite3 "SELECT COUNT(*) FROM his`

---

[← Voltar aos prompts](../06-criacao-estudo-ia.md)

# Relatório — Criação do Estudo de Uso de IA

Registro completo de todos os prompts utilizados na construção do estudo de uso de IA do projeto MentorIA.

## Metadados

| Campo | Valor |
|-------|-------|
| ID da Sessão | `c51c9961-b45d-4686-8fda-2db2c6b465c0` |
| Período | 31/03/2026 21:38 → 31/03/2026 23:56 |
| Total de prompts | 43 |
| Duração | ~2h18min |

---

## Fase 1 — Descoberta e Primeiro Rascunho (21:38–21:48)

| # | Hora | Prompt |
|---|------|--------|
| 1 | 21:38 | voce conhece esse banco de dados? /home/paulo/.local/share/kiro-cli/data.sqlite3 |
| 2 | 21:39 | temos um diretorio dev/work/grupo-6-mentoria. Quero que me de um resumo de tudo que foi feito com kiro nele |
| 3 | 21:42 | quero que crie um .md que detalhe isso, meu professor quer um relatorio do uso de IA nesse projeto. Quero que crie de uma forma que de para ver exemplos reais, com links para exemplos reais dos prompts que eu executei |
| 4 | 21:48 | que ferramenta posso usar que posso navegar entre os .md a partir do sumario? da pra botar uma opcao de voltar em cada md? |
| 5 | 21:49 | sim |

## Fase 2 — Ajustes de Formatação e Navegação (21:54–21:59)

| # | Hora | Prompt |
|---|------|--------|
| 6 | 21:54 | me traga o caminho completo |
| 7 | 21:55 | perai, do terminal voce ja consegue abrir o marktext nesse arquivo ai pra mim? |
| 8 | 21:55 | abriu nada meu nobre |
| 9 | 21:58 | ainda nao ficou legal os prompts reais nao estao sendo apresentados completos, quero ver o paragrafo completo, agora esta aparecendo uma unica linha com scroll |
| 10 | 21:59 | abra pra mim dnv |

## Fase 3 — Enriquecimento do Conteúdo (22:02–22:09)

| # | Hora | Prompt |
|---|------|--------|
| 11 | 22:02 | em cada pagina de prompts coloque um resumo do que foi feito em todos os prompts. Organize isso de uma forma que fique interessante pro meu professor avaliar |
| 12 | 22:04 | sim |
| 13 | 22:07 | docs/tarefas/1-login.md. esses .md mencionados no prompt a gente já tem armazenados ne. daria pra colocar link neles também pra o prof ver eles |
| 14 | 22:08 | sim |
| 15 | 22:09 | o link nao funcionou pro arquivo docs/tarefas/0-fundacao.md. tem q ser o caminho completo eu imagino |

## Fase 4 — Correção de Links (22:10–22:16)

| # | Hora | Prompt |
|---|------|--------|
| 16 | 22:10 | Ah vc colocou o link do github nos arquivos? Por isso ele nao funcionou no marktext? |
| 17 | 22:10 | quero usar os arquivos locais mesmo |
| 18 | 22:11 | sim |
| 19 | 22:12 | ainda nao funcionou o link no marktext. Coloque o caminho absoluto, sem margin pras duvidas |
| 20 | 22:13 | sim |

## Fase 5 — Métricas e Respostas da IA (22:16–22:26)

| # | Hora | Prompt |
|---|------|--------|
| 21 | 22:16 | em cada prompt conseguiriamos colocar mais informações sobre cada prompt ne. Vejo que no banco de dados sqlite tem varias informações legais. Quais informações você acha que ficaria legal colocar, me de sugestoes |
| 22 | 22:17 | Claroo |
| 23 | 22:20 | e a resposta da IA nao conseguiriamos encaixar? Nao precisa ser em cada prompt, mas em um link no prompt principal sabe? Um gatilho pra ir olhar com indice pra voltar |
| 24 | 22:21 | Sim |
| 25 | 22:22 | O link pra ver resposta completa da IA nao ta funcionando. Como voce deixou o link? |
| 26 | 22:24 | sim pode abrir |

## Fase 6 — Migração para Obsidian (22:26–22:32)

| # | Hora | Prompt |
|---|------|--------|
| 27 | 22:26 | para essa documentacao tem um programa melhor que o marktext pra usar? Ta sendo meio ruim navegar entre os arquivos com ele |
| 28 | 22:26 | abra o arquivo readme no obsdian pra mim |
| 29 | 22:27 | deu error |
| 30 | 22:27 | tente denovo |
| 31 | 22:32 | In a few words, summarize our conversation so far. |

## Fase 7 — Correção de Links de Tarefas e Navegação (22:34–22:50)

| # | Hora | Prompt |
|---|------|--------|
| 32 | 22:34 | esse link nao esta funcionando: > Execute a tarefa 1 conforme docs/tarefas/1-login.md. voce criou o link para um arquivo novo que voce criou. Na verdade o arquivo ja existe no repositorio: 1) Procure o arquivo certo, 2) Identifique o padrao e aplique para os demais arquivos da documentação |
| 33 | 22:36 | funcionou agora, mas agora temos que colocar o indice de voltar em cada um dos arquivos. Além disso, para cada arquivo deixe um resumo no começo também informando os pontos fortes de cada tarefa levando em consideracao assertividade com uso da IA |
| 34 | 22:43 | voltar ao indice nao esta funcionando, verifique |
| 35 | 22:46 | .md de tarefas nao tem o voltar |
| 36 | 22:47 | ja tinha o voltar ao indice, mas tem que voltar pro arquivo .md de sessao ne |

## Fase 8 — Identidade e Análise de Qualidade (22:50–23:08)

| # | Hora | Prompt |
|---|------|--------|
| 37 | 22:50 | no readme coloque o Nome do integrante do time, eu sou o Paulo Sérgio Nunes Gonçalves e a resposabilidade dele no projeto |
| 38 | 22:53 | deixe o integrante em forma de tabela tambem e coloque mais informações. Como o numero total de prompts utilizados, e outras informacoes que achar legal colocar |
| 39 | 23:03 | pra cada sessao da pra colocar os pontos fortes e o que pode melhorar no quesito de uso da ia ne. Pra gente usar o estudo pra aprender como melhorar o uso de IA |
| 40 | 23:05 | como voce criou cada ponto forte e pontos de melhoria? Voce analisou com cautela cada sessao? Ate mesmo os arquivos .md de cada tarefa de cada sessao? |
| 41 | 23:06 | Sim, crie uma estrategia de analise .md e mande pra mim aprovar. Só após confirmação seguimos pra implementacao |
| 42 | 23:08 | pode executar |

## Fase 9 — Meta-documentação (23:56)

| # | Hora | Prompt |
|---|------|--------|
| 43 | 23:56 | Precisamos colocar no estudo a criação desse estudo também, voce nao conseguiu identificar porque invés de fazer ele no dir que foi feito o projeto eu usei esse diretorio atual. Pegue do banco essa sessão atual e coloque no estudo também, mais especificamente do começo da criação desse estudo de uso de IA, até a mensagem de agora |

---

## Análise do Processo

### Padrão de Interação

Ciclos curtos e iterativos: usuário pede → IA implementa → usuário valida visualmente → IA corrige.

### Evolução por Fase

| Fase | Foco | Prompts |
|------|------|---------|
| 1 | Descoberta do banco e primeiro .md | 5 |
| 2 | Formatação e abertura no MarkText | 5 |
| 3 | Resumos por sessão e links para tarefas | 5 |
| 4 | Correção de links (GitHub → local → absoluto) | 5 |
| 5 | Métricas do SQLite e respostas da IA | 6 |
| 6 | Migração MarkText → Obsidian | 5 |
| 7 | Links de tarefas e navegação de volta | 5 |
| 8 | Dados do integrante, pontos fortes/fracos, análise rigorosa | 6 |
| 9 | Incluir a própria criação do estudo no estudo | 1 |

### Distribuição dos Prompts

- Confirmações ("sim", "pode", "claro"): ~12 (28%)
- Correções/bugs: ~8 (19%)
- Features/enriquecimento: ~13 (30%)
- Estratégia/planejamento: ~5 (12%)
- Outros (abrir app, caminhos): ~5 (12%)

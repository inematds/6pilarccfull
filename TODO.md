# TODO - 6 Pilares do Claude Code (Full Edition 2026)

**Repo:** git@github.com:inematds/6pilarccfull.git
**Pages:** https://inematds.github.io/6pilarccfull/
**Skill:** formato-curso (usar SEMPRE ao criar paginas HTML)
**Ultima atualizacao:** 2026-03-08

---

## FASE 0 - INFRAESTRUTURA

- [ ] Inicializar git (`git init`)
- [ ] Adicionar remote (`git remote add origin git@github.com:inematds/6pilarccfull.git`)
- [ ] Commit inicial (doc/ + index.html + modulo-1-1.html)
- [ ] Push para main
- [ ] Ativar GitHub Pages (Settings > Pages > Source: main) -- MANUAL

---

## FASE 1 - TRILHA 1: Atalhos e Fundamentos (Emerald)

### Pagina da Trilha
- [ ] `curso/trilha1/index.html` -- Hub com 8 cards de modulo, 48 topicos expansiveis, 8 modais com iframe
  - NOTA: arquivo grande, criar em partes (primeiro esqueleto + cards, depois topicos por modulo)

### Modulos
- [x] `curso/trilha1/modulo-1-1.html` -- Introducao ao Claude Code (6 topicos + exercicio)
- [ ] `curso/trilha1/modulo-1-2.html` -- Comandos Essenciais do Terminal
  - Topicos: /help, /clear, /compact, /cost, /status, Combinando comandos
  - Exercicio: Usar /help, /clear, /compact, /cost numa sessao real
- [ ] `curso/trilha1/modulo-1-3.html` -- Slash Commands Nativos
  - Topicos: /commit, /review, /pr, /init, /doctor, Fluxo completo
  - Exercicio: Executar /commit, /review, /pr num repo de teste
- [ ] `curso/trilha1/modulo-1-4.html` -- Flags de Linha de Comando
  - Topicos: -p (prompt), --model, --resume, --allowedTools, --output-format, Combinando flags
  - Exercicio: Criar 3 comandos com -p, --model, --resume
- [ ] `curso/trilha1/modulo-1-5.html` -- Pipe de Dados e Integracao Unix
  - Topicos: cat | claude, Logs pipe, Multiplos pipes, Redirecionamento, Unix philosophy, Pipelines avancados
  - Exercicio: Criar pipeline cat + grep + claude -p
- [ ] `curso/trilha1/modulo-1-6.html` -- Atalhos de Teclado e Navegacao
  - Topicos: Navegacao sessao, Edicao prompt, Controle execucao, Historico, Multi-line, Atalhos custom
  - Exercicio: Praticar todos os atalhos numa sessao cronometrada
- [ ] `curso/trilha1/modulo-1-7.html` -- Criando Aliases e Scripts
  - Topicos: O que sao aliases, Aliases basicos, Aliases compostos, Scripts bash, Funcoes shell, Organizacao .zshrc
  - Exercicio: Criar 5 aliases no .zshrc/.bashrc
- [ ] `curso/trilha1/modulo-1-8.html` -- Modo Headless e Automacao CLI
  - Topicos: O que e headless, claude -p basico, --output-format json, --allowedTools, Loop bash, CI/CD intro
  - Exercicio: Criar script bash que usa claude -p em loop

### Pos-trilha 1
- [ ] Commit e push trilha 1 completa
- [ ] Testar todos os links e modais

---

## FASE 2 - TRILHA 2: CLAUDE.md e Memoria (Blue)

### Estrutura
- [ ] `curso/trilha2/` -- Criar diretorio
- [ ] `curso/trilha2/index.html` -- Hub com 8 cards

### Modulos
- [ ] `curso/trilha2/modulo-2-1.html` -- O que e CLAUDE.md e Por que Existe
  - Exercicio: Explorar CLAUDE.md de 3 projetos open source
- [ ] `curso/trilha2/modulo-2-2.html` -- Anatomia do CLAUDE.md Perfeito
  - Exercicio: Criar CLAUDE.md completo para projeto pessoal
- [ ] `curso/trilha2/modulo-2-3.html` -- Escopos e Hierarquia de Memoria
  - Exercicio: Criar CLAUDE.md global + projeto + subdiretorio
- [ ] `curso/trilha2/modulo-2-4.html` -- Regras Modulares (.claude/rules/)
  - Exercicio: Criar 3 arquivos de regras modulares
- [ ] `curso/trilha2/modulo-2-5.html` -- Auto-Memory e Persistencia
  - Exercicio: Configurar auto-memory e verificar o que Claude salva
- [ ] `curso/trilha2/modulo-2-6.html` -- /init - Geracao Automatica
  - Exercicio: Rodar /init em 3 projetos e comparar resultados
- [ ] `curso/trilha2/modulo-2-7.html` -- Templates por Stack (Next.js, Python, Go)
  - Exercicio: Criar template CLAUDE.md para 2 stacks diferentes
- [ ] `curso/trilha2/modulo-2-8.html` -- Boas Praticas e Otimizacao (< 200 linhas)
  - Exercicio: Auditar e otimizar CLAUDE.md existente

### Pos-trilha 2
- [ ] Atualizar index.html (T2 disponivel, remover opacity-60)
- [ ] Atualizar nav de trilha1 (link T2 funcional)
- [ ] Commit e push

---

## FASE 3 - TRILHA 3: Workflows (Purple)

### Estrutura
- [ ] `curso/trilha3/` -- Criar diretorio
- [ ] `curso/trilha3/index.html` -- Hub com 9 cards

### Modulos
- [ ] `curso/trilha3/modulo-3-1.html` -- Corrigir um Bug
  - Exercicio: Reproduzir e corrigir bug real num repo de exemplo
- [ ] `curso/trilha3/modulo-3-2.html` -- Construir Feature Nova
  - Exercicio: Implementar feature completa com Plan Mode
- [ ] `curso/trilha3/modulo-3-3.html` -- Refatorar Codigo
  - Exercicio: Refatorar modulo mantendo testes verdes
- [ ] `curso/trilha3/modulo-3-4.html` -- Entender Codebase Novo
  - Exercicio: Clonar repo desconhecido e mapear arquitetura
- [ ] `curso/trilha3/modulo-3-5.html` -- Escrever Testes
  - Exercicio: Aumentar coverage de 40% para 80% num projeto
- [ ] `curso/trilha3/modulo-3-6.html` -- Code Review e Pull Request
  - Exercicio: Fazer review + PR completo com /review e /pr
- [ ] `curso/trilha3/modulo-3-7.html` -- Debug com Logs e Erros
  - Exercicio: Diagnosticar 3 erros diferentes via pipe de logs
- [ ] `curso/trilha3/modulo-3-8.html` -- Migracao Multi-arquivo
  - Exercicio: Executar rename/refactor em 10+ arquivos
- [ ] `curso/trilha3/modulo-3-9.html` -- Agent Teams e Loop Agentico (2026)
  - Exercicio: Configurar agent teams com CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS

### Pos-trilha 3
- [ ] Atualizar index.html (T3 disponivel)
- [ ] Atualizar navs de trilhas anteriores
- [ ] Commit e push

---

## FASE 4 - TRILHA 4: Prompts Estrategicos (Amber)

### Estrutura
- [ ] `curso/trilha4/` -- Criar diretorio
- [ ] `curso/trilha4/index.html` -- Hub com 8 cards

### Modulos
- [ ] `curso/trilha4/modulo-4-1.html` -- Os 5 Prompts Diarios (Daily Drivers)
  - Exercicio: Usar cada um dos 5 prompts numa tarefa real
- [ ] `curso/trilha4/modulo-4-2.html` -- Prompts de Getting Started e Kickoff
  - Exercicio: Iniciar projeto novo usando 95% Confidence + Kickoff
- [ ] `curso/trilha4/modulo-4-3.html` -- Prompts de Building e TDD
  - Exercicio: Construir feature usando Build With Tests prompt
- [ ] `curso/trilha4/modulo-4-4.html` -- Prompts de Debugging e Log Analysis
  - Exercicio: Diagnosticar 3 bugs usando prompts estruturados
- [ ] `curso/trilha4/modulo-4-5.html` -- Prompts de Code Quality e Auditoria
  - Exercicio: Rodar Brutal Audit em codigo proprio e corrigir
- [ ] `curso/trilha4/modulo-4-6.html` -- Prompts de Arquitetura e API Design
  - Exercicio: Projetar API REST completa usando prompts de arquitetura
- [ ] `curso/trilha4/modulo-4-7.html` -- Outcome Delegation (Tecnica 2026)
  - Exercicio: Reescrever 5 prompts imperativos como outcome delegation
- [ ] `curso/trilha4/modulo-4-8.html` -- Verificacao e Prompts Auto-validantes
  - Exercicio: Criar 3 prompts com criterios de verificacao embutidos

### Pos-trilha 4
- [ ] Atualizar index.html (T4 disponivel)
- [ ] Atualizar navs de trilhas anteriores
- [ ] Commit e push

---

## FASE 5 - TRILHA 5: Skills e Plugins (Teal)

### Estrutura
- [ ] `curso/trilha5/` -- Criar diretorio
- [ ] `curso/trilha5/index.html` -- Hub com 8 cards

### Modulos
- [ ] `curso/trilha5/modulo-5-1.html` -- O que sao Skills e Como Funcionam
  - Exercicio: Criar primeira skill seguindo o template padrao
- [ ] `curso/trilha5/modulo-5-2.html` -- Anatomia de uma Skill (Template Completo)
  - Exercicio: Construir skill com Purpose, Steps, Quality Checks
- [ ] `curso/trilha5/modulo-5-3.html` -- Skills Praticas: Screenshot to Website
  - Exercicio: Implementar e testar a skill de screenshot
- [ ] `curso/trilha5/modulo-5-4.html` -- Skills Praticas: Lead Research e Code Review
  - Exercicio: Implementar 2 skills de produtividade
- [ ] `curso/trilha5/modulo-5-5.html` -- Onde Encontrar Skills Prontas
  - Exercicio: Auditar 10 skills de awesome-claude-code
- [ ] `curso/trilha5/modulo-5-6.html` -- Plugins: Arquitetura e Ecossistema (9000+)
  - Exercicio: Instalar e configurar 2 plugins do marketplace
- [ ] `curso/trilha5/modulo-5-7.html` -- Hooks: 12 Eventos do Ciclo de Vida
  - Exercicio: Criar hook PreToolUse + PostToolUse
- [ ] `curso/trilha5/modulo-5-8.html` -- Subagentes e /simplify /batch (2026)
  - Exercicio: Usar /simplify num projeto e analisar resultado

### Pos-trilha 5
- [ ] Atualizar index.html (T5 disponivel)
- [ ] Atualizar navs de trilhas anteriores
- [ ] Commit e push

---

## FASE 6 - TRILHA 6: MCPs e Automacao (Rose)

### Estrutura
- [ ] `curso/trilha6/` -- Criar diretorio
- [ ] `curso/trilha6/index.html` -- Hub com 8 cards

### Modulos
- [ ] `curso/trilha6/modulo-6-1.html` -- O que sao MCPs e o Token Tax
  - Exercicio: Medir overhead de contexto com 0, 2 e 5 MCPs
- [ ] `curso/trilha6/modulo-6-2.html` -- MCP Filesystem e GitHub
  - Exercicio: Instalar ambos e executar tarefa cross-repo
- [ ] `curso/trilha6/modulo-6-3.html` -- MCP Browser e Chrome DevTools
  - Exercicio: Fazer screenshot + scrape de pagina web
- [ ] `curso/trilha6/modulo-6-4.html` -- MCP Database (Postgres/Supabase)
  - Exercicio: Conectar banco, rodar queries, verificar schema
- [ ] `curso/trilha6/modulo-6-5.html` -- MCP Google Sheets e Outros
  - Exercicio: Exportar dados para planilha via MCP
- [ ] `curso/trilha6/modulo-6-6.html` -- Estrategia de Rotacao Ativa
  - Exercicio: Criar tabela pessoal de rotacao por tipo de tarefa
- [ ] `curso/trilha6/modulo-6-7.html` -- Pipelines CI/CD com Claude Headless
  - Exercicio: Criar GitHub Action com claude -p e --allowedTools
- [ ] `curso/trilha6/modulo-6-8.html` -- Claude Cowork e Desktop Agent (2026)
  - Exercicio: Explorar Cowork: scheduling, connectors, skills

### Pos-trilha 6
- [ ] Atualizar index.html (todas as trilhas disponiveis)
- [ ] Atualizar navs de todas as trilhas (links cruzados)
- [ ] Commit e push

---

## FASE 7 - FINALIZACAO

- [ ] Revisao geral de links (nenhum href="#" restante)
- [ ] Testar dark/light mode em todas as paginas
- [ ] Testar responsividade mobile em todas as paginas
- [ ] Verificar todos os modais e iframes
- [ ] Rodar checklist CHECKLIST_REVISAO.md em todas as paginas
- [ ] Adicionar curso ao portal (inema.club) -- courses.ts + Portal.tsx
- [ ] Atualizar relatorio_situacao.md com status final
- [ ] Push final e confirmar GitHub Pages ativo

---

## REGRAS DE EXECUCAO

1. **Sempre usar skill `formato-curso`** ao criar qualquer pagina HTML
2. **6 topicos por modulo** com secoes "O que e / Por que aprender / Conceitos-chave"
3. **Circulos numerados** (1-6), nunca setas
4. **Botoes justify-start** (esquerda), nunca centralizados
5. **Cores por trilha:** T1 Emerald, T2 Blue, T3 Purple, T4 Amber, T5 Teal, T6 Rose
6. **Primary Yellow:** #FACC15 | **INEMA.CLUB links:** text-sky-400
7. **Dark/light mode obrigatorio** com toggle e localStorage
8. **Modais com iframe** apontando para modulo-X-X.html
9. **Exercicio pratico** em cada modulo com passo-a-passo e checklist
10. **Commit por trilha** (nao por modulo individual)
11. **Trilha1/index.html e grande** -- criar esqueleto primeiro, depois preencher topicos em blocos

---

## CONTADORES

| Item | Total | Feito | Falta |
|------|-------|-------|-------|
| Paginas HTML | 62 | 2 | 60 |
| Trilha index | 6 | 0 | 6 |
| Modulos | 49 | 1 | 48 |
| Landing page | 1 | 1 | 0 |
| Topicos | ~294 | 6 | ~288 |
| Exercicios | 49 | 1 | 48 |
| Commits | ~7 | 0 | ~7 |

---

## DOCUMENTOS DE REFERENCIA

| Arquivo | Para que serve |
|---------|---------------|
| `doc/plano_curso_full.md` | Plano completo com todos os modulos e exercicios |
| `doc/relatorio_situacao.md` | Status atual do projeto |
| `doc/6_pilares_claude_code.md` | Conteudo base dos 6 pilares |
| `doc/9_claude_code_workflows.md` | 9 workflows detalhados |
| `doc/claude_ai_skills.md` | Skills e extensibilidade |
| `doc/claude_starter_pack.md` | CLAUDE.md e configuracao |
| `doc/connecting_claude.md` | MCPs e conexoes |
| `doc/executive_prompt_dashboard.md` | Prompts estrategicos |
| `~/.claude/skills/formato-curso/references/MASTER_COMPLETO.md` | Template HTML master |
| `~/.claude/skills/formato-curso/references/CHECKLIST_REVISAO.md` | Checklist de qualidade |

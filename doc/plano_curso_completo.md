# CURSO: Dominando o Claude Code - Os 6 Pilares

**Público-alvo:** Automatizadores de IA, devs e profissionais que querem usar Claude Code como ferramenta de produtividade.

---

## MÓDULO 0 - Introdução
- O que é Claude Code e por que ele muda o jogo
- Diferença entre Claude Chat, Claude Code e Cowork
- Pré-requisitos (conta Anthropic, terminal, Node.js)
- Instalação do Claude Code (`npm install -g @anthropic-ai/claude-code`)
- Primeira sessão: rodando `claude` no terminal

---

## MÓDULO 1 - Atalhos do Claude
*Pilar 1 - Acelere seu uso com shortcuts*

- **Aula 1.1** - Comandos essenciais do terminal (`/help`, `/clear`, `/compact`, `/cost`)
- **Aula 1.2** - Slash commands nativos (`/commit`, `/review`, `/pr`, `/init`)
- **Aula 1.3** - Flags de linha de comando (`-p`, `--model`, `--resume`)
- **Aula 1.4** - Pipe de dados: enviando arquivos e logs pro Claude (`cat | claude -p`)
- **Aula 1.5** - Atalhos de teclado e navegação rápida na sessão
- **Prática:** Criar um alias no shell que roda Claude com suas flags favoritas

---

## MÓDULO 2 - Pacote Inicial (Starter Pack)
*Pilar 2 - Configure Claude pra entender seu projeto em 60 segundos*

- **Aula 2.1** - O que é o `CLAUDE.md` e por que ele existe
- **Aula 2.2** - Anatomia do CLAUDE.md perfeito (stack, comandos, convenções, proibições)
- **Aula 2.3** - Escopos: projeto root vs subdiretório vs global (`~/.claude/CLAUDE.md`)
- **Aula 2.4** - Exemplo real: Next.js SaaS App
- **Aula 2.5** - Exemplo real: Python FastAPI Backend
- **Aula 2.6** - O comando `/init` para gerar CLAUDE.md automaticamente
- **Prática:** Criar o CLAUDE.md de um projeto pessoal do aluno

---

## MÓDULO 3 - 9 Workflows do Claude Code
*Pilar 3 - Os fluxos que cobrem 90% do trabalho real*

- **Aula 3.1** - Workflow 1: Corrigir um Bug (contexto > stack trace > diagnóstico > fix > commit)
- **Aula 3.2** - Workflow 2: Construir Feature Nova (Plan Mode > aprovação > implementação > testes)
- **Aula 3.3** - Workflow 3: Refatorar Código (entender > definir objetivo > diff > testar)
- **Aula 3.4** - Workflow 4: Entender um Codebase Novo (big picture > zoom in > trace flow > /init)
- **Aula 3.5** - Workflow 5: Escrever Testes (gaps > gerar > verificar > coverage)
- **Aula 3.6** - Workflow 6: Code Review (revisão > feedback > re-review)
- **Aula 3.7** - Workflow 7: Criar Pull Request (`/pr` automático)
- **Aula 3.8** - Workflow 8: Debug com Logs e Erros (paste direto ou pipe)
- **Aula 3.9** - Workflow 9: Refatoração Multi-arquivo (plan mode > batches > testes > sweep)
- **Prática:** Pegar um repo open source, clonar, e executar os workflows 4, 1 e 7 em sequência

---

## MÓDULO 4 - Painel Executivo de Prompts
*Pilar 4 - Os prompts que separam amador de operador*

- **Aula 4.1** - Os 5 prompts diários (95% Confidence, Plan Mode, Structured Bug, Brutal Audit, Teach Me)
- **Aula 4.2** - Prompts de Getting Started (kickoff, onboarding)
- **Aula 4.3** - Prompts de Building (feature blueprint, build with tests)
- **Aula 4.4** - Prompts de Debugging (structured bug, log analysis)
- **Aula 4.5** - Prompts de Code Quality (review, refactor guardrails)
- **Aula 4.6** - Prompts de Arquitetura (decisão arquitetural, API design)
- **Aula 4.7** - Prompts de Deployment (prep, CI/CD)
- **Aula 4.8** - Estratégia de uso: quando usar cada prompt
- **Prática:** Montar seu próprio "dashboard de prompts" personalizado pro seu tipo de trabalho

---

## MÓDULO 5 - Habilidades de IA (Skills)
*Pilar 5 - Construa uma vez, use pra sempre*

- **Aula 5.1** - O que são Skills, MCPs e Plugins (e quando usar cada um)
- **Aula 5.2** - Onde as skills vivem (`.claude/commands/`) e como Claude as descobre
- **Aula 5.3** - Template de skill: a estrutura padrão (Purpose > Inputs > Steps > Quality > Output)
- **Aula 5.4** - Skill prática 1: Screenshot to Website
- **Aula 5.5** - Skill prática 2: Lead Research
- **Aula 5.6** - Skill prática 3: Senior Code Review
- **Aula 5.7** - Onde encontrar skills prontas (awesome-claude-code, SkillsMP, SkillHub)
- **Aula 5.8** - Plugins: o game-changer (Supabase, built-ins do Cowork)
- **Aula 5.9** - Sincronizando skills entre Claude Code e Cowork
- **Aula 5.10** - Segurança: o que verificar antes de instalar uma skill
- **Aula 5.11** - Token math: 90% de economia com skills vs re-digitar prompts
- **Prática:** Criar 3 skills personalizadas pro workflow do aluno

---

## MÓDULO 6 - Conectando o Claude (MCPs)
*Pilar 6 - USB ports pro Claude*

- **Aula 6.1** - O que são MCPs e o "Token Tax" (custo de contexto)
- **Aula 6.2** - Framework de decisão: Skill vs MCP
- **Aula 6.3** - MCP #1: Filesystem (acesso a arquivos fora do repo)
- **Aula 6.4** - MCP #2: GitHub (issues, PRs, CI, search)
- **Aula 6.5** - MCP #3: Browser/Chrome DevTools (screenshot, scrape, interação)
- **Aula 6.6** - MCP #4: Database/Supabase (queries, schema, migrations)
- **Aula 6.7** - MCP #5: Google Sheets (leitura/escrita de planilhas)
- **Aula 6.8** - Gerenciando MCPs (`mcp add`, `mcp list`, `mcp remove`)
- **Aula 6.9** - Estratégia de rotação ativa (quais MCPs pra cada tipo de tarefa)
- **Aula 6.10** - Troubleshooting de MCPs
- **Prática:** Instalar Filesystem + GitHub, fazer uma tarefa real conectando os dois

---

## MÓDULO 7 - Projeto Final
*Juntando tudo*

- **Aula 7.1** - Montando seu ambiente completo (CLAUDE.md + skills + MCPs)
- **Aula 7.2** - Projeto prático: Construir uma feature do zero usando todos os 6 pilares
- **Aula 7.3** - Automação pessoal: criando seu "AI OS" com skills customizadas
- **Aula 7.4** - Checklist do Operador: as 10 regras de ouro

---

## Resumo da Estrutura

| Módulo | Aulas | Foco |
|--------|-------|------|
| 0 - Introdução | 5 | Setup |
| 1 - Atalhos | 5 + prática | Velocidade |
| 2 - Starter Pack | 6 + prática | Configuração |
| 3 - Workflows | 9 + prática | Execução |
| 4 - Prompts | 8 + prática | Estratégia |
| 5 - Skills | 11 + prática | Escalabilidade |
| 6 - MCPs | 10 + prática | Integração |
| 7 - Projeto Final | 4 | Consolidação |
| **Total** | **58 aulas** | |

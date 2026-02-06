# Relatório Semanal Técnico - Semana de 03/02 a 06/02/2026 (parcial)

**Organização:** LimaJunior-LegalOps
**Período:** 03/02/2026 - 06/02/2026 (semana em andamento)
**Total de commits:** 50
**Repositórios com atividade:** 7 de 15

---

## Matheus (wansolanso)

**Commits na semana:** 48

### previas-validator
- **Branch(es):** `master`, `fix/manual-operacional-compliance`
- **Commits:** 13
- Merge da branch de compliance operacional para master (`57b0c23`).
- Migração completa do Gmail para Microsoft Graph API (`ed4a6aa`), incluindo melhorias no threading de emails e troca do email padrão (`877ccac`).
- Correção de falsos positivos na validação de documentos (`7660550`, `3fffdf1`), incluindo melhoria na detecção de CONF para ignorar palavras como "confronto" (`a609aef`).
- Suporte a múltiplas URLs do SharePoint em um email (`f89714c`) e URLs com RootFolder e subsites (`e849a01`).
- Envio de notificações de erro para o Discord (`8dd436d`).
- Suporte a múltiplos emails de redirect (`8e01ba2`).
- Correção para evitar criação de múltiplos relatórios no SharePoint (`9f5f804`).
- Correção na classificação de contrarrazões CR-RO/CR-RR (`cd7f3a4`).
- Correção de vários problemas de processamento de emails (`cdf8fcb`).

### limajunior-back
- **Branch(es):** `feat/middleware-refactor`
- **Commits:** 31
- Auditoria de segurança completa do backend, documentada em múltiplas rodadas de revisão (`f462f57`, `32cfea5`, `7736b6a`, `f189c3b`, `0fbe173`, `59fd267`, `c7dd826`, `8d80bd5`).
- **Correções críticas (CRIT):**
  - Middleware stack com correções da auditoria (`e8e4789`).
  - Correção de SQL injection, rate limiting e validação de senha (`d41e5de`).
  - Validação CSRF — CRIT-005 (`15025bd`).
  - Validação de ownership por UUID — CRIT-006 (`180aad7`).
  - Rate limiting por UUID para OTP — CRIT-007 (`d518a4c`).
  - Exigência de senha para leitura admin — CRIT-008 (`525ddd2`).
- **Correções de alta prioridade (HIGH):**
  - Rate limiting e backoff para OTP (`efdd2e7`).
  - Prevenção de timing attack em OTP — HIGH-002 (`b24b056`).
  - Requisitos de senha conforme NIST — HIGH-003 (`75333a5`).
  - Limpeza automática de sessões — HIGH-004 (`a919934`).
  - Validação de secrets na configuração — HIGH-005 (`1a162e2`).
- **Melhorias adicionais:** validação de input (`719fae4`), proteção de endpoint de debug (`568d116`), validador de senha forte (`7eabeba`), depreciação de JWT legado (`2f8c5cd`), retry de email com backoff (`653ce2c`), Dependabot (`b4ffb68`), hardening de Docker (`e7e6d7d`), request ID tracing (`3d1c67f`), health checks de dependências (`0f9828d`).
- **Testes:** infraestrutura pytest (`ba5a0ed`), cobertura abrangente de testes (`7fac91e`), variável SKIP_DB_INIT para testes (`ecc8278`).

### limajunior-base
- **Branch(es):** `master`
- **Commits:** 1
- Merge do PR#1 com suíte completa de testes de API e sistema (`613c886`).

### error-handler-discord
- **Branch(es):** `main`
- **Commits:** 1
- Adição de roteamento de erros baseado em scripts com correspondência fuzzy de canais (`a39a5e4`).

### lj-graphAPI
- **Branch(es):** `main`
- **Commits:** 1
- Adição de documentação da API, testes e melhorias nas rotas de email (`bfaf90d`).

### noticias-automaticas
- **Branch(es):** `main`
- **Commits:** 1
- Criação de scraper para artigos PRO do JOTA Tributos via Playwright (`a6b2b9c`).

---

## Diogo (Polastrine)

**Commits na semana:** 2

### limajunior-back
- **Branch(es):** `feat/middleware-refactor`
- **Commits:** 1
- Commit inicial do backend Python/FastAPI (`eeb69bd`).

### limajunior-front
- **Branch(es):** `main`
- **Commits:** 1
- Commit inicial do frontend React/Vite (`70e10b7`).

---

## PRs da Semana

| PR | Repositório | Título | Status | Autor |
|----|-------------|--------|--------|-------|
| #1 | limajunior-base | feat(tests): add comprehensive API and system test suites | Merged (05/02) | Matheus |

---

## Destaques da Semana

- **Auditoria de segurança massiva no limajunior-back:** 31 commits dedicados a identificar e corrigir vulnerabilidades críticas (SQL injection, CSRF, timing attacks em OTP, rate limiting), com documentação completa de cada rodada de auditoria e implementação de todas as correções até HIGH-005.
- **Estabilização do previas-validator:** migração de Gmail para Microsoft Graph API, correção de falsos positivos, suporte expandido a URLs do SharePoint e integração com Discord para notificações de erro.
- **Início dos projetos limajunior-back e limajunior-front:** Diogo inicializou ambos os repositórios (backend FastAPI e frontend React/Vite), estabelecendo a base para o novo sistema.
- **Novo scraper de notícias:** criação de ferramenta automatizada para captura de artigos PRO do JOTA Tributos, expandindo o monitoramento de informações jurídico-tributárias.
- **Infraestrutura de testes:** suíte completa de testes implementada e integrada via PR no limajunior-base, além de cobertura abrangente adicionada ao limajunior-back durante a auditoria de segurança.

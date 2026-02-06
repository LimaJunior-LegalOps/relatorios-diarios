# Relatório Semanal Técnico - Semana de 20/01 a 26/01/2026

**Organização:** LimaJunior-LegalOps
**Período:** 20/01/2026 - 26/01/2026
**Total de commits:** 23
**Repositórios com atividade:** 3 de 15

---

## Matheus (wansolanso)

**Commits na semana:** 15

### lj-graphAPI
- **Branch(es):** `main`
- **Commits:** 3
- `2b328ba` "feat: API SharePoint com Microsoft Graph"
- `424985a` "feat: add SharePoint sharing URL resolution endpoints"
- `f79362a` "feat: add error reporting and upload endpoints"
- Inicializou o projeto da API de integração com o SharePoint via Microsoft Graph. Implementou endpoints para resolução de URLs de compartilhamento do SharePoint e adicionou endpoints de upload e reporte de erros.

### previas-validator
- **Branch(es):** `fix/manual-operacional-compliance`
- **Commits:** 7
- `e8916a7` "feat: initial implementation of Prévias Validator"
- `573124d` "feat: add OCR support for CONF PDF"
- `496fc03` "fix: improve petition data extraction for ED documents"
- `36794e2` "fix: improve process number validation with correct CNJ algorithm"
- `96ef758` "chore: reduce email polling interval to 1 minute"
- `b82d151` "feat: accept alternative file naming pattern"
- `fbe275e` "fix: identify correct client in multi-defendant cases"
- `b3d7421` "feat: improve email processing and add debug mode"
- Criou o sistema de validação de documentos prévias do zero. Implementou suporte a OCR para PDFs de confirmação, melhorou a extração de dados de petições para documentos ED, corrigiu a validação de números de processo com o algoritmo CNJ correto, reduziu o intervalo de polling de e-mail para 1 minuto, aceitou padrões alternativos de nomenclatura de arquivos, corrigiu a identificação de clientes em casos com múltiplos réus e melhorou o processamento de e-mails com modo debug.

### error-handler-discord
- **Branch(es):** `main`
- **Commits:** 5
- `a8e8661` "feat: initial implementation of Discord error handler bot"
- `4afde8b` "feat: Add automatic channel archiving and config persistence"
- `f35dda6` "docs: add comprehensive README"
- `573bffe` "feat: auto-delete error messages when resolved or ignored"
- Criou o bot de tratamento de erros via Discord. Implementou arquivamento automático de canais e persistência de configuração, adicionou auto-exclusão de mensagens de erro quando resolvidas ou ignoradas, e documentou o projeto com README abrangente.

---

## Diogo (Polastrine)

**Commits na semana:** 8

### lj-graphAPI
- **Branch(es):** `main`
- **Commits:** 5
- `92dd981` "feat: add JWT authentication system"
- `48f1d0d` "feat: add Swagger documentation and integrate auth"
- `6369bce` "refactor: protect routes with JWT and add OpenAPI schemas"
- `40be79c` "deps: upgrade Fastify v5 and add new dependencies"
- `c955c3c` "docs: add project documentation"
- Adicionou o sistema de autenticação JWT à API, integrou documentação Swagger, protegeu rotas com JWT e adicionou schemas OpenAPI, realizou upgrade do Fastify para v5 e documentou o projeto.

### previas-validator
- **Branch(es):** `fix/manual-operacional-compliance`
- **Commits:** 3
- `95911bc` "Adicionar autenticação JWT e documentação Swagger"
- `bb35b2b` "Filtrar apenas e-mails com assunto iniciando em PRÉVIA"
- `5b40f73` "feat: subindo alteracao de ambiente de gmail para outlook atraves do graph-api"
- Adicionou autenticação JWT e documentação Swagger ao validador de prévias, implementou filtro para processar apenas e-mails com assunto iniciando em "PRÉVIA" e migrou o serviço de e-mail do Gmail para Outlook via Graph API.

---

## PRs da Semana

Nenhuma PR aberta, mergeada ou fechada na semana.

## Destaques da Semana

- **Criação do lj-graphAPI:** Matheus inicializou o repositório com integração SharePoint via Microsoft Graph, e Diogo complementou com autenticação JWT, documentação Swagger, schemas OpenAPI e upgrade do Fastify v5. Trabalho colaborativo que resultou numa API robusta e documentada.
- **Criação do previas-validator:** Matheus construiu o sistema de validação de documentos prévias com suporte a OCR, validação CNJ e processamento de e-mails. Diogo adicionou autenticação, filtro de assunto e migrou a integração de e-mail do Gmail para Outlook/Graph API.
- **Criação do error-handler-discord:** Matheus desenvolveu integralmente o bot de tratamento de erros via Discord, com arquivamento automático de canais, persistência de configuração e auto-exclusão de mensagens resolvidas.
- **Semana de alta produtividade:** 23 commits em 3 repositórios, com 3 novos projetos iniciados e funcionais dentro de uma única semana.
- **Padronização de autenticação:** JWT foi implementado tanto no lj-graphAPI quanto no previas-validator, estabelecendo um padrão de segurança consistente entre os serviços.

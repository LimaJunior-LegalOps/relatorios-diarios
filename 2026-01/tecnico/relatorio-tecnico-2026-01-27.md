# Relatório Técnico - 27/01/2026

**Organização:** LimaJunior-LegalOps
**Período:** 27/01/2026 (00:00 - 23:59 BRT)
**Repositórios com atividade:** 2 de 15

---

## Matheus (wansolanso)

### lj-graphAPI

- **Branch:** `main`
- **Commits:**
  - `ca2b525` — feat: add email sending capability via Microsoft Graph Mail API
  - `00d0428` — fix: correct redirect signature for Fastify v5
- **PRs:**
  - PR #1: "feat: transform SharePoint API into general Graph API with Mail support" — MERGED (branch: feature/graph-api-general)

**Resumo:** Matheus expandiu o escopo do repositório lj-graphAPI, transformando-o de uma API exclusiva do SharePoint para uma API geral da Microsoft Graph com suporte a envio de e-mails. O commit principal (`ca2b525`) adiciona a capacidade de envio de e-mails via Microsoft Graph Mail API. Também corrigiu a assinatura de redirect para compatibilidade com o Fastify v5 (`00d0428`). O PR #1 foi aberto e mergeado no mesmo dia, consolidando todas as alterações da branch `feature/graph-api-general` na `main`.

### buscaDOM

- **Branch:** `main`
- **Commits:**
  - `69cfccb` — feat(diario_monitor): implementa serviço automatizado de monitoramento de Diários Oficiais
  - `900fa66` — feat(pdf): implementa download direto SP e geração de relatórios
  - `b5e4768` — feat(search): implementa busca exata com fuzzy matching
  - `e2edf0f` — feat(keywords): adiciona busca por palavras individuais (split_words)
  - `b99bace` — feat(reports): adiciona screenshots do PDF no relatório
  - `36e67a4` — feat(reports): le keywords dos arquivos .txt ao inves do banco
  - `286bd3e` — refactor(search): remove busca por palavras individuais
  - `57980ec` — fix(search): elimina falsos positivos com validação de word boundary
  - `ade5188` — fix(reports): aumenta area de captura e mostra todos os matches
  - `ce0c145` — fix(screenshot): adiciona destaque visual nas keywords encontradas
  - `a172ca1` — config(search): aumenta threshold do fuzzy search para 98%
  - `e154e31` — chore: remove documentação redundante e obsoleta
- **PRs:**
  - PR #1: "feat: serviço automatizado de monitoramento de Diários Oficiais" — ABERTO (branch não especificada; posteriormente fechado em 30/01)

**Resumo:** Dia de intensa atividade no buscaDOM com 12 commits. Matheus implementou um serviço completo de monitoramento automatizado de Diários Oficiais, incluindo: download direto de PDFs do Diário Oficial de SP, busca com fuzzy matching (threshold ajustado para 98%), geração de relatórios com screenshots e destaque visual das keywords encontradas, e leitura de palavras-chave a partir de arquivos `.txt` em vez do banco de dados. Houve iteração significativa no módulo de busca — a funcionalidade de busca por palavras individuais (`split_words`) foi adicionada e posteriormente removida em favor de validação por word boundary para eliminar falsos positivos. Documentação obsoleta foi removida ao final.

---

## Diogo (Polastrine)

### lj-graphAPI

- **Branch:** `main`
- **Commits:**
  - `26d124a` — Merge pull request #1 from LJCF-LegalOps/feature/graph-api-general (merge commit)
- **PRs:** Nenhum aberto por Diogo

**Resumo:** Diogo atuou como revisor e aprovou o merge do PR #1 do Matheus no repositório lj-graphAPI, incorporando a transformação da API do SharePoint em uma API geral da Graph com suporte a envio de e-mails na branch `main`.

---

**PRs do dia:**
- **lj-graphAPI PR #1** (por Matheus): "feat: transform SharePoint API into general Graph API with Mail support" — MERGED em 27/01. Transforma o repositório de API exclusiva do SharePoint para API geral da Microsoft Graph, adicionando envio de e-mails. Mergeado por Diogo.
- **buscaDOM PR #1** (por Matheus): "feat: serviço automatizado de monitoramento de Diários Oficiais" — ABERTO em 27/01. Implementa monitoramento automatizado de Diários Oficiais com download de PDFs, busca fuzzy, e relatórios com screenshots.

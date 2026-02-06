# Relatórios Diários e Semanais — LimaJunior LegalOps

Repositório de relatórios de progresso da equipe de desenvolvimento.

## Estrutura de Pastas

```
YYYY-MM/                        # Pasta mensal (ex: 2026-01, 2026-02)
├── 00-semanal/                 # Relatórios semanais (gerados toda sexta-feira)
│   └── semanal-executivo-YYYY-MM-DD.md
├── tecnico/                    # Relatórios diários técnicos (para o time de dev)
│   └── relatorio-tecnico-YYYY-MM-DD.md
└── executivo/                  # Resumos diários executivos (para gestores)
    └── resumo-executivo-YYYY-MM-DD.md
```

## Tipos de Relatório

| Tipo | Público-alvo | Frequência | Conteúdo |
|------|-------------|------------|----------|
| **Técnico** | Equipe de desenvolvimento | Diário | Commits, branches, PRs, detalhes técnicos por desenvolvedor |
| **Executivo** | Gestores | Diário | Resumo em linguagem acessível, foco em progresso e impacto |
| **Semanal** | Gestores | Sexta-feira | Visão consolidada da semana, próximos passos |

## Navegação

- A pasta `00-semanal` aparece primeiro na listagem por usar o prefixo `00-`, facilitando o acesso rápido aos resumos da semana.
- Dentro de cada mês, os relatórios diários estão separados em `tecnico/` e `executivo/`.
- O nome dos arquivos segue o padrão `YYYY-MM-DD` para ordenação cronológica natural.

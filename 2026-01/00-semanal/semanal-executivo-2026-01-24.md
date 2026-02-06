# Resumo Executivo Semanal - Semana de 20/01 a 26/01/2026

## Visão Geral da Semana

A primeira semana de desenvolvimento foi marcada pela criação de três novos sistemas internos que visam automatizar processos operacionais do escritório. O foco principal foi a construção de uma ferramenta para acessar e gerenciar documentos armazenados no SharePoint, um sistema automatizado de validação de documentos prévias recebidos por e-mail e um canal de notificação de erros via Discord para monitoramento em tempo real. No total, foram realizadas 23 entregas de código entre os dois desenvolvedores, distribuídas em 3 projetos ativos.

---

## Matheus

Matheus liderou a criação dos três novos projetos da semana, sendo responsável pela estrutura inicial de cada um deles. No projeto de integração com o SharePoint, desenvolveu a conexão com a plataforma da Microsoft que permite ao escritório acessar, buscar e enviar documentos de forma automatizada, eliminando a necessidade de acesso manual ao SharePoint para operações rotineiras.

No sistema de validação de prévias, Matheus construiu toda a base do serviço que recebe documentos por e-mail, lê o conteúdo dos PDFs (inclusive com reconhecimento óptico de texto para documentos digitalizados), valida os números de processo conforme o padrão judicial e identifica automaticamente os clientes envolvidos. Esse sistema reduz significativamente o trabalho manual de conferência de documentos pela equipe operacional.

Além disso, criou o sistema de notificação de erros via Discord, que permite à equipe técnica receber alertas automáticos quando algum problema ocorre nos sistemas, com a capacidade de arquivar automaticamente notificações antigas e remover alertas de erros que já foram resolvidos, mantendo o canal de comunicação organizado.

## Diogo

Diogo concentrou seu trabalho na segurança, documentação e melhoria dos sistemas criados na semana. No projeto de integração com o SharePoint, implementou o sistema de controle de acesso que garante que apenas usuários autorizados possam utilizar a ferramenta, além de criar a documentação técnica completa do sistema e atualizar a plataforma para a versão mais recente do servidor.

No sistema de validação de prévias, Diogo adicionou o mesmo controle de acesso seguro, implementou um filtro inteligente que garante que apenas e-mails com assunto relevante (iniciando com "PRÉVIA") sejam processados pelo sistema, evitando o processamento desnecessário de mensagens irrelevantes. Ao final da semana, concluiu a migração do serviço de e-mail do Gmail para o Outlook corporativo, alinhando o sistema com a infraestrutura de e-mail já utilizada pelo escritório.

## Próximos Passos

- Finalização e estabilização dos três sistemas criados na semana, com eventuais ajustes baseados nos primeiros testes em ambiente real.
- Integração entre o sistema de validação de prévias e a ferramenta do SharePoint, permitindo que documentos validados sejam automaticamente armazenados na plataforma do escritório.
- Possível implementação de relatórios automatizados sobre o volume de documentos processados e erros identificados.

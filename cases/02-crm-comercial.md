# CRM comercial e isolamento entre contas

**Frente:** evolução de uma base de CRM e atendimento para rotinas comerciais.

## O problema

Uma operação comercial precisa reunir contatos, carteira, atividades, agenda e documentos. Quando mais de uma conta usa a mesma plataforma, esconder opções na interface é insuficiente: o servidor e o banco também precisam verificar quem pode acessar cada registro.

## A solução trabalhada

Evolução de um portal em React e TypeScript com PostgreSQL/Supabase, incluindo contexto por conta, vínculos de usuários, controles de acesso e ferramentas para o acompanhamento comercial. O trabalho contempla mudanças no modelo de dados e nas integrações que dependem dele.

Outra frente organiza documentos comerciais: a IA auxilia a leitura ou preparação do material, enquanto a revisão humana decide o que será registrado no CRM.

## Decisões técnicas relevantes

- Derivar o acesso do vínculo vigente do usuário com a conta.
- Aplicar isolamento também no banco e nas operações privilegiadas.
- Considerar troca de conta, referências entre registros, arquivos e credenciais.
- Manter credenciais de aplicação no servidor, com armazenamento cifrado.
- Separar geração de documento, revisão, registro e envio.
- Tratar uma visita proposta e uma visita confirmada como estados diferentes.
- Validar leitura e escrita cruzadas entre contas, incluindo os caminhos de recusa.

## O que esta frente demonstra

Evolução de sistemas existentes, modelagem de domínio, autorização, integração entre frontend e backend e preocupação com consistência transacional.

## Estado e limites

O repositório contém a implementação, testes específicos e registros de publicação do painel de contas e das operações humanas. A prontidão de cada automação depende de sua própria validação; liberar um CRM para uso humano não significa liberar automaticamente um agente para enviar mensagens ou executar ações externas.

**Tecnologias:** React, TypeScript, PostgreSQL, Supabase, funções de backend e testes de integração.

[Voltar ao perfil](../README.md)

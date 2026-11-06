# Conteúdo e integrações de produtividade

**Frente:** aplicação para análise de perfis e organização de conteúdo.

## O problema

Análises, ideias e calendários perdem utilidade quando ficam espalhados em ferramentas diferentes. A proposta é estruturar essas informações em uma aplicação navegável e preparar integrações com serviços de IA e de produtividade.

## A solução trabalhada

Uma base em Next.js e TypeScript organiza perfis, análises, concorrentes, ideias e calendário editorial. PostgreSQL e Prisma representam os dados; camadas de serviço encapsulam integrações com OpenAI, Notion e coleta de dados de perfis.

## Decisões técnicas relevantes

- Representar entidades de negócio em um modelo de dados explícito.
- Encapsular provedores externos em serviços separados da interface.
- Validar respostas estruturadas com schemas.
- Identificar quando a aplicação utiliza dados de demonstração.
- Permitir avaliar o fluxo sem depender de todas as integrações externas.
- Manter configuração e credenciais de serviços no backend.

## O que esta frente demonstra

Construção de interfaces e serviços, modelagem relacional, organização de integrações e transformação de saídas de IA em estruturas utilizáveis pela aplicação.

## Estado e limites

A base avaliada contém implementações de serviços e caminhos de demonstração. A autenticação encontrada é um stub de usuário/workspace demo. Algumas integrações dependem de configuração e de conclusão de seus fluxos. Por isso, este estudo apresenta a solução como base funcional/MVP com limitações explícitas, sem afirmar que todos os componentes estejam prontos para produção.

**Tecnologias:** Next.js, TypeScript, React, PostgreSQL, Prisma, Zod, OpenAI e Notion.

[Voltar ao perfil](../README.md)

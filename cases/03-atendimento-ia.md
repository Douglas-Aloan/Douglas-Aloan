# Atendimento com IA e continuidade humana

**Frente:** evolução e sustentação de aplicações de atendimento integradas a CRM.

## O problema

Atendimento por mensagens envolve eventos repetidos, respostas que chegam em momentos diferentes, falhas de integração e necessidade de intervenção da equipe. Uma resposta plausível da IA não garante que a ação comercial esteja autorizada nem que o estado da conversa esteja correto.

## A solução trabalhada

Participação em frentes de atendimento com IA conectadas a caixa de entrada, histórico e rotinas comerciais. O escopo inclui investigação de falhas, melhoria de fluxos, transferência para atendimento humano e validação de regras que controlam as ações do agente.

## Decisões técnicas relevantes

- Diferenciar a mensagem recebida, o processamento da conversa e o efeito externo.
- Considerar duplicidade, retomada e registro do resultado das ações.
- Preservar o contexto necessário para a equipe assumir o atendimento.
- Subordinar ferramentas e ações à autorização e ao estado atual da conversa.
- Separar regras de follow-up da simples geração de texto.
- Usar testes de regressão para comportamentos que já causaram falhas.
- Investigar o caminho completo da mensagem, incluindo integração e persistência.

## O que esta frente demonstra

Integração de serviços, entendimento de sistemas orientados a eventos, sustentação de aplicações e uso de IA com controles operacionais.

## Estado e limites

Há histórico documentado de trabalho em plataformas em produção e fontes locais correspondentes. A atuação varia conforme a frente e inclui bases de terceiros e colaboração com outras pessoas. Este estudo resume padrões de engenharia; não divulga conversas reais, prompts de clientes, configurações de canais ou código operacional. Não atribui ao autor a criação integral dessas plataformas.

**Tecnologias:** TypeScript, React, PostgreSQL/Supabase, APIs HTTP, webhooks e serviços de IA.

[Voltar ao perfil](../README.md)

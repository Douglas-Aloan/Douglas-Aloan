# Dados comerciais e integração com ERP

**Frente:** desenvolvimento e análise de dados para rotinas comerciais e logísticas.

## O problema

Dados de vendas, devoluções, descontos e entregas precisam representar corretamente a operação antes de se tornarem indicadores. Códigos com zeros à esquerda, conversões de unidade e médias calculadas no nível errado podem produzir conclusões incorretas mesmo em uma interface bem apresentada.

## A solução trabalhada

A frente reúne consultas SQL, relatórios parametrizados em Excel e dashboards web. Há uma implementação de API Node.js/Express para leitura de SQL Server e uma camada React para filtros e visualização de descontos. Nos relatórios de histórico comercial, o fluxo conecta parâmetros da planilha, consulta ODBC, tabela de dados e tabela dinâmica.

Também foram construídos protótipos de análise logística com filtros, rankings, distribuição de prazos e acompanhamento de pendências.

## Decisões técnicas relevantes

- Preservar identificadores como texto e definir explicitamente a prioridade dos filtros.
- Separar vendas e devoluções antes de calcular o resultado líquido.
- Recalcular preço médio pela razão entre os totais, evitando médias de médias.
- Tratar conversões inválidas e denominadores nulos sem inventar valores.
- Separar a camada de acesso aos dados dos cálculos e componentes visuais.
- Controlar a ordem de atualização entre consulta, tabela e relatório.

## O que esta frente demonstra

Tradução de regras de negócio em consultas e indicadores; atenção à qualidade dos dados; integração entre ferramentas existentes e aplicações web; validação de casos de borda.

## Estado e limites

O código contempla integração com SQL Server e relatórios entregues. Os protótipos logísticos avaliados utilizam dados simulados em parte de suas versões. A validação de uma planilha ou de uma regra com dados sintéticos não substitui a conciliação dos valores no ERP. Este estudo não apresenta indicadores de ganho financeiro ou de produtividade não mensurados.

**Tecnologias:** SQL Server, SQL, Excel, ODBC, Node.js, Express, React e TypeScript.

[Voltar ao perfil](../README.md)

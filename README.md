# SOBRA

Site de **finanças pessoais** feito em um único arquivo HTML. Controla os gastos, mostra quanto sobra e traz dados do mercado em um só lugar.

> **Projeto criado com ajuda de IA (Claude).** Eu defini as funções que queria, configurei, testei e fui ajustando o resultado.

## O que ele faz

- Controle de gastos e do que sobra, com ciclo mensal ajustável.
- Importação de extrato em PDF (leitura feita no navegador, inclusive PDF com senha).
- Painel de mercado: cotações de ações, bitcoin e ethereum.
- Taxas de CDI, Selic e IPCA e comparação de **renda fixa** e **Tesouro Direto**.
- Radar de ativos e notícias do mercado.
- Tema escuro e claro, perfil de investidor (conservador, moderado ou arrojado).
- Backup: exporta e importa os dados em um arquivo `.json`.

## De onde vêm os dados

| Dado | Fonte |
|---|---|
| CDI, Selic, IPCA | API pública do **Banco Central do Brasil** |
| Ações | [brapi.dev](https://brapi.dev) (precisa de chave gratuita) |
| Criptomoedas | CoinGecko |
| Títulos | Tesouro Direto |
| Gráficos | TradingView |
| Notícias | feeds RSS de portais de economia |

## Tecnologias

HTML, CSS e JavaScript puro, sem framework. Os dados ficam salvos no **navegador** (`localStorage`), então não há servidor nem banco de dados.

## Como usar

1. Baixe o arquivo `index.html`.
2. Abra no navegador.
3. Para ver ações, crie uma chave grátis em brapi.dev e cole no campo de chave do app. A chave fica só no seu navegador e não entra no backup.

## Limitações

- Sem banco de dados: se limpar os dados do navegador, só o backup `.json` recupera.
- Algumas fontes de dados dependem de serviços externos e podem falhar.
- Projeto pessoal, feito para aprender.

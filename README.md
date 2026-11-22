# Sistema modular de análise financeira

> ⚠️ **Estado real do repositório (auditoria de 2026-11-22): não há código executável.**
>
> - `index.html`, `vite.config.js`, `tailwind.config.js` e `postcss.config.js` são arquivos **vazios**.
> - Não existe pasta `src/` nem qualquer arquivo Python ou Power BI.
> - Há apenas `package.json`/`package-lock.json` de um projeto Vite + React chamado `crypto-dashboard`
>   (React 18, D3, axios, react-query, react-simple-maps, Tailwind).
> - `npm run build` falha com `Error: config must export or return an object` (o `vite.config.js` está vazio).

## Proposta original (não implementada)

A descrição original do projeto era um sistema de análise de dados financeiros e criptomoedas com Python e
Power BI: coleta de dados históricos (ex.: Yahoo Finance), engenharia de features (médias móveis),
pré-processamento, modelagem preditiva (ex.: regressão linear) e dashboards no Power BI.
Nada disso está presente no repositório.

## O que dá para fazer hoje

```bash
npm ci --ignore-scripts      # instala as dependências declaradas
npm audit --omit=dev         # auditoria das dependências de produção
```

Não há testes, nem variáveis de ambiente, nem segredos. O CI (`.github/workflows/ci.yml`) só verifica a
instalação e a auditoria das dependências.

## Licença

MIT (arquivo `LICENSE`).

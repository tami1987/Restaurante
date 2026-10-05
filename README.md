# Restaurante

Atividade Avaliativa — Gestão de Projetos de Software (4º ADS)
Professor André Luis Maciel Leme
Instituto Federal de São Paulo — Campus Bragança Paulista

## Integrantes do grupo

- Guilherme Espejo Bueno (@Gui2909)
- Vitor de Oliveira Faria (@Vi1tor)
- Lygio Ursos de Moraes Sobrinho (@Lygiomoraessob)
- Tamiris Carvalho de Oliveira (@tami1987)

## Propósito do projeto

Simular o planejamento e a execução de releases de software usando Git e GitHub, aplicando controle de versão com branches, commits, pull requests, tags e releases.

O projeto é uma miniaplicação web em HTML e JavaScript (sem CSS), com quatro telas: login, erro, administrador e operador.

## Plano de releases

### Release 1 — v0.1.0
- Tela de login construída (`index.html`).
- Ao clicar no botão, exibe a mensagem "em construção" (`working.html`).

### Release 2 — v0.2.0
- Login chama a página do administrador sem validar os campos (`index.html`).
- Página inicial do administrador (`pg001.html`).

### Release 3 — v1.0.0
- Funcionamento completo, validando apenas o campo usuário:
  - usuário em branco → página de erro (`msg.html`);
  - usuário "admin" → tela do administrador (`pg001.html`);
  - qualquer outro valor → tela do operador (`pg002.html`).
- Login atualizado com consistência (`index.html`).
- Página do operador (`pg002.html`).

## Estrutura de arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | Página de login |
| `working.html` | Aviso "em construção" (Release 1) |
| `msg.html` | Mensagem de erro |
| `pg001.html` | Tela do administrador |
| `pg002.html` | Tela do operador |
| `CHANGELOG.md` | Histórico de mudanças por versão |

## Estratégia de branches

| Branch | Uso |
|---|---|
| `main` | Código estável, somente versões liberadas (recebe as tags) |
| `develop` | Integração das funcionalidades em andamento |
| `release1`, `release2`, `release3` | Funcionalidades de cada release |
| `ajustev1`, `correcoes` | Correções de problemas encontrados |

Fluxo: branch de funcionalidade → pull request para `develop` (com revisão de outro membro) → pull request de `develop` para `main` → tag da versão.

## Convenções

- Mensagens de commit curtas e claras, no imperativo (ex.: "Adiciona tela de login").
- Todo pull request deve receber pelo menos um comentário de outro integrante.
- Tags no formato `vMAJOR.MINOR.PATCH` (ex.: `v0.1.0`).

## Como executar

Baixe ou clone o repositório e abra o arquivo `index.html` no navegador.

```bash
git clone https://github.com/tami1987/Restaurante
```

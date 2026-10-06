# Changelog

Todas as mudanças relevantes do projeto *Restaurante* (Sistema Hipotético para Atividade Prática) estão registradas aqui.
O versionamento segue o padrão `MAJOR.MINOR.PATCH`.

## [1.0.1] - 2026-10-05

Correção na tela de login.

### Corrigido
- O campo SENHA do login (`index.html`) passa a ser um campo de senha (`type='password'`), ocultando os caracteres digitados.

## [1.0.0] - 2026-10-05

Release 3: funcionamento completo do login.

### Adicionado
- Tela do operador (`pg002.html`).
- Mensagem de erro "Preencher usuário" (`msg.html`).

### Alterado
- Login (`index.html`) passa a validar o campo usuário:
  - usuário em branco abre a mensagem de erro (`msg.html`);
  - usuário `admin` abre a tela do administrador (`pg001.html`);
  - qualquer outro valor abre a tela do operador (`pg002.html`).
- A senha continua sem validação.

## [0.2.0] - 2026-10-05

Release 2: login abre a tela do administrador.

### Adicionado
- Tela do administrador (`pg001.html`).
- README com integrantes, propósito e plano de releases.

### Alterado
- O botão ENTRAR do login (`index.html`) passa a abrir a tela do administrador, sem validar usuário e senha.

## [0.1.0] - 2026-10-04

Release 1: tela de login.

### Adicionado
- Tela de login (`index.html`).
- Página "Sistema em construção" (`working.html`), aberta pelo botão ENTRAR.
- Logo do campus (`logobra.png`).

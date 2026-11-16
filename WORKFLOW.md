# Como trabalho nesta linha

## Papéis

- **Eu escrevo todo o código**, digitando. O Claude não edita nem commita nos repositórios de código.
- **O Claude guia.** Em cada versão ele responde assim: "arquivo:linha hoje está assim → mude para → por quê (1 a 3 linhas)", e diz como conferir. A teoria não fica na sessão: vai para o livro, que eu dito.
- O Claude pode escrever e commitar documentação neste hub.

## Versões progressivas

Toda issue começa com uma **v0 ingênua**, escrita como um iniciante escreveria. Eu rodo, vejo quebrar, e cada versão seguinte corrige **uma** coisa que eu observei. As issues trazem as versões em checklist. A lista pode mudar no caminho: se quebrar outra coisa, a próxima versão corrige essa.

## GitHub Flow

1. Uma branch por issue: `<tipo>/<n>-<resumo>`, por exemplo `feat/3-live-stream`.
2. Um commit por versão.
3. Um comentário na issue por versão, com o que quebrou, por quê e o que mudou.
4. PR em inglês, merge sem squash, para o histórico de versões ficar no `main`.

## Commits

[Conventional Commits](https://www.conventionalcommits.org/), em inglês. Branches, PRs e código também em inglês.

```
feat(stream): broadcast snapshots over WebSocket

v1 of the live stream: polling made every browser hit the API every 500 ms.
A single WebSocket per client lets the server push each snapshot once.

Refs #3
```

## Repositórios

Ficam todos lado a lado em `C:\Projetos\gclabs\`:

| Pasta | O que é |
| --- | --- |
| `spec-hefesto` | este hub: o livro, as decisões (`docs/adr/`) e este fluxo |
| `tep-ihm-web` | IHM em React |
| `tep-ihm-api` | backend em Node |
| `tep-historian` | historian em Python |
| `tep-ihm` | IHM v1, só para consulta durante o porte |

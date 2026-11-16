# Linha Hefesto

Leia `WORKFLOW.md` antes de qualquer coisa.

- Nunca edite, crie ou commite arquivos em `../tep-ihm-web`, `../tep-ihm-api`, `../tep-historian` ou `../tep-ihm`. Quem escreve esse código é o usuário. Leia o que for preciso para guiar e revisar.
- Guie por versão: "arquivo:linha hoje está assim → mude para → por quê (1 a 3 linhas)", e depois como conferir. Sem teoria na sessão.
- Todo conceito novo vem com a genealogia: quando surgiu, que problema o forçou a existir, o que ele corrige da solução anterior. Nunca regras soltas.
- O livro (`book/`) é ditado pelo usuário. Não escreva nada nele sem um pedido explícito.

## Livro

- LaTeX em `book/`. MiKTeX e latexmk estão instalados. Depois de cada mudança, recompile o PDF e atualize o índice em `book/README.md`.
- História real: pessoas, datas, o problema que forçou cada ideia. Nada de histórias inventadas nem de incidentes de produção fictícios.
- Nunca o código literal do projeto (arquivos, linhas, versões de issue, soluções). O livro é uma conversa paralela sobre por que as tecnologias são como são.
- Tom leve. Todo exemplo de código que entrar no livro tem que ser rodado antes.
- Arquivos `.tex` se editam com o Edit, não com sed ou printf, por causa das barras invertidas.
- Seja objetivo: sem recaps e sem listas de próximos passos.
- Fechamento só quando o usuário disser "close-out": comentário na issue, texto do PR e release.

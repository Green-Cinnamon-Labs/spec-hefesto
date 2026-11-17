# Livro

O livro desta linha: o meu estudo, escrito conforme eu avanço. Sem sumário fixo; os capítulos entram na ordem em que aparecem.

Escrito em inglês. Compilar: `latexmk -pdf main.tex` nesta pasta (gera `main.pdf`).

## Padrão visual

Definido em [hefesto.sty](hefesto.sty).

- Caixa âmbar, `\begin{history}{ano · lugar}`: uma história, com quem, quando e o que forçou a ideia.
- Caixa azul, `\begin{concept}{nome}`: um conceito-chave, com o que é, o que corrige e o que custa.
- Diagramas em TikZ, com uma cor por papel e a mesma em todas as figuras: cinza para a fonte dos dados (planta, aparelho), azul para quem lê (`hf/reader`, setas `hf/ask`), verde para armazenamento (`hf/store`), roxo para o que fica no meio (`hf/bus`, setas `hf/push`) e vermelho para um custo ou uma proibição (`hf/pain`).

## Índice

0. [How to Read This Book](chapters/00-how-to-read.tex): a abordagem (toda ideia com sua genealogia), as duas caixas, a legenda das cores dos diagramas e o mote "fatos exatos, opiniões categóricas".
1. [Who Gets to Talk to the Plant?](chapters/01-who-talks-to-the-plant.tex): do polling do Modbus às assinaturas do OPC UA, de onde vêm DDE, OLE, COM, DCOM e RPC, o historian como único leitor da planta e o barramento publish/subscribe do MQTT.
2. [Talking to the Source](chapters/02-talking-to-the-source.tex): a conexão direta feita do jeito certo. YAGNI (por que não um broker), as camadas de uma conexão OPC UA (canal, sessão, assinatura, item), assinar em vez de perguntar, keep-alive e lifetime, qualidade do dado, reconexão com backoff exponencial e jitter (ALOHAnet, Ethernet, Brooker), republish, o BFF como único cliente da tela, comandos por Write e Call (separação entre comando e consulta) e o ADR (Nygard), inclusive para registrar uma volta atrás.

<p align="center">
  <img src="assets/identidade/Megazord-Toolkit-kit-v1/02-icone-aplicativo/megazord-toolkit-icone-256px.png" width="128" alt="Megazord Toolkit">
</p>

<h1 align="center">Megazord Toolkit</h1>

<p align="center">
  <b>Championship Manager 01/02</b><br>
  <a href="README.en.md">English</a>
</p>

---

**Megazord Toolkit** é um editor para o Championship Manager 01/02 que junta num programa só as funções de várias ferramentas usadas pela comunidade: a edição do jogo em tempo real, a edição do save, o olheiro e a busca dos regens. Ele nasceu do trabalho de reescrever o código do jogo, que permitiu entender como o jogo funciona por dentro (veja a [thread no fórum](https://champman0102.co.uk/viewtopic.php?t=11029)).

**Beta:** faça backup do save antes de usar e relate os bugs [aqui][bugs].

## O que faz

- **Dois modos, as mesmas telas:** edita o jogo enquanto ele roda (lê e grava a memória) ou um `.sav` gravado. Uma barra fixa diz o modo; o que só existe num modo aparece bloqueado no outro, com a explicação.
- **Escolhe o processo do jogo** numa lista, no estilo do Cheat Engine. O executável pode ter qualquer nome.
- **Busca pessoas** por parte do nome, sem diferença de acento ou de maiúscula.
- **Visão de time completa de uma vez:** elenco, comissão técnica, finanças, uniformes e rivais, com as **cores do uniforme** como tema da tela.
- **Ficha da pessoa** com os atributos **como o jogo mostra (1–20)**, com os nomes da tela do jogo.
- **Edição campo a campo:** grava **só o que você mudou**, com a lista "antes → depois" para conferir: contrato completo, clube, estádio, nacionalidades, preferências e a formação preferida do técnico.
- **Na moeda do jogo:** o jogo guarda o dinheiro em libras e mostra na moeda das opções. O editor faz a mesma conta, então você vê e digita em **R$** (ou na moeda que usar).
- **Desfazer:** toda gravação entra no histórico, e o botão **Desfazer** (ou Ctrl+Z) volta a última.
- **Transferências, empréstimos e dispensas**, de jogadores e da comissão técnica.
- **Elenco em grupos:** time principal, reservas e fora do elenco, com ações só num grupo; mudar o jogador de grupo o tira da escalação, como o jogo faz.
- **Liberar jogador na competição:** quando ele "já jogou por outro clube nesta competição", o editor mostra por qual clube ele está registrado e o libera para o clube atual.
- **Olheiro:** busca em todo o banco por posição, idade, CA, PA, nacionalidade, clube e fim do contrato, com **ações em lote** (curar, renovar, pôr à venda…).
- **Regens:** mostra a lista exata dos jogadores que o próprio jogo gerou, com o jogo rodando ou pelo save.
- **Ações rápidas** no elenco e na pessoa: curar lesões, condição, moral, CA/PA +2, renovar ou encerrar contrato.
- Modo claro e escuro, português e inglês.

## Requisitos

- Windows 10 ou 11. O instalador já traz o WebView2; quem usar o zip precisa dele instalado (o Windows 11 já vem com ele).
- Championship Manager 01/02 **3.9.68**, sem patch ou com o patch do NickPatcher (como o CLZ Leagues Patch). Num executável de outra versão, o editor **avisa e não abre**, para não gravar no lugar errado.

## Como usar

1. Instale pelo instalador (`MegazordToolkit-…-setup.exe`) e abra o Megazord Toolkit; ou, com o zip, abra o `MegazordToolkit.exe`.
2. Escolha o processo do jogo (com a carreira carregada) ou um `.sav`.
3. Busque uma pessoa ou escolha um clube na barra lateral. Edite e grave.

## Agradecimentos

O projeto nasceu da admiração pelas ferramentas que mantiveram o jogo vivo por vinte anos. O trabalho dessas pessoas serviu de inspiração e estudo:
- **AnoXic**: CMRTE (Real Time Editor)
- **Graeme Kelly**: SaveGame Editor
- **Michael Nygreen**: CM Scout
- **Yuri Kitashin Jr.**: CMExplorer
- **Dirty Andy**: GPF2 (Generated Players Finder)

---

*Championship Manager* é marca dos seus respectivos donos. Este projeto não tem ligação com a Sports Interactive nem com a Eidos.

[bugs]: https://github.com/CM0102-Rust/Megazord-Toolkit/issues

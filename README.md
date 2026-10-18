<p align="center">
  <img src="cmrte.png" width="128" alt="CMRTE">
</p>

<h1 align="center">CMRTE</h1>

<p align="center">
  <b>Championship Manager 01/02 · Real Time Editor</b><br>
  Rust + Tauri · baseado no CMRTE 0.1.11 de AnoXic · based on AnoXic's CMRTE 0.1.11
</p>

<p align="center"><a href="#português">Português</a> · <a href="#english">English</a></p>

---

## Português

O CMRTE edita o **Championship Manager 01/02 enquanto ele roda**. Ele lê e grava a memória do jogo: jogadores, técnicos, contratos, lesões, clubes e finanças. É uma **reescrita em Rust**, com uma interface nova em **Tauri**, do *CM 01/02 Real Time Editor 0.1.11* de **AnoXic**.

> **Versão alfa.** Use sempre uma cópia do seu save. O editor grava direto no jogo em execução.

### O que faz

- **Escolhe o processo do jogo** numa lista, no estilo do Cheat Engine. Não exige que o executável se chame `cm0102.exe`, então funciona com cópias renomeadas.
- **Busca pessoas** por parte do nome, sem diferença de acento ou de maiúscula.
- **Visão de time completa de uma vez:** elenco, comissão técnica, finanças e dados do clube, com as **cores do uniforme** como tema da tela.
- **Ficha da pessoa** com os atributos **como o jogo mostra (1–20)**. Os intrínsecos são convertidos pelo CA.
- **Edição campo a campo:** grava **só os campos alterados**, com a lista "antes → depois" para conferir.
- **Ações rápidas** no elenco e na pessoa:
  - curar lesões do elenco;
  - condição física, moral e infelicidade;
  - CA/PA +2;
  - renovar ou encerrar contrato;
  - gerar jogador.
- Velocidade do jogo (×0,5 a ×200), modo claro e escuro, português e inglês.

### Requisitos

- Windows 10 ou 11, com o WebView2 (já vem no Windows 11).
- Championship Manager 01/02 **3.9.68**. Os endereços de memória são os dessa versão.

### Como usar

1. Abra o CM 01/02 e carregue a carreira.
2. Abra o `cmrte.exe`, escolha o processo do jogo na lista e clique em **Abrir**.
3. Busque uma pessoa ou escolha um clube na barra lateral. Edite e clique em **Gravar no jogo**.

### Como foi feito

A reescrita foi conferida contra o programa original:
- as rotinas do CMRTE 0.1.11 rodam num emulador e precisam dar **o mesmo resultado byte a byte**;
- um **oráculo** faz a mesma edição no original e na reescrita e compara a memória do jogo.

Os erros do original estão documentados. A interface nova corrige vários deles; por exemplo:
- as datas do contrato não andam mais um dia a cada gravação;
- um contrato não é mais gravado na pessoa errada;
- a data de nascimento vai no dia certo.

### Créditos

- **AnoXic**, autor do *CM 01/02 Real Time Editor*, em que esta reescrita se baseia: <https://champman0102.co.uk/showthread.php?t=8082>.
- **Comunidade do CM 01/02** em [champman0102.co.uk](https://champman0102.co.uk), pelo mapeamento do jogo (endereços, estruturas e o tópico [9CF***]).
- **Ferris**, o caranguejo do Rust, de Karen Rustad Tölva, em domínio público: <https://rustacean.net/>. O ícone é do Lucas.
- *Championship Manager* é marca dos seus respectivos donos. Este projeto não tem ligação com a Sports Interactive nem com a Eidos.

---

## English

CMRTE edits **Championship Manager 01/02 while it runs**. It reads and writes the game's memory: players, staff, contracts, injuries, clubs and finances. It is a **Rust rewrite**, with a new **Tauri** interface, of the *CM 01/02 Real Time Editor 0.1.11* by **AnoXic**.

> **Alpha version.** Always use a copy of your save. The editor writes straight into the running game.

### What it does

- **Picks the game process** from a list, Cheat Engine style. It does not require the executable to be called `cm0102.exe`, so renamed copies work too.
- **Searches people** by part of the name, ignoring accents and case.
- **Full team view in one go:** squad, staff, finances and club data, with the **kit colours** as the screen theme.
- **Person sheet** with attributes **as the game shows them (1–20)**. Intrinsic ones are converted using CA.
- **Field-by-field editing:** writes **only the changed fields**, with a "before → after" list to check.
- **Quick actions** on the squad and on a person:
  - heal squad injuries;
  - condition, morale and unhappiness;
  - CA/PA +2;
  - renew or end a contract;
  - generate a player.
- Game speed (×0.5 to ×200), light and dark mode, Portuguese and English.

### Requirements

- Windows 10 or 11, with WebView2 (built into Windows 11).
- Championship Manager 01/02 **3.9.68**. The memory addresses are those of this version.

### How to use

1. Start CM 01/02 and load your career.
2. Run `cmrte.exe`, pick the game process from the list and click **Open**.
3. Search for a person or pick a club on the side bar. Edit and click **Write to game**.

### How it was made

The rewrite was checked against the original program:
- the CMRTE 0.1.11 routines run in an emulator and must give **the same result byte for byte**;
- an **oracle** makes the same edit with the original and the rewrite and compares the game's memory.

The original's bugs are documented. The new interface fixes several of them; for example:
- contract dates no longer move one day on every save;
- a contract is no longer written to the wrong person;
- the date of birth is written on the right day.

### Credits

- **AnoXic**, author of the *CM 01/02 Real Time Editor* this rewrite is based on: <https://champman0102.co.uk/showthread.php?t=8082>.
- The **CM 01/02 community** at [champman0102.co.uk](https://champman0102.co.uk), for mapping the game (addresses, structures and the [9CF***] thread).
- **Ferris** the Rust crab, by Karen Rustad Tölva, public domain: <https://rustacean.net/>. The icon is Lucas's.
- *Championship Manager* is a trademark of its respective owners. This project is not affiliated with Sports Interactive or Eidos.

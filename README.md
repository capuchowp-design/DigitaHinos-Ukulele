# DigitaHinos Ukulele

Visualizador/compositor MIDI com **ukulele** animado (4 cordas): biblioteca de hinos, escolha de voz, tom automático, acompanhamento (básico ou dedilhado), mão esquerda animada, compositor de tablatura e exportação WAV/MIDI/JSON/PDF. **Todas as funções são gratuitas.**

- Afinações (seletor no app e no editor): **Padrão GCEA** (Sol agudo, reentrante), **Sol grave (low G)** e **Barítono DGBE**.
- Casas 0–15. A pauta é escrita no som real. As vozes fora da extensão (ex.: baixo) são dobradas para a oitava do ukulele.
- Formas de acorde geradas para a afinação escolhida; a mão escolhe a forma mais próxima da melodia.
- Publicação: GitHub Pages (mude `CACHE_NAME` em `sw.js` a cada versão) ou APK pelo workflow `.github/workflows/build-apk.yml` (appId `io.github.capuchowpdesign.digitahinosukulele`).
- Liberação total: `pro-config.js` com `liberarTudo: true` (padrão). O código do modo Pro continua no projeto, desativado.

## Harmonia "Cantoral (livro)"
Em **Harmonia** há a opção *Cantoral (livro)*, que usa as cifras do livro (`hinos/cifras.json`, hino a hino: compasso, tempo, raiz e tipo do acorde). As formas de acorde continuam sendo geradas para a afinação escolhida. Hinos sem cifra no arquivo seguem com a harmonia automática.

## Estilo "Acompanhamento"
Em **Estilo** há: *Fingerstyle · básico*, *Fingerstyle · profissional (dedilhado)* e **Acompanhamento**.
No Acompanhamento o ukulele toca só as cifras e o **soprano toca ao fundo** (flauta, violino, harmônio ou ukulele; campo *Soprano ao fundo*).
- **Ritmo:** *Batida* (golpes ↓ ↑) ou *Dedilhado* (P = 4ª corda, I = 3ª, M = 2ª, A = 1ª).
- **Contagem:** os movimentos seguem a contagem do compasso do hino.
  - *Simples*: um movimento por tempo. Ex.: 6/8 = batida ↓↓↑↓↓↑ e dedilhado P I M A M I; 4/4 = P I M A; 3/4 = P IMA IMA.
  - *Subdividida*: "1 e 2 e 3 e…", o dobro de movimentos.
  - *Mista*: primeira metade do compasso simples e segunda subdividida. Ex.: 4/4 = ↓ ↓ ↑↓↑↓ ↓↑↓↑.

## Correções
- Notas que sumiam na virada do verso para o coro (hinos 6, 41, 61 e outros 30): a numeração das casas de repetição no arquivo começava no 2, e o app pulava o último compasso do verso.
- Cordas soltas: sempre que uma corda solta dá a mesma nota e não está em uso por outra nota, o app usa a corda solta em vez de apertar a casa.

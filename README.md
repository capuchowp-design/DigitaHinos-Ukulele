# Ukulele Bounce

Visualizador/compositor MIDI com **ukulele** animado (4 cordas), derivado do Viola Bounce: biblioteca de hinos, escolha de voz, tom automático, acompanhamento (básico ou dedilhado), mão esquerda animada, compositor de tablatura, exportação WAV/MIDI/JSON/PDF e modo Pro (inclui o PDF da tablatura da versão que está no player).

- Afinações (seletor no app e no editor): **Padrão GCEA** (Sol agudo, reentrante), **Sol grave (low G)** e **Barítono DGBE**.
- Casas 0–15. A pauta é escrita no som real. As vozes que ficam fora da extensão (ex.: baixo) são dobradas para a oitava do ukulele.
- Formas de acorde geradas para a afinação escolhida; a mão escolhe a forma mais próxima da melodia.
- Publicação: GitHub Pages (mude `CACHE_NAME` em `sw.js` a cada versão) ou APK pelo workflow em `.github/workflows/build-apk.yml`.
- Modo Pro: `pro-config.js` usa `app: 'ukulele'`.

# DigitaHinos Ukulele

Visualizador/compositor MIDI com **ukulele** animado (4 cordas): biblioteca de hinos, escolha de voz, tom automático, acompanhamento (básico ou dedilhado), mão esquerda animada, compositor de tablatura e exportação WAV/MIDI/JSON/PDF. **Todas as funções são gratuitas.**

- Afinações (seletor no app e no editor): **Padrão GCEA** (Sol agudo, reentrante), **Sol grave (low G)** e **Barítono DGBE**.
- Casas 0–15. A pauta é escrita no som real. As vozes fora da extensão (ex.: baixo) são dobradas para a oitava do ukulele.
- Formas de acorde geradas para a afinação escolhida; a mão escolhe a forma mais próxima da melodia.
- Publicação: GitHub Pages (mude `CACHE_NAME` em `sw.js` a cada versão) ou APK pelo workflow `.github/workflows/build-apk.yml` (appId `io.github.capuchowpdesign.digitahinosukulele`).
- Liberação total: `pro-config.js` com `liberarTudo: true` (padrão). O código do modo Pro continua no projeto, desativado.

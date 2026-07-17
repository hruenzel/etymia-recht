# Etymia – Rechtstexte

Impressum, Datenschutzerklärung und Nutzungsbedingungen der App **Etymia**,
veröffentlicht über GitHub Pages.

## Nicht von Hand bearbeiten

Diese Dateien sind **generiert**. Die einzige Quelle ist
`lib/services/rechtstexte.dart` im (privaten) App-Repository – so können
App-Text und Website nicht auseinanderlaufen, was im Streitfall die Frage
aufwerfen würde, welche Fassung gilt.

Änderungen laufen immer so:

```
# im App-Repo
dart run tool/webseite_generieren.dart
cp webseite/*.html webseite/robots.txt ../etymia-recht/
# hier
git add -A && git commit -m "Rechtstexte aktualisiert" && git push
```

## Beta-Hinweis

Solange `kBetaNichtIndexieren` im Generator auf `true` steht, tragen alle
Seiten ein `noindex` und die `robots.txt` sperrt Crawler. Grund: In der
Beta steht eine Privatanschrift im Impressum. Vor dem öffentlichen Launch
wird die Anschrift ersetzt und das Flag auf `false` gesetzt.

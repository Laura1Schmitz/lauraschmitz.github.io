# Homepage Laura Schmitz

Statische Seite, kein Build-Schritt, kein Jekyll. Drei Dateien:

```
index.html                     alle Inhalte
assets/style.css               Farben, Schriften, Layout
assets/laura-schmitz.jpg       Portraitfoto (aktuell Platzhalter)
```

## Online stellen (GitHub Pages)

1. Auf github.com ein neues, **öffentliches** Repository anlegen mit dem Namen
   `DEINUSERNAME.github.io` — also z. B. `lauraschmitz.github.io`.
   Der Name entscheidet über die spätere Adresse.
2. Im leeren Repo auf **Add file → Upload files** klicken. Aus dem entpackten
   ZIP `index.html`, `README.md` und den Ordner `assets` hineinziehen —
   Ordner mitsamt Inhalt, GitHub übernimmt die Struktur. Unten auf
   **Commit changes**.
3. **Settings → Pages**: unter „Build and deployment" bei *Source*
   „Deploy from a branch" wählen, Branch `main`, Ordner `/ (root)`, **Save**.
4. Nach ein bis zwei Minuten ist die Seite unter
   `https://DEINUSERNAME.github.io` erreichbar.

Änderungen später: Datei im Repo öffnen, Stiftsymbol, bearbeiten, **Commit**.
Nach etwa einer Minute ist die Seite aktualisiert.

## Foto austauschen

`assets/laura-schmitz.jpg` durch dein eigenes Bild ersetzen — gleicher Dateiname,
Hochformat, mindestens 640 × 800 Pixel. Wenn du einen anderen Dateinamen nimmst,
den Pfad in `index.html` anpassen (Suche nach `laura-schmitz.jpg`).

## Farben ändern

Ganz oben in `assets/style.css` stehen alle Farben an einer Stelle:

| Variable | aktuell | wofür |
|---|---|---|
| `--paper` | `#f1f4ef` | Hintergrund |
| `--band` | `#e3e9df` | abgesetzte Abschnitte |
| `--ink` | `#1b2c28` | Fließtext |
| `--deep` | `#0f4f55` | Überschriften, Links, Buttons |
| `--gold` | `#b07d24` | Akzentlinien, Jahreszahlen, Fotorahmen |

Nur diese Werte tauschen, der Rest zieht automatisch nach. Wenn dir Petrol zu
kühl ist: `--deep: #3c4a6b` (Indigo) oder `--deep: #4a4a3c` (Olive) mit
`--gold: #a8562f` sind gut getestete Alternativen.

## Publikation ergänzen

Einen `<li class="work">`-Block in `index.html` kopieren und ausfüllen:

```html
<li class="work">
  <div class="meta"><span class="venue">Journal</span><span class="year">2027</span></div>
  <div class="body">
    <h4>Titel des Papiers</h4>
    <p class="authors">with Vorname Nachname</p>
    <p class="links"><a href="URL">Working paper</a></p>
  </div>
</li>
```

Optional ein aufklappbares Abstract direkt darunter:

```html
<details><summary>Abstract</summary><p>Text …</p></details>
```

## Noch offen

- CV liegt derzeit auf Google Drive. Sauberer: PDF ins Repo legen
  (z. B. `assets/CV_Laura_Schmitz.pdf`) und den Link in `index.html` ändern.
- Google Scholar, LinkedIn oder Bluesky ergänzen — auskommentiertes Muster
  steht im Hero-Abschnitt der `index.html`.
- Zwei Medienbeiträge („Lasst Kinder und Eltern wählen!", „Lernlücken fürs
  Leben") haben noch keinen Link.
- Affiliation im Hero prüfen.

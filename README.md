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



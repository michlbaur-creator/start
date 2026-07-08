# App-Übersicht „start.mibaso.de" — Veröffentlichen & auf mibaso.de verlinken

Diese Übersichtsseite ist als eigenständige kleine App gebaut — genau wie Flora,
Fauna & Co. (Creme-Stil, offline-fähig, eigenes Icon). Sie liegt im Ordner
`Documents/GitHub/start/`.

---

## Teil 1 — Online stellen (wie deine anderen Apps)

1. **Neues Repo anlegen** (Konto `michlbaur-creator`): in GitHub Desktop
   `Datei → Lokales Repository hinzufügen` → den Ordner **`start`** wählen. Wenn
   gefragt wird, ob ein Repository erstellt werden soll: ja. Dann oben auf
   **„Publish repository"** — Name **`start`**, Häkchen bei „privat" entfernen.
2. **GitHub Pages einschalten:** auf github.com im Repo `start` →
   `Settings → Pages → Source` auf **„GitHub Actions"** stellen (wie bei den
   anderen Häusern). Der mitgelieferte Workflow veröffentlicht dann automatisch.
3. **Domain bei Ionos:** einen neuen **CNAME-Eintrag** anlegen:
   `start` → `michlbaur-creator.github.io` (genau wie bei flora, fauna usw.).
   Die Datei `CNAME` mit `start.mibaso.de` liegt schon im Repo.
4. Nach ein paar Minuten ist **https://start.mibaso.de** live. Bei GitHub unter
   `Settings → Pages` ggf. prüfen, dass die Custom Domain `start.mibaso.de` steht
   und „HTTPS erzwingen" aktiv ist.

Ab jetzt gilt der gewohnte Ablauf: Änderung → Commit → Push → fertig.

---

## Teil 2 — Auf mibaso.de darauf hinweisen

### a) Menüpunkt „Apps" (überall sichtbar, einfachster Schritt)

In WordPress: `Design → Menüs` → **„Individueller Link"** →
URL `https://start.mibaso.de`, Linktext **„Apps"** → „Zum Menü hinzufügen" →
**Menü speichern**.

### b) Hinweisleiste ganz oben (fällt auf, ohne zu stören)

Der fertige Baustein liegt in **`wp-hinweisleiste.html`** — einfach den Inhalt
kopieren und in WordPress in einen **„Custom HTML"-Block** einfügen.

Wo am besten? Am wirkungsvollsten ist die Leiste **oben auf jeder Seite**. Wie das
geht, hängt von deinem WordPress-Theme ab:

- **Einfachste Variante:** Auf der **Startseite** ganz oben einen „Custom HTML"-
  Block einfügen und den Baustein hineinkopieren. (Dann erscheint die Leiste nur
  auf der Startseite — für den Anfang völlig ausreichend.)
- **Auf allen Seiten:** über den Header-Bereich des Themes oder ein kleines
  Plugin wie „WP Header Footer Code". Sag mir, welches Theme du nutzt — dann
  nenne ich dir die genaue Stelle.

> Tipp: Bewusst **kein Pop-up** — das nervt Besucher und bringt Cookie-Fragen mit
> sich. Eine ruhige Leiste plus Menüpunkt wirkt freundlicher und dauerhaft.

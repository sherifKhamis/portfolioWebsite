# Portfolio-Website

Dies ist der Quellcode für meine persönliche Portfolio-Website, erstellt mit Vue.js und Vite.

## Features

-   **Komponentenbasiert:** Gebaut mit Vue.js für eine modulare und wartbare Codebasis.
-   **Modernes Tooling:** Nutzt Vite für eine schnelle Entwicklung und einen optimierten Build-Prozess.
-   **Responsives Design:** (In Arbeit) Passt sich an verschiedene Bildschirmgrößen an.
-   **Einfach anpassbar:** Inhalte und Designdetails können leicht geändert werden.

## Tech-Stack

-   **Framework:** [Vue.js 3](https://vuejs.org/)
-   **Build-Tool:** [Vite](https://vitejs.dev/)
-   **Sprachen:** JavaScript, HTML, CSS

## Projektstruktur

Das Projekt ist in wiederverwendbare Vue-Komponenten unterteilt, um die Organisation und Entwicklung zu vereinfachen.

```
src/
├── assets/
│   └── main.css      # Globale Stile
├── components/
│   ├── About.vue       # "Über mich"-Sektion
│   ├── Contact.vue     # Kontakt-Sektion
│   ├── Experience.vue  # Erfahrungs-Sektion
│   ├── Footer.vue      # Footer
│   ├── Header.vue      # Header & Navigation
│   ├── Intro.vue       # Intro-Sektion
│   └── Projects.vue    # Projekt-Sektion
└── App.vue             # Haupt-Layout-Komponente
└── main.js             # Einstiegspunkt der Anwendung
```

## Setup und lokale Entwicklung

Um das Projekt lokal auszuführen, folgen Sie diesen Schritten:

1.  **Repository klonen:**
    ```bash
    git clone <your-repository-url>
    cd portfolioWebsite
    ```

2.  **Abhängigkeiten installieren:**
    ```bash
    npm install
    ```

3.  **Entwicklungsserver starten:**
    Dieser Befehl startet einen lokalen Server, normalerweise auf `http://localhost:5173`.
    ```bash
    npm run dev
    ```

## Anpassung

### Inhalte ändern

Alle Inhalte sind direkt in den Vue-Komponenten im Verzeichnis `src/components/` hinterlegt. Um Ihre persönlichen Daten einzufügen, bearbeiten Sie einfach den Text in den jeweiligen Dateien.

-   **Intro & Beschreibung:** `src/components/Intro.vue`
-   **Über mich & Skills:** `src/components/About.vue`
-   **Berufserfahrung:** `src/components/Experience.vue`
-   **Projekte:** `src/components/Projects.vue`

### Farben anpassen

Die Hauptfarben sind in den CSS-Stilen der jeweiligen Komponenten definiert. Die primäre Akzentfarbe (aktuell Gold, `#ffca28`) und die Hintergrundfarbe (`#0f0a2f`) können durch Suchen und Ersetzen im gesamten Projekt leicht geändert werden.

## Deployment

Um eine produktionsreife Version der Website zu erstellen, führen Sie den folgenden Befehl aus:

```bash
npm run build
```

Dieser Befehl kompiliert und bündelt alle Dateien in das `dist/`-Verzeichnis. Dieses Verzeichnis kann dann auf einem beliebigen statischen Hosting-Dienst wie Netlify, Vercel oder GitHub Pages bereitgestellt werden.




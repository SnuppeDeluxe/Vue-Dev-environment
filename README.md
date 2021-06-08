# Erstellen und betreiben des VUE-Servers
// Dev-Container startet ohne Fehler, ist aber über Port 3000 nicht erreichbar.
//FEHLERSUCHE LÄUFT NOCH!!!

## Setup
1. im Ordner "setup" den Docker build-Prozess starten
  docker build -t name/vue-setup .

2. in den Ordner "dev" wechseln

3. Container im Interaktiven (-it) Modus starten und nach Fertigstellung (--rm) löschen:
  docker run -it --rm -u $UID:$GID -v ${PWD}:/src name/vue-setup
DEN PUNKT AM ENDE NICHT VERGESSEN!!!

4. Daten entsprechend eingeben.
- JavaScript -> NICHT TypeScript
- NPM als Package-Manager
- Bootstrap Vue als UI-Framework
- Axios
- KEIN Linting Tool
- Test-Framework NONE
- Rendering UNIVERSAL
- Server: Node.js hosting
- GIT verwenden

5. im Ordner "dev" den Docker build-Prozess starten
  docker build -t name/vue-dev .
  
6. "dev/nuxt.config.js" in den Projekt-Ordner kopieren und die vorhandene Datei überschreiben.

7. Docker-Compose-File starten

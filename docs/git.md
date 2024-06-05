# Wichtige Git-Befehle für Lehrlinge

## Grundlegende Git-Befehle

1. **`git init`**
   - Initialisiert ein neues Git-Repository in einem Verzeichnis.
   - **Beispiel:** `git init`

2. **`git clone [URL]`**
   - Klont ein bestehendes Repository von einer URL auf deinen lokalen Rechner.
   - **Beispiel:** `git clone https://github.com/benutzername/repository.git`

3. **`git status`**
   - Zeigt den aktuellen Status des Arbeitsverzeichnisses und des Staging-Bereichs.
   - **Beispiel:** `git status`

4. **`git add [Datei]`**
   - Fügt eine Datei zum Staging-Bereich hinzu.
   - **Beispiel:** `git add datei.txt`
   - Für alle Dateien: `git add .`

5. **`git commit -m "Nachricht"`**
   - Speichert die Änderungen im Staging-Bereich dauerhaft im Repository mit einer Beschreibung.
   - **Beispiel:** `git commit -m "Beschreibung der Änderungen"`

6. **`git push`**
   - Überträgt die lokalen Commits in ein Remote-Repository.
   - **Beispiel:** `git push origin master`

7. **`git pull`**
   - Holt die neuesten Änderungen vom Remote-Repository und integriert sie in die lokale Arbeitskopie.
   - **Beispiel:** `git pull origin master`

8. **`git branch`**
   - Listet alle lokalen Branches auf oder erstellt einen neuen Branch.
   - **Beispiel (Auflisten):** `git branch`
   - **Beispiel (Erstellen):** `git branch neuer-branch`

9. **`git checkout [Branch]`**
   - Wechselt zu einem anderen Branch.
   - **Beispiel:** `git checkout neuer-branch`

10. **`git merge [Branch]`**
    - Integriert die Änderungen eines Branches in den aktuellen Branch.
    - **Beispiel:** `git merge neuer-branch`

## Erweiterte Git-Befehle

1. **`git remote`**
   - Verwalten von Remote-Repositories.
   - **Beispiel:** `git remote add origin https://github.com/benutzername/repository.git`

2. **`git fetch`**
   - Holt die neuesten Änderungen vom Remote-Repository, ohne sie zu integrieren.
   - **Beispiel:** `git fetch origin`

3. **`git log`**
   - Zeigt die Historie der Commits an.
   - **Beispiel:** `git log`

4. **`git reset [--hard] [Commit]`**
   - Setzt den aktuellen Branch auf einen bestimmten Commit zurück.
   - **Beispiel:** `git reset --hard abc1234`

5. **`git stash`**
   - Speichert ungespeicherte Änderungen vorübergehend.
   - **Beispiel:** `git stash`
   - **Wiederherstellen:** `git stash pop`

## Nützliche Links und Referenzen

1. **Offizielle Git-Dokumentation**
   - [Git Documentation](https://git-scm.com/doc)

2. **Pro Git Book** (kostenlos online verfügbar)
   - [Pro Git Book](https://git-scm.com/book/en/v2)

3. **GitHub Learning Lab** (Interaktive Kurse)
   - [GitHub Learning Lab](https://lab.github.com/)

4. **Atlassian Git Tutorial** (Git-Grundlagen und Workflows)
   - [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)

5. **Git Cheat Sheet** (Kurzübersicht der wichtigsten Befehle)
   - [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

Diese Befehle und Ressourcen sollten dir einen guten Start geben, um Git zu lernen und in deiner täglichen Arbeit zu nutzen. Viel Erfolg!
# MeinProjekt
Teilpruefung 3 der Vue.js Schulung

Erstelle eine README-Datei im Wurzelverzeichnis deines lokalen Repositories.
Dokumentiere in der README-Datei die folgenden Punkte:

Die Schritte, die du zum Einrichten des GitHub-Repositorys "MeinProjekt" durchgeführt hast.
Ich habe einen neuen github Account registriert und oben rechts auf das + Symbol geklickt um ein neues Repository zu erstellen.
Dem Verzeichnis habe ich dann den Namen "MeinProjekt" gegeben und habe das Repository öffentlich gestellt, mit dem Klick auf "Create Repository" habe ich es dann final erstellt.

Die Schritte, die du zum Erstellen eines SSH-Schlüssels (falls du keinen bereits hattest) durchgeführt hast.
Als erstes habe ich mir dazu Git Bash runtergeladen da ich mit einem Windows System arbeite.
Mit dem Kommando ssh-keygen -t rsa -b 4096 -C "PetKneter@gmail.com" habe ich einen neuen Schlüssel generiert.
Den generierten Schlüssel habe ich dann unter Settings --> SSH and GPG Keys --> New SSH Key eingefügt und gespeichert.

Die Schritte, die du zum lokalen Klonen des Repositorys, zum Konfigurieren von Git und zum Erstellen der initialen Commits durchgeführt hast.
Um das Repository lokal zu klonen habe ich den Befehl git clone git@github.com:Pruefung/MeinProjekt.git genutzt.
Um auf das Repository zuzugreifen habe ich den Befehl cd MeinProjekt verwendet.
Vor dem initialien Commit habe ich die Befehle git config user.name "Kai Kortsteger" & git config user.email "PetKneter@gmail.com" genutzt der erste Commit wurde dann durch git add main.py & git commit -m "Initialer Commit" durchgeführt.

Die Schritte, die du zum Erstellen des "feature"-Branches, zum Hinzufügen einer neuen Datei zu diesem Branch und zum Committen der Änderungen durchgeführt hast.
Um den Feature Branch zu erstellen nutzte ich den Befehl git checkout -b feature.
Anschließend habe ich die Datei Utils/database.py erstellt dafür nutzte ich git add utils/database.py & git commit -m "Neue Funktion hinzugefügt".
Dann habe ich die Datei bearbeitet und committet, git add main.py & git commit -m "Hauptdatei aktualisiert" sind die Befehle die ich dazu genutzt habe.

Die Schritte, die du zum Mergen des "feature"-Branches in den "master"-Branch und zum Beheben des dabei auftretenden Merge-Konflikts durchgeführt hast.
Um zurück zum "Master" also dem Main branche zu kommen habe ich den Befehl git checkout master genutzt.
Anschließend habe ich die Befehle git add main.py & git commit -m "Hauptdatei aktualisiert" verwendet.
Bei dem Befehl git merge feature kam dann wie erwartet ein Merge Konflikt.
Den Merge Konflikt habe ich gelöst indem ich die main.py Datei von  <<<<<<< HEAD: // =======: >>>>>>> feature: zu print('Hier sind die aktuellen Änderungen der Maindatei') print('Das hier sind meine Änderungen an der Main Datei') angepasst, das hat den Mergekonflikt dann gelöst.
Das Problem ist aufgetreten weil die main.py Datei sowohl in main als auch in feature vorhanden war.
Den Merge habe ich dann mit git add main.py & git commit -m "Merge-Konflikt gelöst"

Zwischen durch und noch einmal am Ende habe ich dann den git push Befehl durchgeführt.


Verwende Screenshots oder Code-Blöcke, um deine Erklärungen zu verdeutlichen.

Die Screenshots lege ich der Zip Datei bei, dort sind die Befehlblöcke vorhanden, außerdem habe ich hoffentlich den Ablauf in der Readme Datei verdeutlichen können.

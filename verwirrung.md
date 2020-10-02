#STAGE & SNAPSHOT
~~~
git status
~~~
Geänderte Datein im Arbeitsverzeichnis anzeigen, welche für nächsten commit bereit gestellt werden
~~~
git add[file]
~~~
Füge die aktuelle Datei dem nächsten commit zu
~~~
git reset [file]
~~~
Erstelle eine andere Datei, während die Änderungen im Arbeitsverzeichnis gespeichert bleiben
~~~
git diff
~~~
Zeige die Unterschiede was geändert, aber noch nicht staged wurde
~~~
git diff --staged
~~~
Zeige die Unterschiede was gestaged wurde aber noch nicht commited
~~~
git commit -m "[deseriptive message]"
~~~
Übernehmen von bereitgestellten Inhalt im neuen commited snapshot

##BRANCH & MERGE
~~~
git branch
~~~
Listen deine branches auf. Ein * wird neben dem aktuellen aktiven branch auftauchen
~~~
git branch [branch-name]
~~~
Erstelle einen neuen branch im aktuellen commit
~~~
git checkout
~~~
Aus dem aktuellen Arbeitsverzeichnis in neuen branch wechseln
~~~
git merge [branch]
~~~
Fügen den abgegebenen branch-Verlauf im  aktuellen branch ein
~~~
git log
~~~
Zeige alle commits im aktuellen branch-Verlauf an


## **Untersuchen & Vergleichen**
### Untersuche logs, diffs und object Informationen

~~~
git log
~~~
Timeline des branches anzeigen

~~~
git log branchB..branchA
~~~
commits in A aber nicht in B
~~~
git log --follow[Datei]
~~~
zeigt commits der Datei (geht über Namensänderungen hinweg)

~~~
git diff branchB...branchA
~~~
was ist in A aber nicht in B

~~~
git show [SHA]
~~~
zeigt jedes Objekt in Git in lesbarem Format

## Pfadänderungen verfolgen
### Versioning, Löschungen und Pfadänderungen
~~~
git rm [Datei]
~~~
Entfernt Datei und staged diese Änderung
~~~
git mv [bestehender Pfad][neuer Pfad]
~~~
Ändere einen Pfad und stage Verschiebung
~~~
git log --stat -M
~~~
Zeigt alle commit logs mit Hervorhebung verschobener Pfade
## Muster Ignorieren
### Ungewollte Stagings und Commits verhindern
~~~
logs/
*.notes
pattern*/
~~~
Speichert Datei mit erwünschtem Mustern als .gitignore mit direkter String-Matches oder wildcard globs.
~~~
git config --global core.excludesfile [Datei]
~~~
Systemwites Ignorationsmuster für alle localen Repositories
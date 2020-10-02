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

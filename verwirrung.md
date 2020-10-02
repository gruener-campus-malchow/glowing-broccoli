<meta charset="utf-8" emacsmode="-*- markdown -*-"><link rel="stylesheet" href="https://casual-effects.com/markdeep/latest/newsmag.css?">

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

<style class="fallback">body{visibility:hidden}</style><script>markdeepOptions={tocStyle:'medium'};</script>
<!-- Markdeep: --><script src="https://casual-effects.com/markdeep/latest/markdeep.min.js?" charset="utf-8"></script>

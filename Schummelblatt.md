## Scheren & Hochdatieren

Hochdaten von einer anderen Deponie empfangen und einheimische Deponien hochdatieren

    git remote add [alias] [url]

füge ein git URL als ein Alias hinzu

    git fetch [alias]

fechte all die Äste von diesem einen Git entlegen

    git merge [alias]/[ast]

verschmelze einen entlegenen Ast in deinen aktuellen Ast um ihn hoch zum Datum zu bringen

    git push [alias] [ast]

übermittle einheimische Astverpflichtungen zu dem entlegenen Deponieast

    git pull

fechte und verschmelze irgendwelche Verpflichtungen von dem verfolgten entlegenen Ast

## Geschichte Neu Schreiben

Äste neuschreiben, Verpflichtungen hochdatieren und Geschichte ausradieren

    git rebase [ast]

aktiviere irgendwelche Verpflichtungen vom aktuellen Ast bevor dem spezifizierten

    git reset --hard [verpflichtung]

Ausradieren des Bühnenareals, Neuschreiben des Arbeitsbaums von spezifizierter Verpflichtung

## Temporäre Verpflichtungen

Temporär modifizierte, verfolgte Dateien speichern, um Äste zu wechseln.

    git stash

spare modifizierte und gebühnte Veränderungen

    git stash list

liste Stapelreihenfolge der versteckten Dateiänderungen

    git stash pop

schreibe arbeitend vom Dach des Versteckungsstapels

    git stash drop

Verwirf die Veränderungen vom Dach des Versteckungsstapels

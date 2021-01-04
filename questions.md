1. Versionshantering innebär att tidigare versioner av dokument, källkodsfiler, program eller webbsidor kan återskapas, och ändringar gjorda i dessa tidigare versioner kan spåras. Möjlighet till parallell utveckling, exempelvis rättning av äldre versioner parallellt med vidareutveckling av nya, är också väsentlig.

2. Slå ihop utvecklingsgrenar. Till exempel används detta när man vill slå ihop koden man har utvecklat i en "feature"-branch med koden i main-branchen.

3. Merge 2 braches
    - `git checkout master` (old) or `git checkout main` (new)
    - `git checkout -b hotfix`
    - `code .`
    - Edit file
    - `git commit -m "Change range from 50 to 25"`
    - `git checkout master` (old) or `git checkout main` (new)
    - `git merge hotfix`
    - `git branch -d hotfix` - Delete branch

4. Apache SVN

5. Git är ett versionshanteringssystem, GitHub är en molnbaserad lösning/tjänst för att spara repon. Så man kan använda Git utan github.

6. En "merge conflict" kan uppstå när två personer editerat samma källkodsfil, speciellt när båda editerat samma rader

7. `git log`

8. Mappen får en dold .git-mapp där i ligger all versionshantering som har med det specifika git repot att göra.

9. För att flera utvecklara kan jobba på separata features/implementeringar samtidigt som main branchen kan hållas ren med fungerande kod.

10. 2 kommandon
    - `git pull` - gör inga änringar på servern då de uppdaterar det lokal repot
    - `git push` - gör änringar på servern då de uppdaterar repot på servern



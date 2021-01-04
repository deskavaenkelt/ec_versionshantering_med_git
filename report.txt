# Rapport

## Beskriv hur du använde dig av Git i inlämningsuppgiften. Vilka Git-kommandon använde du och varför?

Jag använde git för att versionhantera projektet.

## Ej git kommandon
mkdir ec_versionshantering_med_git && cd ec_versionshantering_med_git
echo "# ec_versionshantering_med_git" >> README.md
cat README.md


## git kommandon jag använt
### Skapa git mapp och push till github repo
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/deskavaenkelt/ec_versionshantering_med_git.git
git push -u origin main


### Skapa projektfiler med innehåll i __main__.py
git add .
git status
git push


### Skapa en branch och pusha för att sedan merga på GitHub
git branch important-changes
git checkout important-changes
git status
git add .
git commit -m "Change range from 100 to 50"
git push --set-upstream origin important-changes
git status


### Uppdatera main från GitHub som har senaste versionen
git checkout main
git pull


### Skrev lite kod i main-branch i filen questions.txt stash och flyttar till annan branch samt gör en lokal merge
git stash
git branch questions
git checkout questions
git status
git stash pop
git add .
git commit -m "Answered questions"
git checkout main
git merge questions
git branch -d questions


### Se vilka commits som gjorts
git log


### Clone repo
git clone git@github.com:deskavaenkelt/DevOps-Versionshantering.git
git branch improvements
git checkout improvements
git status
git add .
git commit -m "Change range from 50 to 25"
git push --set-upstream origin improvements


## Vad är fördelen med att använda sig av pull requests när man arbetar i ett team av systemutvecklare?
Man kan granska kod innan den mergas in i master branchen och på så vis säkerställa kodkvalitet.

## Varför är det viktigt att använda sig av versionshantering?
Bland annat om man utvecklar en programvara och av någon anledning får in "breaking changes" så är det ju tex väldigt trevligt att kunna backa till en tidigare fungerande version av koden.
Man kän även jobba på olika features parallelt och integrera allt eftersom.

## Vad var fördelarna i förhållande till inlämningsuppgiften?
Fördelarna är att man kan se hur koden utvecklas över tid och man kan även spåra hur saker skett, samt repitition/träning.

## Vad är fördelarna med versionshantering och Git mer generellt sett?
Fördelen är att flera tusen personer kan jobba på ett projekt parallelt och komma med förbättringar över tid, detta används ju inom open-source.

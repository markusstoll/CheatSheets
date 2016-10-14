** CheatSheat für GIT **



** Erstellen - aus vorhandenen Daten **

cd ~ / my_project_directory
git init
git add.



** ** Clone

git clone ~ / ~ existing_repo / new / repos

git clone [url] und #clone neuen Ordner (url)
git clone git: //host.org/project.git #clone in neuen Ordner "Projekt"
git clone ssh: //user@host.org/project.git

git clone [url] #clone in MyFolder MyFolder

 

** ** Hinzufügen

git add. #add alle aktuellen Änderungen
 git add -v #verbose
 git add. -u #update von allen Änderungen


Fetch Ziehen ** && **

git holen #povlaci alle Brench und / oder Tags (entlang cine "Refs") apdejtuje alle trekovane Brench
Git-Pull-#povlaci alle Änderungen an der Remote-Repository in meinem derzeitigen brench
git pull origin / [brench_name] Änderungen an der Fernbedienung Brench in bestimmten lokalen brench #povlaci



** ** Branching

git remote zeigen Ursprung #list alle Fern Brench
git checkout -b [brench_name] #pravi neue brench und gelangt in den brench
git brench #pokazuje aktuellen brench
git brench -v #pokazuje KoMiT zuletzt die aktuelle Brench
git brench --alle #list alle brench (lokalen und remote)
git push origin [brench_name] #pushuje lokalen brench der Ursprung Remote-Server
git push origin --delete [brench_name] #brise brench mit einem Remote-Server
git brench -d [brench_name] #brise lokale brench
git brench --merged #pokazuje brench ist, die zusammengeführt werden
git brench --no-fusionierten #pokazuje brench die, die noch nicht verschmolzen

Merging ** **

git checkout master #prelazim den Master brench
git merge [brench_name] # merge-mate [brench_name] mit einem Master
git merge origin / Entwicklung uje # merge-devel mit dem Master

** Der Status **


git status #list Dateien, die nicht zusammengeführt werden
git status -UNO #Ich zeigt untracked Dateien (git status --untracked-files = no)
git log #list KoMiT
git ls-Dateien. #list alle Dateien in repou
git ls-Dateien. --ignored --exclude-Standard --others #list git-Dateien ignoriert
git ls-Dateien. --exclude-Standard --others #list untrekovane Dateien
git sauber -FD #brise untracked Dateien


Rückgängig ** **

git reset #undo nach git add.
git reset HEAD ^ --soft #undo nach git commit -m 'update'
git reset HEAD [Dateiname] #undo nach git add [file_name] - rückgängig machen, nachdem eine Datei hinzufügen
git checkout - [Dateiname] #diskarduje Änderungen in einer Datei
git checkout -. #diskarduje Änderungen auf alle Dateien
git revert b53b3c796b6fdd3e7a02e #revert KoMiT - kehrt KoMiT die fälschlicherweise ging (Liste aller KoMiT git log)


** ** Diff

git diff --name-only --diff-filter = U #list alle Dateien, die Konflikte nach dem Stash-a haben
git diff Master Master / Herkunft #razlike zwischen Master und lokaler Herkunft Master
git log --graph --decorate #graph Brench und Ausschüsse
git diff [brench_name] [brench_name] #razlike zwischen zwei Brench
git diff --name-only [brench_name] [brench_name] #razlike zwischen zwei Brench nur Dateien
git diff [local_brench] [Herkunft / remote_brench] #razlika zwischen lokalen und entfernten brench des
git log --oneline [brench_name] ^ Master #razlika KoMiT zwischen zwei brench des
git log --oneline [brench_name] .. Master #isto hundert oben
git diff -R Reverse #diff
    

** ** Stash

git stash #sacuva alle Änderungen und kehrt auf die neueste Version komitovanu
git stash save "Nachricht" #isto hundert und oben ist nur beschreibende Nachricht
git stash Liste bunkern alle #list
git stash gelten Stash @ {0} #vraca Stash @ {0}
git stash Tropfen Stash @ {0} #brise bestimmte Stash (wenn niemand dort nicht den letzten Tupfer ist)
git stash Show -p Stash @ {0} #prikazuje im Versteck sind in
    git diff Stash @ {0} #razlike der Stash


** ** Gitignore #dodavanje gitignore Datei nach Komita

git rm -r --cached.
git add.
git commit -m ".gitignore arbeitet nun"


** Entfernen von Dateien aus Repo **

git rm --cached [Dateiname] #brise Datei aus dem Repository, nicht die physische
git rm -r --cached [DIR_NAME] #brise Verzeichnis im Repository, nicht die physische


** Umbauten **

git tag Veröffentlichungs-0.0.1 -m "Veröffentlichung von Software am 22. Mai" #add bestimmten Tag
git push origin-Freigabe 0.0.1 #pushuje bestimmten Tag auf den Ursprung Fern
# 📝 Git – Cheat Sheet

|Polecenie|Opis|
|---|---|
|`git log`|Pełna historia commitów|
|`git log --oneline --graph --decorate --all`|Skrócona, graficzna historia z gałęziami|
|`git show <commit>`|Szczegóły konkretnego commita|
|`git diff`|Zmiany od ostatniego commita (w plikach)|
|`git diff <commit1> <commit2>`|Różnice między dwoma commitami|

## 🔄 Cofanie i poprawki

| Polecenie                | Opis                                        |
| ------------------------ | ------------------------------------------- |
| `git checkout -- <plik>` | Przywróć plik do stanu z ostatniego commita |
| `git reset HEAD <plik>`  | Cofnij dodanie pliku (`git add`)            |
| `git commit --amend`     | Popraw ostatni commit (np. wiadomość)       |
| `git revert <commit>`    | Utwórz nowy commit cofający zmiany          |

## 🌿 Gałęzie i porządkowanie

| Polecenie                     | Opis                                         |
| ----------------------------- | -------------------------------------------- |
| `git branch`                  | Lista gałęzi lokalnych                       |
| `git branch -a`               | Wszystkie gałęzie (lokalne + zdalne)         |
| `git switch <branch>`         | Zmień gałąź (nowocześniejsze niż `checkout`) |
| `git stash` / `git stash pop` | Schowaj/przywróć lokalne zmiany              |
| `git cherry-pick <commit>`    | Wciągnij pojedynczy commit z innej gałęzi    |
## 🧹 Czyszczenie i diagnostyka

|Polecenie|Opis|
|---|---|
|`git clean -fd`|Usuń nieśledzone pliki i katalogi|
|`git fsck`|Sprawdź spójność repozytorium|
|`git gc`|Optymalizacja repozytorium (garbage collection)|

## 🛰️ Zdalne repo

|Polecenie|Opis|
|---|---|
|`git remote -v`|Lista zdalnych repozytoriów|
|`git fetch --all --prune`|Pobierz wszystko i usuń stare gałęzie|
|`git pull --rebase`|Pobierz zmiany i zastosuj nad swoimi|

## 🔥 Dodatki

|Polecenie|Opis|
|---|---|
|`git blame <plik>`|Pokaż kto zmieniał każdą linię pliku|
|`git shortlog -sn`|Ranking autorów commitów|
|`git reflog`|Historia zmian HEAD/branchy (ratunek przy zgubionych commitach)

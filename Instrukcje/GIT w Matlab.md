1. Instalacja git z [www](https://git-scm.com/downloads)
2. Uruchomienie Git Bash
3. Wykonanie polecenia "ssh-keygen -t ed25519 -C "twoj_email@domena.com""
4. 3 x ENTER, lub wprowadzenie zmian w lokalizacji kluczy na dsyku, i ewentualnie utworzenie hasła ale trzeba będzie je potem podawać.
5. W Matlabie uruchomienie Settings->Version Control->GIT i tam podajemy dane naszego konta w github, klucz prywatny i publiczny.
6. Dodanie klucza publicznego do konta w github. Bez tego nie będzie możliwości wrzucania zmian do zdalnego repozytorium.

# GIT w Git Bash
1. Instalacja git z [www](https://git-scm.com/downloads)
2. Uruchomienie Git Bash
3.  Wykonanie polecenia "ssh-keygen -t ed25519 -C "twoj_email@domena.com"" 
4. 3 x ENTER, lub wprowadzenie zmian w lokalizacji klucza, i ewentualnie utworzenie hasła ale trzeba będzie je potem ciągle podawać.
5. Wykonanie polecenia "eval "$(ssh-agent -s)""
6. Wykonanie polecenia "ssh-add ~/.ssh/id_ed25519" - 
7. Wykonanie polecenia: "cat ~/.ssh/id_ed25519.pub" - dodanie wyświetlonego klucza publicznego do konta w github. Bez tego nie będzie możliwości wrzucania zmian do zdalnego repozytorium.

# Tips and tricks w gitbash
- Wklejanie do Git Bash to SHIFT+INSERT lub prawy przycisk myszki i paste


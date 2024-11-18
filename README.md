# e-doctor


## Opis usługi medycznej oraz dokumentów stworzonych w projekcie.

Proponowaną usługą medyczną w e-doctor są teleporady medyczne realizowane w formie online. W projekcie stworzono analizę ryzyk, plan wdrożenia, a także plan kampanii marketingowej.

## Instrukcje dotyczące pracy z repozytorium, w tym jak pobrać repozytorium, nawigować po gałęziach oraz jak przywrócić wcześniejsze wersje dokumentów.

**git init nazwa_repozytorium** -utworzenie nowego repozytorium

**git status** - sprawdzenie informacji o gałęzi, synchronizacji, zmianach

**git add * ** - dodanie plików do śledzenia

**git commit -a - m "komentarz opisujacy wprowadzone zmiany"** - przesłanie plików do repozytorium z komentarzem

**git touch  nazwa_pliku.txt** - stworzenie nowego pliku txt

**git add nazwa_pliku.txt** - dodanie pliku do śledzenia

**git diff** - polecenie, które porównuje różne wersje pliku i znajduje różnice

przykład **git log**:

b7613c2 2024-01-02 | Dodano nowe pliki (HEAD -> main) [Dominika] 

i wtedy z tym hashem (b7613c2) używa się komendy:

**git checkout b7613c2** - przełączenie się do starszej wersji

**git branch new_branch** - utworzenie nowej gałęzi new_branch

**git checkout new_branch** - przełączenie się na gałąź new_branch

użycie **git checkout nazwa_gałęzi** powoduje przełączenie się do gałezi, do której chcemy inną dołączyć, zazwyczaj jest to gałąź master/main.

 Następnie używamy:
 **git merge nazwa_gałęzi** - aby dołączyć tę gałąź do aktualnie wybranej.


## Informacje o wykorzystanych poleceniach GIT i ich zastosowaniach w projekcie (np. dodawanie plików, tworzenie gałęzi, scalanie).

W projekcie wykorzystano: 

git checkout new_service

git -h

git init new_service - zainicjowanie nowego repozytorium

cd new_service - zmiana katalogu

git commit -a -m "komentarz" -  przesłanie plików do repozytorium z komentarzem

git add * - dodawanie plików nieskomittowanych wcześniej

git push origin tag - dodanie tagu



## Opis napotkanych problemów (jeśli wystąpiły) oraz sposobów, w jaki je rozwiązałeś, np. problemy z konfliktami podczas scalania.

Problemami były:

$ git checkout
fatal: not a git repository (or any of the parent directories): .git

$ git add *
fatal: pathspec '*' did not match any files

$ git tag v1.0 -a "Gotowy plan wdrożenia usługi medycznej"
fatal: Failed to resolve 'Gotowy plan wdrożenia usługi medycznej' as a valid ref.

$ git tag 1.0 -a "Gotowy plan wdrożenia usługi medycznej"
fatal: Failed to resolve 'Gotowy plan wdrożenia usługi medycznej' as a valid ref.

$ git tag 1.0 -m "Gotowy plan wdrożenia usługi medycznej"

$ git remote add origin git@github.com:Fuczaczek/new_service_4807.git

$ git push tag 1.0
fatal: 'tag' does not appear to be a git repository
fatal: Could not read from remote repository.

$ git push tag v1.0
error: src refspec v1.0 does not match any
error: failed to push some refs to 'tag'

Problemy rozwiązywałam przeglądając możliwe rozwiązania na stackoverflow.com oraz metodami prób i błędów. Czasem źle wpisałam nazwę, czasem polecenie - więc próbowałam aż do skutku.





 - 

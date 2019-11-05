# gittesting
Hello there. Tu się bawcie gitem, żeby ogarnąć.
## Po co git?
Żeby się nie musieć wymieniać mailami, czy wiadomościami na messengerze z nowymi wersjami kodu, bo to katorga i nikt tak nigdy nigdzie nie zaszedł.
## Podstawy
### Lokalizacje kodu:
- remote - na serwerze
- lokal - u Ciebie na kompie
### Branche
  Branche służą do wersjonowania kodu. Gdy Tworzymy nowy ficzer nie dodajemy go od razu do "mastera" (głównego brancha) tylko tworzymy osobny branch, gdzie wrzucamy swoje zmiany, tworzymy pull requesta ("żądanie połączenia" naszego brancha do mastera), i po przetestowaniu ich łączymy do mastera.
### "Stany" kodu (wszystkie u Ciebie na kompie):
  - lokalny - u Ciebie na kopmie po pobraniu i zmienieniu czegoś, ale jeszcze nic z gitem nie zrobiłeś
  - sataging area - tu "przenosisz" pliki (lub linijki, ale to na razie olać) poprzez polecenie `git add plik`
  - commited - tu "przenosisz" wszystkie pliki ze staging area poleceniem `git commit -m "Tytuł mojego komita"`
  ![obraz wyjaśniający](https://git-scm.com/figures/18333fig0106-tn.png)
  Historię commitów można przejrzeć polecenie `git log`
  Żeby wrzucić na serwer swoje zmieny używamy `git push -f` (-f bo force)
  
## Skrócony flow dodawania czegoś nowego do projektu
  1. pobierz projekt do folderu na Twoim komputerze `git clone https://github.com/Vulwsztyn/gittesting`
  2. stwórz nowy branch `git checkout -b moj_ficzer` (zmieniasz tym samym branch, na którym się znajdujesz, aby wrócić do mastera użyj `git checkout master`)
  3. napisz swoje zmiany
  4. dodaj je do staging area przy pomocy `git add folder/moj_plik.txt`
  5. skomituj `git commit -m "nowa funkcjonalnosc"`
  6. stwórz pull request

<h1 align="center"> Środowisko pracy informatyka </h1> 

# Opis
To repozytorium zostało stworzone w celu nauki korzystania z Gita za pomocą terminala. Zawiera podstawowe kroki oraz przydatne wskazówki, które pomogą w pracy z repozytoriami.

# Git – Podstawy
1. <b> Tworzenie repozytorium </b></br>
Na początku tworzymy nowe repozytorium na stronie [GitHub](https://github.com)

2. <b> Przemieszczanie się w terminalu </b></br>
Otwieramy terminal i za pomocą komendy ``` cd ``` przechodzimy do katalogu, w którym chcemy sklonować repozytorium. </br>

![Przykład użycia komendy cd](img/cd.jpg?raw=true)

3. <b> Klonowanie repozytorium </b></br> 
Używamy komendy ``` git clone link ``` gdzie "link" to adres URL naszego repozytorium z GitHuba.

![Przykład użycia komendy git clone](img/git_clone.jpg?raw=true)

4. <b> Logowanie do GitHuba </b></br> 
Podczas klonowania może być wymagane logowanie do GitHuba.

5. <b> Praca w repozytorium </b></br> 
Po sklonowaniu repozytorium, przechodzimy do jego folderu ``` cd nazwa_repozytorium ```.

6. <b> Sprawdzanie dostępnych branchy </b></br> 
Za pomocą komendy ``` git branch ``` możemy sprawdzić wszystkie dostępne gałęzie w repozytorium.

7. <b> Tworzenie nowej gałęzi (branch) </b></br> 
``` git branch nazwa ```

8. <b> Usuwanie niepotrzebnych branchy </b></br> 
``` git branch -d nazwa ```

9. <b> Zmiana aktywnej gałęzi </b></br> 
``` git checkout nazwa ```

![Przykład użycia komendy git branch](img/git_branch.jpg?raw=true)

10. <b> Wprowadzanie zmian i commitowanie </b></br> 
Na nowo utworzonej gałęzi wprowadzamy zmiany w plikach. Następnie zapisujemy je w repozytorium lokalnym, używając ``` git commit -m "Opis zmiany" -a ```

11. <b> Wysyłanie zmian do repozytorium na GitHubie </b> 
Aby wysłać zmiany na serwer, używamy ```git push```

</br> UWAGA! Jeśli pojawi się błąd "The current branch nazwa has no upstream branch."
wpisujemy ``` git push --set-upstream origin nazwa ``` 

# Git – Łączenie gałęzi (merge)
Po zakończeniu pracy na danym branchu, możemy połączyć go z główną gałęzią, np. main.

12. <b> Potwierdzenie gałęzi odbiorczej </b></br> 
Upewniamy się, że że wskaźnik HEAD wskazuje na prawidłową gałąź odbiorczą ``` git status ``` </br>
Jeśli wskaźnik HEAD wskazuje na niewłaściwą gałąź, przełącz się na gałąź odbiorczą, np. main, za pomocą komendy ``` git checkout main ```

13. <b> Pobranie najnowszych commitów zdalnych </b></br> 
Upewnij się, że zarówno gałąź odbiorcza, jak i gałąź scalana są zaktualizowane o najnowsze zmiany z repozytorium zdalnego. Wykonaj polecenie ``` git fetch ```. </br>
Po zakończeniu pobierania, upewnij się, że gałąź main zawiera najnowsze zmiany, wykonując ``` git pull ```.

13. <b> Scalanie </b></br> 
Po wykonaniu kroków przygotowawczych możesz przejść do samego scalenia. Użyj komendy ``` git merge nazwa-gałęzi ``` </br>
Gdzie "nazwa-gałęzi" to gałąź, którą chcesz scalić z aktualnie aktywną gałęzią odbiorczą (np. main). </br>

![Przykład przygotowania do scalenia dwóch gałęzi](img/git_merge.jpg?raw=true)


Te przygotowania zapewnią, że scalanie przebiegnie płynnie i bez konfliktów.
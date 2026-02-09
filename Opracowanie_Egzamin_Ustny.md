# Opracowanie na Egzamin Inżynierski (Wersja Ustna)

## Jak korzystać z tego opracowania?
Ten dokument został przygotowany z myślą o egzaminie ustnym. Każde zagadnienie podzielone jest na trzy sekcje:
1. **"Szybki Start" (Co powiedzieć na początku):** Krótka, konkretna definicja, którą możesz wyrecytować, aby zyskać pewność siebie i pokazać, że znasz temat.
2. **"Rozwinięcie" (Kluczowe punkty):** Najważniejsze aspekty, o których warto wspomnieć. Używaj ich jako listy kontrolnej w głowie.
3. **"Mostek" (Jak skręcić z tematu):** Gotowe frazy, które pozwolą Ci płynnie przejść do pokrewnych tematów, jeśli poczujesz, że kończą Ci się pomysły na obecny temat.

---

# MATEMATYKA

## 1. Ekstrema funkcji i gradient, zastosowania w informatyce

### Szybki Start
"Ekstrema funkcji to jej wartości największe (maksima) i najmniejsze (minima). Gradient natomiast to wektor pochodnych cząstkowych, który wskazuje kierunek najszybszego wzrostu funkcji. W informatyce te pojęcia są fundamentem optymalizacji, szczególnie w uczeniu maszynowym."

### Rozwinięcie
*   **Warunki:** Aby istniało ekstremum, pochodna (lub gradient) musi być równa zero (warunek konieczny). Aby potwierdzić, czy to minimum czy maksimum, badamy drugą pochodną (lub macierz Hessego).
*   **Gradient:** Wskazuje "pod górę". Jeśli chcemy coś zminimalizować (np. błąd), idziemy w stronę przeciwną do gradientu.
*   **Zastosowanie:** Metoda **Gradient Descent** (spadek gradientu) – używana do trenowania sieci neuronowych poprzez minimalizację funkcji kosztu.

### Mostek
"Mówiąc o minimalizacji błędu w uczeniu maszynowym, warto wspomnieć, że gradienty wykorzystuje się też w grafice komputerowej, np. do wykrywania krawędzi na obrazach (operator Sobela)."

---

## 2. Wielomian i szereg Taylora funkcji rzeczywistej

### Szybki Start
"Szereg Taylora to sposób na przybliżenie skomplikowanej funkcji (np. sinus czy logarytm) za pomocą prostego wielomianu. Idea polega na tym, że w otoczeniu konkretnego punktu funkcja zachowuje się podobnie do sumy swoich pochodnych."

### Rozwinięcie
*   **Wzór:** Wielomian składa się z wartości funkcji w punkcie oraz kolejnych pochodnych dzielonych przez silnię.
*   **Szereg Maclaurina:** To po prostu szereg Taylora, ale rozwijany w punkcie zero (najczęstszy przypadek).
*   **Zastosowanie:** Komputery nie znają "sinusa" – one obliczają go właśnie za pomocą kilku pierwszych wyrazów szeregu Taylora, bo dla procesora dodawanie i mnożenie jest najszybsze.

### Mostek
"Aproksymacja Taylora jest kluczowa w metodach numerycznych. Jeśli potrzebujemy jeszcze większej precyzji w obliczeniach inżynierskich, często przechodzimy do rozwiązywania układów równań liniowych..."

---

## 3. Układy równań liniowych: metody i liczba rozwiązań

### Szybki Start
"Układ równań liniowych to zestaw równań, które musimy spełnić jednocześnie. W informatyce reprezentujemy je macierzowo jako $Ax = b$. Układ może mieć dokładnie jedno rozwiązanie, nieskończenie wiele lub nie mieć go wcale."

### Rozwinięcie
*   **Liczba rozwiązań:** Zależy od rzędu macierzy (Twierdzenie Kroneckera-Capellego). Jeśli rząd macierzy głównej jest równy rzędowi rozszerzonej i liczbie niewiadomych – mamy jedno rozwiązanie.
*   **Metody:** 
    *   **Dokładne:** Metoda Gaussa (eliminacja zmiennych), wzory Cramera (wyznaczniki).
    *   **Iteracyjne:** Metoda Jacobiego (używana przy bardzo dużych danych, gdzie Gauss byłby za wolny).
*   **Zastosowanie:** Grafika 3D (przekształcenia widoku), kryptografia, analiza sieci elektrycznych.

### Mostek
"Operacje na macierzach w układach równań są ściśle powiązane z pojęciem wartości własnych, które mówią nam o charakterystyce danej macierzy."

---

## 4. Wartości własne macierzy i ich zastosowanie

### Szybki Start
"Wartość własna to taka liczba $\lambda$, dla której przekształcenie macierzowe wektora daje ten sam wektor, tylko przeskalowany. Mówiąc prościej: to 'charakterystyczne' liczby macierzy, które nie zmieniają kierunku pewnych wektorów."

### Rozwinięcie
*   **Równanie:** Szukamy ich rozwiązując równanie charakterystyczne $det(A - \lambda I) = 0$.
*   **Zastosowanie 1: Google PageRank.** Algorytm ocenia ważność stron internetowych, szukając dominującej wartości własnej macierzy linków.
*   **Zastosowanie 2: PCA (Analiza Składowych Głównych).** Redukcja wymiarowości danych – odrzucamy te kierunki (wektory własne), które mają małe wartości własne, bo niosą mało informacji.

### Mostek
"Wartości własne pomagają nam rozumieć strukturę danych, podobnie jak grafy pomagają nam modelować relacje między obiektami."

---

## 5. Grafy i ich typy, metody reprezentacji

### Szybki Start
"Graf to struktura składająca się z wierzchołków i krawędzi łączących te wierzchołki. To najbardziej uniwersalny sposób modelowania relacji w informatyce – od sieci społecznościowych po mapy drogowe."

### Rozwinięcie
*   **Typy:** Skierowane (strzałki), nieskierowane, ważone (krawędzie mają 'koszt'), spójne, cykliczne/acykliczne (np. drzewa).
*   **Reprezentacja:**
    *   **Macierz sąsiedztwa:** Tabela 0/1. Szybka do sprawdzania połączeń, ale zajmuje dużo miejsca ($n^2$).
    *   **Lista sąsiedztwa:** Dla każdego wierzchołka lista jego sąsiadów. Oszczędna dla grafów rzadkich.
*   **Zastosowanie:** Algorytmy GPS, analiza sieci, planowanie zadań.

### Mostek
"Grafy są graficzną reprezentacją relacji binarnych, które są bardziej ogólnym pojęciem matematycznym."

---

# BAZY DANYCH

## 11. Podstawowe cechy relacyjnych baz danych

### Szybki Start
"Relacyjne bazy danych opierają się na modelu tabelarycznym, gdzie dane są zorganizowane w relacje (tabele). Ich najważniejszą cechą jest dbałość o spójność danych, co opisuje akronim ACID."

### Rozwinięcie
*   **ACID:** 
    *   **Atomowość:** Transakcja wykonuje się w całości albo wcale.
    *   **Spójność:** Po transakcji baza jest w poprawnym stanie.
    *   **Izolacja:** Transakcje nie przeszkadzają sobie nawzajem.
    *   **Trwałość:** Raz zapisane dane nie znikną (np. przy awarii zasilania).
*   **Relacje:** Tabele łączą się za pomocą kluczy obcych (Foreign Keys), co pozwala unikać powtarzania danych (redundancji).

### Mostek
"Aby poprawnie zaprojektować takie tabele, musimy najpierw stworzyć model teoretyczny, czyli diagram związków encji (ERD)."

---

## 12. Diagramy związków encji (ERD) i zasady projektowania

### Szybki Start
"Diagram ERD to graficzny plan bazy danych. Składa się z encji (obiektów, np. 'Klient'), atrybutów (cech, np. 'Nazwisko') oraz związków (relacji, np. 'Klient składa Zamówienie')."

### Rozwinięcie
*   **Klucze:** Każda encja musi mieć Klucz Główny (Primary Key), który jednoznacznie ją identyfikuje.
*   **Liczność relacji:** 1:1 (jeden do jednego), 1:N (jeden do wielu – najczęstsza), M:N (wiele do wielu – wymaga tabeli pośredniczącej).
*   **Normalizacja:** Proces porządkowania tabel (np. 1NF, 2NF, 3NF), aby wyeliminować błędy i powtarzanie informacji.

### Mostek
"Dobrze zaprojektowana baza to połowa sukcesu, ale w praktyce musi ona obsługiwać wielu użytkowników naraz, co wymaga mechanizmów współbieżności."

---

## 13. Mechanizm współbieżności w DBMS

### Szybki Start
"Współbieżność pozwala wielu użytkownikom pracować na tej samej bazie w tym samym czasie bez niszczenia sobie nawzajem danych. Głównym narzędziem są tutaj transakcje i blokady."

### Rozwinięcie
*   **Problemy bez kontroli:** "Brudny odczyt" (czytanie danych, które zaraz mogą zostać wycofane) lub "Utracona aktualizacja" (dwie osoby zmieniają to samo, wygrywa ostatnia).
*   **Blokady (Locks):** Baza może zablokować wiersz na czas zapisu, żeby nikt inny go nie zmienił.
*   **Poziomy izolacji:** Możemy ustawić, jak bardzo restrykcyjna ma być baza (np. 'Read Committed' vs 'Serializable').

### Mostek
"Wszystkie te operacje – od tworzenia tabel po zarządzanie transakcjami – wykonujemy za pomocą języka SQL."

---

## 14. Podstawowe obiekty i konstrukcje języka SQL

### Szybki Start
"SQL to standardowy język do komunikacji z bazą danych. Dzieli się na kilka podgrup, z których najważniejsze to DDL (definiowanie struktury) i DML (manipulowanie danymi)."

### Rozwinięcie
*   **DDL (Data Definition):** `CREATE`, `ALTER`, `DROP` (tworzenie tabel).
*   **DML (Data Manipulation):** `SELECT`, `INSERT`, `UPDATE`, `DELETE` (praca na danych).
*   **Złączenia (JOIN):** Kluczowa operacja łącząca dane z wielu tabel (np. `INNER JOIN`, `LEFT JOIN`).
*   **Agregacja:** Funkcje typu `SUM`, `AVG`, `COUNT` używane z klauzulą `GROUP BY`.

### Mostek
"Samo napisanie zapytania to nie wszystko – przy dużych bazach musimy zadbać o to, by działało ono szybko, czyli o optymalizację."

---

## 15. Optymalizacja zapytań i indeksy

### Szybki Start
"Optymalizacja polega na takim sformułowaniu zapytania i struktury bazy, aby czas odpowiedzi był jak najkrótszy. Najpotężniejszym narzędziem optymalizacji są indeksy."

### Rozwinięcie
*   **Indeksy:** Działają jak skorowidz w książce. Zamiast przeszukiwać całą tabelę (Full Table Scan), baza od razu wie, gdzie jest szukany rekord.
*   **Typy indeksów:** B-drzewa (najczęstsze, do zakresów) i Hash (do konkretnych wartości).
*   **Zasady:** Indeksujemy kolumny często używane w `WHERE` i `JOIN`, ale nie przesadzamy, bo indeksy spowalniają zapis (`INSERT`/`UPDATE`).

### Mostek
"Optymalizacja na poziomie bazy danych jest ważna, ale równie istotne jest zrozumienie, jak te dane są fizycznie przetwarzane przez architekturę komputera."

---

# TECHNIKI I ARCHITEKTURA KOMPUTERÓW

## 16. Model von Neumanna a Maszyna Turinga

### Szybki Start
"Maszyna Turinga to model matematyczny, który mówi nam, co w ogóle da się obliczyć. Architektura von Neumanna to natomiast praktyczny przepis na to, jak zbudować fizyczny komputer."

### Rozwinięcie
*   **Maszyna Turinga:** Składa się z nieskończonej taśmy, głowicy i stanów. Udowadnia, że prosty mechanizm może rozwiązać każdy problem algorytmiczny.
*   **Model von Neumanna:** Zakłada, że program i dane są przechowywane w tej samej pamięci. Składa się z: Procesora (ALU + CU), Pamięci, oraz Urządzeń Wejścia/Wyjścia.
*   **Wąskie gardło (Bottleneck):** Problem polegający na tym, że procesor jest znacznie szybszy niż przesył danych z pamięci.

### Mostek
"Fizyczna realizacja tych modeli opiera się na najprostszych elementach logicznych, czyli logice boolowskiej."

---

## 17. Logika boolowska w sprzęcie

### Szybki Start
"Logika boolowska to fundament elektroniki cyfrowej. Operuje na dwóch stanach: Prawda (1) i Fałsz (0), które w sprzęcie odpowiadają obecności lub brakowi napięcia."

### Rozwinięcie
*   **Bramki logiczne:** AND, OR, NOT, XOR, NAND (bramka uniwersalna – z niej można zbudować wszystko).
*   **Zastosowanie:** Z bramek budujemy bardziej złożone układy, takie jak sumatory (do dodawania liczb) czy przerzutniki (do przechowywania 1 bitu informacji w pamięci RAM).

### Mostek
"Dzięki logice boolowskiej możemy wykonywać operacje na liczbach, ale najpierw musimy wiedzieć, jak te liczby zapisać w systemie binarnym."

---

## 18. Zapis binarny i arytmetyka komputerowa

### Szybki Start
"Komputery używają systemu dwójkowego, bo jest on najłatwiejszy do realizacji sprzętowej. Liczby całkowite zapisujemy w systemie U2, a rzeczywiste w standardzie zmiennoprzecinkowym IEEE 754."

### Rozwinięcie
*   **System U2 (Uzupełnień do dwóch):** Pozwala na łatwe odejmowanie liczb poprzez dodawanie ich wartości ujemnych. Pierwszy bit oznacza znak (0 - plus, 1 - minus).
*   **Zmiennoprzecinkowe (Float):** Liczba składa się ze znaku, mantysy i wykładnika. Pozwala to zapisywać bardzo duże i bardzo małe liczby, ale kosztem precyzji (stąd błędy typu 0.1 + 0.2 != 0.3).

### Mostek
"Sposób zapisu danych i szybkość ich przetwarzania bezpośrednio wpływają na miary wydajności całego systemu."

---

## 19. Miary wydajności systemów

### Szybki Start
"Wydajność to nie tylko taktowanie procesora. To zdolność systemu do wykonania określonej pracy w jednostce czasu. Najważniejsze miary to czas odpowiedzi i przepustowość."

### Rozwinięcie
*   **Procesor:** Mierzymy w hercach (taktowanie), ale też w MIPS (miliony instrukcji na sekundę) czy FLOPS (operacje zmiennoprzecinkowe – ważne w AI i grafice).
*   **Pamięć:** Liczy się czas dostępu (opóźnienie/latency) oraz przepustowość (ile danych na sekundę).
*   **Benchmarki:** Specjalne programy testowe, które symulują realne obciążenie (np. renderowanie wideo).

### Mostek
"Wydajność jest kluczowa w dużych serwerach, ale w systemach wbudowanych często ważniejszy jest niski pobór energii i niezawodność."

---

## 20. Systemy wbudowane (Embedded)

### Szybki Start
"System wbudowany to komputer wyspecjalizowany do pełnienia jednej, konkretnej funkcji wewnątrz większego urządzenia (np. w pralce, samochodzie czy termostacie)."

### Rozwinięcie
*   **Cechy:** Ograniczone zasoby (mało RAM, słaby procesor), praca w czasie rzeczywistym (musi zareagować w określonym czasie, np. poduszka powietrzna), wysoka niezawodność.
*   **Budowa:** Zazwyczaj oparta na mikrokontrolerze (wszystko w jednym chipie: CPU, RAM, Flash, I/O).

### Mostek
"Niezależnie od tego, czy mamy do czynienia z systemem wbudowanym, czy potężnym serwerem, każdym z nich zarządza system operacyjny."

---

# SYSTEMY OPERACYJNE

## 21. Rola i zadania systemu operacyjnego

### Szybki Start
"System operacyjny (SO) to pośrednik między użytkownikiem a sprzętem. Jego głównym zadaniem jest zarządzanie zasobami komputera (procesorem, pamięcią, dyskiem) oraz udostępnianie interfejsu dla aplikacji."

### Rozwinięcie
*   **Zadania:** Zarządzanie procesami, pamięcią, systemem plików oraz obsługa urządzeń wejścia/wyjścia.
*   **Jądro (Kernel):** Serce systemu, które działa w trybie uprzywilejowanym i ma bezpośredni dostęp do sprzętu.
*   **Rodzaje:** Wielozadaniowe (Windows, Linux), czasu rzeczywistego (RTOS – dla systemów wbudowanych), rozproszone.

### Mostek
"Najważniejszą jednostką pracy dla systemu operacyjnego jest proces, który wykonuje kod programu."

---

## 22. Procesy i wątki, szeregowanie

### Szybki Start
"Proces to program w trakcie wykonywania, który ma własną pamięć. Wątek to 'lekki proces' wewnątrz procesu – wątki współdzielą pamięć, co pozwala na szybszą komunikację, ale wymaga ostrożności."

### Rozwinięcie
*   **Stany procesu:** Nowy -> Gotowy -> Wykonywany -> Oczekujący -> Zakończony.
*   **Przełączanie kontekstu:** Moment, w którym procesor przestaje wykonywać jeden proces i zaczyna drugi (wymaga zapisania stanu rejestrów).
*   **Szeregowanie (Scheduling):** Algorytmy decydujące, kto teraz dostanie procesor (np. FIFO, Round Robin – każdy dostaje kwant czasu).

### Mostek
"Gdy wiele wątków pracuje na tych samych danych, pojawia się problem ich synchronizacji, aby nie nadpisywały sobie wyników."

---

## 23. Synchronizacja i zakleszczenia (Deadlock)

### Szybki Start
"Synchronizacja to dbanie o to, by procesy nie wchodziły sobie w drogę przy dostępie do wspólnych zasobów. Jeśli zrobimy to źle, może dojść do zakleszczenia, czyli sytuacji, w której wszyscy na siebie czekają i nikt nie może ruszyć."

### Rozwinięcie
*   **Wzajemne wykluczanie:** Tylko jeden proces może być w 'sekcji krytycznej' (np. zapisywać do pliku). Używamy do tego Muteksów lub Semaforów.
*   **Zakleszczenie (Deadlock):** Cztery warunki (np. wzajemne wykluczanie, trzymanie i czekanie). Klasyczny przykład to 'Problem ucztujących filozofów'.

### Mostek
"System operacyjny musi zarządzać nie tylko czasem procesora, ale też miejscem w pamięci operacyjnej."

---

## 24. Zarządzanie pamięcią i pamięć wirtualna

### Szybki Start
"Zarządzanie pamięcią polega na przydzielaniu miejsca w RAM dla procesów. Pamięć wirtualna to technika, która pozwala procesom myśleć, że mają do dyspozycji ogromną, ciągłą pamięć, nawet jeśli fizycznie jest ona rozproszona lub częściowo znajduje się na dysku."

### Rozwinięcie
*   **Stronicowanie (Paging):** Dzielenie pamięci na małe, równe bloki (strony). Rozwiązuje problem fragmentacji.
*   **Segmentacja:** Dzielenie pamięci na logiczne części (kod, dane, stos).
*   **Błąd strony (Page Fault):** Sytuacja, gdy proces chce danych, których nie ma w RAM i trzeba je doczytać z dysku.

### Mostek
"Dane, które nie mieszczą się w RAM lub muszą zostać zachowane na stałe, trafiają do systemu plików."

---

## 25. System plików

### Szybki Start
"System plików to sposób organizacji danych na nośniku (dysku). Pozwala on użytkownikowi widzieć dane jako strukturę plików i folderów, zamiast surowych bloków bajtów."

### Rozwinięcie
*   **Struktura:** Pliki, katalogi, metadane (data utworzenia, uprawnienia).
*   **Implementacja:** Tablice alokacji (np. FAT) lub i-węzły (i-nodes w Linuxie), które przechowują informacje o tym, gdzie fizycznie leżą fragmenty pliku.
*   **Journaling (Kronikowanie):** Zapisywanie planowanych zmian w dzienniku, co chroni system przed uszkodzeniem przy nagłym wyłączeniu prądu (np. NTFS, ext4).

### Mostek
"Systemy plików pozwalają nam przechowywać dane lokalnie, ale w dzisiejszych czasach większość danych przesyłamy przez sieci komputerowe."

---

# SIECI KOMPUTEROWE

## 26. Model ISO/OSI i TCP/IP

### Szybki Start
"Modele warstwowe dzielą proces komunikacji na mniejsze etapy. ISO/OSI ma 7 warstw (teoretyczny), a TCP/IP ma 4 warstwy i jest modelem praktycznym, na którym opiera się dzisiejszy Internet."

### Rozwinięcie
*   **Warstwy (od dołu):** Fizyczna (kable), Łącza danych (MAC), Sieciowa (IP), Transportowa (TCP/UDP), Aplikacji (HTTP).
*   **Enkapsulacja:** Proces pakowania danych w nagłówki kolejnych warstw podczas wysyłania.
*   **TCP vs UDP:** TCP jest niezawodne (potwierdza odbiór), UDP jest szybkie (dobre do gier i streamingu, ale może gubić pakiety).

### Mostek
"Aby dane trafiły do celu, każda warstwa używa odpowiedniej adresacji."

---

## 27. Adresacja: MAC, IP, Porty oraz ARP, DNS, DHCP

### Szybki Start
"Adresacja pozwala zidentyfikować odbiorcę. Adres MAC to stały adres sprzętowy, IP to adres logiczny w sieci, a Port to numer 'okienka' w komputerze, do którego mają trafić dane (np. port 80 dla stron WWW)."

### Rozwinięcie
*   **DHCP:** Automatycznie przydziela adresy IP urządzeniom w sieci.
*   **DNS:** 'Książka telefoniczna' Internetu – zamienia nazwy (google.pl) na adresy IP.
*   **ARP:** Tłumaczy adres IP na adres fizyczny MAC (potrzebne w sieci lokalnej).

### Mostek
"Przesyłanie danych między różnymi sieciami wymaga specjalistycznych urządzeń."

---

## 28. Urządzenia sieciowe: Koncentrator, Przełącznik, Router

### Szybki Start
"To urządzenia kierujące ruchem. Koncentrator (Hub) wysyła wszystko do wszystkich (przestarzałe), Przełącznik (Switch) łączy urządzenia wewnątrz jednej sieci, a Router łączy różne sieci ze sobą."

### Rozwinięcie
*   **Switch:** Działa w warstwie 2 (MAC). Wie, do którego portu podpięty jest dany komputer.
*   **Router:** Działa w warstwie 3 (IP). Decyduje, jaką drogą wysłać pakiet do innej sieci (np. z domu do serwera Google).

### Mostek
"Urządzenia te pozwalają nam korzystać z usług warstwy aplikacji, takich jak przeglądanie stron czy wysyłanie maili."

---

## 29. Protokoły warstwy aplikacji: HTTP, FTP, SMTP

### Szybki Start
"To protokoły, z którymi użytkownik ma bezpośredni kontakt. HTTP służy do stron WWW, FTP do przesyłania plików, a SMTP do wysyłania poczty elektronicznej."

### Rozwinięcie
*   **HTTP/HTTPS:** Protokół bezstanowy (żądanie-odpowiedź). HTTPS dodaje szyfrowanie (SSL/TLS).
*   **SMTP / IMAP / POP3:** SMTP wysyła maila, a IMAP/POP3 służą do jego odbierania z serwera.

### Mostek
"Korzystanie z tych usług wymaga dbania o bezpieczeństwo, aby nasze dane nie wpadły w niepowołane ręce."

---

## 30. Bezpieczeństwo sieci i kryptografia

### Szybki Start
"Bezpieczeństwo w sieci opiera się na trzech filarach (CIA): Poufności, Integralności i Dostępności. Głównym narzędziem do ich zapewnienia jest kryptografia."

### Rozwinięcie
*   **Zagrożenia:** Ataki DoS (blokowanie usług), Phishing (wyłudzanie danych), Malware (złośliwe oprogramowanie).
*   **Ochrona:** Firewall (ściana ogniowa), VPN (bezpieczny tunel), Szyfrowanie.
*   **Kryptografia:** Symetryczna (jeden klucz dla obu stron) i Asymetryczna (para kluczy: publiczny do szyfrowania i prywatny do deszyfrowania).

### Mostek
"Bezpieczeństwo jest kluczowe na każdym etapie tworzenia oprogramowania, od projektu po wdrożenie."

---

# ALGORYTMY I PROGRAMOWANIE

## 31. Cykl życia oprogramowania (SDLC)

### Szybki Start
"Cykl życia oprogramowania to proces tworzenia aplikacji od pomysłu do wyłączenia z użytku. Najpopularniejsze modele to kaskadowy (Waterfall) oraz zwinny (Agile)."

### Rozwinięcie
*   **Etapy:** Analiza wymagań -> Projektowanie -> Implementacja (kodowanie) -> Testowanie -> Wdrożenie i utrzymanie.
*   **Waterfall:** Każdy etap musi się skończyć, zanim zacznie się następny. Sztywny, ale przewidywalny.
*   **Agile:** Praca w krótkich cyklach (iteracjach), szybkie reagowanie na zmiany.

### Mostek
"Niezależnie od modelu, sercem każdego programu są algorytmy, które musimy umieć ocenić pod kątem wydajności."

---

## 32. Analiza algorytmów i złożoność obliczeniowa

### Szybki Start
"Złożoność obliczeniowa mówi nam, jak szybko rośnie czas działania algorytmu (lub zapotrzebowanie na pamięć) wraz ze wzrostem ilości danych. Używamy do tego notacji 'Duże O'."

### Rozwinięcie
*   **Notacja O(n):** 
    *   $O(1)$ – stała (zawsze tak samo szybko).
    *   $O(log n)$ – bardzo szybka (np. wyszukiwanie binarne).
    *   $O(n)$ – liniowa (przejście przez całą tablicę).
    *   $O(n^2)$ – kwadratowa (np. proste sortowania).
*   **Zasada:** Zawsze interesuje nas zachowanie dla bardzo dużych danych (asymptotyka).

### Mostek
"Algorytmy implementujemy w różnych paradygmatach programowania, zależnie od problemu."

---

## 33. Paradygmaty programowania

### Szybki Start
"Paradygmat to styl pisania kodu. Najważniejsze to: Imperatywny (mówimy komputerowi 'jak' ma coś zrobić krok po kroku) oraz Deklaratywny (mówimy 'co' chcemy osiągnąć, np. SQL)."

### Rozwinięcie
*   **Obiektowy (OOP):** Świat jako zbiór współpracujących obiektów (Java, C++).
*   **Funkcyjny:** Opiera się na funkcjach matematycznych i unikaniu zmian stanu (Haskell, częściowo JavaScript).

### Mostek
"Programowanie obiektowe jest obecnie najpopularniejsze w inżynierii oprogramowania i opiera się na kilku kluczowych filarach."

---

## 34. Programowanie obiektowe (OOP)

### Szybki Start
"OOP to sposób pisania programów oparty na Klasach (szablonach) i Obiektach (konkretnych egzemplarzach). Jego celem jest lepsza organizacja i reużywalność kodu."

### Rozwinięcie
*   **Filar 1: Abstrakcja:** Ukrywanie szczegółów, pokazywanie tylko tego, co ważne.
*   **Filar 2: Enkapsulacja (Hermetyzacja):** Ukrywanie danych wewnątrz obiektu (pola prywatne).
*   **Filar 3: Dziedziczenie:** Tworzenie nowych klas na bazie istniejących.
*   **Filar 4: Polimorfizm:** Możliwość używania różnych typów obiektów przez ten sam interfejs.

### Mostek
"Obiekty w programach często przechowujemy w strukturach danych, które dobieramy zależnie od potrzeb."

---

## 35. Podstawowe struktury danych

### Szybki Start
"Struktury danych to sposoby organizowania informacji w pamięci. Wybór struktury decyduje o szybkości działania programu."

### Rozwinięcie
*   **Tablica:** Szybki dostęp po indeksie, ale trudna zmiana rozmiaru.
*   **Lista:** Łatwe dodawanie elementów w środku, ale wolny dostęp (trzeba przejść od początku).
*   **Stos (Stack):** LIFO (Last In, First Out) – jak stos talerzy.
*   **Kolejka (Queue):** FIFO (First In, First Out) – jak kolejka w sklepie.
*   **Drzewo / Graf:** Struktury hierarchiczne i relacyjne.

### Mostek
"Na tych strukturach wykonujemy operacje, z których najczęstszą jest sortowanie."

---

## 36. Algorytmy sortowania

### Szybki Start
"Sortowanie to układanie danych w określonej kolejności. Dzielimy je na proste (wolne) i zaawansowane (szybkie)."

### Rozwinięcie
*   **Proste ($O(n^2)$):** Bąbelkowe, przez wstawianie, przez wybór. Dobre dla bardzo małych zbiorów.
*   **Szybkie ($O(n log n)$):** QuickSort (szybki w praktyce), MergeSort (stabilny, dobry dla dużych danych).

### Mostek
"Po posortowaniu danych możemy znacznie szybciej wyszukiwać w nich informacje."

---

## 37. Algorytmy wyszukiwania

### Szybki Start
"Wyszukiwanie to znajdowanie elementu w zbiorze. Jeśli dane są nieuporządkowane, musimy szukać liniowo. Jeśli są posortowane – możemy użyć wyszukiwania binarnego."

### Rozwinięcie
*   **Liniowe:** Sprawdzamy każdy element po kolei ($O(n)$).
*   **Binarne:** Dzielimy zbiór na pół w każdym kroku ($O(log n)$). To ogromna różnica – w milionie elementów znajdziemy szukany w max 20 krokach!

### Mostek
"Bardziej skomplikowane wyszukiwanie odbywa się na grafach, gdzie szukamy np. najkrótszej drogi."

---

## 38. Algorytmy grafowe (BFS, DFS, Dijkstra)

### Szybki Start
"Algorytmy grafowe pozwalają nam przeszukiwać sieci połączeń. BFS idzie 'wszerz' (warstwami), a DFS 'w głąb'."

### Rozwinięcie
*   **BFS:** Znajduje najkrótszą drogę w grafach bez wag (np. najmniejsza liczba przesiadek).
*   **Dijkstra:** Znajduje najkrótszą drogę w grafach z wagami (np. najszybsza trasa w GPS, gdzie wagi to czas przejazdu).
*   **MST (Minimalne Drzewo Rozpinające):** Algorytmy Kruskala i Prima – jak połączyć wszystkie punkty najniższym kosztem (np. kablem).

### Mostek
"Niektóre problemy grafowe są jednak tak trudne, że komputery nie potrafią ich rozwiązać w rozsądnym czasie, co prowadzi nas do teorii złożoności P i NP."

---

## 39. Klasy złożoności P i NP

### Szybki Start
"Klasa P to problemy, które komputery rozwiązują szybko. Klasa NP to problemy, dla których potrafimy szybko sprawdzić, czy podane rozwiązanie jest poprawne, ale nie wiemy, jak je szybko znaleźć."

### Rozwinięcie
*   **P (Polynomial):** Np. sortowanie, mnożenie liczb.
*   **NP (Nondeterministic Polynomial):** Np. łamanie haseł, problem komiwojażera.
*   **NP-zupełne:** Najtrudniejsze problemy w NP. Jeśli ktoś znajdzie szybki sposób na jeden z nich, rozwiąże wszystkie problemy NP.

### Mostek
"Teoria algorytmów to fundament, ale inżynier musi też znać narzędzia i procesy tworzenia oprogramowania."

---

# INŻYNIERIA OPROGRAMOWANIA I TECHNOLOGIE

## 43. Wzorce projektowe

### Szybki Start
"Wzorce projektowe to sprawdzone, uniwersalne rozwiązania typowych problemów w programowaniu obiektowym. Dzielą się na kreacyjne, strukturalne i behawioralne."

### Rozwinięcie
*   **Kreacyjne:** Jak tworzyć obiekty (np. **Singleton** – tylko jedna instancja klasy w całym programie).
*   **Strukturalne:** Jak składać obiekty w większe struktury (np. **Adapter** – pozwala współpracować klasom o niekompatybilnych interfejsach).
*   **Behawioralne:** Jak obiekty się komunikują (np. **Obserwator** – powiadamianie wielu obiektów o zmianie stanu innego obiektu).

### Mostek
"Stosowanie wzorców ułatwia pisanie kodu, ale aby mieć pewność, że działa on poprawnie, musimy go przetestować."

---

## 44. Testowanie oprogramowania

### Szybki Start
"Testowanie to proces weryfikacji, czy program działa zgodnie z wymaganiami. Dzielimy je na testy białoskrzynkowe (znamy kod) i czarnoskrzynkowe (testujemy tylko funkcjonalność)."

### Rozwinięcie
*   **Poziomy:**
    *   **Jednostkowe (Unit):** Testujemy pojedyncze funkcje.
    *   **Integracyjne:** Sprawdzamy, czy moduły współpracują.
    *   **Systemowe:** Testujemy całą aplikację.
    *   **Akceptacyjne:** Sprawdza klient (czy to jest to, co zamawiał).

### Mostek
"Współczesne testowanie i wdrażanie oprogramowania jest zautomatyzowane dzięki procesom CI/CD i konteneryzacji."

---

## 46. Konteneryzacja i Docker

### Szybki Start
"Konteneryzacja pozwala zapakować aplikację wraz ze wszystkimi jej zależnościami (bibliotekami, konfiguracją) w jeden 'kontener'. Dzięki temu program działa tak samo na każdym komputerze."

### Rozwinięcie
*   **Docker:** Najpopularniejsze narzędzie do kontenerów.
*   **Zaleta:** Rozwiązuje problem "u mnie działa". Kontenery są lekkie, szybko się uruchamiają i pozwalają na łatwe skalowanie aplikacji.

### Mostek
"Kontenery są częścią nowoczesnego podejścia do infrastruktury, podobnie jak chmura obliczeniowa."

---

## 55. Chmura obliczeniowa (Cloud Computing)

### Szybki Start
"Chmura to dostarczanie zasobów IT (serwerów, baz danych) przez Internet w modelu 'płacisz za to, co zużyjesz'. Główne modele to IaaS, PaaS i SaaS."

### Rozwinięcie
*   **IaaS (Infrastructure):** Wynajmujesz 'czysty' serwer (np. AWS EC2).
*   **PaaS (Platform):** Masz gotowe środowisko do uruchomienia kodu (np. Heroku).
*   **SaaS (Software):** Gotowa aplikacja w przeglądarce (np. Gmail, Office 365).

### Mostek
"Chmura daje ogromną moc obliczeniową, która jest niezbędna do trenowania nowoczesnych modeli sztucznej inteligencji."

---

## 56. Uczenie maszynowe (Machine Learning)

### Szybki Start
"Uczenie maszynowe to dziedzina AI, w której algorytmy uczą się na podstawie danych, zamiast być bezpośrednio zaprogramowane. Dzieli się na nadzorowane, nienadzorowane i ze wzmocnieniem."

### Rozwinięcie
*   **Nadzorowane:** Mamy dane z etykietami (np. zdjęcia opisane jako 'kot' lub 'pies'). Algorytm uczy się rozpoznawać wzorce.
*   **Nienadzorowane:** Algorytm sam szuka struktur w danych (np. grupowanie klientów o podobnych cechach).
*   **Ze wzmocnieniem:** Agent uczy się poprzez system kar i nagród (np. AI grająca w szachy).

### Mostek
"Najbardziej zaawansowaną formą uczenia maszynowego jest Deep Learning, oparty na sieciach neuronowych."

---

## 57. Sztuczne sieci neuronowe i Deep Learning

### Szybki Start
"Sieci neuronowe to modele inspirowane budową ludzkiego mózgu. Składają się z warstw neuronów, które przetwarzają informacje. Deep Learning to sieci o bardzo wielu warstwach (głębokie)."

### Rozwinięcie
*   **Zastosowanie:** Rozpoznawanie obrazów, mowy, autonomiczne samochody.
*   **NLP (Natural Language Processing):** Przetwarzanie języka naturalnego – to dzięki temu działają czatboty i tłumacze.

### Mostek
"Rozwój AI niesie ze sobą nie tylko korzyści, ale też wyzwania etyczne i prawne."

---

## 54. Prawne aspekty oprogramowania i licencje

### Szybki Start
"Oprogramowanie jest chronione prawem autorskim. Jako inżynierowie musimy rozumieć różnice między licencjami, aby legalnie korzystać z cudzego kodu."

### Rozwinięcie
*   **Proprietary (Własnościowe):** Kod zamknięty, płatny (np. Windows).
*   **Open Source:** Kod otwarty.
    *   **Permisywne (np. MIT):** Możesz robić prawie wszystko, nawet zamknąć kod w swoim produkcie.
    *   **Copyleft (np. GPL):** Jeśli użyjesz tego kodu, Twój program też musi być Open Source.

### Mostek
"Znajomość prawa i etyki to ostatni element układanki, który czyni z programisty inżyniera odpowiedzialnego za swoje dzieła."

---

# POWODZENIA NA EGZAMINIE!
Pamiętaj: na egzaminie ustnym najważniejszy jest spokój. Jeśli czegoś nie wiesz, użyj "Mostka", aby przejść do tematu, w którym czujesz się pewniej. Powodzenia!

# GRAFIKA I INTERFEJSY

## 40. Grafika rastrowa i wektorowa, modele barw

### Szybki Start
"Grafika rastrowa to obraz zbudowany z pikseli (np. zdjęcie), a wektorowa to obraz zbudowany z matematycznych opisów kształtów (np. logo). Modele barw określają, jak kolory są reprezentowane cyfrowo."

### Rozwinięcie
*   **Rastrowa:** Traci jakość przy skalowaniu, duży rozmiar pliku. Edycja pikseli.
*   **Wektorowa:** Skalowalna bez utraty jakości, mniejszy rozmiar pliku. Edycja obiektów.
*   **Modele barw:**
    *   **RGB:** Addytywny (dodawanie światła), do wyświetlania na ekranach (Red, Green, Blue).
    *   **CMYK:** Subtraktywny (odejmowanie światła), do druku (Cyan, Magenta, Yellow, Key/Black).

### Mostek
"Zrozumienie grafiki jest kluczowe przy projektowaniu interfejsów użytkownika, które muszą być zarówno estetyczne, jak i funkcjonalne."

---

## 41. Interfejsy użytkownika (UI) i interakcja człowiek-komputer (HCI)

### Szybki Start
"Interfejs użytkownika to sposób, w jaki człowiek komunikuje się z maszyną. HCI to szersza dziedzina badająca tę interakcję, aby tworzyć systemy łatwe, efektywne i przyjemne w użyciu."

### Rozwinięcie
*   **Zasady projektowania UI:** 
    *   **Użyteczność:** Łatwość nauki i efektywność użytkowania.
    *   **Dostępność:** Dla osób z różnymi niepełnosprawnościami.
    *   **Spójność:** Podobne elementy zachowują się podobnie.
    *   **Informacja zwrotna:** System reaguje na działania użytkownika.
*   **Typy interfejsów:** Graficzne (GUI), tekstowe (CLI), głosowe (VUI).

### Mostek
"Dobre interfejsy są wynikiem przemyślanej inżynierii oprogramowania, która zaczyna się od wymagań."

---

## 42. Inżynieria wymagań

### Szybki Start
"Inżynieria wymagań to proces zbierania, analizowania, dokumentowania i zarządzania potrzebami użytkowników i systemu. Dzielimy je na funkcjonalne (co system ma robić) i niefunkcjonalne (jak system ma działać)."

### Rozwinięcie
*   **Wymagania funkcjonalne:** Opisują konkretne funkcje, które system musi dostarczyć (np. "system musi pozwalać na logowanie użytkownika").
*   **Wymagania niefunkcjonalne:** Opisują jakość systemu, jego ograniczenia (np. wydajność, bezpieczeństwo, użyteczność, skalowalność).
*   **Proces:** Pozyskiwanie (wywiady, ankiety), analiza, specyfikacja (dokumentacja), walidacja (sprawdzenie, czy są poprawne), zarządzanie (zmiany).

### Mostek
"Dobre zrozumienie wymagań jest kluczowe, aby móc zaprojektować system, a w tym pomagają nam wzorce projektowe."

---

## 6. Relacje binarne, własności i metody reprezentacji

### Szybki Start
"Relacja binarna to sposób powiązania elementów z dwóch zbiorów (lub jednego zbioru ze sobą). Mówiąc prościej, to zbiór par, które spełniają jakąś zależność, np. 'jest większe od' albo 'jest znajomym'."

### Rozwinięcie
*   **Własności:**
    *   **Zwrotność:** Każdy element jest w relacji sam ze sobą (np. 'jest równe').
    *   **Symetryczność:** Jeśli A jest w relacji z B, to B jest w relacji z A (np. 'jest znajomym').
    *   **Przechodniość:** Jeśli A jest w relacji z B, a B z C, to A jest w relacji z C (np. 'jest mniejsze od').
*   **Reprezentacja:**
    *   **Graf:** Wierzchołki to elementy, krawędzie to relacje.
    *   **Macierz:** Tabela 0/1, gdzie 1 oznacza istnienie relacji.

### Mostek
"Relacje binarne są podstawą do zrozumienia wielu struktur danych, a jedną z najważniejszych jest zasada indukcji matematycznej, która pozwala nam udowadniać własności dla nieskończonych zbiorów."

---

## 7. Zasada indukcji matematycznej

### Szybki Start
"Indukcja matematyczna to metoda dowodzenia twierdzeń dla liczb naturalnych. Działa jak domino: jeśli przewrócisz pierwszą kostkę i wiesz, że każda kostka przewróci następną, to przewrócą się wszystkie."

### Rozwinięcie
*   **Kroki:**
    *   **Baza indukcji:** Sprawdzamy, czy twierdzenie jest prawdziwe dla pierwszej wartości (np. n=1).
    *   **Założenie indukcyjne:** Zakładamy, że twierdzenie jest prawdziwe dla pewnego k (dowolnej kostki).
    *   **Krok indukcyjny:** Udowadniamy, że jeśli jest prawdziwe dla k, to jest też prawdziwe dla k+1 (następnej kostki).
*   **Zastosowanie:** Dowodzenie poprawności algorytmów rekurencyjnych, własności struktur danych (np. drzew).

### Mostek
"Indukcja matematyczna to narzędzie do dowodzenia pewności. W statystyce natomiast często operujemy na prawdopodobieństwie, a kluczowym narzędziem jest Twierdzenie Bayesa."

---

## 8. Twierdzenie Bayesa

### Szybki Start
"Twierdzenie Bayesa pozwala nam zaktualizować nasze przekonania o prawdopodobieństwie jakiegoś zdarzenia, gdy dostaniemy nowe dane. Mówiąc prościej: jak nowe informacje zmieniają nasze szanse."

### Rozwinięcie
*   **Wzór:** $P(A|B) = \frac{P(B|A) * P(A)}{P(B)}$
    *   $P(A|B)$: Prawdopodobieństwo A, gdy zaszło B (to, co chcemy obliczyć).
    *   $P(B|A)$: Prawdopodobieństwo B, gdy zaszło A.
    *   $P(A)$: Prawdopodobieństwo A (przed nowymi danymi).
    *   $P(B)$: Prawdopodobieństwo B.
*   **Zastosowanie:** Filtry antyspamowe, diagnostyka medyczna, systemy rekomendacji.

### Mostek
"Twierdzenie Bayesa jest podstawą wnioskowania statystycznego, które często wykorzystujemy do testowania hipotez."

---

## 9. Testowanie hipotez statystycznych

### Szybki Start
"Testowanie hipotez to proces decydowania, czy nasze obserwacje są wystarczająco silne, aby odrzucić jakąś wstępną tezę (hipotezę zerową). Np. czy nowy lek działa, czy to tylko przypadek."

### Rozwinięcie
*   **Hipoteza zerowa ($H_0$):** Zawsze zakładamy, że nie ma różnicy, nie ma efektu (np. "lek nie działa").
*   **Hipoteza alternatywna ($H_1$):** To, co chcemy udowodnić (np. "lek działa").
*   **P-wartość:** Prawdopodobieństwo uzyskania tak ekstremalnych wyników, jeśli $H_0$ jest prawdziwa. Jeśli p-wartość jest mała (np. < 0.05), odrzucamy $H_0$.
*   **Błędy:** Typu I (fałszywie odrzucamy $H_0$) i Typu II (fałszywie akceptujemy $H_0$).

### Mostek
"Testowanie hipotez daje nam odpowiedź tak/nie. Jeśli chcemy wiedzieć, jak bardzo jesteśmy pewni jakiejś wartości, używamy przedziałów ufności."

---

## 10. Wyznaczanie przedziałów ufności

### Szybki Start
"Przedział ufności to zakres wartości, w którym z określonym prawdopodobieństwem (np. 95%) znajduje się prawdziwa wartość parametru populacji. Mówiąc prościej: to nie jest jedna liczba, ale przedział, w którym z dużą pewnością leży to, czego szukamy."

### Rozwinięcie
*   **Poziom ufności:** Najczęściej 95% lub 99%. Im wyższy poziom, tym szerszy przedział.
*   **Margines błędu:** Połowa szerokości przedziału. Zależy od odchylenia standardowego i wielkości próby.
*   **Zastosowanie:** Badania opinii publicznej (słynne +/- 3%), kontrola jakości, szacowanie parametrów modeli.

### Mostek
"Statystyka jest potężnym narzędziem do analizy danych, a jej podstawy matematyczne są kluczowe w wielu dziedzinach informatyki."

---

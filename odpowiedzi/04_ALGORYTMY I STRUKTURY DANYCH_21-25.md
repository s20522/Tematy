# Odpowiedzi na pytania do obrony pracy inżynierskiej - Algorytmy i Struktury Danych

## 21. Szacowanie złożoności algorytmów, klasy złożoności problemów algorytmicznych.

### Szczegółowe wyjaśnienie

**Czym jest złożoność algorytmu?**

Złożoność algorytmu to sposób na formalne opisanie jego **efektywności** – czyli tego, jak bardzo zasobożerny jest dany algorytm w zależności od rozmiaru danych wejściowych. Analizujemy głównie dwa rodzaje złożoności:

1.  **Złożoność czasowa (Time Complexity):** Określa, jak liczba operacji elementarnych (takich jak porównania, przypisania, operacje arytmetyczne) wykonywanych przez algorytm rośnie wraz ze wzrostem rozmiaru danych wejściowych (oznaczanego jako `n`). Mówi nam, jak bardzo **dłużej** będzie działał algorytm, gdy damy mu więcej danych.

2.  **Złożoność pamięciowa (Space Complexity):** Określa, ile dodatkowej pamięci (oprócz tej na dane wejściowe) potrzebuje algorytm do swojego działania. Mówi nam, jak bardzo **więcej pamięci** zużyje algorytm, gdy damy mu więcej danych.

Celem analizy złożoności nie jest dokładne policzenie milisekund czy bajtów, ale zrozumienie **tempa wzrostu** zapotrzebowania na zasoby. Chcemy wiedzieć, czy dla dwukrotnie większej ilości danych algorytm będzie działał dwa razy dłużej, cztery razy dłużej, czy może logarytmicznie szybciej.

**Notacja Wielkiego O (Big O Notation)**

Do opisu złożoności używa się notacji asymptotycznej, z której najważniejsza jest **notacja O (duże O)**. Opisuje ona **górną granicę** tempa wzrostu funkcji w najgorszym możliwym przypadku (pesymistycznym). Ignoruje ona stałe i czynniki niższych rzędów, skupiając się na tym, co dominuje, gdy `n` dąży do nieskończoności.

**Najważniejsze klasy złożoności czasowej:**

*   **O(1) – złożoność stała:** Czas wykonania jest niezależny od rozmiaru danych. Przykład: dostęp do elementu tablicy po indeksie.
*   **O(log n) – złożoność logarytmiczna:** Czas wykonania rośnie bardzo wolno. Podwojenie `n` powoduje tylko niewielki, stały wzrost liczby operacji. Przykład: wyszukiwanie binarne w posortowanej tablicy.
*   **O(n) – złożoność liniowa:** Czas wykonania rośnie proporcjonalnie do rozmiaru danych. Podwojenie `n` powoduje dwukrotne wydłużenie czasu. Przykład: wyszukiwanie elementu w nieposortowanej liście.
*   **O(n log n) – złożoność liniowo-logarytmiczna:** Uważana za bardzo dobrą dla algorytmów sortowania opartych na porównaniach. Przykład: sortowanie przez scalanie (Merge Sort).
*   **O(n²) – złożoność kwadratowa:** Czas wykonania rośnie z kwadratem rozmiaru danych. Podwojenie `n` powoduje czterokrotne wydłużenie czasu. Typowa dla algorytmów z podwójnie zagnieżdżonymi pętlami. Przykład: proste sortowanie bąbelkowe.
*   **O(2ⁿ) – złożoność wykładnicza:** Czas wykonania rośnie ekstremalnie szybko. Algorytmy te są praktycznie bezużyteczne już dla niewielkich `n`. Przykład: naiwne, rekurencyjne obliczanie liczb Fibonacciego.
*   **O(n!) – złożoność rzędu silnia:** Jeszcze gorsza niż wykładnicza. Przykład: rozwiązanie problemu komiwojażera metodą siłową (sprawdzanie wszystkich możliwych tras).

**Klasy złożoności problemów algorytmicznych**

Teoria złożoności klasyfikuje nie algorytmy, ale **problemy obliczeniowe**. Chcemy wiedzieć, jak *trudny* jest dany problem, czyli jaka jest złożoność *najlepszego możliwego* algorytmu, który go rozwiązuje.

1.  **Klasa P (Polynomial Time):**
    *   Zawiera problemy decyzyjne, dla których istnieje algorytm rozwiązujący je w **czasie wielomianowym** (np. O(n), O(n³)).
    *   Są to problemy uważane za **"łatwe"** lub **"obliczalnie trakcyjne"**, ponieważ możemy je efektywnie rozwiązać nawet dla dużych danych.
    *   Przykłady: sortowanie listy, znalezienie najkrótszej ścieżki w grafie, sprawdzenie, czy liczba jest pierwsza.

2.  **Klasa NP (Nondeterministic Polynomial Time):**
    *   Zawiera problemy decyzyjne, dla których **weryfikacja** podanego rozwiązania może być wykonana w czasie wielomianowym. Innymi słowy, jeśli ktoś da nam gotowe rozwiązanie, potrafimy szybko sprawdzić, czy jest ono poprawne.
    *   Nie oznacza to, że potrafimy szybko *znaleźć* to rozwiązanie. Każdy problem z klasy P jest też w klasie NP (bo jeśli umiemy go szybko rozwiązać, to tym bardziej umiemy szybko sprawdzić rozwiązanie).
    *   Przykład: **Problem komiwojażera (w wersji decyzyjnej):** "Czy istnieje trasa o długości mniejszej niż K?". Jeśli ktoś poda nam trasę, bardzo szybko możemy zsumować jej długość i sprawdzić, czy jest mniejsza od K. Ale znalezienie takiej trasy jest bardzo trudne.

3.  **Klasa NP-zupełne (NP-Complete, NPC):**
    *   To podzbiór klasy NP, który zawiera **najtrudniejsze problemy** w tej klasie.
    *   Mają one dwie cechy:
        1.  Należą do klasy NP.
        2.  Każdy inny problem z klasy NP można do nich **zredukować** w czasie wielomianowym. Oznacza to, że gdybyśmy znaleźli efektywny (wielomianowy) algorytm dla *jakiegokolwiek* problemu NP-zupełnego, moglibyśmy go użyć do rozwiązania *wszystkich* problemów z klasy NP.
    *   Przykłady: wspomniany problem komiwojażera, problem spełnialności formuł logicznych (SAT), problem kolorowania grafu.

**Problem P vs NP**

To najważniejszy nierozwiązany problem w informatyce. Pytanie brzmi: **Czy P = NP?** Inaczej mówiąc: czy każdy problem, którego rozwiązanie potrafimy szybko zweryfikować, potrafimy również szybko znaleźć? Powszechnie uważa się, że **P ≠ NP**, ale nikt do tej pory nie potrafił tego udowodnić. Gdyby okazało się, że P = NP, miałoby to rewolucyjne konsekwencje, m.in. złamałoby większość współczesnej kryptografii.


## 22. Najważniejsze algorytmy wyszukiwania i sortowania, przegląd i zastosowania.

### Szczegółowe wyjaśnienie

Wyszukiwanie i sortowanie to dwie z najbardziej fundamentalnych operacji w informatyce. Wybór odpowiedniego algorytmu ma kluczowy wpływ na wydajność aplikacji.

**Algorytmy wyszukiwania**

Celem algorytmów wyszukiwania jest znalezienie określonego elementu (lub jego pozycji) w zbiorze danych.

1.  **Wyszukiwanie liniowe (sekwencyjne):**
    *   **Jak działa:** To najprostszy możliwy algorytm. Polega na przeglądaniu kolekcji element po elemencie, od początku do końca, aż do znalezienia szukanego elementu lub do wyczerpania zbioru.
    *   **Złożoność czasowa:** O(n) – w najgorszym przypadku musimy przejrzeć wszystkie elementy.
    *   **Wymagania:** Brak. Działa na każdym zbiorze, posortowanym lub nie.
    *   **Zastosowania:** Użyteczne tylko dla małych lub nieposortowanych zbiorów danych. Ze względu na swoją prostotę, może być szybsze dla bardzo małych `n` niż bardziej skomplikowane algorytmy.

2.  **Wyszukiwanie binarne:**
    *   **Jak działa:** Niezwykle wydajny algorytm oparty na strategii "dziel i zwyciężaj". Porównuje szukany element z elementem środkowym w kolekcji. Jeśli są równe – element znaleziono. Jeśli szukany element jest mniejszy, algorytm kontynuuje poszukiwania tylko w lewej połowie zbioru. Jeśli jest większy – w prawej. Proces jest powtarzany, za każdym razem redukując przestrzeń poszukiwań o połowę.
    *   **Złożoność czasowa:** O(log n) – logarytmiczna. Dla miliona elementów potrzebuje w najgorszym razie tylko około 20 porównań.
    *   **Wymagania:** Zbiór danych **musi być posortowany**.
    *   **Zastosowania:** Wszędzie tam, gdzie mamy do czynienia z dużymi, posortowanymi zbiorami danych. Jest to standardowy algorytm wyszukiwania w bazach danych (dla indeksów), słownikach, książkach telefonicznych itp.

**Algorytmy sortowania**

Celem algorytmów sortowania jest uporządkowanie elementów w kolekcji według określonego kryterium (np. rosnąco).

**Proste algorytmy (dobre do celów edukacyjnych, niepraktyczne dla dużych zbiorów):**

1.  **Sortowanie bąbelkowe (Bubble Sort):**
    *   **Jak działa:** Wielokrotnie przechodzi przez listę, porównując sąsiednie elementy i zamieniając je miejscami, jeśli są w złej kolejności. Proces jest powtarzany, aż podczas jednego przejścia nie dokona się żadnej zamiany. Nazwa pochodzi od "wypychania" największych elementów na koniec listy, niczym bąbelków na powierzchnię wody.
    *   **Złożoność czasowa:** O(n²)

2.  **Sortowanie przez wstawianie (Insertion Sort):**
    *   **Jak działa:** Dzieli listę na część posortowaną i nieposortowaną. Pobiera kolejne elementy z części nieposortowanej i wstawia je w odpowiednie miejsce w części posortowanej. Działa podobnie do układania kart w ręku.
    *   **Złożoność czasowa:** O(n²). Jest to jednak algorytm **adaptacyjny** – dla danych częściowo posortowanych działa znacznie szybciej, zbliżając się do O(n).
    *   **Zastosowania:** Ze względu na prostotę i niskie narzuty, jest bardzo wydajny dla małych zbiorów danych. Dlatego często jest używany jako część składowa bardziej zaawansowanych algorytmów (np. w sortowaniu introspektywnym).

**Zaawansowane algorytmy (wydajne i praktyczne):**

3.  **Sortowanie przez scalanie (Merge Sort):**
    *   **Jak działa:** Klasyczny przykład algorytmu "dziel i zwyciężaj". Rekurencyjnie dzieli listę na pół, aż do uzyskania jednoelementowych podlist (które z definicji są posortowane). Następnie scala te podlisty z powrotem w większe, posortowane listy.
    *   **Złożoność czasowa:** O(n log n) w każdym przypadku (pesymistycznym, średnim i optymistycznym). Jest to algorytm **stabilny** (nie zmienia względnej kolejności równych elementów).
    *   **Złożoność pamięciowa:** O(n) – wymaga dodatkowej pamięci do przeprowadzenia operacji scalania.
    *   **Zastosowania:** Idealny do sortowania danych, które nie mieszczą się w pamięci (sortowanie zewnętrzne), oraz tam, gdzie stabilność jest kluczowa. Używany w implementacji `Array.prototype.sort()` w wielu przeglądarkach.

4.  **Sortowanie szybkie (Quick Sort):**
    *   **Jak działa:** Również oparty na strategii "dziel i zwyciężaj". Wybiera jeden element jako tzw. **pivot (oś)**. Następnie przestawia elementy w tablicy tak, aby wszystkie mniejsze od pivota znalazły się przed nim, a wszystkie większe – po nim. Na koniec rekurencyjnie sortuje dwie powstałe w ten sposób podtablice.
    *   **Złożoność czasowa:** Średnia i optymistyczna to O(n log n). Pesymistyczna to O(n²), ale występuje ona bardzo rzadko (dla danych już posortowanych przy naiwnym wyborze pivota). W praktyce jest to jeden z najszybszych algorytmów sortowania ogólnego przeznaczenia.
    *   **Złożoność pamięciowa:** O(log n) – sortuje "w miejscu" (in-place), wymaga tylko niewielkiej pamięci na stosie rekursji.
    *   **Zastosowania:** Jest to domyślny algorytm sortowania w wielu standardowych bibliotekach programistycznych ze względu na jego znakomitą średnią wydajność i niskie zapotrzebowanie na pamięć.

**Tabela porównawcza algorytmów sortowania:**

| Algorytm | Złożoność czasowa (średnia) | Złożoność czasowa (pesymistyczna) | Złożoność pamięciowa | Stabilność |
|---|---|---|---|---|
| Bąbelkowe | O(n²) | O(n²) | O(1) | Tak |
| Przez wstawianie | O(n²) | O(n²) | O(1) | Tak |
| Przez scalanie | O(n log n) | O(n log n) | O(n) | Tak |
| Szybkie | O(n log n) | O(n²) | O(log n) | Nie |


## 23. Charakterystyka i zastosowania podstawowych struktur danych: stos, kolejka, kolejka priorytetowa, struktura Find-Union, słownik.

### Szczegółowe wyjaśnienie

Struktury danych to sposoby organizowania i przechowywania danych w pamięci komputera, tak aby można było na nich efektywnie wykonywać operacje. Wybór odpowiedniej struktury jest kluczowy dla wydajności algorytmu.

**1. Stos (Stack)**

*   **Charakterystyka:** Liniowa struktura danych działająca zgodnie z zasadą **LIFO (Last-In, First-Out)** – ostatni element, który został dodany, jest pierwszym, który zostanie usunięty. Działa jak stos talerzy – dokładamy na wierzch i zdejmujemy z wierzchu.
*   **Podstawowe operacje:**
    *   `push`: dodaje element na szczyt stosu.
    *   `pop`: usuwa i zwraca element ze szczytu stosu.
    *   `peek` (lub `top`): zwraca element ze szczytu bez usuwania go.
*   **Zastosowania:**
    *   **Zarządzanie wywołaniami funkcji:** Każde wywołanie funkcji odkłada jej adres powrotu i zmienne lokalne na **stosie wywołań (call stack)**. To fundamentalny mechanizm działania programów.
    *   **Analiza składniowa (parsing):** Sprawdzanie poprawności nawiasów w wyrażeniach.
    *   **Algorytmy przeszukiwania w głąb (DFS):** Stos służy do przechowywania wierzchołków do odwiedzenia.
    *   **Funkcja "Cofnij" (Undo):** Każda operacja jest odkładana na stosie, a cofnięcie polega na jej zdjęciu i odwróceniu.

**2. Kolejka (Queue)**

*   **Charakterystyka:** Liniowa struktura danych działająca zgodnie z zasadą **FIFO (First-In, First-Out)** – pierwszy element, który został dodany, jest pierwszym, który zostanie usunięty. Działa jak kolejka ludzi w sklepie.
*   **Podstawowe operacje:**
    *   `enqueue` (lub `push`): dodaje element na koniec kolejki.
    *   `dequeue` (lub `pop`): usuwa i zwraca element z początku kolejki.
*   **Zastosowania:**
    *   **Zarządzanie zadaniami:** Buforowanie zadań do wykonania, np. w systemach operacyjnych (kolejka procesów), serwerach druku (kolejka wydruków).
    *   **Algorytmy przeszukiwania wszerz (BFS):** Kolejka służy do przechowywania wierzchołków do odwiedzenia na danym poziomie.
    *   **Bufory w komunikacji:** Wyrównywanie prędkości między producentem a konsumentem danych (np. streaming wideo).

**3. Kolejka priorytetowa (Priority Queue)**

*   **Charakterystyka:** Abstrakcyjna struktura danych podobna do kolejki, ale każdy element ma dodatkowo przypisany **priorytet**. Element o **najwyższym priorytecie** jest usuwany jako pierwszy, niezależnie od kolejności dodawania.
*   **Implementacja:** Najczęściej implementowana za pomocą **kopca (heap)**, co zapewnia logarytmiczną złożoność operacji dodawania i usuwania elementu o najwyższym priorytecie (O(log n)).
*   **Zastosowania:**
    *   **Algorytmy grafowe:** Algorytm Dijkstry (znajdowanie najkrótszej ścieżki) i algorytm Prima (znajdowanie minimalnego drzewa rozpinającego) używają kolejki priorytetowej do efektywnego wybierania wierzchołka o najmniejszej wadze.
    *   **Systemy operacyjne:** Szeregowanie procesów (procesy o wyższym priorytecie są wykonywane wcześniej).
    *   **Kompresja danych:** Algorytm Huffmana używa kolejki priorytetowej do budowy drzewa kodów.

**4. Struktura Zbiorów Rozłącznych (Find-Union / Disjoint-Set Union, DSU)**

*   **Charakterystyka:** Struktura danych, która przechowuje zbiór elementów podzielonych na pewną liczbę **rozłącznych (nieprzecinających się) podzbiorów**. Każdy podzbiór ma swojego reprezentanta.
*   **Podstawowe operacje:**
    *   `find(x)`: zwraca reprezentanta zbioru, do którego należy element `x`.
    *   `union(x, y)`: łączy dwa zbiory zawierające elementy `x` i `y` w jeden.
*   **Implementacja:** Zwykle jako las drzew, z dwiema ważnymi optymalizacjami: **łączenie według rangi/wielkości** i **kompresja ścieżki**, które sprawiają, że operacje te mają niemal stałą (amortyzowaną) złożoność czasową.
*   **Zastosowania:**
    *   **Wykrywanie cykli w grafie:** Niezwykle efektywny sposób na sprawdzanie, czy dodanie nowej krawędzi do grafu stworzy cykl.
    *   **Algorytm Kruskala:** Znajdowanie minimalnego drzewa rozpinającego.
    *   **Przetwarzanie obrazów:** Grupowanie sąsiadujących pikseli w regiony.

**5. Słownik (Dictionary / Map / Hash Table)**

*   **Charakterystyka:** Struktura danych, która przechowuje pary **(klucz, wartość)**. Klucze muszą być unikalne. Umożliwia błyskawiczny dostęp do wartości na podstawie jej klucza.
*   **Implementacja:** Najczęściej jako **tablica mieszająca (hash table)**. Klucz jest przepuszczany przez **funkcję skrótu (hash function)**, która zamienia go na indeks w tablicy. Pozwala to na osiągnięcie średniej złożoności czasowej **O(1)** dla operacji dodawania, usuwania i wyszukiwania.
*   **Kolizje:** Problem pojawia się, gdy dwa różne klucze dają ten sam indeks (tzw. kolizja). Rozwiązuje się to np. metodą **łańcuchową** (przechowywanie listy elementów pod danym indeksem) lub **adresowaniem otwartym**.
*   **Zastosowania:**
    *   **Praktycznie wszędzie:** Jest to jedna z najważniejszych i najczęściej używanych struktur danych w programowaniu.
    *   **Implementacja obiektów i klas:** W wielu językach skryptowych obiekty są wewnętrznie implementowane jako słowniki.
    *   **Zliczanie wystąpień:** np. liczenie, ile razy każde słowo występuje w tekście.
    *   **Pamięć podręczna (cache):** Przechowywanie wyników kosztownych obliczeń pod unikalnymi kluczami.


## 24. Drzewa binarne i drzewa n-arne w algorytmice. Charakterystyka, sposoby implementacji i zastosowania.

### Szczegółowe wyjaśnienie

Drzewa to nieliniowe, hierarchiczne struktury danych, które składają się z **węzłów** (przechowujących dane) połączonych **krawędziami**. Są niezwykle ważne w informatyce, ponieważ w naturalny sposób modelują wiele rzeczywistych problemów i hierarchii.

**Podstawowa terminologia:**
*   **Korzeń (root):** Węzeł na samej górze drzewa, który nie ma rodzica.
*   **Rodzic (parent):** Węzeł, który ma potomków.
*   **Dziecko (child):** Węzeł, który ma rodzica.
*   **Liść (leaf):** Węzeł, który nie ma dzieci.
*   **Wysokość drzewa:** Długość najdłuższej ścieżki od korzenia do liścia.

**Drzewa binarne**

*   **Charakterystyka:** To drzewa, w których każdy węzeł ma **co najwyżej dwoje dzieci**, nazywane tradycyjnie **lewym** i **prawym dzieckiem**. To najważniejszy i najczęściej spotykany typ drzewa w informatyce.
*   **Sposoby implementacji:** Najczęściej implementuje się je za pomocą struktur lub klas. Każdy węzeł (obiekt) przechowuje:
    *   Dane (wartość).
    *   Wskaźnik na lewe dziecko.
    *   Wskaźnik na prawe dziecko.
    Jeśli któreś z dzieci nie istnieje, odpowiedni wskaźnik ma wartość `null`.

*   **Szczególny typ: Binarne Drzewo Poszukiwań (BST - Binary Search Tree)**
    *   To drzewo binarne, które ma dodatkową, kluczową właściwość: dla każdego węzła `W`, wszystkie wartości w jego **lewym poddrzewie są mniejsze** od wartości `W`, a wszystkie wartości w jego **prawym poddrzewie są większe** od wartości `W`.
    *   Ta właściwość sprawia, że wyszukiwanie elementu w BST jest bardzo wydajne. Działa podobnie do wyszukiwania binarnego – zaczynamy od korzenia i w zależności od tego, czy szukana wartość jest mniejsza czy większa od wartości w bieżącym węźle, przechodzimy do lewego lub prawego dziecka. Dla **zrównoważonego** drzewa BST (gdzie wysokość lewego i prawego poddrzewa dla każdego węzła różni się co najwyżej o 1), złożoność operacji wyszukiwania, wstawiania i usuwania wynosi **O(log n)**.

*   **Zastosowania drzew binarnych:**
    *   **Binarne Drzewa Poszukiwań (BST):** Implementacja wydajnych słowników i zbiorów. Indeksy w bazach danych często wykorzystują warianty BST.
    *   **Kopce (Heaps):** Specjalny typ drzewa binarnego używany do implementacji kolejek priorytetowych.
    *   **Drzewa wyrażeń:** Reprezentacja wyrażeń arytmetycznych, gdzie liście to liczby, a węzły wewnętrzne to operatory.
    *   **Drzewa Huffmana:** Używane w algorytmach kompresji danych.

**Drzewa n-arne (k-arne)**

*   **Charakterystyka:** To uogólnienie drzew binarnych, w którym węzeł może mieć **dowolną, ale ograniczoną (do `n`) liczbę dzieci**. Węzeł przechowuje wtedy listę lub tablicę wskaźników do swoich dzieci.
*   **Sposoby implementacji:** Podobnie jak drzewa binarne, za pomocą struktur, ale zamiast dwóch wskaźników, węzeł zawiera kolekcję (np. listę, wektor) wskaźników na dzieci.

*   **Szczególny typ: B-Drzewa (B-Trees)**
    *   To specjalny, **zrównoważony** typ drzewa n-arnego, zoptymalizowany pod kątem systemów, które odczytują i zapisują duże bloki danych – czyli **systemów plików i baz danych**.
    *   Węzły w B-drzewie mogą przechowywać **wiele kluczy** (a nie tylko jeden) i mają odpowiednio więcej dzieci. Dzięki temu drzewo jest bardzo "płaskie" i "szerokie" – ma bardzo małą wysokość. Ponieważ dostęp do dysku jest operacją bardzo wolną, minimalizacja wysokości drzewa (a więc liczby odczytów bloków dysku potrzebnych do znalezienia danych) jest kluczowa dla wydajności.

*   **Zastosowania drzew n-arnych:**
    *   **Systemy plików:** Struktura katalogów w systemie operacyjnym jest klasycznym przykładem drzewa n-arnego.
    *   **Bazy danych:** B-drzewa i ich warianty (B+ drzewa) są standardową strukturą używaną do implementacji indeksów bazodanowych.
    *   **Reprezentacja hierarchii:** Struktura organizacyjna firmy, drzewo genealogiczne, struktura dokumentu HTML (DOM).
    *   **Drzewa trie (drzewa prefiksowe):** Specjalny typ drzewa n-arnego używany do wydajnego przechowywania i wyszukiwania słów w słowniku (np. w systemach autouzupełniania).

**Porównanie**

| Cecha | Drzewo binarne | Drzewo n-arne |
|---|---|---|
| **Liczba dzieci** | Co najwyżej 2 | Co najwyżej `n` |
| **Implementacja węzła** | Wartość, wskaźnik lewy, wskaźnik prawy | Wartość, kolekcja wskaźników na dzieci |
| **Główne zastosowania** | BST, kopce, drzewa wyrażeń | Systemy plików, indeksy baz danych (B-drzewa), drzewa trie |
| **Optymalizacja** | Głównie dla operacji w pamięci RAM | B-drzewa są zoptymalizowane dla operacji dyskowych |


## 25. Algorytmy rekurencyjne vs algorytmy iteracyjne, porównanie i omówienie podstawowych założeń konstrukcyjnych.

### Szczegółowe wyjaśnienie

Rekurencja i iteracja to dwa fundamentalnie różne podejścia do rozwiązywania problemów, które polegają na wielokrotnym wykonywaniu pewnego zestawu operacji. Wybór między nimi to klasyczny kompromis między elegancją i czytelnością kodu a wydajnością i zużyciem pamięci.

**Algorytmy iteracyjne**

*   **Założenia konstrukcyjne:** Iteracja polega na jawnym, wielokrotnym powtarzaniu bloku kodu za pomocą **konstrukcji pętli** (`for`, `while`, `do-while`). Stan algorytmu jest przechowywany w zmiennych, które są modyfikowane w każdej iteracji pętli. Pętla wykonuje się tak długo, aż zostanie spełniony określony warunek zakończenia.

*   **Przykład (obliczanie silni):**
    ```
    function silnia_iteracyjnie(n) {
      let wynik = 1;
      for (let i = 2; i <= n; i++) {
        wynik = wynik * i;
      }
      return wynik;
    }
    ```

*   **Charakterystyka:**
    *   **Stan:** Jawnie zarządzany przez programistę w zmiennych (np. `wynik`, `i`).
    *   **Zakończenie:** Pętla kończy się, gdy warunek (np. `i <= n`) staje się fałszywy.
    *   **Złożoność pamięciowa:** Zazwyczaj O(1) (stała), ponieważ używamy tylko kilku zmiennych, niezależnie od rozmiaru problemu.
    *   **Wydajność:** Zwykle szybsze od rekurencji, ponieważ unika się narzutu związanego z wielokrotnym wywoływaniem funkcji.

**Algorytmy rekurencyjne (rekursyjne)**

*   **Założenia konstrukcyjne:** Rekurencja to technika, w której funkcja **wywołuje samą siebie** w celu rozwiązania mniejszej wersji tego samego problemu. Kluczowe jest zdefiniowanie dwóch przypadków:
    1.  **Przypadek bazowy (warunek stopu):** Najprostsza wersja problemu, którą można rozwiązać bezpośrednio, bez dalszych wywołań rekurencyjnych. Jest to absolutnie niezbędne, aby zapobiec nieskończonej pętli wywołań.
    2.  **Krok rekurencyjny:** Definiuje, jak sprowadzić większy problem do mniejszej, prostszej instancji tego samego problemu.

*   **Przykład (obliczanie silni):**
    ```
    function silnia_rekurencyjnie(n) {
      // Przypadek bazowy
      if (n <= 1) {
        return 1;
      }
      // Krok rekurencyjny
      return n * silnia_rekurencyjnie(n - 1);
    }
    ```

*   **Charakterystyka:**
    *   **Stan:** Niejawnie zarządzany na **stosie wywołań (call stack)**. Każde wywołanie funkcji odkłada na stosie swoje parametry i zmienne lokalne.
    *   **Zakończenie:** Wywołania kończą się, gdy osiągnięty zostanie przypadek bazowy.
    *   **Złożoność pamięciowa:** Zazwyczaj O(n), ponieważ każde wywołanie rekurencyjne zajmuje miejsce na stosie. Dla głębokiej rekurencji może to prowadzić do błędu **przepełnienia stosu (stack overflow)**.
    *   **Czytelność:** Kod rekurencyjny jest często bardziej elegancki, zwięzły i bliższy matematycznej definicji problemu. Jest to szczególnie widoczne w przypadku problemów, które mają naturalnie rekurencyjną strukturę (np. operacje na drzewach, algorytmy "dziel i zwyciężaj").

**Porównanie: Rekurencja vs Iteracja**

| Cecha | Algorytm iteracyjny | Algorytm rekurencyjny |
|---|---|---|
| **Mechanizm** | Pętle (`for`, `while`) | Wywołania funkcji przez samą siebie |
| **Złożoność czasowa** | Zwykle taka sama jak w rekurencji | Zwykle taka sama jak w iteracji (ale z większym narzutem) |
| **Złożoność pamięciowa** | **O(1)** (stała) | **O(n)** (liniowa, zależy od głębokości rekursji) |
| **Wydajność** | **Wyższa** (brak narzutu na wywołania funkcji) | **Niższa** (narzut na zarządzanie stosem wywołań) |
| **Ryzyko** | Nieskończona pętla (jeśli warunek stopu jest błędny) | **Przepełnienie stosu (stack overflow)** dla dużych `n` |
| **Czytelność kodu** | Może być bardziej złożony i mniej intuicyjny | Często **bardziej elegancki i łatwiejszy do zrozumienia** dla problemów o rekurencyjnej naturze |

**Kiedy czego używać?**

*   **Użyj iteracji, gdy:**
    *   Wydajność i zużycie pamięci są krytyczne.
    *   Problem ma naturalnie iteracyjną strukturę (np. proste przeglądanie listy).
    *   Istnieje ryzyko głębokiej rekurencji, która mogłaby spowodować przepełnienie stosu.

*   **Użyj rekurencji, gdy:**
    *   Problem ma naturalnie rekurencyjną definicję (np. algorytmy "dziel i zwyciężaj" jak Merge Sort, operacje na drzewach, liczby Fibonacciego).
    *   Czytelność i prostota kodu są ważniejsze niż maksymalna wydajność.
    *   Głębokość rekurencji jest ograniczona i nie ma ryzyka przepełnienia stosu.

Każdy algorytm rekurencyjny można przepisać na wersję iteracyjną (czasem wymaga to użycia własnej struktury stosu do symulowania rekurencji), ale często odbywa się to kosztem czytelności kodu.


---

# Odpowiedzi "to the point" na obronę

## 21. Szacowanie złożoności algorytmów, klasy złożoności problemów algorytmicznych.

Złożoność algorytmów opisuje, jak rośnie ich zapotrzebowanie na czas i pamięć wraz ze wzrostem rozmiaru danych. Używamy do tego **notacji O**, która określa górną granicę tempa wzrostu w najgorszym przypadku, np. O(n) dla złożoności liniowej czy O(log n) dla logarytmicznej. Problemy algorytmiczne klasyfikujemy na klasy złożoności. Klasa **P** to problemy "łatwe", rozwiązywalne w czasie wielomianowym. Klasa **NP** to problemy, których rozwiązanie można szybko zweryfikować. **NP-zupełne** to najtrudniejsze problemy w NP. Najważniejsze pytanie informatyki, **"Czy P=NP?"**, pozostaje nierozwiązane.

## 22. Najważniejsze algorytmy wyszukiwania i sortowania, przegląd i zastosowania.

Dwa podstawowe algorytmy wyszukiwania to **liniowe** (O(n)), które działa na każdym zbiorze, oraz **binarne** (O(log n)), które jest znacznie szybsze, ale wymaga posortowanych danych. Wśród algorytmów sortowania wyróżniamy proste, ale wolne, jak **sortowanie bąbelkowe** (O(n²)), oraz wydajne, oparte na strategii "dziel i zwyciężaj", jak **Merge Sort** i **Quick Sort** (oba o średniej złożoności O(n log n)). Quick Sort jest w praktyce jednym z najszybszych, a Merge Sort jest stabilny i używany do sortowania zewnętrznego.

## 23. Charakterystyka i zastosowania podstawowych struktur danych: stos, kolejka, kolejka priorytetowa, struktura Find-Union, słownik.

*   **Stos (LIFO):** Działa jak stos talerzy. Używany do zarządzania wywołaniami funkcji i w algorytmie DFS.
*   **Kolejka (FIFO):** Działa jak kolejka w sklepie. Używana do zarządzania zadaniami i w algorytmie BFS.
*   **Kolejka priorytetowa:** Usuwa element o najwyższym priorytecie. Implementowana jako kopiec, kluczowa w algorytmach Dijkstry i Prima.
*   **Find-Union (DSU):** Zarządza zbiorami rozłącznymi. Używana do szybkiego wykrywania cykli w grafach i w algorytmie Kruskala.
*   **Słownik (Hash Table):** Przechowuje pary klucz-wartość z dostępem w czasie O(1). Jedna z najczęściej używanych struktur, np. do cachowania i implementacji obiektów.

## 24. Drzewa binarne i drzewa n-arne w algorytmice. Charakterystyka, sposoby implementacji i zastosowania.

Drzewa to hierarchiczne struktury danych. **Drzewa binarne**, gdzie węzeł ma do dwojga dzieci, są fundamentem algorytmiki. Ich specjalny typ, **Binarne Drzewo Poszukiwań (BST)**, pozwala na szybkie wyszukiwanie, wstawianie i usuwanie (O(log n) dla drzew zrównoważonych). **Drzewa n-arne** uogólniają tę koncepcję na `n` dzieci. Ich najważniejszym wariantem są **B-drzewa**, które dzięki dużej liczbie kluczy w węźle minimalizują wysokość drzewa i są standardem w implementacji **indeksów baz danych i systemów plików**.

## 25. Algorytmy rekurencyjne vs algorytmy iteracyjne, porównanie i omówienie podstawowych założeń konstrukcyjnych.

**Iteracja** używa pętli (`for`, `while`) i jawnie zarządza stanem w zmiennych. Ma stałą złożoność pamięciową (O(1)) i jest zazwyczaj szybsza. **Rekurencja** polega na wywoływaniu funkcji przez samą siebie i niejawnym zarządzaniu stanem na stosie wywołań. Jej kod jest często bardziej elegancki, ale ma liniową złożoność pamięciową (O(n)), co grozi **przepełnieniem stosu**. Wybór zależy od problemu: rekurencja jest naturalna dla algorytmów "dziel i zwyciężaj" i operacji na drzewach, a iteracja jest bezpieczniejsza i wydajniejsza dla prostych powtórzeń.

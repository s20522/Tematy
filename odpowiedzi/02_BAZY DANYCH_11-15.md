# Odpowiedzi na pytania do obrony pracy inżynierskiej - Bazy Danych

## 11. Podstawowe cechy relacyjnych baz danych.

### Szczegółowe wyjaśnienie

Relacyjne bazy danych, od czasu ich teoretycznego opracowania przez Edgara F. Codda w 1970 roku, stały się absolutnym standardem w przechowywaniu i zarządzaniu danymi. Ich sukces opiera się na kilku kluczowych cechach, które razem tworzą spójny i niezawodny system.

**1. Struktura oparta na relacjach (tabelach)**

Podstawową i najbardziej charakterystyczną cechą jest to, że wszystkie dane przechowywane są w **relacjach**, które dla użytkownika wyglądają jak proste, dwuwymiarowe **tabele**. Każda tabela składa się z:
*   **Wierszy (rekordów, krotek):** Reprezentują pojedyncze obiekty lub zdarzenia, np. jednego konkretnego studenta, jeden produkt, jedno zamówienie.
*   **Kolumn (atrybutów, pól):** Opisują cechy tych obiektów, np. imię studenta, cena produktu, data zamówienia. Każda kolumna ma ściśle określony **typ danych** (np. tekst, liczba, data), co zapewnia porządek i integralność.

Ten model jest bardzo intuicyjny i łatwy do zrozumienia dla człowieka, przypominając arkusz kalkulacyjny.

**2. Integralność danych zapewniana przez klucze**

Model relacyjny wprowadza mechanizmy, które pilnują, aby dane były poprawne i spójne. Służą do tego głównie klucze:
*   **Klucz podstawowy (Primary Key):** To jedna lub więcej kolumn, których wartość **jednoznacznie identyfikuje każdy wiersz** w tabeli. Wartości w tej kolumnie nie mogą się powtarzać i nie mogą być puste (NULL). Dzięki niemu mamy pewność, że nie ma dwóch identycznych rekordów, np. dwóch studentów o tym samym numerze albumu.
*   **Klucz obcy (Foreign Key):** To kolumna (lub zestaw kolumn) w jednej tabeli, która odwołuje się do klucza podstawowego w innej tabeli. Klucz obcy jest fundamentem **tworzenia powiązań (relacji)** między tabelami. Zapewnia on **integralność referencyjną** – pilnuje, aby nie można było np. złożyć zamówienia dla klienta, który nie istnieje w tabeli klientów.

**3. Język SQL jako standardowy interfejs**

Do komunikacji z relacyjną bazą danych służy ustandaryzowany język **SQL (Structured Query Language)**. Niezależnie od tego, czy pracujemy z PostgreSQL, MySQL, Oracle czy SQL Server, podstawowe polecenia SQL będą takie same. SQL pozwala na definiowanie struktury bazy (tworzenie tabel), manipulowanie danymi (dodawanie, modyfikowanie, usuwanie) oraz, co najważniejsze, na zadawanie złożonych zapytań w celu odczytania danych.

**4. Właściwości ACID dla transakcji**

Systemy zarządzania relacyjnymi bazami danych (RDBMS) gwarantują, że operacje na danych, zwłaszcza te składające się z wielu kroków (nazywane **transakcjami**), będą wykonane w sposób niezawodny. Gwarancję tę opisuje akronim **ACID**:
*   **Atomicity (Atomowość):** Transakcja jest niepodzielna – albo wszystkie jej operacje wykonają się poprawnie, albo żadna. Jeśli w trakcie przelewu bankowego (wyciągnięcie z jednego konta, dodanie na drugie) nastąpi błąd, cała operacja jest wycofywana. Nie ma możliwości, żeby pieniądze "zniknęły".
*   **Consistency (Spójność):** Transakcja zawsze przeprowadza bazę danych z jednego spójnego stanu w drugi spójny stan. Oznacza to, że po zakończeniu transakcji wszystkie reguły integralności (np. klucze obce, ograniczenia) muszą być spełnione.
*   **Isolation (Izolacja):** Transakcje wykonywane współbieżnie (w tym samym czasie) są od siebie odizolowane. Z punktu widzenia jednej transakcji wygląda to tak, jakby była jedyną operacją wykonywaną w danym momencie na bazie danych. Zapobiega to problemom, gdy wiele osób naraz próbuje modyfikować te same dane.
*   **Durability (Trwałość):** Gdy transakcja zostanie pomyślnie zakończona (zatwierdzona), jej wyniki są trwale zapisane i nie zostaną utracone, nawet w przypadku awarii systemu (np. nagłego braku zasilania).

**5. Normalizacja danych**

Model relacyjny promuje proces **normalizacji**, czyli organizowania kolumn i tabel w bazie danych w taki sposób, aby zminimalizować **redundancję (powtarzanie się) danych**. Celem jest, aby każda informacja była przechowywana tylko w jednym miejscu. Np. zamiast w każdym zamówieniu przechowywać pełny adres klienta, przechowujemy tylko jego identyfikator (klucz obcy), a adres znajduje się w tabeli klientów. Normalizacja zapobiega anomaliom przy modyfikacji danych i oszczędza miejsce.


## 12. Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych.

### Szczegółowe wyjaśnienie

**Diagram Związków Encji (ERD - Entity-Relationship Diagram)**

Diagram związków encji to **graficzny, koncepcyjny model danych**. Jest to wizualny plan, który tworzy się na samym początku projektowania bazy danych, jeszcze zanim napiszemy choćby jedną linijkę kodu SQL. Jego celem jest zidentyfikowanie najważniejszych obiektów w systemie, ich cech oraz powiązań między nimi. Służy jako uniwersalny język komunikacji między analitykami, programistami a klientem, pozwalając upewnić się, że wszyscy tak samo rozumieją logikę biznesową systemu.

**Podstawowe elementy ERD:**

1.  **Encja (Entity):**
    *   Reprezentuje klasę obiektów (rzeczywistych lub abstrakcyjnych), o których chcemy przechowywać informacje. Encja to "coś", co da się jednoznacznie zidentyfikować.
    *   Przykłady: `Student`, `Wykładowca`, `Kurs`, `Samochód`, `Zamówienie`.
    *   Na diagramie przedstawiana jest zazwyczaj jako **prostokąt** z nazwą w środku.

2.  **Atrybut (Attribute):**
    *   Reprezentuje pojedynczą cechę lub właściwość danej encji.
    *   Przykłady: Dla encji `Student` atrybutami mogą być `Imię`, `Nazwisko`, `NumerAlbumu`, `DataUrodzenia`.
    *   Na diagramie przedstawiany jest jako **elipsa** połączona z encją. Często atrybut, który będzie kluczem podstawowym, jest podkreślony.

3.  **Związek (Relationship):**
    *   Opisuje powiązanie lub interakcję między dwiema (lub więcej) encjami.
    *   Przykłady: `Student` **zapisuje się na** `Kurs`; `Wykładowca` **prowadzi** `Kurs`; `Klient` **składa** `Zamówienie`.
    *   Na diagramie przedstawiany jest jako **romb** łączący powiązane encje.

**Krotność (Liczebność) Związku:**

To kluczowy element opisu związku, który precyzuje, ile instancji jednej encji może być powiązanych z ile instancjami drugiej. Wyróżniamy trzy główne typy:

*   **Jeden do jednego (1:1):** Jedna instancja encji A jest powiązana z co najwyżej jedną instancją encji B (i na odwrót). Przykład: `Mąż` - `Żona` (w systemie monogamicznym), `Kraj` - `Stolica`.
*   **Jeden do wielu (1:N):** Jedna instancja encji A może być powiązana z wieloma instancjami encji B, ale jedna instancja B jest powiązana z tylko jedną instancją A. To najczęstszy typ związku. Przykład: `Wykładowca` - `Kurs` (jeden wykładowca prowadzi wiele kursów, ale kurs jest prowadzony przez jednego wykładowcę).
*   **Wiele do wielu (N:M):** Wiele instancji encji A może być powiązanych z wieloma instancjami encji B. Przykład: `Student` - `Kurs` (jeden student może zapisać się na wiele kursów, a na jeden kurs może być zapisanych wielu studentów). W relacyjnych bazach danych związki N:M są implementowane za pomocą dodatkowej **tabeli łączącej**.

**Zasady prawidłowego projektowania schematów bazy danych**

Stworzenie dobrego schematu bazy danych to sztuka kompromisu, ale opiera się na kilku fundamentalnych zasadach, które mają na celu zapewnienie integralności, wydajności i elastyczności.

1.  **Unikaj redundancji (powielania danych):** To najważniejsza zasada. Każda informacja powinna być przechowywana tylko w jednym miejscu. Jeśli adres klienta jest zapisany w 100 jego zamówieniach, to zmiana adresu wymaga aktualizacji 100 rekordów, co jest nieefektywne i grozi niespójnością. Rozwiązaniem jest **normalizacja**.

2.  **Stosuj normalizację:** Normalizacja to formalny proces dekompozycji tabel w celu eliminacji redundancji i anomalii (problemów przy wstawianiu, aktualizacji i usuwaniu danych). Najczęściej stosuje się trzy pierwsze postacie normalne:
    *   **Pierwsza postać normalna (1NF):** Wszystkie atrybuty w tabeli muszą być atomowe (niepodzielne), a tabela nie może zawierać grup powtarzających się. Np. nie tworzymy kolumn `Telefon1`, `Telefon2` - zamiast tego tworzymy osobną tabelę `Telefony` powiązaną ze studentem.
    *   **Druga postać normalna (2NF):** Tabela musi być w 1NF, a wszystkie atrybuty niekluczowe muszą w pełni zależeć od *całego* klucza podstawowego (dotyczy kluczy złożonych z wielu kolumn).
    *   **Trzecia postać normalna (3NF):** Tabela musi być w 2NF, a wszystkie atrybuty niekluczowe muszą zależeć *tylko* od klucza podstawowego, a nie od innych atrybutów niekluczowych.

3.  **Używaj kluczy konsekwentnie:** Każda tabela musi mieć swój klucz podstawowy. Do tworzenia powiązań używaj kluczy obcych, które odwołują się do kluczy podstawowych. Nadawaj kluczom spójne i zrozumiałe nazwy (np. `StudentID` w tabeli `Studenci` i `StudentID` jako klucz obcy w tabeli `Zapisy`).

4.  **Wybieraj odpowiednie typy danych:** Używaj najbardziej restrykcyjnego typu danych, który pasuje do informacji (np. `DATE` dla daty, a nie `VARCHAR`). Zapewnia to integralność danych i oszczędza miejsce.

5.  **Dokumentuj schemat:** Stworzony diagram ERD oraz dodatkowe opisy tabel i kolumn są bezcenną dokumentacją, która ułatwia zrozumienie i rozwój bazy danych w przyszłości.

6.  **Myśl o przyszłości, ale nie przesadzaj (YAGNI - You Ain't Gonna Need It):** Projektuj schemat tak, aby był elastyczny i pozwalał na przyszły rozwój, ale unikaj tworzenia nadmiarowych tabel i kolumn "na zapas", jeśli nie ma pewności, że będą potrzebne. Zawsze można rozszerzyć schemat w przyszłości.


## 13. Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych.

### Szczegółowe wyjaśnienie

**Problem współbieżności**

Systemy baz danych są z natury systemami wielodostępowymi – oznacza to, że w tym samym czasie wielu użytkowników (lub wiele aplikacji) może próbować odczytywać i modyfikować te same dane. Ta jednoczesna aktywność, nazywana **współbieżnością**, jest pożądana, ale rodzi też poważne problemy. Gdyby system na to pozwalał bez żadnej kontroli, mogłoby dojść do chaosu i uszkodzenia danych. 

Wyobraźmy sobie prostą sytuację: dwie osoby w tym samym momencie próbują zarezerwować ostatnie miejsce w kinie. Obie odczytują informację, że jest jedno wolne miejsce. Obie dokonują rezerwacji. W efekcie sprzedano dwa bilety na jedno miejsce, a baza danych jest w stanie niespójnym. 

Aby temu zapobiec, systemy zarządzania bazami danych (RDBMS) implementują zaawansowane **mechanizmy kontroli współbieżności**. Ich głównym celem jest zapewnienie **izolacji** transakcji, czyli stworzenie iluzji, że każda transakcja działa na bazie danych samotnie, bez zakłóceń ze strony innych.

**Główne metody kontroli współbieżności**

Istnieją dwa fundamentalnie różne podejścia do zarządzania współbieżnością:

**1. Blokowanie pesymistyczne (Pessimistic Locking)**

*   **Idea:** To podejście jest "pesymistyczne" – zakłada, że konflikty będą się zdarzać często, więc lepiej im zapobiegać z góry. Zanim transakcja zacznie modyfikować jakieś dane (wiersz, tabelę), musi najpierw założyć na nie **blokadę (lock)**.
*   **Rodzaje blokad:**
    *   **Blokada na odczyt (Shared Lock, S):** Kilka transakcji może jednocześnie posiadać blokadę na odczyt tych samych danych. Pozwala to wielu użytkownikom naraz czytać te same informacje.
    *   **Blokada na zapis (Exclusive Lock, X):** Tylko jedna transakcja może w danym momencie posiadać blokadę na zapis. Co więcej, jeśli na danych jest jakakolwiek blokada (nawet na odczyt), żadna inna transakcja nie może uzyskać blokady na zapis, dopóki poprzednie blokady nie zostaną zwolnione. 
*   **Działanie:** Gdy transakcja chce zmodyfikować dane, prosi o blokadę X. Jeśli dane są już zablokowane przez inną transakcję, musi **czekać**, aż blokada zostanie zwolniona. Dane są odblokowywane dopiero po zakończeniu transakcji (zatwierdzeniu lub wycofaniu).
*   **Zalety:** Gwarantuje wysoką spójność. Jest to bezpieczny i sprawdzony mechanizm.
*   **Wady:** Może prowadzić do obniżenia wydajności, gdy wiele transakcji czeka na zwolnienie blokad. Może też prowadzić do **zakleszczeń (deadlocks)**.

**Zakleszczenie (Deadlock):** To sytuacja, w której dwie (lub więcej) transakcje wzajemnie na siebie czekają. Transakcja A zablokowała zasób X i czeka na zasób Y, podczas gdy transakcja B zablokowała zasób Y i czeka na zasób X. Żadna z nich nie może kontynuować. Systemy baz danych potrafią wykrywać zakleszczenia i automatycznie rozwiązują je, **wycofując jedną z transakcji** (tzw. "ofiarę").

**2. Blokowanie optymistyczne / Wersjonowanie (Optimistic Locking / MVCC)**

*   **Idea:** To podejście jest "optymistyczne" – zakłada, że konflikty zdarzają się rzadko, więc nie ma sensu blokować danych i spowalniać systemu. Pozwólmy wszystkim pracować, a konfliktami zajmiemy się tylko wtedy, gdy faktycznie wystąpią.
*   **Działanie (MVCC - Multi-Version Concurrency Control):** To najpopularniejsza implementacja blokowania optymistycznego. Zamiast nadpisywać dane, baza danych przechowuje **wiele wersji** tego samego wiersza. Gdy transakcja rozpoczyna pracę, dostaje "migawkę" (snapshot) bazy danych z tego momentu. Odczyty nie blokują zapisów, a zapisy nie blokują odczytów, ponieważ każda transakcja pracuje na swojej własnej, spójnej wersji danych. Dopiero w momencie próby zatwierdzenia zmian, system sprawdza, czy w międzyczasie inna transakcja nie zmodyfikowała tych samych danych. Jeśli tak – wystąpił konflikt, a transakcja, która próbowała zapisać dane jako druga, jest **wycofywana** i musi spróbować ponownie.
*   **Zalety:** Znacznie wyższa współbieżność, zwłaszcza w systemach, gdzie jest dużo odczytów. Czytelnicy nie blokują pisarzy i pisarze nie blokują czytelników.
*   **Wady:** Większy narzut na przechowywanie wielu wersji danych. Może prowadzić do "głodzenia" transakcji, które są ciągle wycofywane z powodu konfliktów.

**Poziomy Izolacji Transakcji**

Standard SQL definiuje cztery poziomy izolacji, które są kompromisem między wydajnością a spójnością. Im wyższy poziom, tym większa ochrona przed anomaliami, ale potencjalnie mniejsza współbieżność.

1.  **Read Uncommitted:** Najniższy poziom. Transakcja może odczytać dane, które zostały zmodyfikowane przez inną transakcję, ale **jeszcze niezatwierdzone** (tzw. "brudny odczyt"). Rzadko stosowany.
2.  **Read Committed:** Domyślny poziom w wielu bazach (np. PostgreSQL, SQL Server). Gwarantuje, że transakcja widzi tylko zatwierdzone zmiany. Zapobiega "brudnym odczytom", ale wciąż mogą wystąpić inne anomalie (np. "niepowtarzalny odczyt" - dwukrotny odczyt tych samych danych w tej samej transakcji może dać różne wyniki).
3.  **Repeatable Read:** Gwarantuje, że jeśli transakcja odczyta dane, to ponowny odczyt tych samych danych w tej samej transakcji zawsze zwróci tę samą wartość, nawet jeśli inne transakcje w międzyczasie je zmodyfikowały i zatwierdziły. Wciąż możliwe są tzw. "odczyty fantomowe".
4.  **Serializable:** Najwyższy, najbardziej restrykcyjny poziom. Gwarantuje pełną izolację. Działanie transakcji jest równoważne wykonaniu ich po kolei (szeregowo). Eliminuje wszystkie anomalie, ale kosztem najniższej współbieżności.


## 14. Podstawowe obiekty, konstrukcje i znaczenie języka SQL.

### Szczegółowe wyjaśnienie

**Znaczenie języka SQL**

SQL (Structured Query Language) to **deklaratywny język zapytań**, który jest standardowym, uniwersalnym interfejsem do komunikacji z relacyjnymi bazami danych. Jego znaczenie jest fundamentalne – to właśnie SQL pozwala użytkownikom i aplikacjom definiować, manipulować i odpytywać dane w sposób niezależny od konkretnego systemu zarządzania bazą danych (np. PostgreSQL, MySQL, Oracle).

"Deklaratywność" SQL oznacza, że użytkownik **określa, *co* chce uzyskać**, a nie *jak* system ma to zrobić. Mówimy "daj mi listę studentów z Krakowa", a optymalizator zapytań w bazie danych sam decyduje, w jaki sposób najefektywniej te dane odnaleźć i zwrócić.

**Podział języka SQL**

Język SQL dzieli się na kilka podjęzyków, w zależności od przeznaczenia poleceń:

1.  **DDL (Data Definition Language) - Język Definicji Danych:**
    *   Służy do definiowania i zarządzania strukturą bazy danych i jej obiektami.
    *   **`CREATE`**: Tworzy nowe obiekty. Najważniejsze to `CREATE DATABASE` (tworzy nową bazę) i `CREATE TABLE` (tworzy nową tabelę, definiując jej kolumny, typy danych i ograniczenia).
    *   **`ALTER`**: Modyfikuje istniejące obiekty, np. `ALTER TABLE` pozwala dodawać, usuwać lub modyfikować kolumny w tabeli.
    *   **`DROP`**: Usuwa obiekty z bazy danych, np. `DROP TABLE` trwale usuwa tabelę wraz ze wszystkimi danymi.

2.  **DML (Data Manipulation Language) - Język Manipulacji Danymi:**
    *   Służy do pracy na danych przechowywanych w tabelach.
    *   **`SELECT`**: To najważniejsze i najczęściej używane polecenie. Służy do odpytywania i pobierania danych z bazy. Jest to serce SQL.
    *   **`INSERT`**: Dodaje nowe wiersze (rekordy) do tabeli.
    *   **`UPDATE`**: Modyfikuje istniejące dane w tabeli.
    *   **`DELETE`**: Usuwa wiersze z tabeli.

3.  **DCL (Data Control Language) - Język Kontroli Danych:**
    *   Służy do zarządzania uprawnieniami i dostępem do bazy danych.
    *   **`GRANT`**: Nadaje użytkownikom uprawnienia do wykonywania określonych operacji (np. `GRANT SELECT ON Studenci TO 'user1'`).
    *   **`REVOKE`**: Odbiera nadane wcześniej uprawnienia.

4.  **TCL (Transaction Control Language) - Język Kontroli Transakcji:**
    *   Służy do zarządzania transakcjami.
    *   **`COMMIT`**: Trwale zatwierdza wszystkie zmiany wykonane w ramach bieżącej transakcji.
    *   **`ROLLBACK`**: Wycofuje wszystkie zmiany wykonane w ramach bieżącej transakcji.
    *   **`SAVEPOINT`**: Ustawia punkt kontrolny wewnątrz transakcji, do którego można się później cofnąć.

**Podstawowe obiekty w bazie danych**

SQL operuje na różnych obiektach, z których najważniejsze to:

*   **Tabela (Table):** Podstawowy obiekt przechowujący dane w formie wierszy i kolumn.
*   **Widok (View):** Wirtualna tabela, która jest wynikiem zapytania `SELECT`. Nie przechowuje fizycznie danych, ale jest zapisanym zapytaniem, które można odpytywać jak zwykłą tabelę. Używany do upraszczania skomplikowanych zapytań, ukrywania złożoności schematu lub ograniczania dostępu do danych.
*   **Indeks (Index):** Specjalna struktura danych (najczęściej B-drzewo), która przyspiesza wyszukiwanie danych w tabeli. Działa jak skorowidz w książce – pozwala szybko zlokalizować wiersze spełniające określone warunki, bez potrzeby skanowania całej tabeli.
*   **Sekwencja (Sequence):** Obiekt generujący unikalne, kolejne numery, często używany do automatycznego tworzenia wartości dla kluczy podstawowych.
*   **Procedura składowana (Stored Procedure):** Zestaw poleceń SQL zapisany pod jedną nazwą w bazie danych. Może przyjmować parametry i być wywoływany przez aplikację. Pozwala na hermetyzację logiki biznesowej i zmniejszenie ruchu sieciowego.

**Podstawowe konstrukcje w zapytaniu `SELECT`**

Zapytanie `SELECT` jest najbardziej rozbudowanym poleceniem i składa się z wielu klauzul, które są przetwarzane w określonej kolejności:

1.  **`FROM`**: Wskazuje tabelę (lub tabele), z których pobieramy dane.
2.  **`JOIN`**: Służy do łączenia danych z wielu tabel na podstawie powiązań między nimi (np. `INNER JOIN`, `LEFT JOIN`).
3.  **`WHERE`**: Filtruje wiersze, pozostawiając tylko te, które spełniają określony warunek (np. `WHERE Miasto = 'Kraków'`).
4.  **`GROUP BY`**: Grupuje wiersze na podstawie wartości w określonej kolumnie, co pozwala na użycie **funkcji agregujących** (np. `COUNT`, `SUM`, `AVG`) dla każdej grupy.
5.  **`HAVING`**: Filtruje grupy utworzone przez `GROUP BY` (działa jak `WHERE`, ale dla grup).
6.  **`SELECT`**: Określa, które kolumny mają zostać zwrócone w wyniku.
7.  **`ORDER BY`**: Sortuje wynikowe wiersze rosnąco (`ASC`) lub malejąco (`DESC`).
8.  **`LIMIT` / `OFFSET`**: Ogranicza liczbę zwracanych wierszy i pozwala na implementację paginacji (stronicowania) wyników.


## 15. Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych.

### Szczegółowe wyjaśnienie

**Czym jest optymalizacja zapytań?**

Optymalizacja zapytań to proces, w którym system zarządzania bazą danych (RDBMS) stara się znaleźć **najbardziej efektywny sposób wykonania** danego zapytania SQL. Gdy wysyłamy do bazy deklaratywne zapytanie (mówiąc *co* chcemy dostać), **optymalizator zapytań (query optimizer)** analizuje je i generuje wiele możliwych **planów wykonania (execution plans)**. Plan wykonania to szczegółowa, proceduralna instrukcja, która krok po kroku opisuje, jak baza danych ma fizycznie uzyskać dostęp do danych (np. czy użyć indeksu, w jakiej kolejności połączyć tabele, jaki algorytm złączenia zastosować). Następnie, na podstawie wewnętrznych statystyk dotyczących danych, optymalizator szacuje **koszt** każdego planu (zwykle wyrażony w abstrakcyjnych jednostkach czasu i operacji I/O) i wybiera ten o najniższym koszcie.

Celem optymalizacji jest zminimalizowanie czasu odpowiedzi i zużycia zasobów (CPU, pamięć, I/O dyskowe).

**Znaczenie i rola indeksów**

**Indeksy są absolutnie kluczowym i najważniejszym narzędziem w optymalizacji zapytań.**

**Czym jest indeks?** Indeks to specjalna, dodatkowa struktura danych, która jest tworzona dla jednej lub więcej kolumn tabeli. Działa on analogicznie do **skorowidzu w książce**. Zamiast przeglądać całą książkę strona po stronie (co odpowiada **pełnemu skanowaniu tabeli - Full Table Scan**), aby znaleźć interesujące nas hasło, zaglądamy do posortowanego alfabetycznie skorowidzu, który natychmiast wskazuje nam numer strony. W bazie danych indeks przechowuje posortowane wartości z indeksowanej kolumny wraz ze wskaźnikami do fizycznej lokalizacji odpowiadających im wierszy na dysku.

**Jak działa indeks?** Najczęściej indeksy są implementowane jako **B-Drzewa (B-Trees)**. Jest to zrównoważona struktura drzewiasta, która pozwala na wyszukiwanie, wstawianie i usuwanie danych w czasie logarytmicznym (O(log n)). Dzięki temu, zamiast skanować miliony wierszy w tabeli, baza danych może zlokalizować poszukiwany wiersz po wykonaniu zaledwie kilku operacji odczytu, nawigując w dół drzewa indeksu.

**Kiedy stosować indeksy?**
Indeksy znacząco przyspieszają operacje, które filtrują lub sortują dane. Należy je zakładać przede wszystkim na kolumnach, które:
*   Są często używane w klauzuli **`WHERE`** do filtrowania danych.
*   Są używane do łączenia tabel w klauzuli **`JOIN`** (indeksy na kluczach obcych są absolutnie niezbędne!).
*   Są używane w klauzuli **`ORDER BY`** do sortowania wyników.

**Koszt indeksów:** Indeksy nie są darmowe. Zajmują dodatkowe miejsce na dysku i, co ważniejsze, **spowalniają operacje zapisu (`INSERT`, `UPDATE`, `DELETE`)**. Każda modyfikacja danych w tabeli wymaga również aktualizacji wszystkich powiązanych z nią indeksów. Dlatego sztuką jest znalezienie złotego środka – indeksowanie tylko tych kolumn, które przyniosą największy zysk przy odczycie, bez nadmiernego spowalniania zapisów.

**Rodzaje indeksów**

*   **Indeks jednokolumnowy / złożony:** Indeks może obejmować jedną kolumnę lub wiele kolumn (indeks złożony). Kolejność kolumn w indeksie złożonym ma kluczowe znaczenie.
*   **Indeks unikalny (Unique Index):** Gwarantuje, że wszystkie wartości w indeksowanej kolumnie (lub kombinacji kolumn) są unikalne. Klucze podstawowe automatycznie mają zakładany indeks unikalny.
*   **Indeks klastrowy (Clustered Index):** To specjalny typ indeksu, który **fizycznie sortuje wiersze danych na dysku** zgodnie z porządkiem indeksu. W efekcie sama tabela staje się indeksem. Może istnieć tylko jeden indeks klastrowy na tabelę. Zapewnia on błyskawiczny dostęp do danych przy wyszukiwaniu zakresów (np. `WHERE ID BETWEEN 100 AND 200`).
*   **Indeks nieklastrowy (Non-clustered Index):** To standardowy typ indeksu. Struktura indeksu jest oddzielona od fizycznych danych. Indeks zawiera wskaźniki do wierszy, które mogą być rozrzucone po całym dysku.

**Podstawowe zasady optymalizacji zapytań (z perspektywy programisty)**

Chociaż optymalizator jest bardzo inteligentny, możemy mu pomóc, pisząc "lepsze" zapytania:

1.  **`SELECT` tylko potrzebne kolumny:** Zamiast `SELECT *`, zawsze wymieniaj jawnie tylko te kolumny, których naprawdę potrzebujesz. Zmniejsza to ilość przesyłanych danych i może pozwolić na użycie tzw. "covering index" (indeksu pokrywającego), gdzie wszystkie potrzebne dane znajdują się już w samym indeksie, bez potrzeby sięgania do tabeli.
2.  **Unikaj funkcji na kolumnach w `WHERE`:** Zapytanie `WHERE YEAR(DataZamowienia) = 2023` uniemożliwi użycie indeksu na kolumnie `DataZamowienia`. Lepszym, **SARGable** (Search Argument-able) odpowiednikiem jest `WHERE DataZamowienia >= '2023-01-01' AND DataZamowienia < '2024-01-01'`, co pozwala na efektywne wykorzystanie indeksu.
3.  **Zapewnij odpowiednie indeksy:** Analizuj zapytania (używając narzędzia `EXPLAIN PLAN`, które pokazuje plan wykonania) i upewnij się, że kolumny używane w `WHERE`, `JOIN` i `ORDER BY` są odpowiednio zindeksowane.
4.  **Uważaj na `LIKE` z `_` lub `%` na początku:** Zapytanie `WHERE Nazwisko LIKE '%Kowalski'` również uniemożliwia użycie standardowego indeksu B-drzewa, ponieważ nie wiadomo, od jakiej litery zacząć poszukiwania. Wymusza to pełne skanowanie tabeli.
5.  **Pobieraj mniej danych:** Używaj `LIMIT` do paginacji wyników i filtruj dane jak najwcześniej (w klauzuli `WHERE`), aby kolejne operacje (łączenie, sortowanie) działały na mniejszym zbiorze danych.


---

# Odpowiedzi "to the point" na obronę

## 11. Podstawowe cechy relacyjnych baz danych.

Relacyjne bazy danych opierają się na modelu matematycznym, gdzie dane przechowuje się w **tabelach** (relacjach) składających się z wierszy i kolumn. Ich kluczowe cechy to: **integralność danych** zapewniana przez klucze podstawowe i obce, ustandaryzowany język zapytań **SQL** oraz gwarancja niezawodności operacji dzięki **transakcjom o właściwościach ACID** (Atomowość, Spójność, Izolacja, Trwałość). Model ten promuje również **normalizację**, czyli minimalizację powtarzania się danych.

## 12. Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych.

Diagram związków encji (ERD) to graficzny, koncepcyjny plan bazy danych. Jego podstawowe elementy to **encje** (obiekty, np. Student), **atrybuty** (cechy, np. Imię) oraz **związki** (powiązania między encjami, np. "zapisuje się na"). Znaczenie ERD polega na wizualizacji logiki biznesowej i ułatwieniu komunikacji przed implementacją. Główne zasady projektowania to: **unikanie redundancji danych** poprzez **normalizację** (do 3. postaci normalnej włącznie), konsekwentne stosowanie kluczy podstawowych i obcych oraz dobór odpowiednich typów danych.

## 13. Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych.

Mechanizm współbieżności zarządza jednoczesnym dostępem wielu użytkowników do tych samych danych, zapobiegając chaosowi i zapewniając ich spójność. Istnieją dwie główne strategie: **blokowanie pesymistyczne**, gdzie transakcja zakłada blokadę na dane przed ich modyfikacją, co zmusza innych do czekania, oraz **blokowanie optymistyczne (MVCC)**, gdzie baza przechowuje wiele wersji danych, a konflikty są wykrywane dopiero przy próbie zapisu. Poziom ochrony przed anomaliami regulują **poziomy izolacji transakcji**, z których najpopularniejszy to `Read Committed`.

## 14. Podstawowe obiekty, konstrukcje i znaczenie języka SQL.

SQL to standardowy, deklaratywny język do komunikacji z relacyjnymi bazami danych. Dzieli się na podjęzyki: **DDL** do definicji struktury (`CREATE`, `ALTER`), **DML** do manipulacji danymi (`SELECT`, `INSERT`, `UPDATE`, `DELETE`), **DCL** do zarządzania uprawnieniami (`GRANT`, `REVOKE`) i **TCL** do kontroli transakcji (`COMMIT`, `ROLLBACK`). Podstawowe obiekty to **tabele**, **widoki** i **indeksy**. Najważniejsza konstrukcja to zapytanie `SELECT`, które za pomocą klauzul `FROM`, `WHERE`, `GROUP BY`, `ORDER BY` i `JOIN` pozwala na filtrowanie, grupowanie, sortowanie i łączenie danych.

## 15. Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych.

Optymalizacja zapytań to proces, w którym baza danych wybiera najefektywniejszy **plan wykonania** zapytania. Kluczowym narzędziem są **indeksy** – specjalne struktury (najczęściej B-drzewa), które działają jak skorowidz w książce, pozwalając na błyskawiczne wyszukiwanie danych bez potrzeby skanowania całej tabeli. Indeksy zakłada się głównie na kolumnach używanych w klauzulach `WHERE`, `JOIN` i `ORDER BY`. Podstawowe zasady optymalizacji to: tworzenie odpowiednich indeksów, unikanie funkcji na kolumnach w `WHERE` oraz wybieranie w `SELECT` tylko potrzebnych kolumn zamiast `SELECT *`.

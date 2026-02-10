# Odpowiedzi na pytania do obrony pracy inżynierskiej - Inżynieria Oprogramowania

## 36. Zarządzanie projektem budowy oprogramowania: rodzaje działań, dobór metodyki oraz kontekst pozatechniczny.

### Szczegółowe wyjaśnienie

Zarządzanie projektem budowy oprogramowania to proces planowania, organizowania, prowadzenia i kontrolowania wszystkich działań związanych z wytworzeniem systemu informatycznego, od koncepcji do wdrożenia i utrzymania. Celem jest dostarczenie produktu, który spełnia wymagania klienta, mieści się w budżecie i zostaje ukończony w założonym czasie.

**Rodzaje działań w zarządzaniu projektem**

Niezależnie od wybranej metodyki, każdy projekt informatyczny obejmuje kilka kluczowych obszarów działań:

1.  **Zarządzanie zakresem (Scope Management):** Definiowanie, co dokładnie ma zostać zrobione, a co znajduje się poza zakresem projektu. Kluczowe jest unikanie tzw. "pełzania zakresu" (scope creep), czyli niekontrolowanego dodawania nowych funkcjonalności w trakcie trwania projektu.
2.  **Zarządzanie czasem (Time Management):** Planowanie i harmonogramowanie zadań, szacowanie czasu ich wykonania (estymacja), monitorowanie postępów i zarządzanie opóźnieniami. Tworzy się tu harmonogramy, np. w postaci wykresów Gantta.
3.  **Zarządzanie kosztami (Cost Management):** Szacowanie kosztów, tworzenie budżetu i kontrolowanie wydatków, aby nie przekroczyć założonych ram finansowych.
4.  **Zarządzanie jakością (Quality Management):** Definiowanie standardów jakości, planowanie i przeprowadzanie testów, przeglądy kodu – wszystko po to, aby finalny produkt był niezawodny i wolny od błędów.
5.  **Zarządzanie zasobami ludzkimi (Human Resource Management):** Budowanie zespołu projektowego, przydzielanie ról i odpowiedzialności, motywowanie i rozwiązywanie konfliktów.
6.  **Zarządzanie komunikacją (Communication Management):** Zapewnienie efektywnego przepływu informacji między wszystkimi interesariuszami projektu (zespołem, klientem, kierownictwem). Obejmuje to regularne spotkania, raportowanie postępów itp.
7.  **Zarządzanie ryzykiem (Risk Management):** Identyfikacja potencjalnych zagrożeń dla projektu (technicznych, biznesowych, organizacyjnych), ocena ich prawdopodobieństwa i wpływu oraz planowanie działań zapobiegawczych i naprawczych.
8.  **Zarządzanie zaopatrzeniem (Procurement Management):** Jeśli projekt wymaga zakupu sprzętu, oprogramowania lub usług od zewnętrznych dostawców, ten obszar zajmuje się procesem wyboru dostawców i zawierania umów.

**Dobór metodyki**

Metodyka to zbiór zasad, praktyk i procesów, które określają, w jaki sposób projekt będzie prowadzony. Wybór odpowiedniej metodyki jest jedną z najważniejszych decyzji i zależy od charakteru projektu. Dwie główne rodziny metodyk to:

1.  **Metodyki tradycyjne (kaskadowe, ang. Waterfall):**
    *   **Charakterystyka:** Proces jest podzielony na sekwencyjne, następujące po sobie fazy (np. analiza wymagań, projektowanie, implementacja, testowanie, wdrożenie). Przejście do następnej fazy jest możliwe dopiero po całkowitym zakończeniu poprzedniej.
    *   **Zalety:** Prosta, przewidywalna struktura, łatwe planowanie i kontrola, dokładna dokumentacja.
    *   **Wady:** Mała elastyczność, trudność we wprowadzaniu zmian, późne wykrywanie błędów, klient widzi produkt końcowy dopiero na samym końcu.
    *   **Kiedy stosować?** W projektach, gdzie **wymagania są bardzo dobrze znane, stabilne i mało prawdopodobne, że się zmienią**. Np. w projektach rządowych, militarnych, lub przy adaptacji istniejącego, dobrze zdefiniowanego systemu.

2.  **Metodyki zwinne (agile):**
    *   **Charakterystyka:** Podejście iteracyjno-przyrostowe. Projekt jest dzielony na krótkie cykle (iteracje, sprinty), trwające zwykle 1-4 tygodnie. W każdej iteracji zespół dostarcza mały, ale działający fragment oprogramowania. Kładzie się nacisk na bliską współpracę z klientem, szybkie dostosowywanie się do zmian i ciągłe doskonalenie.
    *   **Najpopularniejsze metodyki zwinne:**
        *   **Scrum:** Najbardziej popularna metodyka zwinna. Definiuje role (Product Owner, Scrum Master, Zespół Deweloperski), wydarzenia (Sprint, Planowanie Sprintu, Codzienny Scrum, Przegląd Sprintu, Retrospektywa Sprintu) i artefakty (Backlog Produktu, Backlog Sprintu). Jest to framework do zarządzania złożonymi projektami.
        *   **Kanban:** Koncentruje się na wizualizacji przepływu pracy (za pomocą tablicy Kanban) i ograniczaniu pracy w toku (WIP - Work In Progress). Celem jest maksymalizacja przepływu i minimalizacja czasu od rozpoczęcia do zakończenia zadania. Jest mniej restrykcyjny niż Scrum.
    *   **Zalety:** Duża elastyczność, szybkie dostosowywanie się do zmian, wczesne i częste dostarczanie wartości klientowi, lepsza jakość dzięki ciągłej integracji i testowaniu.
    *   **Wady:** Mniejsza przewidywalność w długim terminie, wymaga dużego zaangażowania klienta, ryzyko "pełzania zakresu" jeśli nie jest dobrze zarządzane.
    *   **Kiedy stosować?** W większości nowoczesnych projektów informatycznych, zwłaszcza tam, gdzie **wymagania są niepewne, mogą się często zmieniać**, a kluczowe jest szybkie dostarczenie produktu na rynek.

**Kontekst pozatechniczny**

Sukces projektu informatycznego rzadko zależy wyłącznie od technologii. Kontekst pozatechniczny jest równie, a często nawet bardziej, istotny.

*   **Biznesowy:** Jaki problem biznesowy rozwiązuje projekt? Jakie są cele biznesowe? Jaki jest zwrot z inwestycji (ROI)? Projekt musi mieć sens z perspektywy biznesowej, inaczej nie uzyska finansowania i wsparcia.
*   **Organizacyjny:** Jak projekt wpisuje się w strukturę i kulturę organizacji? Czy firma jest gotowa na zmianę, jaką wprowadzi nowy system? Czy kluczowi interesariusze (sponsorzy, przyszli użytkownicy) wspierają projekt?
*   **Ludzki:** Jakie są umiejętności i doświadczenie członków zespołu? Jakie są ich motywacje? Jak wygląda komunikacja i relacje w zespole? Dobry zespół potrafi przezwyciężyć problemy techniczne, ale zły zespół może zniweczyć nawet najprostszy projekt.
*   **Prawny i etyczny:** Czy projekt jest zgodny z przepisami prawa (np. RODO/GDPR)? Czy nie narusza praw autorskich? Czy jest etyczny? Ignorowanie tych aspektów może prowadzić do poważnych konsekwencji prawnych i wizerunkowych.

Efektywne zarządzanie projektem wymaga od Project Managera nie tylko wiedzy technicznej, ale przede wszystkim umiejętności miękkich: komunikacji, negocjacji, przywództwa i rozumienia szerokiego kontekstu, w którym projekt jest realizowany.


## 37. Język UML – charakterystyka oraz sposób wsparcia różnorodnych modeli danych.

### Szczegółowe wyjaśnienie

**Charakterystyka języka UML**

**UML (Unified Modeling Language)**, czyli Zunifikowany Język Modelowania, to standardowy, graficzny język służący do **wizualizacji, specyfikowania, konstruowania i dokumentowania** systemów informatycznych. UML nie jest metodyką programowania – nie mówi, *jak* projektować systemy. Jest to **notacja**, czyli zbiór zdefiniowanych symboli i reguł, która pozwala w jednoznaczny i zrozumiały sposób przedstawić projekt systemu.

Jego głównym celem jest dostarczenie wspólnego języka dla wszystkich interesariuszy projektu – analityków, projektantów, programistów i klientów – aby mogli oni efektywnie komunikować się na temat złożonego systemu.

**Kluczowe cechy UML:**

*   **Ujednolicony:** Powstał z połączenia trzech wcześniejszych, popularnych notacji obiektowych (Booch, OMT, OOSE), stając się uniwersalnym standardem.
*   **Wizualny:** Opiera się na diagramach, co ułatwia zrozumienie złożonych struktur i zależności, które byłyby trudne do opisania słowami.
*   **Niezależny od platformy i języka programowania:** Modele UML można tworzyć niezależnie od technologii, w której system zostanie zaimplementowany.
*   **Skalowalny:** Nadaje się zarówno do modelowania małych, jak i bardzo dużych, złożonych systemów.

**Rodzaje diagramów UML**

Diagramy UML dzielą się na dwie główne kategorie, które opisują system z różnych perspektyw:

1.  **Diagramy strukturalne (Structural Diagrams):** Pokazują **statyczną strukturę** systemu – jego komponenty i relacje między nimi. Odpowiadają na pytanie "Z czego składa się system?".
    *   **Diagram Klas (Class Diagram):** Najważniejszy diagram strukturalny. Przedstawia klasy, ich atrybuty, metody oraz relacje między nimi (asocjacje, agregacje, kompozycje, dziedziczenie). Jest to fundament modelowania obiektowego.
    *   **Diagram Komponentów (Component Diagram):** Pokazuje, jak system jest podzielony na fizyczne komponenty (np. pliki, biblioteki, moduły) i jakie są między nimi zależności.
    *   **Diagram Wdrożenia (Deployment Diagram):** Opisuje fizyczną architekturę systemu – na jakich serwerach (węzłach) będą uruchamiane poszczególne komponenty oprogramowania.
    *   **Diagram Obiektów (Object Diagram):** Pokazuje konkretne instancje klas (obiekty) i ich relacje w danym momencie czasu. Jest to jakby "migawka" systemu.

2.  **Diagramy behawioralne (zachowania, Behavioral Diagrams):** Pokazują **dynamiczne zachowanie** systemu – jak jego komponenty współpracują ze sobą w czasie. Odpowiadają na pytanie "Jak działa system?".
    *   **Diagram Przypadków Użycia (Use Case Diagram):** Przedstawia funkcjonalność systemu z perspektywy użytkownika (aktora). Pokazuje, jakie akcje (przypadki użycia) użytkownik może wykonać w systemie. Jest kluczowy na etapie zbierania wymagań.
    *   **Diagram Sekwencji (Sequence Diagram):** Pokazuje interakcje między obiektami w porządku chronologicznym. Doskonale nadaje się do modelowania przepływu sterowania w ramach jednego przypadku użycia.
    *   **Diagram Aktywności (Activity Diagram):** Przedstawia przepływ pracy (workflow) w systemie, podobnie do schematu blokowego. Modeluje kroki, decyzje i równoległe działania.
    *   **Diagram Stanów (State Machine Diagram):** Opisuje cykl życia jednego obiektu – wszystkie możliwe stany, w jakich może się znajdować, oraz przejścia między tymi stanami w odpowiedzi na zdarzenia.

**Sposób wsparcia różnorodnych modeli danych**

Chociaż UML jest językiem ogólnego przeznaczenia, doskonale nadaje się do modelowania danych na różnych poziomach abstrakcji i w różnych paradygmatach. Wsparcie to realizowane jest głównie przez **Diagram Klas**, ale także przez inne diagramy, które nadają mu kontekst.

1.  **Modelowanie konceptualne (Conceptual Data Modeling):**
    *   Na tym etapie skupiamy się na **pojęciach biznesowych** i relacjach między nimi, niezależnie od technologii. Celem jest zrozumienie domeny problemu.
    *   **Diagram Klas** jest tu używany do przedstawienia kluczowych encji biznesowych (jako klas), ich najważniejszych atrybutów oraz relacji (asocjacji) między nimi. Nie interesują nas jeszcze typy danych ani metody.
    *   **Przykład:** W systemie bibliotecznym modelujemy klasy `Książka`, `Czytelnik`, `Wypożyczenie` i relacje między nimi (np. `Czytelnik` *wypożycza* `Książkę`).

2.  **Modelowanie logiczne (Logical Data Modeling):**
    *   Na tym etapie przekształcamy model konceptualny w model, który może być zaimplementowany w konkretnym paradygmacie, np. w **relacyjnej bazie danych**.
    *   **Diagram Klas** jest nadal głównym narzędziem. Klasy z modelu konceptualnego są mapowane na tabele, atrybuty na kolumny, a asocjacje na klucze obce.
    *   UML pozwala na precyzyjne definiowanie **krotności relacji** (np. 1, 0..1, *), co jest kluczowe dla poprawnego zdefiniowania kluczy obcych i więzów integralności.
    *   Relacje dziedziczenia z modelu obiektowego można zamapować na model relacyjny na kilka sposobów (np. jedna tabela dla całej hierarchii, osobna tabela dla każdej klasy).
    *   UML można rozszerzać za pomocą **profili**. Istnieją specjalne profile UML (np. **Data Modeling Profile**), które dodają stereotypy (`<<Table>>`, `<<Column>>`, `<<PK>>`, `<<FK>>`) pozwalające na jeszcze bardziej precyzyjne modelowanie schematów baz danych bezpośrednio w UML.

3.  **Modelowanie fizyczne (Physical Data Modeling):**
    *   Na tym etapie model logiczny jest dostosowywany do konkretnego systemu zarządzania bazą danych (DBMS), np. PostgreSQL czy Oracle.
    *   W modelu UML (często przy użyciu profili) można już specyfikować konkretne typy danych dostępne w danym DBMS (np. `VARCHAR(255)`, `INTEGER`), definicje indeksów, ograniczeń (`constraints`) i innych fizycznych aspektów implementacji.

Podsumowując, UML, a w szczególności Diagram Klas, jest niezwykle elastycznym narzędziem, które wspiera cały proces modelowania danych – od wysokopoziomowego, biznesowego modelu konceptualnego, przez model logiczny, aż po szczegółowy model fizyczny gotowy do implementacji w bazie danych. Pozwala na płynne przejście od świata obiektów do świata relacji, zachowując spójność i czytelność projektu.



## 38. Wzorce projektowe oraz ramy programistyczne (frameworks) – charakterystyka, przykłady, zastosowania.

### Szczegółowe wyjaśnienie

Wzorce projektowe i frameworki to dwa fundamentalne koncepty w nowoczesnej inżynierii oprogramowania, które mają na celu przyspieszenie i ułatwienie procesu tworzenia aplikacji poprzez dostarczanie gotowych rozwiązań i struktur. Mimo że oba promują reużywalność kodu, pełnią zupełnie inne role.

**Wzorce projektowe (Design Patterns)**

*   **Charakterystyka:** Wzorzec projektowy to **uniwersalne, sprawdzone w praktyce, koncepcyjne rozwiązanie** często pojawiającego się, powtarzalnego problemu projektowego w danym kontekście. To nie jest gotowy fragment kodu, który można skopiować, ale raczej **opis, przepis lub schemat postępowania**, który pokazuje, jak zorganizować klasy i obiekty, aby rozwiązać dany problem w elegancki i elastyczny sposób. Wzorce dostarczają wspólnego słownictwa dla programistów, ułatwiając komunikację.

*   **Kategorie wzorców (wg "bandy czworga" - Gang of Four):**
    1.  **Kreacyjne (Creational):** Koncentrują się na procesie **tworzenia obiektów**, starając się uniezależnić system od tego, jak jego obiekty są tworzone, komponowane i reprezentowane.
        *   **Przykład: Fabryka (Factory Method):** Definiuje interfejs do tworzenia obiektu, ale pozwala podklasom decydować, którą konkretnie klasę utworzyć. Umożliwia to delegowanie logiki tworzenia obiektów do podklas.
        *   **Przykład: Singleton:** Zapewnia, że klasa ma tylko jedną instancję i dostarcza globalny punkt dostępu do niej. Używany np. do zarządzania połączeniem z bazą danych lub logowaniem.

    2.  **Strukturalne (Structural):** Opisują, jak **łączyć klasy i obiekty w większe struktury**, zachowując ich elastyczność i wydajność.
        *   **Przykład: Dekorator (Decorator):** Pozwala na dynamiczne dodawanie nowej funkcjonalności do obiektu poprzez "opakowanie" go w obiekt dekoratora. Jest elastyczną alternatywą dla dziedziczenia.
        *   **Przykład: Adapter:** Pozwala na współpracę obiektów o niekompatybilnych interfejsach. Działa jak przejściówka między dwoma różnymi "gniazdkami".

    3.  **Behawioralne (Czynnościowe, Behavioral):** Zajmują się **algorytmami i komunikacją między obiektami**, definiując wzorce ich współpracy.
        *   **Przykład: Strategia (Strategy):** Definiuje rodzinę algorytmów, umieszcza każdy z nich w osobnej klasie i sprawia, że stają się one wymienialne. Pozwala to na zmianę algorytmu w trakcie działania programu.
        *   **Przykład: Obserwator (Observer):** Definiuje relację subskrypcji, w której wiele obiektów (obserwatorów) jest powiadamianych o zmianie stanu jednego obiektu (obserwowanego).

*   **Zastosowania:** Wzorce projektowe są stosowane wszędzie tam, gdzie programiści napotykają typowe problemy projektowe. Ich znajomość pozwala pisać kod, który jest bardziej elastyczny, reużywalny, skalowalny i łatwiejszy w utrzymaniu.

**Ramy programistyczne (Frameworks)**

*   **Charakterystyka:** Framework to **szkielet, rusztowanie do budowy aplikacji**. Jest to zbiór gotowych, zintegrowanych ze sobą bibliotek, komponentów i narzędzi, który narzuca pewną strukturę i architekturę aplikacji. Framework dostarcza gotowe rozwiązania dla typowych problemów (np. routing, dostęp do bazy danych, uwierzytelnianie), pozwalając programiście skupić się na pisaniu logiki biznesowej specyficznej dla jego aplikacji.

*   **Inwersja sterowania (Inversion of Control - IoC):** To kluczowa cecha odróżniająca framework od zwykłej biblioteki. W przypadku biblioteki, to **twój kod wywołuje kod biblioteki**. W przypadku frameworka, to **framework wywołuje twój kod**. Ty wypełniasz określone przez framework "puste miejsca" swoją logiką, a framework zarządza całym przepływem sterowania aplikacji. To zjawisko nazywane jest też **"Zasadą Hollywood"**: "Nie dzwoń do nas, my zadzwonimy do ciebie".

*   **Przykłady i zastosowania:**
    *   **Frameworki webowe back-endowe:** Dostarczają narzędzi do budowy logiki po stronie serwera.
        *   **Spring (Java):** Kompleksowy framework do budowy aplikacji korporacyjnych w Javie. Oferuje m.in. wstrzykiwanie zależności (DI), programowanie aspektowe (AOP) i moduły do obsługi web, danych, bezpieczeństwa itp.
        *   **Django (Python):** Framework typu "batteries-included", który dostarcza niemal wszystko, co potrzebne do budowy aplikacji webowej, w tym ORM, panel administracyjny i system szablonów.
        *   **.NET (C#):** Platforma od Microsoftu do budowy różnego rodzaju aplikacji, w tym webowych (ASP.NET Core).

    *   **Frameworki webowe front-endowe:** Dostarczają narzędzi do budowy interfejsu użytkownika w przeglądarce.
        *   **React, Angular, Vue.js (JavaScript/TypeScript):** Najpopularniejsze frameworki do tworzenia nowoczesnych, interaktywnych aplikacji jednostronicowych (SPA - Single Page Applications).

**Porównanie: Wzorzec projektowy vs Framework**

| Cecha | Wzorzec projektowy | Framework |
|---|---|---|
| **Czym jest?** | **Koncepcja**, przepis, schemat rozwiązania problemu. | **Gotowy kod**, szkielet aplikacji, zbiór narzędzi. |
| **Poziom abstrakcji** | Wysoki (idea). | Niski (konkretna implementacja). |
| **Inwersja sterowania (IoC)** | Nie dotyczy. Twój kod implementuje wzorzec. | **Kluczowa cecha.** Framework wywołuje twój kod. |
| **Jak się używa?** | **Implementujesz** go w swoim kodzie. | **Rozszerzasz** go i **wypełniasz** swoim kodem. |
| **Relacja** | Twoja aplikacja **używa** wzorców projektowych. | Twoja aplikacja **jest budowana na** frameworku. |
| **Analogia** | Przepis na ciasto. | Gotowy zestaw do pieczenia ciasta (z foremką, mikserem i częścią składników). |

Podsumowując, wzorce projektowe to abstrakcyjne idee, które pomagają w podejmowaniu decyzji projektowych, podczas gdy frameworki to konkretne narzędzia, które dostarczają gotową strukturę dla aplikacji. Frameworki często same w sobie implementują wiele wzorców projektowych (np. Spring intensywnie korzysta z Fabryki, Singletona, Proxy i wielu innych).


## 39. Zapewnienie jakości oraz testowanie oprogramowania – normy, metody, kryteria.

### Szczegółowe wyjaśnienie

**Zapewnienie jakości (Quality Assurance - QA)** to szeroki proces, którego celem jest zapewnienie, że tworzone oprogramowanie będzie spełniać określone wymagania i osiągnie pożądany poziom jakości. QA to nie tylko testowanie – to proaktywne działania na każdym etapie cyklu życia oprogramowania, mające na celu **zapobieganie powstawaniu błędów**.

**Testowanie oprogramowania (Software Testing)** jest kluczowym elementem QA. Jest to proces **weryfikacji i walidacji** oprogramowania, polegający na jego uruchamianiu w celu znalezienia błędów (defektów). Celem testowania jest **wykrywanie błędów**, a nie udowadnianie, że ich nie ma.

**Normy jakości oprogramowania**

Normy dostarczają ram i wytycznych dla procesów związanych z jakością. Pomagają ustandaryzować działania i zapewnić ich powtarzalność.

*   **ISO/IEC 9126 (obecnie część ISO/IEC 25010):** Definiuje model jakości oprogramowania, dzieląc go na sześć głównych charakterystyk:
    1.  **Funkcjonalność (Functionality):** Zdolność oprogramowania do realizacji zadań zgodnych z wymaganiami.
    2.  **Niezawodność (Reliability):** Zdolność do bezawaryjnej pracy przez określony czas.
    3.  **Użyteczność (Usability):** Łatwość, z jaką użytkownik może nauczyć się obsługi i korzystać z oprogramowania.
    4.  **Wydajność (Efficiency):** Stosunek wyników (efektów działania) do zużytych zasobów (np. czasu procesora, pamięci).
    5.  **Pielęgnowalność (Maintainability):** Łatwość, z jaką oprogramowanie może być modyfikowane (naprawiane, ulepszane, adaptowane).
    6.  **Przenośność (Portability):** Łatwość, z jaką oprogramowanie może być przeniesione do innego środowiska.
*   **ISO/IEC 9001:** Ogólna norma dotycząca systemów zarządzania jakością w organizacjach. Jej wdrożenie świadczy o tym, że firma ma zdefiniowane i powtarzalne procesy, co przekłada się również na jakość oprogramowania.

**Metody i poziomy testowania**

Testowanie można klasyfikować na wiele sposobów. Najpopularniejszy podział dotyczy poziomów testów, które odpowiadają kolejnym etapom integracji systemu.

1.  **Testy jednostkowe (Unit Tests):**
    *   **Cel:** Testowanie najmniejszych, izolowanych fragmentów kodu (jednostek) – pojedynczych metod lub klas.
    *   **Kto wykonuje:** Zazwyczaj programiści.
    *   **Charakterystyka:** Są szybkie, zautomatyzowane i stanowią podstawę piramidy testów. Powinno ich być najwięcej.

2.  **Testy integracyjne (Integration Tests):**
    *   **Cel:** Weryfikacja, czy kilka połączonych ze sobą modułów lub komponentów poprawnie współpracuje.
    *   **Kto wykonuje:** Programiści lub testerzy.
    *   **Charakterystyka:** Sprawdzają interfejsy między komponentami, np. czy moduł A poprawnie wywołuje usługi modułu B, czy aplikacja poprawnie komunikuje się z bazą danych.

3.  **Testy systemowe (System Tests):**
    *   **Cel:** Testowanie całego, zintegrowanego systemu w celu weryfikacji, czy spełnia on zdefiniowane wymagania funkcjonalne i niefunkcjonalne.
    *   **Kto wykonuje:** Zazwyczaj dedykowany zespół testerów.
    *   **Charakterystyka:** Testy te są przeprowadzane z perspektywy "czarnej skrzynki" (bez znajomości wewnętrznej budowy kodu), na środowisku jak najbardziej zbliżonym do produkcyjnego.

4.  **Testy akceptacyjne (Acceptance Tests):**
    *   **Cel:** Walidacja, czy system spełnia potrzeby biznesowe klienta i jest gotowy do wdrożenia. Odpowiadają na pytanie: "Czy zbudowaliśmy właściwy produkt?".
    *   **Kto wykonuje:** Klient, użytkownicy końcowi lub ich przedstawiciele.
    *   **Charakterystyka:** Ostatni etap testów przed wdrożeniem. Mogą przybierać formę testów alfa (wewnątrz organizacji) lub beta (udostępnienie szerszej grupie zewnętrznych użytkowników).

**Inne klasyfikacje testów:**

*   **Podział ze względu na znajomość implementacji:**
    *   **Testy białoskrzynkowe (White-box):** Tester zna wewnętrzną strukturę kodu i projektuje przypadki testowe tak, aby pokryć określone ścieżki w kodzie.
    *   **Testy czarnoskrzynkowe (Black-box):** Tester nie zna implementacji. Testuje system wyłącznie przez jego zewnętrzny interfejs (np. GUI, API), na podstawie specyfikacji wymagań.
    *   **Testy szaroskrzynkowe (Grey-box):** Połączenie obu podejść – tester ma częściową wiedzę o budowie systemu.

*   **Podział ze względu na cel:**
    *   **Testy funkcjonalne:** Sprawdzają, **co** system robi (czy funkcje działają zgodnie z wymaganiami).
    *   **Testy niefunkcjonalne:** Sprawdzają, **jak** system działa (np. testy wydajności, bezpieczeństwa, użyteczności).
    *   **Testy regresji:** Sprawdzają, czy wprowadzone zmiany (np. nowa funkcja, poprawka błędu) nie zepsuły istniejącej, działającej wcześniej funkcjonalności.

**Kryteria zakończenia testów**

Testowanie można prowadzić w nieskończoność. Dlatego kluczowe jest zdefiniowanie kryteriów, które określają, kiedy można uznać proces testowania za zakończony. Przykładowe kryteria:

*   **Pokrycie kodu (Code Coverage):** Osiągnięcie założonego procentu pokrycia kodu przez testy jednostkowe (np. 80% linii kodu).
*   **Pokrycie wymagań:** Wszystkie zdefiniowane wymagania zostały przetestowane.
*   **Liczba i priorytet błędów:** Osiągnięcie stanu, w którym nie ma już żadnych znanych błędów krytycznych lub blokujących, a liczba błędów o niższym priorytecie jest na akceptowalnym poziomie.
*   **Upływ czasu / budżetu:** Testowanie kończy się, gdy wyczerpie się na nie czas lub budżet (jest to kryterium ryzykowne, ale często spotykane w praktyce).

## 40. Rodzaje, metody specyfikowania oraz rola wymagań w procesie wytwarzania oprogramowania.

### Szczegółowe wyjaśnienie

**Rola wymagań**

Wymagania są **fundamentem** całego procesu wytwarzania oprogramowania. Są to formalne opisy potrzeb, oczekiwań i ograniczeń dotyczących systemu, który ma powstać. Od ich jakości zależy sukces lub porażka projektu. Błędy popełnione na etapie zbierania i analizy wymagań są najdroższe do naprawienia, ponieważ ich konsekwencje propagują się na wszystkie kolejne etapy – projektowanie, implementację i testowanie.

**Główne role wymagań:**

*   **Podstawa do projektowania i implementacji:** Mówią zespołowi deweloperskiemu, **co** ma zbudować.
*   **Podstawa do testowania:** Na ich podstawie tworzone są przypadki testowe, które weryfikują, czy system działa poprawnie.
*   **Podstawa do planowania projektu:** Pozwalają oszacować pracochłonność, koszty i czas potrzebny na realizację projektu.
*   **Podstawa umowy z klientem:** Stanowią formalne uzgodnienie między zamawiającym a wykonawcą, co do zakresu i funkcjonalności systemu.

**Rodzaje wymagań**

Wymagania dzieli się na kilka głównych kategorii:

1.  **Wymagania biznesowe (Business Requirements):**
    *   Wysokopoziomowe cele, jakie organizacja chce osiągnąć dzięki systemowi. Odpowiadają na pytanie "Dlaczego budujemy ten system?".
    *   **Przykład:** "Zwiększenie sprzedaży internetowej o 20% w ciągu roku" lub "Skrócenie czasu obsługi klienta o 50%".

2.  **Wymagania użytkownika (User Requirements):**
    *   Opisują cele i zadania, jakie użytkownicy będą mogli realizować za pomocą systemu. Są często formułowane w języku naturalnym.
    *   **Przykład:** "Użytkownik musi mieć możliwość wyszukania produktu po nazwie i kategorii" lub "Użytkownik chce otrzymać e-mail z potwierdzeniem złożenia zamówienia".

3.  **Wymagania systemowe (System Requirements):**
    *   Jest to szczegółowy, precyzyjny opis usług, jakie system ma świadczyć, oraz ograniczeń, w jakich ma działać. Dzielą się na dwie kluczowe podkategorie:
        *   **Wymagania funkcjonalne (Functional Requirements):**
            *   Opisują, **co** system ma robić – jakie funkcje i usługi ma udostępniać. Definiują zachowanie systemu w odpowiedzi na określone dane wejściowe.
            *   **Przykład:** "System ma uwierzytelniać użytkownika na podstawie loginu i hasła" lub "Po kliknięciu przycisku 'Dodaj do koszyka', wybrany produkt ma zostać dodany do koszyka zakupowego użytkownika".
        *   **Wymagania niefunkcjonalne (Non-functional Requirements):**
            *   Opisują, **jak** system ma działać. Są to ograniczenia i kryteria jakościowe dotyczące systemu.
            *   **Przykłady:**
                *   **Wydajność:** "Czas odpowiedzi na zapytanie o produkt nie może przekraczać 2 sekund".
                *   **Niezawodność:** "System musi być dostępny przez 99.9% czasu".
                *   **Bezpieczeństwo:** "Wszystkie hasła użytkowników muszą być przechowywane w postaci zaszyfrowanej".
                *   **Użyteczność:** "Nowy użytkownik powinien być w stanie złożyć zamówienie w czasie krótszym niż 5 minut bez potrzeby czytania instrukcji".

**Metody specyfikowania wymagań**

Specyfikacja wymagań to proces ich dokumentowania. Wybór metody zależy od metodyki projektu i poziomu szczegółowości.

1.  **Język naturalny:**
    *   Najprostsza i najbardziej naturalna forma. Wymagania są spisywane w postaci zdań w języku polskim lub angielskim. Stosuje się często numerowane listy i szablony zdań (np. "System powinien...").
    *   **Zalety:** Zrozumiały dla wszystkich (w tym dla klienta).
    *   **Wady:** Może prowadzić do niejednoznaczności, nieścisłości i niekompletności.

2.  **Specyfikacja ustrukturyzowana:**
    *   Kompromis między językiem naturalnym a notacjami formalnymi. Używa się predefiniowanych szablonów i formularzy do opisu wymagań, co narzuca pewną strukturę i zmniejsza ryzyko niejednoznaczności.

3.  **Przypadki użycia (Use Cases):**
    *   Bardzo popularna technika opisu wymagań funkcjonalnych. Przypadek użycia opisuje interakcję między użytkownikiem (aktorem) a systemem, która prowadzi do osiągnięcia określonego celu.
    *   Składa się z nazwy, aktorów, warunków początkowych, warunków końcowych oraz opisu scenariusza głównego (happy path) i scenariuszy alternatywnych/wyjątkowych.
    *   Graficzną reprezentacją przypadków użycia jest **diagram przypadków użycia UML**.

4.  **Historyjki użytkownika (User Stories):**
    *   Główna technika specyfikowania wymagań w **metodykach zwinnych (Agile)**.
    *   Jest to krótkie, proste zdanie opisujące funkcjonalność z perspektywy użytkownika, zapisane według szablonu:
        **Jako** <typ użytkownika>, **chcę** <wykonać jakąś akcję>, **aby** <osiągnąć jakiś cel>.
    *   **Przykład:** "Jako zarejestrowany klient, chcę dodać produkt do listy życzeń, aby móc go kupić w przyszłości".
    *   Historyjka użytkownika to nie jest szczegółowa specyfikacja, ale **obietnica rozmowy**. Szczegóły są doprecyzowywane w trakcie bezpośredniej konwersacji z Product Ownerem tuż przed implementacją.

5.  **Notacje graficzne (np. UML):**
    *   Diagramy UML, takie jak **diagramy aktywności** czy **diagramy stanów**, mogą być używane do precyzyjnego modelowania złożonych procesów biznesowych i cykli życia obiektów, uzupełniając tekstowy opis wymagań.

6.  **Metody formalne:**
    *   Używają języków opartych na notacji matematycznej (np. logika, teoria zbiorów) do stworzenia w pełni jednoznacznej i weryfikowalnej specyfikacji. Są bardzo rzadko stosowane w komercyjnych projektach ze względu na wysoki koszt i trudność, ale znajdują zastosowanie w systemach o krytycznym znaczeniu (np. sterowanie lotem, systemy medyczne).


---

# Odpowiedzi "to the point" na obronę

## 36. Zarządzanie projektem budowy oprogramowania: rodzaje działań, dobór metodyki oraz kontekst pozatechniczny.

Zarządzanie projektem IT to proces planowania i kontrolowania działań w celu dostarczenia oprogramowania na czas i w budżecie. Kluczowe działania to zarządzanie zakresem, czasem, kosztem, jakością i ryzykiem. Metodykę dobiera się do projektu: **tradycyjną (Waterfall)**, gdy wymagania są stałe, lub **zwinną (Agile, np. Scrum, Kanban)**, gdy wymagania są zmienne. Sukces zależy też od **kontekstu pozatechnicznego**: celów biznesowych, wsparcia organizacji i kompetencji zespołu.

## 37. Język UML – charakterystyka oraz sposób wsparcia różnorodnych modeli danych.

**UML (Unified Modeling Language)** to standardowy, graficzny język do wizualizacji, specyfikowania i dokumentowania systemów IT. Nie jest to metodyka, a notacja. Składa się z diagramów **strukturalnych** (np. Diagram Klas), które pokazują z czego system się składa, i **behawioralnych** (np. Diagram Przypadków Użycia), które pokazują jak system działa. UML wspiera modelowanie danych na każdym etapie: od **konceptualnego** (pojęcia biznesowe), przez **logiczny** (mapowanie na tabele), aż po **fizyczny** (specyficzny dla danej bazy danych), głównie za pomocą Diagramu Klas.

## 38. Wzorce projektowe oraz ramy programistyczne (frameworks) – charakterystyka, przykłady, zastosowania.

**Wzorzec projektowy** to koncepcyjny, sprawdzony schemat rozwiązania typowego problemu projektowego (np. Singleton, Fabryka, Strategia). To przepis, a nie gotowy kod. **Framework** to szkielet aplikacji, czyli zbiór gotowych bibliotek i narzędzi, który narzuca jej strukturę (np. Spring, React). Kluczową różnicą jest **inwersja sterowania (IoC)** – to framework wywołuje nasz kod, a nie odwrotnie. Aplikacja używa wzorców, ale jest budowana na frameworku.

## 39. Zapewnienie jakości oraz testowanie oprogramowania – normy, metody, kryteria.

**Zapewnienie jakości (QA)** to proces zapobiegania błędom na każdym etapie projektu. **Testowanie** to element QA polegający na wykrywaniu błędów. Główne poziomy testów to: **jednostkowe** (testowanie małych fragmentów kodu przez programistów), **integracyjne** (testowanie współpracy modułów), **systemowe** (testowanie całego systemu) i **akceptacyjne** (wykonywane przez klienta). Testy kończy się po spełnieniu kryteriów, np. osiągnięciu wymaganego pokrycia kodu lub gdy nie ma już błędów krytycznych.

## 40. Rodzaje, metody specyfikowania oraz rola wymagań w procesie wytwarzania oprogramowania.

Wymagania to fundament projektu – opisują, co system ma robić. Dzielimy je na **funkcjonalne** (co system robi, np. "użytkownik może się zalogować") i **niefunkcjonalne** (jak system działa, np. wydajność, bezpieczeństwo). W metodykach tradycyjnych specyfikuje się je za pomocą języka naturalnego i **przypadków użycia (Use Cases)**. W metodykach zwinnych używa się **historyjek użytkownika (User Stories)**, które są krótkim opisem funkcjonalności z perspektywy użytkownika i stanowią obietnicę dalszej rozmowy.

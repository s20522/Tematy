# Odpowiedzi na pytania do obrony pracy inżynierskiej - Metody Programowania

## 26. Konstrukcja obiektów i zarządzanie pamięcią operacyjną w Javie i C++.

### Szczegółowe wyjaśnienie

Java i C++ to języki obiektowe, ale podchodzą do kluczowych kwestii konstrukcji obiektów i zarządzania pamięcią w fundamentalnie różny sposób. Różnice te wynikają z ich filozofii: C++ daje programiście pełną kontrolę (i odpowiedzialność) nad zasobami, podczas gdy Java stawia na bezpieczeństwo i automatyzację, zdejmując z programisty część obowiązków.

**Konstrukcja obiektów**

Proces tworzenia obiektu, czyli instancji klasy, jest inicjowany przez **konstruktor**. Jest to specjalna metoda, której zadaniem jest zainicjowanie stanu obiektu (ustawienie początkowych wartości jego pól).

*   **W C++:**
    *   Obiekty można tworzyć na **stosie** (jako zmienne lokalne) lub na **stercie** (dynamicznie, za pomocą operatora `new`).
    *   **Konstrukcja na stosie:** `MojaKlasa obiekt;` – obiekt jest tworzony automatycznie przy wejściu do zakresu (np. funkcji) i **automatycznie niszczony** przy wyjściu z tego zakresu. Wywoływany jest wtedy **destruktor** (`~MojaKlasa()`), który zwalnia zasoby zajęte przez obiekt.
    *   **Konstrukcja na stercie:** `MojaKlasa* wskaznik = new MojaKlasa();` – obiekt jest tworzony w wolnej pamięci (na stercie). Taki obiekt **nie jest niszczony automatycznie**. Programista jest **odpowiedzialny** za jego ręczne zwolnienie za pomocą operatora `delete wskaznik;`. Niezrobienie tego prowadzi do **wycieku pamięci (memory leak)**.
    *   **Destruktory:** Są kluczowym elementem w C++. Pozwalają na implementację wzorca **RAII (Resource Acquisition Is Initialization)**, gdzie pozyskanie zasobu (np. otwarcie pliku, blokada mutexu) odbywa się w konstruktorze, a jego zwolnienie – w destruktorze. Gwarantuje to zwolnienie zasobu niezależnie od tego, jak zakończy się działanie w danym zakresie (normalnie czy przez wyjątek).

*   **W Javie:**
    *   **Wszystkie obiekty są tworzone wyłącznie na stercie** za pomocą operatora `new`. Nie ma możliwości jawnego tworzenia obiektów na stosie.
    *   `MojaKlasa obiekt = new MojaKlasa();` – zmienna `obiekt` jest referencją (wskaźnikiem) do obiektu na stercie.
    *   **Brak destruktorów i ręcznego zwalniania pamięci:** Java posiada **automatyczny mechanizm odśmiecania pamięci (Garbage Collector, GC)**. Programista po prostu przestaje używać obiektu (traci do niego wszystkie referencje). Garbage Collector okresowo przeszukuje stertę, identyfikuje obiekty, do których nie ma już żadnych odwołań, i automatycznie zwalnia zajmowaną przez nie pamięć.
    *   **Metoda `finalize()`:** Jest to odpowiednik destruktora, ale jego użycie jest **zdecydowanie odradzane**. Jest wywoływany przez GC tuż przed usunięciem obiektu, ale nie ma żadnej gwarancji, *kiedy* (i *czy* w ogóle) zostanie wywołany. Nie nadaje się do zwalniania krytycznych zasobów.

**Zarządzanie pamięcią operacyjną**

| Cecha | C++ | Java |
|---|---|---|
| **Alokacja obiektów** | Na stosie (automatycznie) lub na stercie (ręcznie przez `new`) | **Tylko na stercie** (przez `new`) |
| **Zwalnianie pamięci** | **Ręczne** (przez `delete` dla obiektów na stercie) lub automatyczne (dla obiektów na stosie) | **Automatyczne** (przez Garbage Collector) |
| **Odpowiedzialność** | **Programista** jest w pełni odpowiedzialny za zarządzanie pamięcią. | **Środowisko uruchomieniowe (JVM)** jest odpowiedzialne za zwalnianie pamięci. |
| **Ryzyko** | **Wycieki pamięci** (gdy zapomnimy o `delete`), **wiszące wskaźniki** (gdy używamy wskaźnika do już zwolnionej pamięci). | **Brak** ryzyka typowych wycieków pamięci. Możliwe są jednak wycieki logiczne (gdy trzymamy niepotrzebne referencje). |
| **Wydajność** | Potencjalnie **wyższa wydajność** i mniejszy narzut pamięciowy dzięki alokacji na stosie i pełnej kontroli. | Narzut związany z działaniem Garbage Collectora (tzw. "pauzy GC"), ale nowoczesne algorytmy GC są bardzo wydajne. |
| **Bezpieczeństwo** | Mniejsze bezpieczeństwo, błędy w zarządzaniu pamięcią są częstym źródłem krytycznych błędów i luk bezpieczeństwa. | **Wysokie bezpieczeństwo**, eliminacja całej klasy błędów związanych z pamięcią. |

**Podsumowanie filozofii:**

*   **C++** mówi: "Ufam ci, programisto. Daję ci potężne narzędzia (wskaźniki, ręczne zarządzanie pamięcią, RAII) i oczekuję, że użyjesz ich poprawnie. Twoja nagroda to maksymalna wydajność i kontrola."
*   **Java** mówi: "Chcę cię chronić przed błędami. Zajmę się za ciebie brudną robotą (zarządzanie pamięcią), abyś mógł skupić się na logice aplikacji. Twoja nagroda to większe bezpieczeństwo i szybszy rozwój oprogramowania."


## 27. Rola klas, interfejsów i mixinów w programowaniu na przykładzie języka Java.

### Szczegółowe wyjaśnienie

Klasy, interfejsy i (w pewnym sensie) mixiny to fundamentalne narzędzia programowania obiektowego w Javie, które służą do modelowania rzeczywistości, definiowania kontraktów i promowania reużywalności kodu. Każde z nich pełni jednak inną, specyficzną rolę.

**1. Klasy (Classes)**

*   **Rola:** Klasa to **szablon lub plan (blueprint)**, na podstawie którego tworzone są **obiekty**. Jest to podstawowy budulec programowania obiektowego. Klasa definiuje dwie rzeczy:
    1.  **Stan (atrybuty, pola):** Zmienne, które przechowują dane charakteryzujące obiekt (np. dla klasy `Samochod` atrybutami mogą być `kolor`, `predkosc`, `marka`).
    2.  **Zachowanie (metody):** Funkcje, które operują na stanie obiektu i definiują, co obiekt potrafi robić (np. `przyspiesz()`, `hamuj()`, `zmienBieg()`).

*   **Przykład:** Klasa jest jak przepis na ciasto. Definiuje składniki (stan) i kroki do wykonania (zachowanie). Obiekt to konkretne, upieczone ciasto, stworzone według tego przepisu.
*   **W Javie:** Klasa jest konkretną implementacją. Może dziedziczyć po **jednej** innej klasie (Java nie wspiera wielokrotnego dziedziczenia klas), ale może implementować **wiele** interfejsów.

**2. Interfejsy (Interfaces)**

*   **Rola:** Interfejs to **kontrakt**, który definiuje zestaw **abstrakcyjnych metod** (zachowań), jakie klasa implementująca ten interfejs **musi** dostarczyć. Interfejs mówi, **co** obiekt potrafi robić, ale nie mówi, **jak** to robi. Jest to czysta abstrakcja, która oddziela definicję funkcjonalności od jej implementacji.

*   **Przykład:** Interfejs `Jezdzacy` może definiować metody `jedz()` i `zatrzymajSie()`. Każda klasa, która go implementuje (np. `Samochod`, `Rower`, `Hulajnoga`), musi dostarczyć własną, konkretną implementację tych metod. Dzięki temu możemy traktować wszystkie te obiekty w sposób polimorficzny – jako obiekty typu `Jezdzacy`, nie martwiąc się o ich konkretny typ.

*   **W Javie (od wersji 8):** Interfejsy zyskały na mocy. Oprócz metod abstrakcyjnych, mogą zawierać:
    *   **Metody domyślne (default methods):** Metody z gotową implementacją. Pozwalają na dodawanie nowej funkcjonalności do interfejsów bez psucia istniejących klas, które je implementują.
    *   **Metody statyczne:** Metody pomocnicze związane z interfejsem, ale niewymagające instancji klasy.

**3. Mixiny (Mixins) - symulacja w Javie**

*   **Rola:** Mixin to koncepcja, która pozwala na "domieszanie" gotowej funkcjonalności do klasy bez użycia dziedziczenia. Jest to sposób na kompozycję zachowań z wielu źródeł. Języki takie jak Ruby czy Python mają wbudowane wsparcie dla mixinów. **Java nie posiada bezpośredniego wsparcia dla mixinów**, ale można symulować ich działanie.

*   **Symulacja w Javie:** Od Javy 8, najlepszym sposobem na symulację mixinów jest użycie **interfejsów z metodami domyślnymi**. Możemy stworzyć interfejs, który dostarcza kompletną, gotową do użycia funkcjonalność w postaci metod domyślnych. Klasa, która chce "domieszać" tę funkcjonalność, po prostu implementuje ten interfejs.

*   **Przykład:** Chcemy dodać funkcjonalność logowania do wielu różnych klas. Możemy stworzyć interfejs `Logujacy` z metodą domyślną `log(String wiadomosc)`. Każda klasa, która zaimplementuje ten interfejs, automatycznie zyska możliwość logowania, bez potrzeby dziedziczenia po wspólnej klasie bazowej `LogujacaKlasa`.

**Porównanie i podsumowanie ról**

| Cecha | Klasa | Interfejs | Mixin (symulowany w Javie) |
|---|---|---|---|
| **Główna rola** | **Szablon** do tworzenia obiektów, definiuje stan i zachowanie. | **Kontrakt**, który definiuje, co obiekt musi potrafić robić. | **Domieszka** gotowej funkcjonalności, reużycie kodu. |
| **Zawartość** | Pola (stan), metody (implementacja). | Metody abstrakcyjne, metody domyślne, metody statyczne, stałe. **Brak stanu instancji.** | Metody domyślne (implementacja). |
| **Relacja** | Klasa **jest** czymś (np. `Samochod` jest `Pojazdem`). | Klasa **potrafi robić** coś (np. `Samochod` potrafi `Jezdzic`). | Klasa **zyskuje** jakąś cechę (np. `Samochod` zyskuje zdolność `Logowania`). |
| **Dziedziczenie** | Może dziedziczyć po **jednej** klasie. | Klasa może implementować **wiele** interfejsów. | Osiągane przez implementację interfejsu. |

Użycie tych trzech narzędzi pozwala na tworzenie elastycznych, modułowych i łatwych w utrzymaniu systemów. Klasy definiują konkretne byty, interfejsy tworzą abstrakcyjne kontrakty, które pozwalają na polimorfizm i luźne powiązania między komponentami, a mixiny (symulowane przez metody domyślne) pozwalają na reużycie kodu w sposób horyzontalny, omijając ograniczenia pojedynczego dziedziczenia.


## 28. Pojęcie dziedziczenia na przykładzie języków Java i C++.

### Szczegółowe wyjaśnienie

**Istota dziedziczenia**

Dziedziczenie to jeden z trzech filarów programowania obiektowego (obok enkapsulacji i polimorfizmu). Jest to mechanizm, który pozwala na tworzenie nowej klasy (nazywanej **klasą pochodną**, **podklasą** lub **dzieckiem**) na bazie już istniejącej klasy (nazywanej **klasą bazową**, **nadklasą** lub **rodzicem**). Klasa pochodna **dziedziczy** (przejmuje) publiczne i chronione pola oraz metody klasy bazowej, a następnie może:

*   **Dodawać nowe** pola i metody.
*   **Nadpisywać (override)** istniejące metody, aby dostarczyć ich własną, specjalistyczną implementację.

Dziedziczenie modeluje relację **"jest rodzajem" (is-a)**. Jeśli klasa `Pies` dziedziczy po klasie `Ssak`, oznacza to, że `Pies` *jest rodzajem* `Ssaka`. Każdy `Pies` ma wszystkie cechy `Ssaka` (np. oddycha płucami), ale może mieć też swoje własne, specyficzne cechy (np. szczeka).

Głównym celem dziedziczenia jest **reużywalność kodu** (unikanie jego powielania) oraz tworzenie hierarchii klas, która w naturalny sposób odzwierciedla relacje między pojęciami w modelowanym świecie.

**Dziedziczenie w Javie**

*   **Składnia:** Używa się słowa kluczowego `extends`. `class Pies extends Ssak { ... }`
*   **Rodzaj dziedziczenia:** Java wspiera tylko **dziedziczenie proste (pojedyncze)**. Oznacza to, że jedna klasa może dziedziczyć bezpośrednio tylko po **jednej** innej klasie. Ma to na celu uniknięcie problemów związanych z wielokrotnym dziedziczeniem, takich jak problem diamentowy.
*   **Klasa `Object`:** W Javie wszystkie klasy, jeśli nie dziedziczą jawnie po innej klasie, **niejawnie dziedziczą po klasie `Object`**. Jest to uniwersalna klasa bazowa dla całej hierarchii klas w Javie.
*   **Symulacja wielokrotnego dziedziczenia:** Chociaż klasa nie może dziedziczyć po wielu klasach, może **implementować wiele interfejsów**. Od Javy 8, dzięki metodom domyślnym w interfejsach, można w ten sposób symulować dziedziczenie zachowań z wielu źródeł.
*   **Konstruktory:** Konstruktor klasy pochodnej **musi** wywołać konstruktor klasy bazowej. Odbywa się to za pomocą słowa kluczowego `super()`, które musi być pierwszą instrukcją w konstruktorze klasy pochodnej. Jeśli nie zrobimy tego jawnie, kompilator spróbuje automatycznie wywołać bezparametrowy konstruktor klasy bazowej.

**Dziedziczenie w C++**

*   **Składnia:** Używa się dwukropka `:` po nazwie klasy pochodnej. `class Pies : public Ssak { ... };`
*   **Rodzaj dziedziczenia:** C++ wspiera zarówno **dziedziczenie proste**, jak i **wielokrotne (wielodziedziczenie)**. Klasa może dziedziczyć po wielu klasach bazowych jednocześnie: `class Amfibia : public Pojazd, public Lodz { ... };`
*   **Problem diamentowy:** Wielokrotne dziedziczenie wprowadza tzw. "problem diamentowy". Jeśli klasy B i C dziedziczą po A, a klasa D dziedziczy po B i C, to D odziedziczyłoby składowe z A dwiema różnymi ścieżkami, co prowadzi do niejednoznaczności. C++ rozwiązuje ten problem za pomocą **dziedziczenia wirtualnego** (słowo kluczowe `virtual` przy dziedziczeniu), które zapewnia, że klasa bazowa (A) będzie istnieć tylko w jednej kopii w obiekcie klasy D.
*   **Specyfikatory dostępu w dziedziczeniu:** C++ wprowadza dodatkowy poziom kontroli. Można dziedziczyć w trybie `public`, `protected` lub `private`.
    *   **`public`:** Publiczne składowe klasy bazowej stają się publicznymi składowymi klasy pochodnej, a chronione – chronionymi. Jest to najczęstszy i najbardziej intuicyjny typ dziedziczenia, odpowiadający relacji "is-a".
    *   **`protected` / `private`:** Ograniczają dostęp do odziedziczonych składowych. Są rzadziej używane i modelują raczej relację "jest zaimplementowane za pomocą" (is-implemented-in-terms-of).
*   **Konstruktory:** Podobnie jak w Javie, konstruktor klasy pochodnej musi wywołać konstruktory klas bazowych. Robi się to za pomocą **listy inicjalizacyjnej** konstruktora: `Pies() : Ssak() { ... }`.

**Tabela porównawcza**

| Cecha | Java | C++ |
|---|---|---|
| **Składnia** | `class A extends B` | `class A : public B` |
| **Wielokrotne dziedziczenie** | **Nie** (tylko dla interfejsów) | **Tak** |
| **Problem diamentowy** | Nie występuje (dzięki braku wielodziedziczenia klas) | Występuje, rozwiązywany przez **dziedziczenie wirtualne** |
| **Uniwersalna klasa bazowa** | Tak, klasa `Object` | **Nie** |
| **Kontrola dostępu dziedziczenia** | Zawsze `public` | `public`, `protected`, `private` |
| **Wywołanie konstruktora bazowego** | `super()` | Lista inicjalizacyjna (`: Base()`) |

Podsumowując, Java wybiera prostotę i bezpieczeństwo, rezygnując z wielokrotnego dziedziczenia na rzecz interfejsów. C++ oferuje większą elastyczność i moc (wielodziedziczenie), ale kosztem większej złożoności i konieczności ręcznego rozwiązywania problemów takich jak problem diamentowy.


## 29. Istota i zastosowania polimorfizmu na przykładzie języków Java i C++.

### Szczegółowe wyjaśnienie

**Istota polimorfizmu**

Polimorfizm (z greckiego "wielopostaciowość") to trzeci, obok enkapsulacji i dziedziczenia, filar programowania obiektowego. Jest to mechanizm, który pozwala na traktowanie obiektów różnych klas, ale powiązanych przez wspólne dziedziczenie lub interfejs, w jednolity, wspólny sposób. Inaczej mówiąc, pozwala nam używać jednego interfejsu (jednej nazwy metody) do reprezentowania różnych implementacji.

Jego istotą jest możliwość, aby zmienna typu klasy bazowej (lub interfejsu) mogła przechowywać referencję do obiektu dowolnej klasy pochodnej. Gdy na takiej zmiennej wywołujemy metodę, mechanizm polimorfizmu zapewnia, że zostanie uruchomiona **właściwa wersja tej metody – ta z klasy rzeczywistego obiektu**, a nie ta z klasy, do której należy referencja.

**Przykład:** Mamy klasę bazową `Zwierze` z metodą `wydajDzwiek()` oraz klasy pochodne `Pies` i `Kot`, które nadpisują tę metodę. Dzięki polimorfizmowi możemy stworzyć tablicę obiektów typu `Zwierze`, w której umieścimy zarówno obiekty `Pies`, jak i `Kot`. Następnie, iterując po tej tablicy i wywołując dla każdego elementu metodę `wydajDzwiek()`, usłyszymy raz "Hau!", a raz "Miau!", mimo że za każdym razem wywołujemy metodę na zmiennej tego samego typu (`Zwierze`).

**Rodzaje polimorfizmu**

1.  **Polimorfizm statyczny (czasu kompilacji):**
    *   Decyzja o tym, która wersja metody ma zostać wywołana, jest podejmowana **w trakcie kompilacji** programu.
    *   Głównym przykładem jest **przeciążanie metod (method overloading)**. Polega ono na istnieniu w jednej klasie wielu metod o tej samej nazwie, ale różniących się **listą parametrów** (ich liczbą, typem lub kolejnością). Kompilator, na podstawie argumentów użytych w wywołaniu, decyduje, którą wersję metody uruchomić.

2.  **Polimorfizm dynamiczny (czasu wykonania):**
    *   Decyzja o tym, która wersja metody ma zostać wywołana, jest podejmowana **w trakcie działania** programu, na podstawie rzeczywistego typu obiektu.
    *   Jest to "prawdziwy" polimorfizm obiektowy. Jego podstawą jest **nadpisywanie metod (method overriding)** w klasach pochodnych.
    *   Mechanizm, który to umożliwia, nazywa się **późnym wiązaniem (late binding)** lub **dynamicznym wiązaniem (dynamic binding)**.

**Polimorfizm w Javie**

*   **Polimorfizm dynamiczny jest domyślny:** W Javie **wszystkie metody instancji (niestatyczne) są domyślnie wirtualne**. Oznacza to, że mechanizm dynamicznego wiązania działa automatycznie dla każdej nadpisanej metody. Nie trzeba używać żadnych specjalnych słów kluczowych.
*   **Nadpisywanie metod:** Aby nadpisać metodę, musi ona mieć w klasie pochodnej identyczną sygnaturę (nazwę i listę parametrów) jak w klasie bazowej. Dobrą praktyką jest używanie adnotacji `@Override`, która pozwala kompilatorowi sprawdzić, czy faktycznie nadpisujemy jakąś metodę, chroniąc nas przed literówkami.
*   **Wiązanie:** Wywołanie `obiekt.metoda()` jest rozwiązywane w czasie wykonania. JVM sprawdza rzeczywisty typ obiektu, na który wskazuje referencja `obiekt`, i wywołuje wersję `metoda()` z tej właśnie klasy.

**Polimorfizm w C++**

*   **Polimorfizm dynamiczny jest opcjonalny:** W C++ programista musi **jawnie zadeklarować**, że dana metoda ma być częścią mechanizmu polimorfizmu dynamicznego. Robi się to za pomocą słowa kluczowego `virtual` w deklaracji metody w klasie bazowej.
    *   `virtual void wydajDzwiek();`
*   **Nadpisywanie metod:** W klasie pochodnej metodę nadpisującą również oznacza się słowem kluczowym `virtual`, a od standardu C++11 zalecane jest używanie słowa `override`, które pełni tę samą rolę co adnotacja w Javie – zapewnia poprawność nadpisania.
*   **Wiązanie:** Jeśli metoda **nie jest** wirtualna, C++ używa **wczesnego wiązania (early binding)** – wersja metody do wywołania jest wybierana w czasie kompilacji na podstawie typu wskaźnika lub referencji. Jeśli metoda **jest** wirtualna, używane jest **późne wiązanie (late binding)**, tak jak w Javie. Mechanizm ten jest implementowany za pomocą **tablicy metod wirtualnych (vtable)**, którą posiada każdy obiekt klasy polimorficznej.
*   **Czyste funkcje wirtualne:** C++ pozwala na zdefiniowanie "czystej" funkcji wirtualnej: `virtual void wydajDzwiek() = 0;`. Klasa zawierająca choć jedną taką funkcję staje się **klasą abstrakcyjną**, po której nie można tworzyć obiektów. Jest to odpowiednik metody abstrakcyjnej w Javie.

**Zastosowania polimorfizmu**

Polimorfizm jest kluczem do tworzenia elastycznego i rozszerzalnego oprogramowania. Jego główne zastosowania to:

*   **Redukcja złożoności kodu:** Pozwala pisać kod, który operuje na abstrakcjach (klasach bazowych, interfejsach), nie martwiąc się o konkretne typy obiektów. Zamiast pisać oddzielne funkcje `obsluzPsa(Pies p)`, `obsluzKota(Kot k)`, piszemy jedną: `obsluzZwierze(Zwierze z)`.
*   **Zwiększenie elastyczności i rozszerzalności:** Umożliwia łatwe dodawanie nowych klas pochodnych do systemu bez konieczności modyfikowania istniejącego kodu, który z nich korzysta. Jeśli dodamy nową klasę `Krowa extends Zwierze`, nasza funkcja `obsluzZwierze()` będzie z nią działać od razu.
*   **Implementacja wzorców projektowych:** Wiele fundamentalnych wzorców projektowych, takich jak Fabryka, Strategia czy Dekorator, opiera swoje działanie na polimorfizmie.


## 30. Użycie tablic oraz innych struktur danych w Javie i C++. Java Collections Framework.

### Szczegółowe wyjaśnienie

Zarówno Java, jak i C++ oferują wbudowane mechanizmy do pracy z kolekcjami danych, jednak ich podejście, filozofia i poziom abstrakcji znacznie się różnią.

**Tablice**

Tablica to podstawowa, niskopoziomowa struktura danych – ciągły blok pamięci przechowujący elementy tego samego typu. Dostęp do elementu po indeksie jest bardzo szybki (O(1)).

*   **W C++:**
    *   **Tablice statyczne w stylu C:** `int tab[10];`. Ich rozmiar musi być znany w czasie kompilacji. Są alokowane na stosie. Nie przechowują informacji o swoim rozmiarze, co jest częstym źródłem błędów (wyjście poza zakres).
    *   **`std::array` (od C++11):** Bezpieczniejsza, obiektowa otoczka na tablicę statyczną. `std::array<int, 10> arr;`. Przechowuje informacje o rozmiarze i oferuje interfejs podobny do innych kontenerów STL.
    *   **Tablice dynamiczne:** Tworzone na stercie za pomocą `new int[rozmiar]`. Programista jest odpowiedzialny za ich zwolnienie przez `delete[]`. Również nie przechowują informacji o rozmiarze.

*   **W Javie:**
    *   Tablice są **obiektami**. `int[] tab = new int[10];`.
    *   Są zawsze alokowane na **stercie**.
    *   Zawsze przechowują informację o swoim rozmiarze, dostępną przez pole `tab.length`.
    *   Dostęp poza zakres tablicy jest zawsze sprawdzany i skutkuje rzuceniem wyjątku `ArrayIndexOutOfBoundsException`, co znacznie zwiększa bezpieczeństwo.
    *   Ich rozmiar jest **stały** po utworzeniu.

**Zaawansowane struktury danych**

Oba języki dostarczają bogate biblioteki standardowe do pracy z bardziej zaawansowanymi strukturami danych.

**C++ i Standard Template Library (STL)**

STL to potężny zbiór szablonów (templates) klas i funkcji. Jego główne komponenty to **kontenery** (struktury danych), **iteratory** (abstrakcja dostępu do elementów) i **algorytmy** (operacje na kontenerach).

*   **Kontenery sekwencyjne:**
    *   **`std::vector`:** Odpowiednik `ArrayList` z Javy. Dynamiczna tablica, która automatycznie zarządza swoją pojemnością. Szybki dostęp losowy, ale wstawianie/usuwanie w środku jest wolne.
    *   **`std::list`:** Lista dwukierunkowa. Szybkie wstawianie/usuwanie w dowolnym miejscu, ale brak szybkiego dostępu losowego (trzeba iterować).
    *   **`std::deque`:** Kolejka dwustronna, kompromis między wektorem a listą. Szybkie dodawanie/usuwanie na początku i na końcu.
*   **Kontenery asocjacyjne (sortowane):**
    *   **`std::map`:** Słownik implementowany jako zrównoważone drzewo binarne (najczęściej czerwono-czarne). Przechowuje posortowane, unikalne klucze. Złożoność operacji to O(log n).
    *   **`std::set`:** Zbiór unikalnych, posortowanych wartości. Również oparty na drzewach.
*   **Nieuporządkowane kontenery asocjacyjne (od C++11):**
    *   **`std::unordered_map`:** Słownik implementowany jako tablica mieszająca (hash table). Zapewnia średnią złożoność operacji O(1). Odpowiednik `HashMap` z Javy.
    *   **`std::unordered_set`:** Zbiór oparty na tablicy mieszającej.

**Java i Java Collections Framework (JCF)**

JCF to ujednolicona architektura do reprezentowania i manipulowania kolekcjami. Jest w pełni obiektowa i oparta na **interfejsach**.

*   **Główne interfejsy:**
    *   **`Collection`:** Korzeń hierarchii. Definiuje podstawowe operacje, jak `add()`, `remove()`, `size()`.
    *   **`List`:** Uporządkowana kolekcja (sekwencja), która dopuszcza duplikaty. Główne implementacje:
        *   **`ArrayList`:** Dynamiczna tablica. Domyślny wybór dla list.
        *   **`LinkedList`:** Lista dwukierunkowa.
    *   **`Set`:** Kolekcja przechowująca unikalne elementy. Główne implementacje:
        *   **`HashSet`:** Oparta na tablicy mieszającej. Najszybsza, nie gwarantuje kolejności.
        *   **`LinkedHashSet`:** Zachowuje kolejność wstawiania.
        *   **`TreeSet`:** Przechowuje elementy posortowane (oparta na drzewie czerwono-czarnym).
    *   **`Queue`:** Kolejka (FIFO). Implementacja `LinkedList` lub `ArrayDeque`.
    *   **`Map`:** Interfejs dla słowników (nie dziedziczy po `Collection`). Główne implementacje:
        *   **`HashMap`:** Oparta na tablicy mieszającej. Najszybsza, nie gwarantuje kolejności. Domyślny wybór dla map.
        *   **`LinkedHashMap`:** Zachowuje kolejność wstawiania.
        *   **`TreeMap`:** Przechowuje klucze posortowane.

**Porównanie filozofii**

| Cecha | C++ (STL) | Java (JCF) |
|---|---|---|
| **Podstawa** | Szablony (templates), programowanie generyczne. | Interfejsy, polimorfizm, programowanie obiektowe. |
| **Zarządzanie pamięcią** | Ręczne (dla wskaźników) lub automatyczne (dla obiektów). | W pełni automatyczne (Garbage Collector). |
| **Bezpieczeństwo typów** | Mniejsze (możliwość operacji na surowych wskaźnikach). | Pełne bezpieczeństwo typów. |
| **Wydajność** | Potencjalnie wyższa, kod jest kompilowany do natywnego kodu maszynowego, brak narzutu maszyny wirtualnej. | Wysoka, ale z narzutem JVM i GC. |
| **Oddzielenie algorytmów od danych** | Silne. Algorytmy (np. `std::sort`) działają na iteratorach, co czyni je niezależnymi od konkretnego kontenera. | Słabsze. Metody operujące na kolekcjach są często częścią ich interfejsów. Od Javy 8, API Strumieni (Stream API) promuje bardziej funkcyjne podejście. |

## 31. Programowanie współbieżne - mechanizmy i narzędzia na przykładzie języka Java.

### Szczegółowe wyjaśnienie

Programowanie współbieżne polega na projektowaniu programów, w których wiele zadań (wątków) może być wykonywanych "w tym samym czasie", dzieląc zasoby procesora. Jest to kluczowe dla wydajności nowoczesnych aplikacji, które działają na wielordzeniowych procesorach. Java od samego początku była projektowana z myślą o współbieżności i oferuje bogaty zestaw narzędzi do jej obsługi.

**Podstawowy model: Wątki (Threads)**

Podstawową jednostką wykonania w Javie jest **wątek**. Każdy program Javy ma co najmniej jeden wątek – główny. Nowe wątki można tworzyć na dwa sposoby:
1.  **Dziedzicząc po klasie `Thread`** i nadpisując jej metodę `run()`.
2.  **Implementując interfejs `Runnable`** i przekazując jego instancję do konstruktora klasy `Thread`. Jest to podejście preferowane, ponieważ pozwala na oddzielenie logiki zadania od mechanizmu wątku.

**Problemy współbieżności**

Gdy wiele wątków próbuje jednocześnie odczytywać i modyfikować te same dane (tzw. **stan współdzielony**), pojawiają się dwa fundamentalne problemy:
1.  **Warunki wyścigu (Race Conditions):** Wynik operacji zależy od nieprzewidywalnej kolejności wykonania instrukcji przez różne wątki. Prowadzi to do niespójności danych.
2.  **Zakleszczenie (Deadlock):** Dwa (lub więcej) wątki wpadają w stan wzajemnego oczekiwania, gdzie każdy z nich czeka na zasób zablokowany przez inny wątek.

**Mechanizmy synchronizacji**

Aby rozwiązać te problemy, Java dostarcza mechanizmy synchronizacji, które pozwalają na kontrolowanie dostępu do stanu współdzielonego.

1.  **Słowo kluczowe `synchronized`:**
    *   To podstawowy, wbudowany w język mechanizm blokujący. Każdy obiekt w Javie posiada wewnętrzną **blokadę (lock)**, zwaną też **monitorem**.
    *   `synchronized` można użyć na dwa sposoby:
        *   **Metoda zsynchronizowana:** `public synchronized void metoda() { ... }`. Gdy wątek wchodzi do takiej metody, automatycznie pozyskuje blokadę na obiekcie `this`. Inne wątki próbujące wywołać *jakąkolwiek* zsynchronizowaną metodę na *tym samym obiekcie* muszą czekać, aż blokada zostanie zwolniona.
        *   **Blok zsynchronizowany:** `synchronized(obiekt) { ... }`. Pozwala na zsynchronizowanie tylko krytycznego fragmentu kodu i jawne wskazanie obiektu, którego blokada ma być użyta. Jest to bardziej elastyczne rozwiązanie.

2.  **Słowo kluczowe `volatile`:**
    *   Gwarantuje, że odczyty i zapisy do oznaczonej nim zmiennej są zawsze widoczne dla wszystkich wątków (nie będą cachowane w rejestrach procesora). Nie zapewnia jednak atomowości operacji złożonych (jak inkrementacja), więc nie zastępuje `synchronized` w każdym przypadku.

**Zaawansowane narzędzia w pakiecie `java.util.concurrent`**

Pakiet ten, wprowadzony w Javie 5, dostarcza potężny zestaw wysokopoziomowych narzędzi do programowania współbieżnego, które są bardziej elastyczne i wydajne niż podstawowe `synchronized`.

*   **Blokady (Locks):**
    *   Interfejs `Lock` (i jego implementacja `ReentrantLock`) to bardziej elastyczny odpowiednik `synchronized`. Pozwala m.in. na próbę pozyskania blokady bez czekania (`tryLock()`) czy przerywanie wątku czekającego na blokadę.

*   **Kolekcje współbieżne:**
    *   Specjalne implementacje interfejsów z JCF, które są bezpieczne do użytku w środowisku wielowątkowym (thread-safe), np. `ConcurrentHashMap`, `CopyOnWriteArrayList`. Eliminują potrzebę ręcznej synchronizacji dostępu do kolekcji.

*   **Klasy atomowe:**
    *   Klasy takie jak `AtomicInteger` czy `AtomicLong` dostarczają atomowych operacji (np. `incrementAndGet()`), które są wykonywane jako jedna, niepodzielna operacja, bez potrzeby używania blokad. Są znacznie wydajniejsze dla prostych liczników.

*   **Egzekutory (Executor Framework):**
    *   Wysokopoziomowe API do zarządzania cyklem życia wątków. Zamiast ręcznie tworzyć i uruchamiać wątki, tworzymy **pulę wątków (`ThreadPoolExecutor`)** i zlecamy jej zadania do wykonania. Egzekutor sam zarządza wątkami, co jest znacznie wydajniejsze i pozwala uniknąć kosztu ciągłego tworzenia i niszczenia wątków.
    *   Interfejsy `Callable<V>` (zadanie zwracające wynik) i `Future<V>` (reprezentuje wynik asynchronicznego obliczenia) pozwalają na tworzenie bardziej złożonych przepływów zadań.

*   **Synchronizatory:**
    *   Narzędzia do koordynacji pracy między wątkami, np. `Semaphore` (ogranicza liczbę wątków mających dostęp do zasobu), `CountDownLatch` (pozwala jednemu lub więcej wątkom czekać na zakończenie operacji przez inne wątki), `CyclicBarrier` (pozwala grupie wątków czekać na siebie nawzajem w określonym punkcie).

## 32. Typy i metody sparametryzowane (generics) w Javie. Szablony (templates) w C++.

### Szczegółowe wyjaśnienie

Zarówno typy generyczne w Javie, jak i szablony w C++ służą temu samemu celowi: umożliwieniu pisania **kodu ogólnego (generycznego)**, który może działać na różnych typach danych bez utraty bezpieczeństwa typów. Pozwalają na tworzenie klas, interfejsów i metod, gdzie konkretny typ danych jest parametrem. Mimo wspólnego celu, ich implementacja i działanie są fundamentalnie różne.

**Typy i metody sparametryzowane (Generics) w Javie**

*   **Idea:** Typy generyczne pozwalają na zdefiniowanie klasy lub metody z "parametrem typu", np. `List<T>`. Podczas tworzenia instancji, podajemy konkretny typ, np. `List<String>`. Dzięki temu kompilator wie, że dana lista może przechowywać tylko obiekty typu `String` i pilnuje tego, zapobiegając błędom w czasie kompilacji.

*   **Implementacja – Wymazywanie typów (Type Erasure):**
    *   To kluczowa cecha generyków w Javie. Informacje o typach generycznych **istnieją tylko w czasie kompilacji**. Po skompilowaniu, wszystkie parametry typów są **wymazywane** i zastępowane ich górnym ograniczeniem (domyślnie klasą `Object`). `List<String>` w kodzie źródłowym staje się po prostu `List` w kodzie bajtowym. Kompilator dodaje niezbędne rzutowania automatycznie.
    *   **Konsekwencje:**
        *   **Zgodność wsteczna:** Mechanizm ten został wprowadzony w Javie 5 w taki sposób, aby zachować zgodność z kodem napisanym wcześniej (który operował na "surowych" kolekcjach, np. `List`).
        *   **Ograniczenia:** Nie można np. tworzyć instancji typu generycznego (`new T()`), tworzyć tablic typów generycznych (`new T[10]`) ani używać `instanceof` z parametrem typu, ponieważ w czasie wykonania informacja o typie `T` jest niedostępna.

*   **Wildcardy (`?`):**
    *   Pozwalają na tworzenie bardziej elastycznego kodu. `List<?>` oznacza listę nieznanego typu. Można też ograniczać typy, np. `List<? extends Number>` (lista przechowująca obiekty typu `Number` lub jego podklasy) lub `List<? super Integer>` (lista przechowująca obiekty typu `Integer` lub jego nadklasy).

**Szablony (Templates) w C++**

*   **Idea:** Szablony to mechanizm metaprogramowania, który pozwala kompilatorowi **generować kod** na podstawie użytych typów. Definiujemy szablon klasy lub funkcji, np. `template<typename T> class Wektor { ... }`.

*   **Implementacja – Generowanie kodu (Code Generation):**
    *   Gdy używamy szablonu z konkretnym typem, np. `Wektor<int>`, kompilator C++ **generuje zupełnie nową, osobną klasę `Wektor<int>`**, w której wszystkie wystąpienia `T` zostały zastąpione przez `int`. Jeśli użyjemy `Wektor<string>`, powstanie kolejna, niezależna klasa `Wektor<string>`.
    *   **Konsekwencje:**
        *   **Wydajność:** Kod jest w pełni zoptymalizowany dla konkretnego typu, co może prowadzić do wyższej wydajności (brak narzutu związanego z rzutowaniem czy polimorfizmem).
        *   **Elastyczność:** Szablony są znacznie potężniejsze niż generyki w Javie. Pozwalają na specjalizację szablonów dla konkretnych typów, używanie wartości (nie tylko typów) jako parametrów szablonu, a także na zaawansowane techniki metaprogramowania (np. SFINAE).
        *   **Rozmiar kodu:** Może prowadzić do tzw. "code bloat" – znacznego zwiększenia rozmiaru pliku wykonywalnego, ponieważ dla każdego użytego typu generowana jest osobna wersja kodu.
        *   **Komunikaty o błędach:** Błędy w kodzie szablonów są często bardzo długie i trudne do zrozumienia, ponieważ pojawiają się dopiero na etapie konkretyzacji szablonu.

**Tabela porównawcza**

| Cecha | Java Generics | C++ Templates |
|---|---|---|
| **Mechanizm** | **Wymazywanie typów (Type Erasure)** | **Generowanie kodu (Code Generation)** |
| **Kiedy działa?** | Tylko w czasie kompilacji. | W czasie kompilacji (generowanie kodu). |
| **Informacja o typie w czasie wykonania** | **Brak** (jest wymazywana). | **Pełna** (każda konkretyzacja to osobny typ). |
| **Elastyczność** | Ograniczona (np. brak `new T()`). | **Bardzo wysoka** (specjalizacja, metaprogramowanie). |
| **Rozmiar kodu wynikowego** | Mały (jedna wersja kodu dla wszystkich typów). | **Duży** (osobna wersja kodu dla każdego typu). |
| **Wydajność** | Potencjalnie mniejsza (narzut na rzutowanie). | **Potencjalnie wyższa** (kod specjalizowany dla typu). |
| **Zgodność wsteczna** | Tak, to był główny cel projektowy. | Nie dotyczy. |

## 33. Lambda - wyrażenia i interfejsy funkcyjne w języku Java.

### Szczegółowe wyjaśnienie

Wyrażenia lambda, wprowadzone w Javie 8, to jedna z najważniejszych zmian w historii języka. Pozwoliły one na wprowadzenie do Javy elementów **programowania funkcyjnego**, czyniąc kod bardziej zwięzłym, czytelnym i ekspresyjnym, zwłaszcza przy pracy z kolekcjami.

**Czym jest wyrażenie lambda?**

Wyrażenie lambda to **anonimowa funkcja** – zwięzły sposób na zdefiniowanie krótkiego, jednorazowego bloku kodu, który można przekazywać jako argument do metod lub przechowywać w zmiennych. Jest to w zasadzie implementacja metody z interfejsu funkcyjnego.

**Składnia:**

` (parametry) -> { ciało funkcji } `

*   ` (parametry) `: Lista parametrów, jakie przyjmuje funkcja (np. `(int a, int b)`). Nawiasy można pominąć, jeśli jest tylko jeden parametr bez typu.
*   ` -> `: Strzałka, oddzielająca parametry od ciała funkcji.
*   ` { ciało funkcji } `: Blok kodu do wykonania. Nawiasy klamrowe i słowo `return` można pominąć, jeśli ciało składa się tylko z jednej instrukcji.

**Przykład:**

Tradycyjny sposób (klasa anonimowa):
```java
Comparator<String> comparator = new Comparator<String>() {
    @Override
    public int compare(String s1, String s2) {
        return s1.length() - s2.length();
    }
};
```

Z użyciem wyrażenia lambda:
```java
Comparator<String> comparator = (s1, s2) -> s1.length() - s2.length();
```
Kod jest znacznie krótszy i bardziej czytelny.

**Interfejsy funkcyjne**

Wyrażenia lambda w Javie są nierozerwalnie związane z **interfejsami funkcyjnymi**. Interfejs funkcyjny to taki interfejs, który posiada **dokładnie jedną metodę abstrakcyjną**. Jest to warunek konieczny, aby kompilator mógł "domyślić się", którą metodę implementuje dane wyrażenie lambda.

*   **Adnotacja `@FunctionalInterface`:** Jest to opcjonalna, ale zalecana adnotacja. Jeśli oznaczymy nią interfejs, kompilator sprawdzi, czy faktycznie posiada on tylko jedną metodę abstrakcyjną. Chroni to przed przypadkowym dodaniem drugiej metody, co zepsułoby kontrakt interfejsu funkcyjnego.

*   **Wbudowane interfejsy funkcyjne (pakiet `java.util.function`):** Java 8 wprowadziła szereg gotowych, standardowych interfejsów funkcyjnych, aby nie trzeba było tworzyć własnych dla typowych zastosowań. Najważniejsze z nich to:
    *   **`Predicate<T>`:** Przyjmuje argument typu `T`, zwraca `boolean`. Służy do testowania warunków (np. filtrowania). Metoda: `boolean test(T t);`
    *   **`Function<T, R>`:** Przyjmuje argument typu `T`, zwraca wynik typu `R`. Służy do transformacji (mapowania) obiektów. Metoda: `R apply(T t);`
    *   **`Consumer<T>`:** Przyjmuje argument typu `T`, nic nie zwraca (`void`). Służy do wykonywania akcji na obiekcie. Metoda: `void accept(T t);`
    *   **`Supplier<T>`:** Nie przyjmuje argumentów, zwraca obiekt typu `T`. Służy do dostarczania/tworzenia obiektów. Metoda: `T get();`
    *   **`UnaryOperator<T>`:** Szczególny przypadek `Function`, gdzie typ wejściowy i wyjściowy są takie same (`Function<T, T>`).
    *   **`BinaryOperator<T>`:** Przyjmuje dwa argumenty typu `T`, zwraca wynik typu `T`. Służy do agregacji/redukcji (np. sumowanie). Metoda: `T apply(T t1, T t2);`

**Zastosowania wyrażeń lambda**

Wyrażenia lambda zrewolucjonizowały sposób pracy z kolekcjami w Javie, stając się podstawą **Stream API**.

*   **Przekazywanie zachowania:** Pozwalają na przekazywanie zachowania (kodu) jako argumentu do metod. Metoda `sort` z interfejsu `List` przyjmuje `Comparator` – możemy go dostarczyć w postaci lambdy.
*   **Stream API:** Całe API Strumieni opiera się na przekazywaniu lambd do metod takich jak `filter` (przyjmuje `Predicate`), `map` (przyjmuje `Function`), `forEach` (przyjmuje `Consumer`).
*   **Programowanie współbieżne:** Upraszczają tworzenie zadań do wykonania w pulach wątków (np. przekazanie lambdy do `executor.submit()`).
*   **Obsługa zdarzeń:** W aplikacjach GUI (np. JavaFX) pozwalają na zwięzłe definiowanie akcji do wykonania po kliknięciu przycisku.

## 34. Przetwarzanie strumieniowe (środki pakietu java.util.stream).

### Szczegółowe wyjaśnienie

**Stream API**, wprowadzone w Javie 8, to potężne narzędzie do **deklaratywnego przetwarzania sekwencji danych**. Strumień (`Stream`) to nie jest struktura danych, która przechowuje elementy. Jest to raczej **abstrakcja reprezentująca potok (pipeline) operacji**, które mają być wykonane na danych pochodzących z jakiegoś źródła (np. kolekcji, tablicy, pliku).

**Główne cechy Stream API:**

*   **Deklaratywność:** Opisujemy **co** chcemy zrobić z danymi, a nie **jak** (nie piszemy pętli, warunków `if` itp.). To sprawia, że kod jest bardziej zwięzły i czytelny.
*   **Leniwe przetwarzanie (Lazy Evaluation):** Operacje pośrednie (jak `filter`, `map`) nie są wykonywane natychmiast. Budują one tylko specyfikację potoku. Obliczenia ruszają dopiero w momencie wywołania **operacji terminalnej** (kończącej), np. `collect`.
*   **Jednorazowość:** Strumień można przetworzyć tylko raz. Po wywołaniu operacji terminalnej strumień jest "zużyty".
*   **Możliwość zrównoleglenia:** Ten sam potok operacji można bardzo łatwo wykonać współbieżnie, wywołując metodę `parallelStream()` zamiast `stream()`. Framework sam zajmie się podziałem pracy na wiele wątków.

**Budowa potoku strumieniowego (Pipeline)**

Typowy potok składa się z trzech części:

1.  **Źródło:** Skąd pochodzą dane. Najczęściej jest to kolekcja, na której wywołujemy metodę `stream()` lub `parallelStream()`.
    `List<String> lista = ...;`
    `Stream<String> strumien = lista.stream();`

2.  **Operacje pośrednie (Intermediate Operations):**
    *   Są to operacje, które przyjmują strumień i zwracają **nowy strumień**. Można je łączyć w łańcuchy.
    *   Są **leniwe** – nie wykonują żadnych obliczeń, tylko modyfikują definicję potoku.
    *   Najważniejsze operacje pośrednie:
        *   **`filter(Predicate<T> predicate)`:** Filtruje elementy, pozostawiając tylko te, które spełniają warunek (predykat).
        *   **`map(Function<T, R> mapper)`:** Transformuje każdy element strumienia w inny obiekt (np. zamienia obiekty `Samochod` na ich `String`-owe nazwy).
        *   **`sorted()` / `sorted(Comparator<T> comparator)`:** Sortuje elementy.
        *   **`distinct()`:** Usuwa duplikaty.
        *   **`limit(long maxSize)`:** Skraca strumień do podanej liczby elementów.

3.  **Operacja terminalna (Terminal Operation):**
    *   Jest to operacja, która **uruchamia przetwarzanie** całego potoku i produkuje wynik lub efekt uboczny. Kończy życie strumienia.
    *   Najważniejsze operacje terminalne:
        *   **`collect(Collector<T, A, R> collector)`:** Najważniejsza operacja. Służy do zebrania wyników do nowej kolekcji (np. `Collectors.toList()`, `Collectors.toSet()`, `Collectors.groupingBy()`).
        *   **`forEach(Consumer<T> action)`:** Wykonuje daną akcję dla każdego elementu.
        *   **`count()`:** Zwraca liczbę elementów w strumieniu.
        *   **`reduce(...)`:** Agreguje elementy strumienia do pojedynczej wartości (np. suma, minimum, maksimum).
        *   **`anyMatch()`, `allMatch()`, `noneMatch()`:** Sprawdzają, czy jakikolwiek/wszystkie/żaden element spełnia warunek.
        *   **`findFirst()`, `findAny()`:** Zwracają pierwszy/dowolny element (w postaci obiektu `Optional`).

**Przykład:**

Mając listę transakcji, chcemy znaleźć sumę wartości wszystkich transakcji z Warszawy z tego roku, posortowanych malejąco według wartości.

Kod imperatywny (tradycyjny):
```java
List<Transaction> warszawskieTransakcje = new ArrayList<>();
for (Transaction t : transactions) {
    if (t.getCity().equals("Warszawa") && t.getYear() == 2023) {
        warszawskieTransakcje.add(t);
    }
}
Collections.sort(warszawskieTransakcje, new Comparator<Transaction>() {
    public int compare(Transaction t1, Transaction t2) {
        return t2.getValue().compareTo(t1.getValue());
    }
});
int suma = 0;
for (Transaction t : warszawskieTransakcje) {
    suma += t.getValue();
}
```

Kod deklaratywny (Stream API):
```java
int suma = transactions.stream()
    .filter(t -> t.getCity().equals("Warszawa"))
    .filter(t -> t.getYear() == 2023)
    .sorted(Comparator.comparing(Transaction::getValue).reversed())
    .mapToInt(Transaction::getValue)
    .sum();
```
Kod jest nie tylko krótszy, ale przede wszystkim znacznie lepiej opisuje **intencję** programisty, a nie techniczną implementację pętli i warunków.

## 35. Narzędzia programowania operacji wejście-wyjścia w języku Java.

### Szczegółowe wyjaśnienie

Operacje wejścia-wyjścia (I/O) są kluczowe dla każdej aplikacji, która musi komunikować się ze światem zewnętrznym – czytać pliki, łączyć się z siecią, itp. Java oferuje kilka różnych API do obsługi I/O, które ewoluowały na przestrzeni lat.

**1. Klasyczne I/O (pakiet `java.io`)**

To oryginalne API, obecne w Javie od wersji 1.0. Jest oparte na **strumieniach (streams)**, które są jednokierunkowe i **blokujące**.

*   **Rodzaje strumieni:**
    *   **Strumienie bajtowe:** Operują na surowych bajtach. Ich klasy bazowe to `InputStream` (do odczytu) i `OutputStream` (do zapisu). Używane do pracy z danymi binarnymi (np. pliki graficzne, wykonywalne).
    *   **Strumienie znakowe:** Operują na znakach (Unicode). Ich klasy bazowe to `Reader` (do odczytu) i `Writer` (do zapisu). Używane do pracy z danymi tekstowymi. Automatycznie obsługują kodowanie znaków.

*   **Wzorzec Dekorator:** API `java.io` intensywnie wykorzystuje wzorzec projektowy Dekorator. Podstawowe strumienie (np. `FileInputStream`) łączą się z konkretnym źródłem danych. Można je "opakować" w kolejne strumienie-dekoratory, aby dodać nową funkcjonalność, np.:
    *   **Buforowanie:** `BufferedInputStream` / `BufferedReader` – znacznie zwiększają wydajność przez odczytywanie/zapisywanie danych w większych blokach, zamiast bajt po bajcie.
    *   **Obsługa typów prostych:** `DataInputStream` / `DataOutputStream` – pozwalają na odczyt/zapis typów prymitywnych Javy (`int`, `double` itp.).
    *   **Obsługa obiektów (Serializacja):** `ObjectInputStream` / `ObjectOutputStream` – pozwalają na zapisywanie całych obiektów do strumienia i ich późniejsze odtwarzanie.

*   **Charakterystyka:**
    *   **Blokujące:** Gdy wątek wywołuje operację `read()` na strumieniu, jest on **blokowany** do czasu, aż dane będą dostępne. W aplikacjach serwerowych o dużej współbieżności prowadzi to do problemu, gdzie jeden wątek jest potrzebny do obsługi jednego połączenia, co jest bardzo nieefektywne.
    *   **Proste w użyciu** dla prostych, sekwencyjnych operacji.

**2. Nowe I/O - NIO (pakiet `java.nio`)**

Wprowadzone w Javie 1.4, NIO (New I/O) to alternatywne API, zaprojektowane w celu rozwiązania problemów wydajnościowych klasycznego I/O. Jest oparte na **kanałach (channels)** i **buforach (buffers)** i wspiera **nieblokujące operacje I/O**.

*   **Główne komponenty:**
    *   **Bufory (`Buffer`):** Kontenery na dane, na których operujemy. Dane są najpierw wczytywane z kanału do bufora, a następnie przetwarzane z bufora. Podobnie, dane do zapisu są najpierw umieszczane w buforze, a potem zapisywane do kanału.
    *   **Kanały (`Channel`):** Abstrakcja reprezentująca połączenie z obiektem zdolnym do wykonywania operacji I/O (np. plik, gniazdo sieciowe). Są dwukierunkowe.
    *   **Selektory (`Selector`):** Kluczowy element nieblokującego I/O. Pozwalają jednemu wątkowi monitorować **wiele kanałów** jednocześnie i sprawdzać, który z nich jest gotowy do wykonania operacji (np. odczytu lub zapisu). Dzięki temu jeden wątek może obsługiwać setki, a nawet tysiące połączeń sieciowych, reagując tylko na te, na których faktycznie coś się dzieje.

*   **Charakterystyka:**
    *   **Nieblokujące:** Pozwala na budowanie wysoce skalowalnych serwerów.
    *   **Bardziej skomplikowane** w użyciu niż klasyczne I/O.
    *   Sercem większości nowoczesnych, wysokowydajnych frameworków sieciowych w Javie (np. Netty) jest właśnie NIO.

**3. NIO.2 (pakiet `java.nio.file`)**

Wprowadzone w Javie 7, NIO.2 to nowoczesne API do pracy z **systemem plików**. Nie zastępuje ono NIO, ale stanowi ogromne ulepszenie w stosunku do starej klasy `java.io.File`.

*   **Główne komponenty:**
    *   **`Path`:** Interfejs reprezentujący ścieżkę w systemie plików. Jest niezależny od systemu operacyjnego.
    *   **`Paths`:** Klasa fabryczna do tworzenia obiektów `Path`.
    *   **`Files`:** Klasa narzędziowa z ogromną liczbą statycznych, wygodnych metod do operacji na plikach i katalogach, np.:
        *   `Files.readAllBytes(path)` / `Files.readAllLines(path)`: Proste metody do wczytania całego pliku.
        *   `Files.write(path, bytes)`: Prosta metoda do zapisu.
        *   `Files.copy(from, to)`, `Files.move(from, to)`, `Files.delete(path)`.
        *   `Files.walkFileTree(...)`: Potężny mechanizm do rekurencyjnego przechodzenia po drzewie katalogów.
        *   Zarządzanie atrybutami plików, linkami symbolicznymi itp.

*   **Charakterystyka:**
    *   Znacznie bardziej **rozbudowane i wygodne** API niż klasa `File`.
    *   Lepsza obsługa błędów (używa wyjątków dziedziczących po `IOException`).
    *   Jest to obecnie **standardowy i zalecany** sposób na wykonywanie operacji na systemie plików w Javie.


---

# Odpowiedzi "to the point" na obronę

## 26. Konstrukcja obiektów i zarządzanie pamięcią operacyjną w Javie i C++.

W C++ obiekty można tworzyć na stosie (zarządzane automatycznie, z destruktorami) lub na stercie (zarządzane ręcznie przez `new`/`delete`), co daje wysoką wydajność, ale grozi wyciekami pamięci. W Javie wszystkie obiekty tworzone są na stercie, a pamięcią zarządza automatyczny **Garbage Collector**. Eliminuje to całą klasę błędów pamięci i upraszcza programowanie, kosztem niewielkiego narzutu wydajnościowego.

## 27. Rola klas, interfejsów i mixinów w programowaniu na przykładzie języka Java.

*   **Klasa** to szablon, który definiuje stan i zachowanie obiektu. Modeluje relację "jest czymś".
*   **Interfejs** to kontrakt, który definiuje, co obiekt musi potrafić robić, ale nie jak. Modeluje relację "potrafi robić". Pozwala na osiągnięcie polimorfizmu i luźnych powiązań.
*   **Mixin** to domieszka gotowej funkcjonalności. W Javie nie ma bezpośredniego wsparcia, ale symuluje się je za pomocą **interfejsów z metodami domyślnymi**, co pozwala na reużycie kodu bez dziedziczenia.

## 28. Pojęcie dziedziczenia na przykładzie języków Java i C++.

Dziedziczenie to mechanizm, w którym klasa pochodna przejmuje cechy klasy bazowej, modelując relację "jest rodzajem". Jego celem jest reużycie kodu. Java wspiera tylko **dziedziczenie proste** (po jednej klasie), co jest bezpieczniejsze. C++ wspiera **dziedziczenie wielokrotne**, co jest bardziej elastyczne, ale wprowadza **problem diamentowy**, rozwiązywany przez dziedziczenie wirtualne.

## 29. Istota i zastosowania polimorfizmu na przykładzie języków Java i C++.

Polimorfizm to zdolność obiektów różnych klas do reagowania na to samo wywołanie metody w specyficzny dla siebie sposób. Umożliwia traktowanie obiektów klas pochodnych przez interfejs klasy bazowej. W Javie polimorfizm dynamiczny jest **domyślny** dla wszystkich metod. W C++ jest **opcjonalny** i wymaga jawnego użycia słowa kluczowego `virtual`. Polimorfizm jest kluczem do tworzenia elastycznego i rozszerzalnego kodu.

## 30. Użycie tablic oraz innych struktur danych w Javie i C++. Java Collections Framework.

Tablice w Javie są bezpiecznymi obiektami ze sprawdzaniem granic, podczas gdy w C++ są bliższe niskopoziomowej pamięci. Do zaawansowanych struktur C++ używa **STL** (Standard Template Library) opartego na szablonach (np. `std::vector`, `std::map`). Java używa **JCF** (Java Collections Framework) opartego na interfejsach (np. `List`, `Map`) i klasach implementujących (`ArrayList`, `HashMap`). JCF jest w pełni obiektowy i bezpieczny, STL jest potencjalnie wydajniejszy.

## 31. Programowanie współbieżne - mechanizmy i narzędzia na przykładzie języka Java.

Programowanie współbieżne w Javie opiera się na **wątkach**. Podstawowym mechanizmem synchronizacji jest słowo kluczowe `synchronized`, które zapewnia wyłączny dostęp do obiektu. Nowoczesne podejście wykorzystuje jednak wysokopoziomowe narzędzia z pakietu `java.util.concurrent`, takie jak **pule wątków (ExecutorService)** do zarządzania wątkami, **kolekcje współbieżne** (`ConcurrentHashMap`) oraz **klasy atomowe** (`AtomicInteger`), które są wydajniejsze i bardziej elastyczne.

## 32. Typy i metody sparametryzowane (generics) w Javie. Szablony (templates) w C++.

Oba mechanizmy pozwalają pisać kod generyczny, działający dla wielu typów. Jednak ich implementacja jest inna. Generyki w Javie działają przez **wymazywanie typów (type erasure)** – informacja o typie istnieje tylko w czasie kompilacji. Szablony w C++ działają przez **generowanie kodu** – dla każdego użytego typu kompilator tworzy osobną wersję klasy/funkcji. Szablony C++ są potężniejsze i potencjalnie wydajniejsze, ale mogą prowadzić do większego rozmiaru kodu.

## 33. Lambda - wyrażenia i interfejsy funkcyjne w języku Java.

Wyrażenia lambda, wprowadzone w Javie 8, to zwięzły sposób na reprezentację **anonimowej funkcji**. Są one implementacją **interfejsu funkcyjnego**, czyli interfejsu z dokładnie jedną metodą abstrakcyjną. Lambdy pozwalają na przekazywanie zachowania jako argumentu do metod, co jest podstawą programowania funkcyjnego i kluczowym elementem API Strumieni (Stream API), czyniąc kod bardziej deklaratywnym i czytelnym.

## 34. Przetwarzanie strumieniowe (środki pakietu java.util.stream).

Stream API w Javie to nowoczesny, deklaratywny sposób na przetwarzanie kolekcji danych. Strumień reprezentuje **potok operacji** (pipeline), składający się ze źródła, operacji pośrednich (np. `filter`, `map`), które są leniwe, oraz operacji terminalnej (np. `collect`, `sum`), która uruchamia przetwarzanie. Pozwala to na pisanie bardziej zwięzłego i czytelnego kodu, który dodatkowo można łatwo zrównoleglić.

## 35. Narzędzia programowania operacji wejście-wyjścia w języku Java.

Java oferuje trzy główne API do obsługi I/O:
1.  **Klasyczne I/O (`java.io`):** Oparte na blokujących strumieniach bajtowych (`InputStream`/`OutputStream`) i znakowych (`Reader`/`Writer`).
2.  **NIO (`java.nio`):** Wprowadza nieblokujące I/O oparte na kanałach i buforach, kluczowe dla wysokowydajnych serwerów.
3.  **NIO.2 (`java.nio.file`):** Nowoczesne API do operacji na systemie plików, oparte na interfejsie `Path` i klasie narzędziowej `Files`. Jest to obecnie zalecany sposób pracy z plikami.

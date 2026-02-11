# Odpowiedzi na pytania do obrony pracy inżynierskiej - Podstawy Elektroniki i Techniki Cyfrowej

## 51. Implementacje podstawowych elementów pasywnych (rezystorów, kondensatorów i cewek).

### Szczegółowe wyjaśnienie

**Elementy pasywne (bierne)** to fundamentalne komponenty elektroniczne, które nie wytwarzają energii, a jedynie ją zużywają (rozpraszają) lub magazynują w polu elektrycznym lub magnetycznym. Nie potrafią wzmacniać sygnału i do działania nie wymagają zewnętrznego źródła zasilania. Trzy podstawowe elementy pasywne to rezystory, kondensatory i cewki.

**1. Rezystory (Oporniki)**

*   **Rola w obwodzie:** Głównym zadaniem rezystora jest **ograniczanie przepływu prądu elektrycznego**. Zgodnie z prawem Ohma (U = I * R), rezystor powoduje spadek napięcia proporcjonalny do płynącego przez niego prądu. Są one używane m.in. jako dzielniki napięcia, do polaryzacji tranzystorów czy jako elementy obciążające.

*   **Implementacja i budowa:**
    *   **Materiał oporowy (rezystywny):** Sercem rezystora jest materiał o określonej rezystywności. W zależności od technologii może to być warstwa węgla, tlenków metali, stopów metali lub drut oporowy.
    *   **Korpus i wyprowadzenia:** Materiał rezystywny jest umieszczony na ceramicznym korpusie, który zapewnia izolację i stabilność mechaniczną. Do korpusu przymocowane są metalowe wyprowadzenia służące do wlutowania elementu w obwód.

*   **Rodzaje implementacji:**
    *   **Rezystory do montażu przewlekanego (THT - Through-Hole Technology):** Klasyczne rezystory z długimi, drutowymi wyprowadzeniami, które przechodzą przez otwory w płytce drukowanej (PCB) i są lutowane od spodu. Są większe, ale łatwiejsze w montażu ręcznym.
        *   **Węglowe:** Tanie, ale o mniejszej precyzji i stabilności.
        *   **Metalizowane:** Najpopularniejszy typ. Cienka warstwa stopu metalu napylona na ceramiczny rdzeń zapewnia dobrą precyzję i stabilność w szerokim zakresie temperatur.
    *   **Rezystory do montażu powierzchniowego (SMD - Surface-Mount Device):** Miniaturowe, prostopadłościenne elementy bez drutowych wyprowadzeń, lutowane bezpośrednio do pól lutowniczych na powierzchni PCB. Są standardem w nowoczesnej, zminiaturyzowanej elektronice. Ich wartość jest kodowana za pomocą cyfr na obudowie.

**2. Kondensatory**

*   **Rola w obwodzie:** Głównym zadaniem kondensatora jest **magazynowanie energii w polu elektrycznym**. Kondensator przewodzi prąd zmienny, a blokuje prąd stały. Jest używany do filtrowania napięć (wygładzania tętnień w zasilaczach), w układach czasowych, do blokowania składowej stałej sygnału oraz w obwodach rezonansowych.

*   **Implementacja i budowa:**
    *   **Okładki:** Kondensator składa się z dwóch przewodzących powierzchni, zwanych okładkami.
    *   **Dielektryk:** Okładki są rozdzielone cienką warstwą materiału izolacyjnego, zwanego dielektrykiem. To właśnie rodzaj dielektryka w dużej mierze definiuje właściwości i zastosowanie kondensatora.

*   **Rodzaje implementacji:**
    *   **Kondensatory ceramiczne:** Najpopularniejszy typ, szczególnie w małych pojemnościach. Dielektrykiem jest materiał ceramiczny. Są małe, tanie i dobrze sprawdzają się w obwodach wysokiej częstotliwości. Występują zarówno w wersji THT, jak i SMD.
    *   **Kondensatory elektrolityczne:** Charakteryzują się **dużą pojemnością** przy niewielkich rozmiarach. Dielektrykiem jest bardzo cienka warstwa tlenku metalu, wytworzona chemicznie na jednej z okładek. Mają **biegunowość** (polaryzację) – muszą być podłączone do obwodu we właściwy sposób (+ do +, - do -), w przeciwnym razie mogą ulec uszkodzeniu lub eksplodować. Używane głównie do filtrowania napięcia w zasilaczach.
    *   **Kondensatory tantalowe:** Podtyp kondensatorów elektrolitycznych, oferujący jeszcze większą gęstość pojemności i lepszą stabilność niż aluminiowe, ale są droższe. Również mają biegunowość.
    *   **Kondensatory foliowe:** Dielektrykiem jest cienka folia z tworzywa sztucznego (np. poliester, polipropylen). Charakteryzują się dużą stabilnością i precyzją. Używane w obwodach audio i precyzyjnych układach analogowych.

**3. Cewki (Dławiki, Induktory)**

*   **Rola w obwodzie:** Głównym zadaniem cewki jest **magazynowanie energii w polu magnetycznym**. Cewka "przeciwstawia się" zmianom prądu – prąd nie może w niej narastać i opadać w sposób gwałtowny. Jest używana w filtrach, przetwornicach napięcia (impulsowych) oraz obwodach rezonansowych.

*   **Implementacja i budowa:**
    *   **Uzwojenie:** Cewka to po prostu przewodnik (najczęściej drut miedziany w emalii) nawinięty w postaci zwojów.
    *   **Rdzeń:** Uzwojenie może być nawinięte na powietrzu (cewka powietrzna) lub na **rdzeniu magnetycznym** (np. z ferrytu, proszku żelaznego). Rdzeń koncentruje pole magnetyczne i wielokrotnie zwiększa indukcyjność cewki.

*   **Rodzaje implementacji:**
    *   **Cewki z rdzeniem ferrytowym:** Najpopularniejszy typ. Ferryt to materiał ceramiczny o dobrych właściwościach magnetycznych w szerokim zakresie częstotliwości. Stosowane w zasilaczach impulsowych i filtrach przeciwzakłóceniowych.
    *   **Cewki z rdzeniem proszkowym:** Rdzeń wykonany ze sprasowanego proszku żelaznego. Dobrze radzą sobie z dużymi prądami bez nasycania się. Stosowane w przetwornicach dużej mocy.
    *   **Cewki powietrzne:** Bez rdzenia. Mają małą indukcyjność, ale charakteryzują się dużą liniowością (ich indukcyjność nie zależy od prądu) i brakiem strat w rdzeniu. Stosowane w obwodach radiowych bardzo wysokiej częstotliwości.
    *   Podobnie jak rezystory i kondensatory, cewki również występują w wersjach **THT** i **SMD**.


## 52. Filtr dolnoprzepustowy RC. Co to jest częstotliwość graniczna i pasmo przenoszenia filtru.

### Szczegółowe wyjaśnienie

**Filtr dolnoprzepustowy RC**

**Filtr dolnoprzepustowy** to układ elektroniczny, który **przepuszcza sygnały o częstotliwościach niższych** od pewnej częstotliwości granicznej, a **tłumi (osłabia) sygnały o częstotliwościach wyższych**. Działa jak selektywna bramka dla częstotliwości.

Najprostszą realizacją takiego filtru jest pasywny **filtr RC**, zbudowany z jednego rezystora (R) i jednego kondensatora (C).

*   **Budowa i działanie:**
    *   W najczęstszej konfiguracji, sygnał wejściowy (Vin) jest podawany na szeregowo połączony rezystor i kondensator. Sygnał wyjściowy (Vout) jest zdejmowany z kondensatora.
    *   Działanie filtru opiera się na właściwościach kondensatora, którego **reaktancja (opór dla prądu zmiennego) maleje wraz ze wzrostem częstotliwości**.
        *   **Dla niskich częstotliwości (i prądu stałego):** Kondensator ma bardzo dużą reaktancję, zachowuje się prawie jak przerwa w obwodzie. Prąd przez niego nie płynie, więc nie ma spadku napięcia na rezystorze R. W rezultacie napięcie wyjściowe jest niemal równe wejściowemu (`Vout ≈ Vin`). Sygnał jest przepuszczany.
        *   **Dla wysokich częstotliwości:** Kondensator ma bardzo małą reaktancję, zachowuje się prawie jak zwarcie do masy. Wysokie częstotliwości "znajdują" w kondensatorze łatwą drogę do masy, omijając wyjście. Powoduje to duży spadek napięcia na rezystorze R, a napięcie wyjściowe dąży do zera. Sygnał jest tłumiony.

*   **Zastosowania:**
    *   **Wygładzanie napięcia w zasilaczach:** Usuwanie tętnień (składowych zmiennych) z wyprostowanego napięcia stałego.
    *   **Filtry przeciwzakłóceniowe:** Eliminowanie szumów i zakłóceń o wysokiej częstotliwości z sygnałów.
    *   **W obwodach audio:** Jako proste regulatory barwy tonu (odcinanie wysokich tonów) lub w zwrotnicach głośnikowych do kierowania niskich częstotliwości do głośnika niskotonowego (woofera).
    *   **Integratory:** W pewnych warunkach układ RC może działać jako integrator sygnału.

**Częstotliwość graniczna (Cutoff Frequency)**

**Częstotliwość graniczna (oznaczana jako `fc` lub `fg`)** to kluczowy parametr każdego filtru. Jest to częstotliwość, która **rozdziela pasmo przepustowe od pasma zaporowego**. Innymi słowy, jest to punkt na charakterystyce częstotliwościowej filtru, w którym jego działanie znacząco się zmienia.

*   **Definicja:** Dla prostych filtrów pasywnych, częstotliwość graniczna jest zdefiniowana jako częstotliwość, przy której **moc sygnału na wyjściu filtru spada o połowę (-3 dB)** w stosunku do mocy na wejściu. Odpowiada to spadkowi **amplitudy napięcia do około 70.7%** jego wartości maksymalnej (`1/√2`).

*   **Wzór dla filtru RC:** Częstotliwość graniczna dla filtru dolnoprzepustowego RC zależy wyłącznie od wartości rezystora i kondensatora i jest obliczana ze wzoru:

    `fc = 1 / (2 * π * R * C)`

    Gdzie:
    *   `fc` - częstotliwość graniczna w Hercach (Hz)
    *   `R` - rezystancja w Omach (Ω)
    *   `C` - pojemność w Faradach (F)

    Zmieniając wartości R i C, możemy precyzyjnie "stroić" nasz filtr, decydując, które częstotliwości ma przepuszczać, a które tłumić.

**Pasmo przenoszenia (Passband)**

**Pasmo przenoszenia** to **zakres częstotliwości, które filtr przepuszcza bez znaczącego tłumienia**. Jest to fundamentalny parametr opisujący działanie filtru.

*   **Definicja:** Formalnie, jest to zakres częstotliwości, dla których tłumienie wprowadzane przez filtr jest mniejsze niż pewna ustalona wartość, najczęściej wspomniane **-3 dB**.

*   **Charakterystyka dla różnych typów filtrów:**
    *   **Filtr dolnoprzepustowy:** Pasmo przenoszenia rozciąga się **od 0 Hz do częstotliwości granicznej `fc`**.
    *   **Filtr górnoprzepustowy:** Pasmo przenoszenia rozciąga się **od częstotliwości granicznej `fc` do nieskończoności**.
    *   **Filtr środkowoprzepustowy:** Pasmo przenoszenia jest ograniczone przez **dwie częstotliwości graniczne** (dolną i górną).
    *   **Filtr środkowozaporowy:** Posiada **dwa pasma przenoszenia**, rozdzielone pasmem zaporowym.

Podsumowując, **pasmo przenoszenia** określa, **"co"** filtr przepuszcza, a **częstotliwość graniczna** jest kluczowym punktem, który definiuje **"gdzie"** kończy się to pasmo. Dla filtru dolnoprzepustowego RC, pasmo przenoszenia to wszystkie częstotliwości od zera aż do częstotliwości granicznej, którą wyznaczają wartości R i C.


## 53. Architektura harwardzka a architektura von Neumana.

### Szczegółowe wyjaśnienie

Architektura harwardzka i architektura von Neumanna to dwa fundamentalne, konkurencyjne modele organizacji systemu komputerowego. Główna różnica między nimi sprowadza się do sposobu, w jaki procesor uzyskuje dostęp do pamięci, w której przechowywane są rozkazy (kod programu) i dane.

**Architektura von Neumanna (Architektura Princeton)**

Jest to historycznie późniejsza, ale bardziej rozpowszechniona koncepcja, zaproponowana przez Johna von Neumanna w 1945 roku. Jej kluczowym założeniem jest **wspólna pamięć dla rozkazów i danych**.

*   **Kluczowe cechy:**
    1.  **Jedna, współdzielona przestrzeń pamięci:** Zarówno instrukcje programu, jak i dane, na których ten program operuje, znajdują się w tej samej pamięci operacyjnej.
    2.  **Jedna magistrala (szyna):** Procesor komunikuje się z pamięcią za pomocą jednej, wspólnej magistrali adresowej i jednej magistrali danych. Oznacza to, że w danym momencie procesor może albo pobierać z pamięci rozkaz, albo odczytywać/zapisywać dane – **nigdy obu tych rzeczy jednocześnie**.

*   **Cykl rozkazowy:** Z powodu jednej magistrali, cykl wykonania instrukcji jest sekwencyjny:
    1.  Pobierz instrukcję z pamięci.
    2.  Zdekoduj instrukcję.
    3.  Jeśli instrukcja tego wymaga, pobierz dane z pamięci (lub zapisz dane do pamięci).
    4.  Wykonaj instrukcję.

*   **Zalety:**
    *   **Prostota i elastyczność:** Architektura jest prostsza w implementacji. Pamięć może być elastycznie przydzielana między kod a dane w zależności od potrzeb programu.
    *   **Uniwersalność:** Umożliwia łatwe tworzenie programów, które mogą modyfikować same siebie w trakcie działania (choć dziś jest to rzadko stosowane i uważane za złą praktykę).

*   **Wady:**
    *   **Wąskie gardło von Neumanna (Von Neumann bottleneck):** Ponieważ procesor i pamięć dzielą jedną magistralę, jej przepustowość staje się głównym ograniczeniem wydajności całego systemu. Procesor często musi czekać na zakończenie operacji pamięci (pobranie instrukcji lub danych), zanim będzie mógł kontynuować pracę.

*   **Zastosowanie:** Komputery osobiste (PC), laptopy, serwery. W praktyce, współczesne procesory w tych komputerach stosują **zmodyfikowaną architekturę von Neumanna**, która łagodzi problem "wąskiego gardła" poprzez zastosowanie oddzielnych, szybkich pamięci podręcznych (cache) L1 dla instrukcji i danych, mimo że główna pamięć RAM pozostaje wspólna.

**Architektura harwardzka**

Jest to koncepcja starsza, wywodząca się z komputera Harvard Mark I. Jej kluczowym założeniem jest **fizyczne rozdzielenie pamięci na rozkazy i dane**.

*   **Kluczowe cechy:**
    1.  **Dwie oddzielne pamięci:** Istnieje osobna pamięć dla kodu programu (pamięć programu) i osobna pamięć dla danych (pamięć danych).
    2.  **Dwie niezależne magistrale:** Procesor jest połączony z każdą z tych pamięci za pomocą oddzielnych magistral adresowych i danych.

*   **Cykl rozkazowy:** Dzięki oddzielnym magistralom, procesor może wykonywać operacje **jednocześnie (równolegle)**:
    *   W tym samym cyklu zegara procesor może **pobierać kolejną instrukcję** z pamięci programu i jednocześnie **odczytywać lub zapisywać dane** w pamięci danych, które były potrzebne do wykonania poprzedniej instrukcji.

*   **Zalety:**
    *   **Wysoka wydajność:** Równoległy dostęp do pamięci eliminuje "wąskie gardło von Neumanna", co prowadzi do znacznie szybszego wykonywania programów. Jest to kluczowe w systemach, gdzie liczy się szybkość i determinizm działania.
    *   **Większe bezpieczeństwo:** Rozdzielenie pamięci utrudnia (lub uniemożliwia) przypadkowe nadpisanie kodu programu przez błędy w operacjach na danych. Utrudnia też ataki polegające na wstrzyknięciu i wykonaniu złośliwego kodu w obszarze danych.

*   **Wady:**
    *   **Bardziej złożona budowa:** Wymaga bardziej skomplikowanej architektury procesora i podwójnego systemu magistral.
    *   **Mniejsza elastyczność:** Pamięć jest sztywno podzielona. Jeśli program ma bardzo mało kodu, a dużo danych, to wolna pamięć programu nie może być wykorzystana na dane (i na odwrót).

*   **Zastosowanie:** **Mikrokontrolery** (np. z rodzin AVR, PIC, ARM Cortex-M), procesory sygnałowe **(DSP)**. W tych zastosowaniach kluczowa jest szybkość przetwarzania danych ze świata zewnętrznego (np. z czujników) i przewidywalny czas reakcji, a programy są zazwyczaj na stałe zapisane w pamięci Flash (pamięć programu) i operują na danych w pamięci RAM (pamięć danych).

**Porównanie: Architektura harwardzka vs von Neumanna**

| Cecha | Architektura von Neumanna | Architektura harwardzka |
|---|---|---|
| **Pamięć** | **Jedna**, wspólna dla kodu i danych | **Dwie**, oddzielne dla kodu i danych |
| **Magistrala** | **Jedna**, współdzielona | **Dwie**, niezależne |
| **Dostęp do pamięci** | Sekwencyjny (albo kod, albo dane) | **Równoległy** (kod i dane jednocześnie) |
| **Wydajność** | Ograniczona przez "wąskie gardło" | **Wysoka**, brak "wąskiego gardła" |
| **Złożoność** | Prostsza | Bardziej złożona |
| **Elastyczność pamięci** | Wysoka | Niska |
| **Główne zastosowanie** | Komputery PC, serwery | **Mikrokontrolery, procesory DSP** |


## 54. Sposoby obsługi zdarzeń w mikrokontrolerze.

### Szczegółowe wyjaśnienie

Mikrokontroler to "komputer w jednej kostce", który musi w czasie rzeczywistym reagować na sygnały i zdarzenia pochodzące ze świata zewnętrznego (np. wciśnięcie przycisku, dane z czujnika, nadejście sygnału przez interfejs komunikacyjny). Istnieją dwa fundamentalnie różne podejścia do obsługi takich zdarzeń:

**1. Odpytywanie (Polling)**

*   **Zasada działania:** Program główny mikrokontrolera działa w **nieskończonej pętli**, w której **cyklicznie i aktywnie sprawdza** stan wszystkich interesujących go wejść lub flag statusowych. Jest to podejście synchroniczne.

    ```c
    void main() {
        setup(); // Inicjalizacja
        while(1) { // Nieskończona pętla główna
            if (przycisk_wcisniety()) {
                obsluz_przycisk();
            }
            if (dane_przyszly_z_uart()) {
                obsluz_uart();
            }
            // ... inne zadania ...
        }
    }
    ```

*   **Zalety:**
    *   **Prostota:** Jest to najprostszy do zrozumienia i zaimplementowania model programowy. Przepływ sterowania jest liniowy i łatwy do śledzenia.
    *   **Przewidywalność:** Kolejność sprawdzania i obsługi zdarzeń jest ściśle zdeterminowana przez kod w pętli.

*   **Wady:**
    *   **Marnotrawstwo czasu procesora:** Procesor spędza większość czasu na bezproduktywnym sprawdzaniu warunków, które przez większość czasu są fałszywe. Jest to bardzo nieefektywne energetycznie.
    *   **Opóźniona reakcja:** Zdarzenie zostanie obsłużone dopiero wtedy, gdy program dojdzie do odpowiedniej instrukcji `if` w pętli. Jeśli pętla główna wykonuje jakieś czasochłonne zadania, czas reakcji na zdarzenie może być długi i niedeterministyczny.
    *   **Ryzyko zgubienia zdarzeń:** Jeśli zdarzenie jest bardzo krótkim impulsem (krótszym niż czas jednego obiegu pętli), program może go w ogóle nie zauważyć.

*   **Zastosowanie:** W bardzo prostych aplikacjach, gdzie czas reakcji nie jest krytyczny, a mikrokontroler nie ma wielu innych zadań do wykonania.

**2. Przerwania (Interrupts)**

*   **Zasada działania:** Jest to mechanizm **sprzętowy**, który pozwala urządzeniom peryferyjnym na **asynchroniczne przerwanie** normalnego wykonywania programu głównego w celu natychmiastowej obsługi pilnego zdarzenia.

    1.  **Wystąpienie zdarzenia:** Urządzenie peryferyjne (np. timer, pin wejściowy, moduł UART) generuje sygnał żądania przerwania (IRQ - Interrupt Request).
    2.  **Przerwanie programu:** Jeśli przerwania są globalnie włączone i dane przerwanie nie jest zamaskowane, procesor kończy wykonywać bieżącą instrukcję maszynową, automatycznie odkłada na stos adres powrotu (i ewentualnie inne rejestry), a następnie skacze pod z góry zdefiniowany adres w pamięci programu.
    3.  **Wykonanie procedury obsługi przerwania (ISR - Interrupt Service Routine):** Pod tym adresem znajduje się specjalna funkcja, napisana przez programistę, która obsługuje zdarzenie. Procedura ISR powinna być **jak najkrótsza i jak najszybsza**.
    4.  **Powrót do programu głównego:** Po zakończeniu ISR, procesor wykonuje specjalną instrukcję powrotu z przerwania, która zdejmuje ze stosu adres powrotu i wznawia wykonywanie przerwanego programu dokładnie od miejsca, w którym zostało ono przerwane. Z perspektywy programu głównego, cała operacja jest "przezroczysta".

*   **Zalety:**
    *   **Natychmiastowa reakcja:** Zdarzenia są obsługiwane niemal natychmiast po ich wystąpieniu, z minimalnym i przewidywalnym opóźnieniem (latency).
    *   **Efektywność:** Procesor nie marnuje czasu na odpytywanie. Może wykonywać inne zadania lub zostać uśpiony w celu oszczędzania energii, a "obudzi się" tylko wtedy, gdy wydarzy się coś ważnego.
    *   **Niezawodność:** Trudno jest "przegapić" zdarzenie (o ile nie jest to seria bardzo szybkich przerwań tego samego typu).

*   **Wady:**
    *   **Większa złożoność:** Programowanie z użyciem przerwań jest trudniejsze. Może prowadzić do problemów ze współbieżnością (np. gdy ISR modyfikuje dane używane w pętli głównej – tzw. warunki wyścigu) i wymaga starannego zarządzania zasobami.
    *   **Trudniejsze debugowanie:** Asynchroniczna natura przerwań sprawia, że błęgi mogą być trudne do zreprodukowania i zdiagnozowania.

*   **Zastosowanie:** Jest to standardowy i preferowany sposób obsługi zdarzeń w praktycznie wszystkich zaawansowanych systemach wbudowanych, gdzie liczy się czas reakcji i efektywność.

**Porównanie: Odpytywanie vs Przerwania**

| Cecha | Odpytywanie (Polling) | Przerwania (Interrupts) |
|---|---|---|
| **Natura** | Programowa, synchroniczna | **Sprzętowa**, asynchroniczna |
| **Inicjatywa** | Program aktywnie pyta peryferia | **Peryferia aktywnie informują** program |
| **Czas reakcji** | Długi, zmienny, nieprzewidywalny | **Krótki**, stały, przewidywalny |
| **Efektywność CPU** | Niska (ciągłe sprawdzanie) | **Wysoka** (reakcja tylko na zdarzenia) |
| **Złożoność** | Proste | Złożone (problemy współbieżności) |
| **Zastosowanie** | Proste, niekrytyczne czasowo aplikacje | **Systemy czasu rzeczywistego**, efektywne energetycznie aplikacje |

## 55. Popularne interfejsy komunikacyjne w mikrokontrolerze.

### Szczegółowe wyjaśnienie

Mikrokontrolery muszą komunikować się z innymi układami scalonymi (czujnikami, pamięciami, innymi mikrokontrolerami) oraz z urządzeniami zewnętrznymi (np. komputerem). Służą do tego zunifikowane **interfejsy (protokoły) komunikacyjne**, które definiują zarówno warstwę fizyczną (linie sygnałowe, poziomy napięć), jak i warstwę protokołu (format danych, sposób inicjowania transmisji). Najpopularniejsze interfejsy to:

**1. UART (Universal Asynchronous Receiver-Transmitter)**

*   **Charakterystyka:** Jest to prosty, **asynchroniczny** protokół szeregowy. "Asynchroniczny" oznacza, że nie ma wspólnej linii zegarowej – synchronizacja odbywa się na podstawie samego sygnału danych, który jest obudowany w bity startu i stopu.
*   **Linie sygnałowe:** Wymaga tylko **dwóch linii**:
    *   **TX (Transmit):** Linia do wysyłania danych.
    *   **RX (Receive):** Linia do odbierania danych.
    Linia TX jednego urządzenia jest łączona z linią RX drugiego i na odwrót. Wymaga również wspólnej masy (GND).
*   **Komunikacja:** Jest to protokół **point-to-point**, przeznaczony do komunikacji między dwoma urządzeniami. Działa w trybie **full-duplex** (może jednocześnie nadawać i odbierać).
*   **Zastosowanie:** Bardzo popularny do komunikacji z komputerem PC (przez wirtualny port COM, np. do debugowania), modułami GPS, modułami Bluetooth, GSM.

**2. I²C (Inter-Integrated Circuit)**

*   **Charakterystyka:** Jest to **synchroniczny**, wielopunktowy interfejs szeregowy, zaprojektowany do komunikacji między układami scalonymi na tej samej płytce drukowanej. "Synchroniczny" oznacza, że transmisji towarzyszy sygnał zegarowy.
*   **Linie sygnałowe:** Wymaga tylko **dwóch linii**:
    *   **SDA (Serial Data):** Linia danych.
    *   **SCL (Serial Clock):** Linia zegarowa.
*   **Komunikacja:** Jest to magistrala typu **multi-master, multi-slave**. Oznacza to, że do jednej, tej samej pary przewodów można podłączyć **wiele urządzeń** (zarówno masterów, jak i slave'ów). Każde urządzenie podrzędne (slave) ma unikalny, 7-bitowy adres. Komunikację zawsze inicjuje urządzenie nadrzędne (master), które najpierw wysyła adres slave'a, z którym chce rozmawiać. Działa w trybie **half-duplex**.
*   **Zastosowanie:** Idealny do komunikacji na krótkie odległości z wolniejszymi urządzeniami. Powszechnie używany do obsługi czujników (temperatury, ciśnienia), pamięci EEPROM, zegarów czasu rzeczywistego (RTC), sterowników LED.

**3. SPI (Serial Peripheral Interface)**

*   **Charakterystyka:** Jest to bardzo szybki, **synchroniczny** protokół szeregowy, również przeznaczony do komunikacji między układami na jednej płytce.
*   **Linie sygnałowe:** Zazwyczaj wymaga **czterech linii**:
    *   **MISO (Master In, Slave Out):** Linia danych od slave'a do mastera.
    *   **MOSI (Master Out, Slave In):** Linia danych od mastera do slave'a.
    *   **SCK (Serial Clock):** Linia zegarowa.
    *   **SS / CS (Slave Select / Chip Select):** Linia do wybierania konkretnego urządzenia slave. Każdy slave na magistrali musi mieć swoją osobną linię SS.
*   **Komunikacja:** Działa w architekturze **single-master, multi-slave**. Jest jeden master, który kontroluje całą komunikację. Może komunikować się z wieloma slave'ami, ale musi aktywować każdego z nich osobno za pomocą dedykowanej linii SS. Działa w trybie **full-duplex**.
*   **Zastosowanie:** Wszędzie tam, gdzie wymagana jest **wysoka prędkość transmisji**. Powszechnie używany do obsługi kart SD, wyświetlaczy graficznych, szybkich przetworników ADC/DAC, pamięci Flash.

**Porównanie popularnych interfejsów**

| Cecha | UART | I²C | SPI |
|---|---|---|---|
| **Typ** | Asynchroniczny | **Synchroniczny** | **Synchroniczny** |
| **Liczba linii** | **2** (TX, RX) | **2** (SDA, SCL) | **4** (MISO, MOSI, SCK, SS) |
| **Topologia** | Point-to-point | **Magistrala** (wiele urządzeń) | Point-to-multipoint |
| **Adresowanie** | Brak (połączenie 1-do-1) | **Programowe** (7-bitowy adres) | **Sprzętowe** (linia SS) |
| **Prędkość** | Niska | Średnia | **Bardzo wysoka** |
| **Tryb pracy** | Full-duplex | Half-duplex | Full-duplex |
| **Złożoność** | Prosty | Średnia | Prosty |
| **Główne zalety** | Prostota, mało linii | **Mało linii, wiele urządzeń** | **Prędkość** |

# Odpowiedzi na pytania do obrony pracy inżynierskiej - Systemy Operacyjne

## 56. Klasyfikacja systemów operacyjnych.

### Szczegółowe wyjaśnienie

System operacyjny (SO) to oprogramowanie zarządzające zasobami sprzętowymi komputera i tworzące środowisko do uruchamiania programów użytkowych. Ze względu na ogromną różnorodność zastosowań komputerów, systemy operacyjne można klasyfikować według różnych kryteriów.

**1. Kryterium liczby użytkowników i zadań:**

*   **Jednoużytkownikowe, jednozadaniowe:** Najprostszy typ. W danym momencie tylko jeden użytkownik może pracować i uruchamiać tylko jeden program. Historyczny przykład to **MS-DOS**.
*   **Jednoużytkownikowe, wielozadaniowe:** System pozwala jednemu użytkownikowi na uruchomienie wielu programów (procesów) jednocześnie. System operacyjny zarządza podziałem czasu procesora między te programy. Jest to standard dla współczesnych komputerów osobistych. Przykłady: **Windows, macOS, Linux (w wersji desktopowej)**.
*   **Wieloużytkownikowe, wielozadaniowe:** Wielu użytkowników może jednocześnie pracować na tym samym komputerze (np. poprzez zdalne terminale), a każdy z nich może uruchamiać wiele zadań. System musi zarządzać zasobami (CPU, pamięć, dysk) dla wszystkich użytkowników i zapewniać izolację między nimi. Przykłady: **systemy serwerowe (Linux, Windows Server), systemy uniksowe**.

**2. Kryterium sposobu przetwarzania (interakcji):**

*   **Systemy wsadowe (Batch systems):** Historycznie pierwsze systemy. Użytkownik przygotowywał "wsad" zadań (np. na kartach perforowanych), który był następnie w całości przekazywany do komputera i wykonywany bez żadnej interakcji. System optymalizował kolejność wykonywania zadań w celu maksymalnego wykorzystania zasobów. Brak interakcji z użytkownikiem w trakcie działania programu.
*   **Systemy interakcyjne (konwersacyjne):** Umożliwiają bezpośrednią interakcję użytkownika z systemem i uruchomionymi programami za pomocą wiersza poleceń lub interfejsu graficznego. Użytkownik na bieżąco otrzymuje odpowiedzi na swoje działania. Wszystkie nowoczesne systemy operacyjne są interakcyjne.

**3. Kryterium ograniczeń czasowych (determinizmu):**

*   **Systemy czasu rzeczywistego (RTOS - Real-Time Operating Systems):** Kluczowym parametrem jest tutaj nie tyle szybkość, co **gwarancja i przewidywalność czasu reakcji** na zdarzenia. System musi zagwarantować, że krytyczne zadanie zostanie wykonane w ściśle określonym, maksymalnym czasie.
    *   **Twarde systemy czasu rzeczywistego (Hard RTOS):** Niedotrzymanie terminu jest traktowane jako katastrofalny błąd systemu. Używane w systemach o krytycznym znaczeniu dla bezpieczeństwa. Przykłady: sterowniki ABS w samochodzie, systemy sterowania lotem w samolocie, sterowanie ramieniem robota na linii produkcyjnej. (np. QNX, VxWorks)
    *   **Miękkie systemy czasu rzeczywistego (Soft RTOS):** Niedotrzymanie terminu powoduje jedynie degradację jakości działania, a nie katastrofę. Zadania krytyczne czasowo mają wyższy priorytet, ale nie ma absolutnych gwarancji. Przykłady: systemy do streamingu wideo, telefonia internetowa. (np. Linux z odpowiednimi rozszerzeniami)

**4. Kryterium architektury i zastosowania:**

*   **Systemy dla komputerów osobistych (Desktop OS):** Zoptymalizowane pod kątem łatwości obsługi, interakcji z jednym użytkownikiem i obsługi szerokiej gamy oprogramowania multimedialnego i biurowego. Przykłady: **Windows 11, macOS, Ubuntu**.
*   **Systemy serwerowe (Server OS):** Zoptymalizowane pod kątem stabilności, niezawodności, wydajności i bezpieczeństwa. Zaprojektowane do ciągłej pracy (24/7) i obsługi wielu użytkowników oraz usług sieciowych (np. serwery WWW, bazy danych). Przykłady: **Linux (Debian, Red Hat), Windows Server**.
*   **Systemy wbudowane (Embedded OS):** Działają na urządzeniach o specjalnym przeznaczeniu, które są częścią większego systemu (np. router, pralka, system infotainment w samochodzie). Są skrojone na miarę, zoptymalizowane pod kątem minimalnego zużycia zasobów (pamięci, energii) i często mają charakter systemów czasu rzeczywistego. Przykłady: **FreeRTOS, Zephyr, Embedded Linux**.
*   **Systemy mobilne (Mobile OS):** Zaprojektowane dla smartfonów i tabletów. Kładą nacisk na interfejs dotykowy, zarządzanie energią, łączność bezprzewodową i bezpieczeństwo aplikacji (sandboxing). Przykłady: **Android, iOS**.

## 57. Problem szeregowania procesów/wątków w systemach operacyjnych.

### Szczegółowe wyjaśnienie

We współczesnych, wielozadaniowych systemach operacyjnych, wiele procesów (lub wątków w ramach jednego procesu) rywalizuje o dostęp do ograniczonej liczby rdzeni procesora (CPU). **Problem szeregowania (scheduling)** polega na decydowaniu, **który z gotowych do wykonania procesów powinien otrzymać dostęp do procesora, na jak długo i w jakiej kolejności**.

Komponent systemu operacyjnego odpowiedzialny za te decyzje nazywa się **planistą (schedulerem)**. Jego głównym celem jest takie zarządzanie czasem procesora, aby zoptymalizować system pod kątem różnych, często sprzecznych ze sobą, kryteriów.

**Cele i kryteria szeregowania:**

*   **Sprawiedliwość (Fairness):** Każdy proces powinien otrzymać sprawiedliwy udział w czasie procesora, aby uniknąć "głodzenia" (starvation) procesów o niskim priorytecie.
*   **Wydajność (Throughput):** Maksymalizacja liczby zadań ukończonych w jednostce czasu.
*   **Czas odpowiedzi (Response Time):** Minimalizacja czasu od zgłoszenia żądania (np. kliknięcia myszą) do pojawienia się pierwszej reakcji systemu (ważne w systemach interakcyjnych).
*   **Czas oczekiwania (Waiting Time):** Minimalizacja sumarycznego czasu, jaki procesy spędzają w kolejce procesów gotowych, czekając na przydział procesora.
*   **Czas realizacji (Turnaround Time):** Minimalizacja całkowitego czasu od uruchomienia procesu do jego zakończenia.

**Rodzaje algorytmów szeregowania:**

Algorytmy szeregowania można podzielić na dwie główne kategorie:

1.  **Algorytmy bez wywłaszczania (Non-preemptive):**
    *   **Zasada:** Gdy proces otrzyma procesor, nie można mu go odebrać, dopóki sam go nie zwolni (np. zakończy się lub przejdzie w stan oczekiwania na operację I/O).
    *   **Charakterystyka:** Proste w implementacji, ale nie nadają się do systemów interakcyjnych, ponieważ jeden długi proces może zablokować cały system.
    *   **Przykłady:**
        *   **FCFS (First-Come, First-Served):** Najprostszy algorytm. Procesy są obsługiwane w kolejności, w jakiej zgłosiły się do kolejki gotowych (jak kolejka w sklepie). Może prowadzić do "efektu konwoju", gdzie krótki proces musi długo czekać na zakończenie długiego procesu, który przybył przed nim.
        *   **SJF (Shortest Job First):** Do wykonania wybierany jest proces, który ma najkrótszy szacowany czas wykonania. Jest to algorytm optymalny pod względem minimalizacji średniego czasu oczekiwania, ale wymaga znajomości przyszłości (czasu wykonania), co jest trudne do zrealizowania w praktyce.

2.  **Algorytmy z wywłaszczaniem (Preemptive):**
    *   **Zasada:** System operacyjny (planista) może w dowolnym momencie **przerwać (wywłaszczyć)** aktualnie wykonywany proces i przydzielić procesor innemu, ważniejszemu zadaniu.
    *   **Charakterystyka:** Standard w nowoczesnych systemach operacyjnych. Pozwalają na realizację wielozadaniowości i zapewniają responsywność systemów interakcyjnych.
    *   **Przykłady:**
        *   **Round Robin (karuzelowy):** Każdy proces otrzymuje procesor na stały, krótki odcinek czasu, zwany **kwantem czasu**. Jeśli proces nie zakończy się w tym czasie, jest wywłaszczany, przenoszony na koniec kolejki gotowych, a procesor jest przydzielany następnemu procesowi z kolejki. Prosty i sprawiedliwy, kluczowy dla systemów z podziałem czasu.
        *   **Szeregowanie priorytetowe (Priority Scheduling):** Każdy proces ma przypisany priorytet. Procesor jest zawsze przydzielany procesowi o najwyższym priorytecie spośród gotowych do wykonania. Może prowadzić do głodzenia procesów o niskim priorytecie. Aby temu zapobiec, stosuje się techniki takie jak **starzenie (aging)**, czyli stopniowe zwiększanie priorytetu procesów, które długo czekają.
        *   **Wielopoziomowe kolejki sprzężenia zwrotnego (Multilevel Feedback Queues):** Najbardziej złożony, ale i najczęściej stosowany w praktyce algorytm (używany m.in. w Linuxie i Windows). Istnieje wiele kolejek gotowych, każda o innym priorytecie i (potencjalnie) innym kwancie czasu. Procesy mogą migrować między kolejkami. Nowy proces trafia do kolejki o najwyższym priorytecie. Jeśli zużyje swój kwant czasu, jest przenoszony do kolejki o niższym priorytecie (z dłuższym kwantem czasu). Procesy związane z I/O (interaktywne) pozostają w kolejkach o wysokim priorytecie, a procesy intensywnie obliczeniowe (wsadowe) naturalnie "spadają" do kolejek o niskim priorytecie. Jest to algorytm adaptacyjny, który dobrze radzi sobie z różnymi typami zadań.

## 58. Problem synchronizacji procesów/wątków w programach komputerowych oraz przedstaw jakie wsparcie w tym zakresie oferują systemy komputerowe i operacyjne.

### Szczegółowe wyjaśnienie

**Problem synchronizacji** pojawia się w systemach wielozadaniowych, gdy wiele procesów lub wątków próbuje uzyskać dostęp do **współdzielonych zasobów** (np. wspólnej zmiennej, pliku, urządzenia I/O) w sposób, który może prowadzić do niespójności danych lub nieprzewidywalnych wyników. Główną przyczyną problemów jest **przeplot instrukcji** wykonywanych przez różne wątki oraz fakt, że operacje, które w kodzie źródłowym wyglądają na atomowe (np. `x++`), w rzeczywistości składają się z wielu niepodzielnych instrukcji maszynowych (odczyt, modyfikacja, zapis).

**Przykład: Warunki wyścigu (Race Condition)**

Wyobraźmy sobie dwa wątki, które jednocześnie wykonują operację `licznik++` na współdzielonej zmiennej `licznik`, której wartość początkowa wynosi 5.

1.  Wątek A odczytuje wartość `licznik` (5).
2.  *W tym momencie planista wywłaszcza Wątek A i przydziela procesor Wątkowi B.*
3.  Wątek B odczytuje wartość `licznik` (wciąż 5).
4.  Wątek B inkrementuje swoją lokalną kopię (do 6) i zapisuje ją z powrotem do `licznik` (teraz `licznik` = 6).
5.  *Planista przywraca Wątek A.*
6.  Wątek A (który nic nie wie o działaniach Wątka B) inkrementuje swoją lokalną kopię (z 5 do 6) i zapisuje ją z powrotem do `licznik`.

Ostateczna wartość `licznik` wynosi 6, podczas gdy spodziewaliśmy się 7. Jest to klasyczny **warunek wyścigu** – wynik operacji zależy od przypadkowej kolejności wykonania instrukcji.

**Sekcja krytyczna** to fragment kodu, w którym proces uzyskuje dostęp do współdzielonego zasobu. Aby zapobiec warunkom wyścigu, musimy zapewnić **wzajemne wykluczanie (mutual exclusion)** – w danym momencie tylko jeden wątek może znajdować się w swojej sekcji krytycznej.

**Wsparcie w zakresie synchronizacji**

Zarówno sprzęt, jak i systemy operacyjne oferują mechanizmy (prymitywy synchronizacyjne), które pozwalają programistom na bezpieczne zarządzanie dostępem do współdzielonych zasobów.

**1. Wsparcie sprzętowe:**

Nowoczesne procesory dostarczają specjalnych, **atomowych instrukcji maszynowych**, które wykonują się w sposób niepodzielny. Są one fundamentem, na którym budowane są wszystkie mechanizmy programowe.

*   **Test-and-Set:** Atomowo odczytuje wartość zmiennej (flagi), ustawia ją na `true` i zwraca jej *poprzednią* wartość. Pozwala to na zaimplementowanie prostego zamka (locka).
*   **Compare-and-Swap (CAS):** Atomowo porównuje wartość w pamięci z oczekiwaną wartością i, tylko jeśli są równe, zamienia ją na nową wartość. Jest to podstawa wielu zaawansowanych, "bezzamkowych" (lock-free) struktur danych.
*   **Wyłączanie przerwań:** Na systemach jednoprocesorowych, wyłączenie przerwań na czas wykonywania sekcji krytycznej gwarantuje, że żaden inny proces nie zostanie uruchomiony. Jest to jednak operacja ryzykowna i niedostępna dla programów na poziomie użytkownika.

**2. Wsparcie systemu operacyjnego i bibliotek programistycznych:**

System operacyjny, wykorzystując wsparcie sprzętowe, udostępnia programistom wysokopoziomowe obiekty synchronizacyjne:

*   **Mutex (Mutual Exclusion lock):** Najprostszy i najpopularniejszy mechanizm. Jest to zamek, który może być w jednym z dwóch stanów: zamknięty lub otwarty. Wątek, który chce wejść do sekcji krytycznej, musi najpierw "zamknąć" (pozyskać) mutex. Jeśli mutex jest już zamknięty przez inny wątek, wątek próbujący go pozyskać jest **usypiany** (blokowany) przez system operacyjny, aż mutex zostanie zwolniony. Zapobiega to aktywnemu oczekiwaniu (busy-waiting).

*   **Semafor:** Uogólnienie mutexu. Jest to licznik chroniony operacjami atomowymi `wait()` (lub `P`) i `signal()` (lub `V`).
    *   `wait()`: Jeśli licznik jest większy od zera, dekrementuje go i kontynuuje. Jeśli jest równy zero, blokuje wątek.
    *   `signal()`: Inkrementuje licznik i, jeśli są jakieś zablokowane wątki, budzi jeden z nich.
    *   **Semafor binarny** (o wartościach 0 i 1) działa dokładnie jak mutex.
    *   **Semafor zliczający** (o wartościach > 1) pozwala na jednoczesny dostęp do puli zasobów przez ograniczoną liczbę wątków (np. ograniczona liczba połączeń z bazą danych).

*   **Zmienne warunkowe (Condition Variables):** Używane zawsze w parze z mutexem. Pozwalają wątkom na oczekiwanie na spełnienie jakiegoś **warunku**. Wątek zamyka mutex, sprawdza warunek, a jeśli nie jest on spełniony, wywołuje `wait()` na zmiennej warunkowej. Operacja ta **atomowo zwalnia mutex i usypia wątek**. Inny wątek, który zmienia stan i powoduje spełnienie warunku, wywołuje `signal()` lub `broadcast()` na zmiennej warunkowej, budząc jeden lub wszystkie oczekujące wątki. Obudzony wątek ponownie próbuje pozyskać mutex i sprawdzić warunek.

*   **Monitory:** Wysokopoziomowy koncept programistyczny (obecny np. w Javie jako słowo kluczowe `synchronized`), który łączy w sobie sekcję krytyczną (mutex) i zmienne warunkowe. Jest to obiekt lub moduł, którego metody mogą być wykonywane tylko przez jeden wątek w danym momencie, co automatycznie zapewnia wzajemne wykluczanie.

## 59. Mechanizmy obsługi pamięci operacyjnej wykorzystywane w systemach operacyjnych.

### Szczegółowe wyjaśnienie

Zarządzanie pamięcią operacyjną (RAM) jest jednym z najważniejszych i najbardziej złożonych zadań systemu operacyjnego. Jego celem jest efektywny przydział pamięci wielu procesom, zapewnienie im ochrony i izolacji, a także umożliwienie współdzielenia kodu i danych.

**Podstawowe wymagania:**

*   **Relokacja:** Programista nie wie, w którym miejscu w pamięci fizycznej zostanie umieszczony jego program. System musi zapewnić, że program będzie działał poprawnie niezależnie od tego miejsca.
*   **Ochrona:** System musi uniemożliwić jednemu procesowi dostęp do przestrzeni adresowej innego procesu (oraz do przestrzeni adresowej samego jądra SO).
*   **Współdzielenie:** Umożliwienie wielu procesom korzystania z tej samej kopii kodu (np. bibliotek systemowych) w celu oszczędności pamięci.
*   **Logiczna organizacja:** Umożliwienie programiście postrzegania pamięci jako logicznej przestrzeni adresowej, niezależnej od fizycznego układu RAM.

**Ewolucja mechanizmów zarządzania pamięcią:**

**1. Przydział ciągły (Contiguous Allocation)**

Historycznie pierwsze techniki, w których każdy proces otrzymywał jeden, ciągły blok pamięci fizycznej.

*   **Partycje stałe:** Pamięć była dzielona na stałe partycje przy starcie systemu. Proces był ładowany do najmniejszej partycji, która mogła go pomieścić. Prowadziło to do **fragmentacji wewnętrznej** (niewykorzystane miejsce wewnątrz przydzielonej partycji).
*   **Partycje zmienne:** Pamięć jest traktowana jako jeden duży blok. Proces otrzymuje dokładnie tyle pamięci, ile potrzebuje. Z czasem, po załadowaniu i zwolnieniu wielu procesów, w pamięci powstaje wiele małych, nieciągłych wolnych bloków. Prowadzi to do **fragmentacji zewnętrznej** (dostępna jest wystarczająca ilość wolnej pamięci, ale jest ona pofragmentowana na małe kawałki i nie da się jej przydzielić nowemu, dużemu procesowi).

**2. Stronicowanie (Paging)**

Jest to fundamentalny mechanizm stosowany we wszystkich nowoczesnych systemach operacyjnych, który rozwiązuje problem fragmentacji zewnętrznej.

*   **Zasada działania:**
    *   **Pamięć fizyczna** jest dzielona na małe, równej wielkości bloki, zwane **ramkami (frames)** (np. 4 KB).
    *   **Logiczna przestrzeń adresowa** każdego procesu jest również dzielona na bloki tej samej wielkości, zwane **stronami (pages)**.
    *   Gdy proces jest uruchamiany, jego strony mogą być ładowane do **dowolnych, niekoniecznie sąsiadujących ze sobą** wolnych ramek w pamięci fizycznej.

*   **Translacja adresów:**
    *   Adres generowany przez procesor (adres logiczny) składa się z dwóch części: **numeru strony** i **przesunięcia (offsetu)** w obrębie tej strony.
    *   System operacyjny dla każdego procesu utrzymuje **tablicę stron (page table)**. Tablica ta przechowuje mapowanie: dla każdego numeru strony logicznej podaje numer ramki w pamięci fizycznej, w której ta strona się znajduje.
    *   Sprzętowy moduł **MMU (Memory Management Unit)** używa tablicy stron do tłumaczenia każdego adresu logicznego na adres fizyczny. Proces ten jest przezroczysty dla programu.

*   **Zalety:** Całkowicie eliminuje fragmentację zewnętrzną. Umożliwia łatwe współdzielenie pamięci (wystarczy, że wpisy w tablicach stron dwóch procesów będą wskazywać na tę samą ramkę fizyczną).
*   **Wady:** Występuje niewielka fragmentacja wewnętrzna (jeśli proces nie zajmuje wielokrotności rozmiaru strony, ostatnia strona jest częściowo pusta). Tablice stron mogą zajmować dużo miejsca w pamięci.

**3. Segmentacja (Segmentation)**

*   **Zasada działania:** Pamięć jest postrzegana nie jako liniowa tablica bajtów, ale jako zbiór logicznych **segmentów** o zmiennej długości. Typowe segmenty to: segment kodu, segment danych, segment stosu.
*   **Translacja adresów:** Adres logiczny składa się z **numeru segmentu** i **przesunięcia** w jego obrębie. System utrzymuje **tablicę segmentów**, która dla każdego segmentu przechowuje jego adres bazowy w pamięci fizycznej i jego długość.
*   **Zalety:** Odzwierciedla logiczną strukturę programu, ułatwia ochronę (np. segment kodu można oznaczyć jako "tylko do odczytu") i współdzielenie całych segmentów.
*   **Wady:** Cierpi na problem **fragmentacji zewnętrznej**, podobnie jak partycje zmienne.

**4. Segmentacja ze stronicowaniem**

Jest to rozwiązanie hybrydowe, które łączy zalety obu technik (stosowane np. w architekturze x86). Przestrzeń adresowa jest najpierw dzielona na logiczne segmenty, a następnie każdy segment jest stronicowany. Jest to jednak rozwiązanie bardzo złożone. We współczesnych systemach 64-bitowych rola segmentacji została zmarginalizowana na rzecz "płaskiego" modelu pamięci opartego niemal wyłącznie na stronicowaniu.

## 60. Istota mechanizmu pamięci wirtualnej - wady i zalety tego rozwiązania.

### Szczegółowe wyjaśnienie

**Pamięć wirtualna** to potężna abstrakcja i jeden z najważniejszych mechanizmów w nowoczesnych systemach operacyjnych. Jest to technika, która daje każdemu procesowi iluzję posiadania **własnej, prywatnej, ciągłej i bardzo dużej przestrzeni adresowej**, niezależnej od fizycznie dostępnej pamięci RAM.

**Istota mechanizmu:**

Pamięć wirtualna jest najczęściej implementowana w oparciu o **stronicowanie na żądanie (demand paging)**.

*   **Stronicowanie na żądanie:** Gdy proces jest uruchamiany, system operacyjny **nie ładuje** od razu wszystkich jego stron do pamięci RAM. Zamiast tego, tworzy w pamięci tablicę stron dla tego procesu, ale ładuje do ramek tylko te strony, które są absolutnie niezbędne do rozpoczęcia jego działania (lub nie ładuje żadnej).
*   **Błąd strony (Page Fault):** Gdy proces próbuje odwołać się do adresu w stronie, której nie ma aktualnie w pamięci RAM (w tablicy stron jest ona oznaczona jako "nieobecna"), sprzęt MMU generuje specjalny wyjątek, zwany **błędem strony (page fault)**. Jest to pułapka (trap) do jądra systemu operacyjnego.
*   **Obsługa błędu strony:** System operacyjny przejmuje kontrolę i:
    1.  Sprawdza, czy odwołanie było legalne (czy adres należy do logicznej przestrzeni procesu).
    2.  Znajduje żądaną stronę na dysku twardym (w specjalnym pliku wymiany - swap file, lub w pliku wykonywalnym programu).
    3.  Znajduje wolną ramkę w pamięci RAM. Jeśli wolnej ramki nie ma, musi wybrać jedną z zajętych ramek (należącą do tego lub innego procesu) i "ofiarować" ją. Jeśli zawartość tej ramki-ofiary była modyfikowana, musi najpierw zapisać ją z powrotem na dysk. Ten proces nazywa się **wymianą stron (swapping)**.
    4.  Wczytuje żądaną stronę z dysku do zwolnionej ramki.
    5.  Aktualizuje tablicę stron, aby odzwierciedlała nową lokalizację strony.
    6.  Wznawia wykonanie przerwanej instrukcji, która teraz może już odwołać się do danych w pamięci.

Cały ten proces jest całkowicie **przezroczysty** dla programu. Z jego perspektywy, po prostu uzyskał dostęp do pamięci, choć z pewnym opóźnieniem.

**Zalety pamięci wirtualnej:**

1.  **Możliwość uruchamiania programów większych niż fizyczna pamięć RAM:** Jest to największa zaleta. W pamięci RAM muszą znajdować się tylko te fragmenty programu i danych, które są aktualnie używane. Reszta może spokojnie rezydować na znacznie większym, ale i wolniejszym dysku twardym.
2.  **Zwiększona wielozadaniowość:** Ponieważ każdy proces zajmuje w pamięci RAM tylko tyle miejsca, ile aktualnie potrzebuje, system może uruchomić znacznie więcej procesów jednocześnie, co prowadzi do lepszego wykorzystania procesora.
3.  **Izolacja i ochrona przestrzeni adresowych:** Każdy proces działa we własnej, odizolowanej przestrzeni wirtualnej. Jeden proces nie ma żadnej możliwości, aby odwołać się do pamięci innego procesu, co drastycznie zwiększa stabilność i bezpieczeństwo systemu.
4.  **Uproszczone zarządzanie pamięcią dla programisty:** Programista nie musi martwić się o to, ile jest dostępnej pamięci RAM. Może zakładać, że ma do dyspozycji ogromną, liniową przestrzeń adresową (np. 2^64 bajtów w systemach 64-bitowych).
5.  **Efektywne współdzielenie pamięci:** Wiele procesów może mapować te same strony fizyczne (np. z kodem bibliotek systemowych) do swoich wirtualnych przestrzeni adresowych, co pozwala na załadowanie danej biblioteki do RAM tylko raz, oszczędzając pamięć.
6.  **Szybsze uruchamianie programów:** Program może zacząć działać, zanim zostanie w całości wczytany z dysku. Reszta jest doładowywana "na żądanie".

**Wady pamięci wirtualnej:**

1.  **Spadek wydajności:** Obsługa błędu strony jest operacją bardzo kosztowną czasowo, ponieważ wymaga dostępu do dysku twardego, który jest o rzędy wielkości wolniejszy niż pamięć RAM. Jeśli system spędza zbyt dużo czasu na obsłudze błędów stron (tzw. **szamotanie się, thrashing**), jego wydajność drastycznie spada.
2.  **Złożoność sprzętowa i programowa:** Wymaga skomplikowanego wsparcia sprzętowego (MMU) oraz bardzo złożonych algorytmów w systemie operacyjnym (np. algorytmów zastępowania stron, które decydują, którą stronę usunąć z pamięci, gdy brakuje wolnych ramek).
3.  **Zwiększone zapotrzebowanie na przestrzeń dyskową:** Wymaga dedykowanego miejsca na dysku na plik wymiany (swap file).


---

# Odpowiedzi "to the point" na obronę

## 51. Implementacje podstawowych elementów pasywnych (rezystorów, kondensatorów i cewek).

*   **Rezystor:** Ogranicza prąd. Implementowany jako warstwa materiału oporowego (węgiel, metal) na ceramicznym rdzeniu. Występuje w wersji przewlekanej (THT) i miniaturowej powierzchniowej (SMD).
*   **Kondensator:** Magazynuje energię w polu elektrycznym. Zbudowany z dwóch okładek rozdzielonych dielektrykiem. Najpopularniejsze to ceramiczne (małe pojemności, wysokie częstotliwości) i elektrolityczne (duże pojemności, do filtrowania zasilania, mają biegunowość).
*   **Cewka:** Magazynuje energię w polu magnetycznym. Zbudowana z drutu nawiniętego na rdzeniu (np. ferrytowym) lub bez niego (powietrzna). Używana w przetwornicach i filtrach.

## 52. Filtr dolnoprzepustowy RC. Co to jest częstotliwość graniczna i pasmo przenoszenia filtru.

**Filtr dolnoprzepustowy RC** to prosty układ z rezystora i kondensatora, który przepuszcza niskie częstotliwości, a tłumi wysokie. **Częstotliwość graniczna (`fc`)** to punkt, w którym moc sygnału spada o połowę (-3 dB). Wyznacza ona granicę między tym, co filtr przepuszcza, a co tłumi. Oblicza się ją ze wzoru `fc = 1 / (2πRC)`. **Pasmo przenoszenia** to zakres częstotliwości, które filtr przepuszcza, czyli dla filtru dolnoprzepustowego jest to zakres od 0 Hz do częstotliwości granicznej.

## 53. Architektura harwardzka a architektura von Neumana.

Są to dwa modele organizacji komputera. Główna różnica to sposób dostępu do pamięci.
*   **Architektura von Neumanna:** Posiada **jedną, wspólną pamięć** dla kodu i danych oraz jedną magistralę. Jest prostsza, ale jej wydajność ogranicza tzw. "wąskie gardło von Neumanna". Stosowana w komputerach PC.
*   **Architektura harwardzka:** Posiada **dwie oddzielne pamięci** i dwie niezależne magistrale – jedną dla kodu, drugą dla danych. Pozwala to na równoległy dostęp do obu pamięci, co znacznie zwiększa wydajność. Stosowana w mikrokontrolerach i procesorach DSP.

## 54. Sposoby obsługi zdarzeń w mikrokontrolerze.

Istnieją dwa główne sposoby:
*   **Odpytywanie (Polling):** Program w nieskończonej pętli **cyklicznie sprawdza** stan wejść. Jest to proste, ale nieefektywne i powoduje opóźnienia w reakcji.
*   **Przerwania (Interrupts):** Jest to mechanizm **sprzętowy**. Zdarzenie (np. wciśnięcie przycisku) automatycznie przerywa główny program i uruchamia specjalną funkcję obsługi przerwania (ISR). Jest to bardzo efektywne i zapewnia natychmiastową reakcję. To standard w systemach wbudowanych.

## 55. Popularne interfejsy komunikacyjne w mikrokontrolerze.

*   **UART:** Prosta, asynchroniczna komunikacja szeregowa na 2 liniach (TX, RX). Używany do komunikacji z PC, modułami GPS, Bluetooth.
*   **I²C:** Synchroniczna magistrala na 2 liniach (SDA, SCL), która pozwala podłączyć **wiele urządzeń** do tych samych przewodów. Każde urządzenie ma swój adres. Używany do wolniejszych peryferiów, jak czujniki, pamięci EEPROM.
*   **SPI:** Bardzo szybka, synchroniczna komunikacja na 4 liniach. Idealna do wymagających dużej przepustowości urządzeń, jak karty SD, wyświetlacze graficzne, szybkie przetworniki.

---

## 56. Klasyfikacja systemów operacyjnych.

Systemy operacyjne klasyfikujemy m.in. ze względu na:
*   **Liczbę użytkowników i zadań:** Jedno- i wielozadaniowe, jedno- i wieloużytkownikowe (np. MS-DOS vs Windows vs Linux Server).
*   **Ograniczenia czasowe:** **Systemy czasu rzeczywistego (RTOS)**, które gwarantują czas reakcji (np. w ABS), w przeciwieństwie do systemów ogólnego przeznaczenia.
*   **Zastosowanie:** **Desktopowe** (Windows, macOS), **serwerowe** (Linux Server), **mobilne** (Android, iOS) i **wbudowane** (FreeRTOS).

## 57. Problem szeregowania procesów/wątków w systemach operacyjnych.

**Szeregowanie** to zadanie planisty systemu operacyjnego, polegające na decydowaniu, który z gotowych procesów ma otrzymać procesor i na jak długo. Celem jest m.in. sprawiedliwość i wydajność. Algorytmy z **wywłaszczaniem** (jak **Round Robin** czy **wielopoziomowe kolejki sprzężenia zwrotnego** stosowane w nowoczesnych SO) pozwalają na przerwanie procesu i przydzielenie CPU innemu, co jest kluczowe dla wielozadaniowości i responsywności systemu.

## 58. Problem synchronizacji procesów/wątków w programach komputerowych oraz przedstaw jakie wsparcie w tym zakresie oferują systemy komputerowe i operacyjne.

**Problem synchronizacji** występuje, gdy wiele wątków uzyskuje dostęp do współdzielonych danych, co może prowadzić do **warunków wyścigu** i niespójności danych. Aby temu zapobiec, stosuje się **wzajemne wykluczanie**. Sprzęt oferuje **atomowe instrukcje** (np. Test-and-Set). System operacyjny buduje na nich wysokopoziomowe prymitywy, takie jak **mutexy** (zamki zapewniające wyłączny dostęp), **semafory** (liczniki kontrolujące dostęp do puli zasobów) oraz **zmienne warunkowe**.

## 59. Mechanizmy obsługi pamięci operacyjnej wykorzystywane w systemach operacyjnych.

Nowoczesne systemy operacyjne używają **stronicowania (paging)**. Pamięć fizyczna jest dzielona na **ramki**, a logiczna przestrzeń procesu na **strony**. Strony mogą być umieszczane w dowolnych, nieciągłych ramkach. Sprzętowy moduł **MMU** tłumaczy adresy logiczne na fizyczne za pomocą **tablicy stron** prowadzonej dla każdego procesu. Stronicowanie eliminuje problem fragmentacji zewnętrznej i ułatwia ochronę oraz współdzielenie pamięci.

## 60. Istota mechanizmu pamięci wirtualnej - wady i zalety tego rozwiązania.

**Pamięć wirtualna** to technika dająca każdemu procesowi iluzję posiadania własnej, ogromnej przestrzeni adresowej, niezależnej od fizycznego RAMu. Jest implementowana przez **stronicowanie na żądanie**: strony są wczytywane z dysku do RAMu dopiero wtedy, gdy są potrzebne (po wystąpieniu **błędu strony**).
*   **Zalety:** Możliwość uruchamiania programów większych niż RAM, większa wielozadaniowość, izolacja procesów.
*   **Wady:** Spadek wydajności, gdy system musi często wczytywać strony z wolnego dysku (tzw. szamotanie się).

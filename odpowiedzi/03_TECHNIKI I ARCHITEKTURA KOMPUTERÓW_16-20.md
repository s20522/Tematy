# Odpowiedzi na pytania do obrony pracy inżynierskiej - Techniki i Architektura Komputerów

## 16. Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce.

### Szczegółowe wyjaśnienie

To pytanie dotyczy dwóch fundamentalnych, ale różnych koncepcji, które leżą u podstaw całej współczesnej informatyki. Maszyna Turinga to **model teoretyczny** tego, co w ogóle da się obliczyć, podczas gdy architektura von Neumanna to **praktyczny schemat budowy** komputera, który te obliczenia wykonuje.

**Maszyna Turinga - Model Obliczeniowy**

*   **Czym jest?** Maszyna Turinga, opisana przez Alana Turinga w 1936 roku, to **abstrakcyjny, matematyczny model obliczeń**. Nie jest to fizyczne urządzenie, ale koncepcja, która formalizuje pojęcie algorytmu. Składa się z trzech głównych elementów:
    1.  **Nieskończonej taśmy**, podzielonej na komórki, z których każda może zawierać jeden symbol.
    2.  **Głowicy**, która może odczytywać i zapisywać symbole na taśmie oraz przesuwać się w lewo lub w prawo.
    3.  **Układu sterującego**, który posiada skończoną liczbę stanów i tablicę reguł (program). Reguła mówi, co maszyna ma zrobić (zapisać symbol, przesunąć głowicę, zmienić stan) na podstawie bieżącego stanu i odczytanego symbolu.

*   **Rola w informatyce:** Rola maszyny Turinga jest absolutnie kluczowa dla **teorii obliczeń**.
    *   **Definicja obliczalności:** **Teza Churcha-Turinga** mówi, że każdy problem, który da się rozwiązać za pomocą jakiegokolwiek intuicyjnie rozumianego algorytmu, da się też rozwiązać za pomocą maszyny Turinga. Oznacza to, że maszyna Turinga definiuje granice tego, co jest w ogóle **obliczalne**. Jeśli czegoś nie da się obliczyć na maszynie Turinga (np. problem stopu), to nie da się tego obliczyć na żadnym komputerze, ani obecnym, ani przyszłym.
    *   **Podstawa teorii złożoności:** Analiza liczby kroków, jaką maszyna Turinga musi wykonać, aby rozwiązać problem, jest podstawą do klasyfikacji problemów na klasy złożoności (np. P, NP).
    *   **Uniwersalna Maszyna Turinga:** Turing pokazał, że można skonstruować jedną, uniwersalną maszynę, która potrafi symulować działanie każdej innej, specjalistycznej maszyny Turinga. Wystarczy na jej taśmie zapisać opis (program) maszyny do zasymulowania oraz jej dane wejściowe. Jest to teoretyczna podstawa dla idei **komputera ogólnego przeznaczenia**, który może wykonywać dowolne programy.

**Architektura von Neumanna - Model Architekturalny**

*   **Czym jest?** Architektura von Neumanna, opisana przez Johna von Neumanna w 1945 roku, to **praktyczny projekt budowy komputera cyfrowego**. To właśnie według tego schematu zbudowana jest zdecydowana większość dzisiejszych komputerów, od smartfonów po superkomputery. Składa się ona z trzech głównych, połączonych ze sobą komponentów:
    1.  **Jednostki centralnej (CPU)**, która zawiera:
        *   **Jednostkę arytmetyczno-logiczną (ALU)** do wykonywania obliczeń.
        *   **Układ sterowania (Control Unit)** do interpretowania instrukcji i kierowania przepływem danych.
    2.  **Pamięci operacyjnej**, która przechowuje dane.
    3.  **Urządzeń wejścia/wyjścia (I/O)** do komunikacji ze światem zewnętrznym.

*   **Kluczowa koncepcja - Stored-Program Computer:** Najważniejszą innowacją w architekturze von Neumanna jest to, że **program (instrukcje) jest przechowywany w tej samej pamięci co dane**. CPU pobiera z pamięci zarówno instrukcje do wykonania, jak i dane, na których ma operować. Oznacza to, że program może być traktowany jak dane – można go modyfikować, tworzyć i ładować w trakcie działania komputera. To właśnie ta cecha odróżnia komputery von Neumanna od wcześniejszych maszyn, które trzeba było fizycznie przeprogramowywać (np. przez przełączanie kabli).

*   **Rola w informatyce:** Architektura von Neumanna to **praktyczny fundament współczesnych komputerów**.
    *   **Uniwersalność:** Dzięki koncepcji przechowywanego programu, komputery stały się urządzeniami uniwersalnymi, zdolnymi do wykonywania dowolnych zadań poprzez załadowanie odpowiedniego oprogramowania.
    *   **Wąskie gardło (Bottleneck):** Wspólna magistrala dla danych i instrukcji, łącząca CPU z pamięcią, jest jednocześnie największą słabością tej architektury. Nazywa się to **"wąskim gardłem von Neumanna"**, ponieważ przepustowość tej magistrali ogranicza ogólną wydajność systemu – CPU często musi czekać na dane z wolniejszej pamięci.

**Podsumowanie porównania**

| Cecha | Maszyna Turinga | Architektura von Neumanna |
|---|---|---|
| **Rodzaj modelu** | Teoretyczny model obliczeń | Praktyczny model budowy komputera |
| **Cel** | Zdefiniowanie granic obliczalności | Stworzenie uniwersalnego komputera |
| **Pamięć** | Nieskończona taśma | Skończona, adresowalna pamięć operacyjna |
| **Program** | Zapisany w tablicy stanów | Przechowywany w pamięci razem z danymi |
| **Dostęp do pamięci** | Sekwencyjny (przesuwanie głowicy) | Losowy (dostęp do dowolnej komórki po adresie) |
| **Rola w informatyce** | Podstawa teorii obliczeń i złożoności | Podstawa budowy praktycznie wszystkich komputerów |


## 17. Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów.

### Szczegółowe wyjaśnienie

**Czym jest logika boolowska?**

Logika boolowska, nazwana tak na cześć George'a Boole'a, to dział logiki i matematyki, który operuje na dwóch wartościach: **prawda (True)** i **fałsz (False)**. W kontekście komputerów, wartości te są reprezentowane przez dwa stany napięcia elektrycznego: wysoki (np. +5V), oznaczający **1 (prawda)**, i niski (np. 0V), oznaczający **0 (fałsz)**. Cała potęga logiki boolowskiej polega na tym, że definiuje ona proste operacje, które pozwalają na manipulowanie tymi dwiema wartościami.

**Podstawowe operacje (operatory) logiki Boole'a:**

1.  **Koniunkcja (AND - "i"):** Wynik jest prawdą (1) tylko wtedy, gdy **oba** argumenty są prawdą. Wystarczy jeden fałsz, aby wynik był fałszem.
    *   `1 AND 1 = 1`
    *   `1 AND 0 = 0`
    *   `0 AND 1 = 0`
    *   `0 AND 0 = 0`

2.  **Alternatywa (OR - "lub"):** Wynik jest prawdą (1), jeśli **przynajmniej jeden** z argumentów jest prawdą. Wynik jest fałszem (0) tylko wtedy, gdy oba argumenty są fałszem.
    *   `1 OR 1 = 1`
    *   `1 OR 0 = 1`
    *   `0 OR 1 = 1`
    *   `0 OR 0 = 0`

3.  **Negacja (NOT - "nie"):** Operator jednoargumentowy, który **odwraca** wartość logiczną. Prawdę zamienia na fałsz, a fałsz na prawdę.
    *   `NOT 1 = 0`
    *   `NOT 0 = 1`

Te trzy podstawowe operacje stanowią kompletny system, co oznacza, że za ich pomocą można wyrazić każdą, dowolnie skomplikowaną funkcję logiczną.

**Zastosowanie w warstwie sprzętowej - Bramki logiczne**

Logika boolowska jest fundamentem, na którym zbudowana jest cała cyfrowa elektronika. Fizyczną realizacją operacji boolowskich w sprzęcie są **bramki logiczne**. Bramka logiczna to prosty układ elektroniczny (zbudowany najczęściej z tranzystorów), który ma jedno lub więcej wejść i jedno wyjście. Stan na wyjściu (napięcie wysokie lub niskie) jest funkcją logiczną stanów na wejściach.

*   Bramka **AND** realizuje operację koniunkcji.
*   Bramka **OR** realizuje operację alternatywy.
*   Bramka **NOT** (nazywana też inwerterem) realizuje operację negacji.

Istnieją też inne, pochodne bramki, które są bardzo popularne ze względu na prostotę implementacji:

*   **NAND (NOT AND):** Działa jak bramka AND, ale z zanegowanym wyjściem. Jest to bramka uniwersalna – za pomocą samych bramek NAND można zbudować każdą inną bramkę (AND, OR, NOT).
*   **NOR (NOT OR):** Działa jak bramka OR z zanegowanym wyjściem. Również jest bramką uniwersalną.
*   **XOR (Exclusive OR - "albo"):** Wynik jest prawdą (1) tylko wtedy, gdy wejścia są **różne**. Jest to kluczowa bramka w arytmetyce komputerowej.

**Od bramek logicznych do procesora**

Geniusz inżynierii cyfrowej polega na tym, że z tych niezwykle prostych klocków (bramek logicznych) można budować coraz bardziej złożone układy, które realizują konkretne zadania:

1.  **Sumator (Adder):** Łącząc bramki XOR i AND, można zbudować **półsumator**, który dodaje dwie pojedyncze cyfry binarne, dając w wyniku sumę i przeniesienie. Łącząc dwa półsumatory i bramkę OR, otrzymujemy **pełny sumator**, który dodaje trzy bity (dwa bity danych i bit przeniesienia z poprzedniej pozycji).

2.  **Jednostka arytmetyczno-logiczna (ALU):** Łącząc szeregowo wiele pełnych sumatorów, można zbudować układ, który dodaje całe liczby wielobitowe (np. 64-bitowe). Dodając do tego układy realizujące inne operacje (odejmowanie, mnożenie, operacje logiczne), otrzymujemy serce każdego procesora – **ALU**.

3.  **Pamięć (przerzutniki):** Odpowiednio łącząc bramki logiczne (np. dwie bramki NAND), można stworzyć **przerzutnik (flip-flop)**. Jest to układ, który potrafi "zapamiętać" jeden bit informacji – pozostaje w stanie 0 lub 1, dopóki nie zostanie zmieniony przez sygnał zewnętrzny. Przerzutniki są podstawowym budulcem ultraszybkiej pamięci podręcznej (cache) i rejestrów procesora.

4.  **Układy sterujące:** Z bramek i przerzutników buduje się multipleksery (wybierają jeden z wielu sygnałów), demultipleksery (kierują sygnał na jedno z wielu wyjść), dekodery (interpretują kod instrukcji) i liczniki. Te elementy tworzą **układ sterowania** procesora, który orkiestruje całym procesem wykonywania programu.

Podsumowując, logika boolowska dostarcza teoretycznych podstaw, a bramki logiczne są fizycznymi klockami, z których, niczym z LEGO, buduje się całą skomplikowaną architekturę współczesnego komputera. Każda operacja, od prostego dodawania, przez wyświetlanie grafiki, po działanie systemu operacyjnego, sprowadza się na najniższym poziomie do miliardów operacji na zerach i jedynkach, wykonywanych przez bramki logiczne.


## 18. Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa.

### Szczegółowe wyjaśnienie

Komputery, na najniższym poziomie, operują wyłącznie na bitach, czyli zerach i jedynkach. Dlatego, aby móc wykonywać obliczenia, konieczne jest przedstawienie wszystkich typów liczb – zarówno całkowitych, jak i rzeczywistych – w systemie binarnym. Sposób tego zapisu ma fundamentalne znaczenie dla arytmetyki komputerowej.

**Zapis binarny liczb całkowitych**

Liczby całkowite można zapisywać na kilka sposobów, w zależności od tego, czy potrzebujemy reprezentować liczby ujemne.

1.  **Naturalny Kod Binarny (NKB):**
    *   Służy do zapisu **liczb naturalnych (nieujemnych)**.
    *   Jest to standardowy system dwójkowy, w którym każda pozycja ma wagę kolejnej potęgi liczby 2. Np. liczba `1011` w NKB to `1*2³ + 0*2² + 1*2¹ + 1*2⁰ = 8 + 0 + 2 + 1 = 11`.
    *   Na `n` bitach można zapisać liczby z zakresu od 0 do `2ⁿ - 1`.

2.  **Kod Znak-Moduł (ZM):**
    *   Prosty sposób na zapis liczb ujemnych. Najstarszy (najbardziej znaczący) bit jest traktowany jako **bit znaku** (0 dla liczb dodatnich, 1 dla ujemnych), a pozostałe bity reprezentują **moduł (wartość bezwzględną)** liczby w NKB.
    *   Przykład (na 8 bitach): `00000101` to `+5`, a `10000101` to `-5`.
    *   **Wady:** Posiada dwie reprezentacje zera (`+0` i `-0`), co jest niejednoznaczne. Arytmetyka w tym kodzie jest skomplikowana – trzeba osobno rozpatrywać znaki i moduły liczb.

3.  **Kod Uzupełnieniowy do Dwóch (U2 / ZU2):**
    *   To **standardowy i powszechnie stosowany** sposób zapisu liczb całkowitych ze znakiem we współczesnych komputerach.
    *   Liczby dodatnie zapisuje się tak samo jak w NKB (z najstarszym bitem równym 0).
    *   Liczbę ujemną `-x` tworzy się poprzez wykonanie **negacji bitowej** na zapisie liczby dodatniej `x`, a następnie **dodanie jedynki**.
    *   Przykład (na 8 bitach): Aby zapisać `-5`, bierzemy `+5` (`00000101`), negujemy bity (`11111010`) i dodajemy 1, co daje `11111011`.
    *   **Zalety:** Ma tylko jedną reprezentację zera. Co najważniejsze, **operacja dodawania działa tak samo dla liczb dodatnich i ujemnych**, co drastycznie upraszcza budowę jednostki arytmetyczno-logicznej (ALU). Odejmowanie `A - B` realizuje się jako dodawanie `A + (-B)`.

**Zapis zmiennoprzecinkowy liczb rzeczywistych (Standard IEEE 754)**

Liczby rzeczywiste (ułamkowe) są reprezentowane w komputerach zgodnie ze standardem **IEEE 754**. Jest to rodzaj **notacji naukowej w systemie binarnym**. Każda liczba jest przedstawiana w postaci:

`Liczba = Znak * Mantysa * 2 ^ Wykładnik`

Standard IEEE 754 definiuje kilka formatów precyzji, z których najpopularniejsze to:

*   **Pojedyncza precyzja (single-precision, `float`, 32 bity):**
    *   **1 bit znaku (S):** 0 dla dodatnich, 1 dla ujemnych.
    *   **8 bitów wykładnika (E):** Przechowuje wykładnik potęgi dwójki z przesunięciem (bias), aby móc reprezentować zarówno duże, jak i małe liczby.
    *   **23 bity mantysy (M):** Reprezentuje cyfry znaczące liczby. Warto zauważyć, że w znormalizowanej postaci pierwsza cyfra mantysy jest zawsze równa 1, więc nie jest ona jawnie zapisywana (tzw. "ukryty bit"), co daje dodatkowy bit precyzji.

*   **Podwójna precyzja (double-precision, `double`, 64 bity):**
    *   **1 bit znaku (S)**
    *   **11 bitów wykładnika (E)**
    *   **52 bity mantysy (M)**

**Arytmetyka komputerowa**

Arytmetyka komputerowa to dziedzina zajmująca się realizacją operacji arytmetycznych w systemach cyfrowych. Ze względu na skończoną liczbę bitów do reprezentacji liczb, ma ona swoje specyficzne cechy:

*   **Ograniczony zakres i precyzja:** Liczby całkowite mają ograniczony zakres (np. 32-bitowy `int` może przechowywać wartości od ok. -2 miliardów do +2 miliardów). Przekroczenie tego zakresu prowadzi do błędu **przepełnienia (overflow)**. Liczby zmiennoprzecinkowe mają ograniczoną precyzję, co oznacza, że nie każdą liczbę rzeczywistą da się dokładnie zapisać. Prowadzi to do **błędów zaokrągleń**.

*   **Błędy arytmetyki zmiennoprzecinkowej:** Ze względu na błędy zaokrągleń, wyniki operacji na liczbach zmiennoprzecinkowych mogą być nieintuicyjne. Na przykład, `0.1 + 0.2` w komputerze nie jest idealnie równe `0.3`. Dlatego nigdy nie należy porównywać liczb zmiennoprzecinkowych za pomocą operatora ścisłej równości (`==`). Zamiast tego, należy sprawdzać, czy ich różnica jest mniejsza od pewnej małej wartości (epsilon).

*   **Operacje na poziomie sprzętowym:**
    *   **Dodawanie/Odejmowanie:** Dla liczb całkowitych w kodzie U2 jest realizowane przez prosty układ sumatora. Dla liczb zmiennoprzecinkowych jest to bardziej skomplikowane – wymaga wyrównania wykładników, dodania mantys i normalizacji wyniku.
    *   **Mnożenie/Dzielenie:** Są to operacje bardziej złożone, realizowane sprzętowo za pomocą algorytmów opartych na wielokrotnym dodawaniu i przesunięciach bitowych.
    *   **Operacje bitowe:** Procesory potrafią bardzo szybko wykonywać operacje logiczne (AND, OR, XOR, NOT) oraz przesunięcia bitowe, które są podstawą wielu algorytmów niskopoziomowych.


## 19. Miary efektywności obliczeniowej procesorów, pojemności pamięci komputerowej oraz wydajności systemów obliczeniowych.

### Szczegółowe wyjaśnienie

Ocena wydajności komputerów i ich komponentów jest zadaniem złożonym, ponieważ "wydajność" może oznaczać co innego w zależności od zastosowania. Dlatego stosuje się różne miary i metryki, które pozwalają na ilościowe porównanie różnych systemów.

**Miary efektywności obliczeniowej procesorów (CPU)**

Historycznie i obecnie stosuje się kilka kluczowych miar do oceny "surowej" mocy obliczeniowej procesora:

1.  **Częstotliwość taktowania (wyrażana w Hercach - Hz, megahercach - MHz, gigahercach - GHz):**
    *   **Co mierzy:** Liczbę cykli zegara, jakie procesor wykonuje w ciągu jednej sekundy. 1 GHz oznacza miliard cykli na sekundę.
    *   **Znaczenie:** Przez wiele lat była to podstawowa miara wydajności – im wyższe taktowanie, tym szybszy procesor. Jednak dzisiaj jest to miara **bardzo myląca**, jeśli porównujemy procesory o różnej architekturze. Nowoczesny procesor o taktowaniu 3 GHz może być wielokrotnie szybszy od starszego procesora 4 GHz, ponieważ potrafi wykonać znacznie więcej pracy w jednym cyklu zegara.

2.  **IPC (Instructions Per Cycle - Instrukcje na cykl):**
    *   **Co mierzy:** Średnią liczbę instrukcji maszynowych, jaką procesor jest w stanie wykonać w jednym cyklu zegara.
    *   **Znaczenie:** To kluczowa miara efektywności **architektury** procesora. Nowoczesne procesory są "superskalarne", co oznacza, że potrafią wykonywać wiele instrukcji jednocześnie (równolegle) w jednym cyklu. Wyższy wskaźnik IPC oznacza bardziej zaawansowaną i wydajną architekturę.

3.  **MIPS (Million Instructions Per Second - Miliony instrukcji na sekundę):**
    *   **Co mierzy:** Ogólną liczbę instrukcji (w milionach), jaką procesor wykonuje w ciągu sekundy. Jest to iloczyn taktowania i IPC: `Wydajność [MIPS] = Taktowanie [MHz] * IPC`.
    *   **Znaczenie:** Jest to bardziej kompleksowa miara niż samo taktowanie, ale wciąż ma wady. Różne instrukcje mają różny stopień skomplikowania (np. proste dodawanie vs. skomplikowane dzielenie), a MIPS traktuje je wszystkie jednakowo. Dlatego nie jest to dobra miara do porównywania procesorów o różnych zestawach instrukcji (np. RISC vs. CISC).

4.  **FLOPS (Floating-Point Operations Per Second - Operacje zmiennoprzecinkowe na sekundę):**
    *   **Co mierzy:** Liczbę operacji na liczbach zmiennoprzecinkowych (dodawanie, mnożenie), jaką procesor może wykonać w ciągu sekundy. Używa się przedrostków: mega- (MFLOPS), giga- (GFLOPS), tera- (TFLOPS), peta- (PFLOPS).
    *   **Znaczenie:** To **standardowa i najważniejsza miara wydajności w obliczeniach naukowych i inżynierskich (HPC - High-Performance Computing)**, grafice komputerowej, uczeniu maszynowym i wszędzie tam, gdzie kluczowe są obliczenia na liczbach rzeczywistych. Wydajność superkomputerów jest mierzona właśnie we FLOPS.

**Miary pojemności pamięci komputerowej**

Pojemność pamięci (zarówno RAM, jak i dyskowej) jest mierzona w **bajtach (B)** i jego wielokrotnościach. Jeden bajt to 8 bitów.

*   **Kilobajt (KB):** 1024 bajty (2¹⁰ B)
*   **Megabajt (MB):** 1024 KB (2²⁰ B)
*   **Gigabajt (GB):** 1024 MB (2³⁰ B)
*   **Terabajt (TB):** 1024 GB (2⁴⁰ B)

**Uwaga:** Producenci dysków twardych często używają przedrostków dziesiętnych (1 KB = 1000 B), co powoduje, że dysk o pojemności "1 TB" w rzeczywistości ma około 931 GiB (gibibajtów) pojemności widzianej przez system operacyjny, który używa przedrostków binarnych.

Oprócz pojemności, dla pamięci RAM kluczowe są też inne parametry wydajnościowe, takie jak **taktowanie** (w MHz) i **opóźnienia (timingi, CL - CAS Latency)**, które razem wpływają na jej przepustowość.

**Miary wydajności systemów obliczeniowych**

Surowa moc procesora to nie wszystko. Wydajność całego systemu zależy od współpracy wielu komponentów. Dlatego do oceny ogólnej wydajności używa się **benchmarków**.

**Benchmark** to specjalny program lub zestaw programów, który wykonuje standardowy zestaw zadań, mierząc czas ich wykonania. Wynik benchmarku pozwala na obiektywne porównanie wydajności różnych systemów w konkretnych zastosowaniach.

*   **Benchmarki syntetyczne:** Mierzą wydajność w sposób abstrakcyjny, np. Linpack (używany do tworzenia listy TOP500 najszybszych superkomputerów, mierzy wydajność we FLOPS), Dhrystone (mierzy wydajność w operacjach na liczbach całkowitych).
*   **Benchmarki aplikacyjne:** Symulują rzeczywiste scenariusze użycia komputera. Są znacznie bardziej miarodajne dla końcowego użytkownika. Przykłady:
    *   **SPEC (Standard Performance Evaluation Corporation):** Zestaw benchmarków symulujących różne zadania, od pracy biurowej po skomplikowane obliczenia naukowe (np. SPECint, SPECfp).
    *   **Benchmarki w grach:** Mierzą liczbę klatek na sekundę (FPS - Frames Per Second) w określonej grze i ustawieniach graficznych.
    *   **Benchmarki do renderowania:** Mierzą czas potrzebny na wyrenderowanie sceny 3D (np. Cinebench).
    *   **Benchmarki dyskowe:** Mierzą prędkość odczytu i zapisu danych (np. CrystalDiskMark).

Ostatecznie, najlepszą miarą wydajności jest **czas wykonania konkretnego zadania, na którym zależy użytkownikowi**. Benchmarki pomagają ten czas oszacować bez konieczności fizycznego testowania każdego systemu.


## 20. Prawo Moore’a i implikacje z niego wynikające w kontekście rozwoju sprzętu komputerowego.

### Szczegółowe wyjaśnienie

**Czym jest Prawo Moore’a?**

Prawo Moore’a to nie jest prawo fizyki, ale **obserwacja empiryczna** sformułowana w 1965 roku przez Gordona Moore’a, współzałożyciela firmy Intel. W swojej pierwotnej formie, obserwacja ta stwierdzała, że **liczba tranzystorów w układzie scalonym (o optymalnym koszcie produkcji) podwaja się mniej więcej co rok**. W 1975 roku Moore zrewidował swoją prognozę, wydłużając ten okres do **około dwóch lat**.

Choć często jest ono mylnie interpretowane jako prawo mówiące o podwajaniu się mocy obliczeniowej, jego sedno dotyczy **miniaturyzacji i gęstości upakowania tranzystorów**. Tranzystor to podstawowy element budulcowy mikroprocesorów, działający jak miniaturowy przełącznik. Im więcej tranzystorów można zmieścić na tej samej powierzchni krzemu, tym bardziej złożone i potężniejsze układy można budować.

Prawo Moore’a przez ponad 50 lat było samospełniającą się przepowiednią i siłą napędową całej branży półprzewodnikowej. Wyznaczało ono cykl rozwojowy (tzw. "tick-tock" Intela), motywując firmy do inwestowania miliardów dolarów w badania i rozwój, aby utrzymać tempo miniaturyzacji i pozostać konkurencyjnym.

**Implikacje Prawa Moore’a**

Konsekwencje tego wykładniczego wzrostu gęstości tranzystorów były i są ogromne, kształtując całą naszą cyfrową cywilizację.

1.  **Wykładniczy wzrost mocy obliczeniowej:** Więcej tranzystorów na tej samej powierzchni pozwalało na implementację coraz bardziej zaawansowanych architektur procesorów: dłuższych potoków przetwarzania, większej liczby jednostek wykonawczych, bardziej zaawansowanego przewidywania skoków i wreszcie – **procesorów wielordzeniowych**. To bezpośrednio przekładało się na wykładniczy wzrost wydajności komputerów, mierzony w MIPS czy FLOPS.

2.  **Spadek kosztu mocy obliczeniowej:** Ponieważ koszt produkcji wafla krzemowego pozostawał względnie stały, podwajanie liczby tranzystorów oznaczało, że **koszt pojedynczego tranzystora spadał o połowę** co dwa lata. Moc obliczeniowa, która kiedyś była dostępna tylko dla superkomputerów, stawała się dostępna dla masowego konsumenta, co doprowadziło do rewolucji PC, a następnie rewolucji mobilnej.

3.  **Miniaturyzacja urządzeń:** Mniejsze tranzystory zużywają mniej energii i emitują mniej ciepła. To pozwoliło na tworzenie coraz mniejszych i bardziej energooszczędnych urządzeń – od laptopów, przez smartfony i smartwatche, aż po urządzenia Internetu Rzeczy (IoT).

4.  **Rozwój oprogramowania i nowych technologii:** Dostępność taniej i ogromnej mocy obliczeniowej umożliwiła rozwój dziedzin, które kiedyś były niemożliwe do zrealizowania. Bez prawa Moore’a nie byłoby rewolucji w **grafice komputerowej** (fotorealistyczne gry i filmy), **sztucznej inteligencji** (trenowanie głębokich sieci neuronowych wymaga gigantycznej mocy obliczeniowej), **bioinformatyce** (sekwencjonowanie genomu) czy analizie **Big Data**.

**Koniec Prawa Moore’a?**

Od kilku lat obserwujemy wyraźne spowolnienie tempa dyktowanego przez prawo Moore’a. Dalsza miniaturyzacja tranzystorów napotyka na fundamentalne bariery fizyczne i ekonomiczne:

*   **Bariery fizyczne:** Gdy rozmiar tranzystora zbliża się do kilku nanometrów (rozmiarów pojedynczych atomów), zaczynają dominować **niepożądane zjawiska kwantowe**, takie jak tunelowanie elektronów, które zakłócają jego pracę jako niezawodnego przełącznika.
*   **Bariery ekonomiczne:** Koszt budowy fabryk (tzw. fabów) zdolnych do produkcji w coraz niższych procesach technologicznych rośnie wykładniczo, sięgając dziesiątek miliardów dolarów. Coraz mniej firm stać na takie inwestycje.
*   **Problem z odprowadzaniem ciepła:** Zwiększanie gęstości upakowania tranzystorów prowadzi do ogromnego wzrostu gęstości mocy (ilości ciepła emitowanego z jednostki powierzchni), co staje się krytycznym problemem w chłodzeniu układów.

**Implikacje spowolnienia i przyszłość ("More than Moore")**

Koniec ery klasycznego prawa Moore’a nie oznacza końca postępu w informatyce. Zmienia się jedynie jego charakter. Branża przechodzi od prostego skalowania (więcej, mniejszych tranzystorów) do bardziej kreatywnych sposobów na zwiększanie wydajności. Ten nowy paradygmat określa się jako **"More than Moore"**:

*   **Specjalizacja i akceleratory:** Zamiast jednego, uniwersalnego CPU, które robi wszystko, projektuje się **wyspecjalizowane układy (akceleratory)**, które są ekstremalnie wydajne w jednym, konkretnym typie zadań. Przykładem są **GPU** (procesory graficzne) do obliczeń równoległych, **TPU** (Tensor Processing Units) od Google do obliczeń AI, czy **FPGA** do rekonfigurowalnych obliczeń.
*   **Zaawansowane techniki pakowania (3D Stacking):** Zamiast układać tranzystory płasko, firmy zaczynają układać je **warstwowo, w trzech wymiarach** (np. technologia HBM - High Bandwidth Memory), co pozwala na drastyczne zwiększenie gęstości i skrócenie ścieżek komunikacji.
*   **Nowe architektury:** Poszukiwanie alternatyw dla klasycznej architektury von Neumanna, np. **obliczenia neuromorficzne** (naśladujące budowę mózgu) czy **obliczenia w pamięci (in-memory computing)**.
*   **Nowe materiały i technologie:** Badania nad następcami krzemu, takimi jak nanorurki węglowe, grafen, oraz nad zupełnie nowymi paradygmatami obliczeń, jak **komputery kwantowe**.


---

# Odpowiedzi "to the point" na obronę

## 16. Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce.

Maszyna Turinga to **abstrakcyjny model teoretyczny**, który definiuje granice tego, co jest w ogóle obliczalne. Jej rolą jest fundament teorii obliczeń i złożoności. Architektura von Neumanna to z kolei **praktyczny schemat budowy** niemal wszystkich współczesnych komputerów. Jej kluczową cechą jest wspólna pamięć dla programu i danych, co umożliwia tworzenie uniwersalnych maszyn, które można programować do dowolnych zadań. Krótko mówiąc, maszyna Turinga mówi nam *co* można obliczyć, a architektura von Neumanna *jak* zbudować maszynę, która to robi.

## 17. Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów.

Logika boolowska operuje na dwóch wartościach – prawda (1) i fałsz (0) – oraz na operacjach takich jak AND, OR i NOT. Jest to absolutny fundament sprzętu komputerowego, ponieważ te operacje są fizycznie realizowane przez **bramki logiczne** (zbudowane z tranzystorów). Z tych prostych bramek, jak z klocków, buduje się bardziej złożone układy, takie jak sumatory, przerzutniki (pamięć) i dekodery, które ostatecznie tworzą całą jednostkę arytmetyczno-logiczną (ALU) i układ sterowania procesora.

## 18. Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa.

Liczby całkowite w komputerach zapisuje się standardowo w **kodzie uzupełnieniowym do dwóch (U2)**, ponieważ drastycznie upraszcza on arytmetykę – dodawanie i odejmowanie wykonuje się w ten sam sposób. Liczby rzeczywiste zapisuje się zgodnie ze **standardem IEEE 754**, który jest binarną notacją naukową, składającą się ze znaku, wykładnika i mantysy. Arytmetyka komputerowa jest ograniczona skończoną liczbą bitów, co prowadzi do problemów takich jak **przepełnienie (overflow)** dla liczb całkowitych i **błędy zaokrągleń** dla liczb zmiennoprzecinkowych.

## 19. Miary efektywności obliczeniowej procesorów, pojemności pamięci komputerowej oraz wydajności systemów obliczeniowych.

Wydajność procesorów mierzy się za pomocą **taktowania (w GHz)**, które jest mylące, oraz **IPC** (instrukcje na cykl), które opisuje efektywność architektury. Bardziej kompleksową miarą jest **MIPS** (miliony instrukcji na sekundę), a w obliczeniach naukowych i AI standardem są **FLOPS** (operacje zmiennoprzecinkowe na sekundę). Pojemność pamięci mierzy się w **bajtach** i ich wielokrotnościach (KB, MB, GB, TB). Ogólną wydajność systemów ocenia się za pomocą **benchmarków** – specjalnych programów (np. Cinebench, SPEC), które symulują realne zadania i mierzą czas ich wykonania.

## 20. Prawo Moore’a i implikacje z niego wynikające w kontekście rozwoju sprzętu komputerowego.

Prawo Moore’a to obserwacja, że **liczba tranzystorów w układzie scalonym podwaja się co około dwa lata**. Przez 50 lat napędzało to wykładniczy **wzrost mocy obliczeniowej**, **spadek kosztu** tej mocy oraz **miniaturyzację** urządzeń, co umożliwiło rewolucję PC, mobilną i AI. Obecnie prawo to zwalnia z powodu barier fizycznych i ekonomicznych. W odpowiedzi branża IT przechodzi do ery "More than Moore", skupiając się na **specjalistycznych akceleratorach (jak GPU, TPU)**, **zaawansowanym pakowaniu 3D** i poszukiwaniu nowych architektur obliczeniowych.

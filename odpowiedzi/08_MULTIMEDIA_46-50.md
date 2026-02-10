# Odpowiedzi na pytania do obrony pracy inżynierskiej - Multimedia

## 46. Modele barw.

### Szczegółowe wyjaśnienie

**Model barw** to abstrakcyjny, matematyczny model opisujący, w jaki sposób można reprezentować barwy jako zestawy liczb (krotki). Jest to formalny sposób na zdefiniowanie i komunikowanie informacji o kolorze. Każdy model definiuje swoją **przestrzeń barw** – podzbiór wszystkich kolorów, które można w danym modelu przedstawić.

Modele barw można podzielić na dwie główne kategorie, w zależności od tego, jak tworzą kolory:

**1. Modele addytywne (mieszanie świateł)**

*   **Zasada działania:** Kolory powstają przez **dodawanie** do siebie świateł o różnych barwach. Punktem wyjścia jest czerń (brak światła). Im więcej światła dodamy, tym jaśniejszy kolor uzyskamy. Zmieszanie wszystkich składowych w maksymalnym natężeniu daje biel.
*   **Zastosowanie:** Wszędzie tam, gdzie mamy do czynienia z urządzeniami **emitującymi światło**, takimi jak monitory, ekrany smartfonów, projektory, skanery.

*   **Przykład: Model RGB**
    *   **Składowe:** **R**ed (czerwony), **G**reen (zielony), **B**lue (niebieski). Są to trzy podstawowe barwy, na które najbardziej czułe są czopki w ludzkim oku.
    *   **Reprezentacja:** Każdy kolor jest opisywany jako trójka liczb, określających natężenie każdej ze składowych. Najczęściej używa się wartości z zakresu 0-255 dla każdej składowej (co odpowiada 8 bitom na kanał i daje łącznie 24 bity na piksel, czyli ponad 16 milionów kolorów).
        *   ` (0, 0, 0) ` – czarny
        *   ` (255, 255, 255) ` – biały
        *   ` (255, 0, 0) ` – czerwony
        *   ` (255, 255, 0) ` – żółty (czerwony + zielony)

**2. Modele subtraktywne (mieszanie pigmentów)**

*   **Zasada działania:** Kolory powstają przez **odejmowanie** (pochłanianie, subtrakcję) pewnych długości fal od światła białego, które pada na powierzchnię. Punktem wyjścia jest biel (papier). Im więcej barwnika (pigmentu) nałożymy, tym ciemniejszy kolor uzyskamy, ponieważ więcej światła jest pochłaniane.
*   **Zastosowanie:** Wszędzie tam, gdzie mamy do czynienia z **drukiem** i farbami (drukarki, prasa, malarstwo).

*   **Przykład: Model CMYK**
    *   **Składowe:** **C**yan (cyjan, odcień niebieskiego), **M**agenta (magenta, odcień purpury), **Y**ellow (żółty), **K**ey (kluczowy, czarny).
    *   **Rola czarnego (K):** Teoretycznie zmieszanie C, M i Y powinno dać kolor czarny. W praktyce daje brudny, ciemnobrązowy kolor. Dodatkowo, użycie trzech kolorowych tuszów do druku czarnego tekstu byłoby nieekonomiczne i mogłoby prowadzić do przemoczenia papieru. Dlatego dodaje się osobny, czarny pigment, który zapewnia głęboką czerń i ostrość detali.
    *   **Reprezentacja:** Każdy kolor jest opisywany jako czwórka liczb, najczęściej procentowych (0-100%), określających stopień pokrycia farbą dla każdej ze składowych.

**3. Modele percepcyjne (zorientowane na człowieka)**

Modele RGB i CMYK są zorientowane na sprzęt. Modele percepcyjne próbują opisywać kolory w sposób bardziej intuicyjny dla człowieka, używając pojęć takich jak odcień, nasycenie i jasność.

*   **Przykład: Model HSV (lub HSB)**
    *   **Składowe:**
        *   **H (Hue - barwa):** Czysty kolor, czyli to, co potocznie nazywamy "kolorem" (czerwony, zielony, fioletowy). Jest określany jako kąt na kole barw (0-360°).
        *   **S (Saturation - nasycenie):** Intensywność, "czystość" koloru. Wartość 100% oznacza żywy, w pełni nasycony kolor. Wartość 0% oznacza odcień szarości.
        *   **V (Value) lub B (Brightness - jasność/wartość):** Jasność koloru. Wartość 100% oznacza najjaśniejszy możliwy kolor. Wartość 0% zawsze daje czerń, niezależnie od barwy i nasycenia.
    *   **Zastosowanie:** Jest bardzo intuicyjny dla użytkowników w programach graficznych (np. w okienkach wyboru koloru), ponieważ pozwala na łatwą zmianę jednego atrybutu koloru (np. rozjaśnienie) bez zmiany pozostałych.

**Porównanie i konwersja**

| Cecha | RGB | CMYK | HSV/HSB |
|---|---|---|---|
| **Typ** | **Addytywny** | **Subtraktywny** | Percepcyjny |
| **Składowe** | Czerwony, Zielony, Niebieski | Cyjan, Magenta, Żółty, Czarny | Barwa, Nasycenie, Jasność |
| **Punkt wyjścia** | Czerń (brak światła) | Biel (brak farby) | Zależy od definicji |
| **Główne zastosowanie** | **Ekrany, monitory, web** | **Druk** | Interfejsy użytkownika, analiza obrazu |

Przestrzeń barw, którą można uzyskać w modelu RGB (tzw. gamut), jest inna niż w modelu CMYK. RGB jest w stanie odwzorować bardziej jaskrawe, żywe kolory. Dlatego pliki graficzne przeznaczone do druku muszą być **konwertowane** z przestrzeni RGB do CMYK. Proces ten może spowodować, że niektóre kolory staną się mniej nasycone i "przygaszone", ponieważ nie da się ich uzyskać za pomocą farb drukarskich.


## 47. Techniki cieniowania (shadery).

### Szczegółowe wyjaśnienie

**Czym jest cieniowanie i shader?**

**Cieniowanie (shading)** w grafice komputerowej to proces obliczania koloru każdego piksela na powierzchni renderowanego obiektu 3D. Celem jest stworzenie iluzji głębi, materiału i oświetlenia, co sprawia, że płaski, jednolity model wygląda realistycznie. Cieniowanie uwzględnia takie czynniki jak kolor samego obiektu, położenie i rodzaj źródeł światła, właściwości materiału (np. czy jest matowy czy błyszczący) oraz położenie i orientację kamery.

**Shader** to **mały program komputerowy**, który jest wykonywany bezpośrednio na **procesorze graficznym (GPU)**. Shadery dają programiście bezpośrednią kontrolę nad poszczególnymi etapami **potoku renderowania (rendering pipeline)**, pozwalając na implementację niestandardowych algorytmów cieniowania i efektów wizualnych. Dzięki nim możliwe jest tworzenie fotorealistycznych materiałów, wody, ognia, cieni i wielu innych zaawansowanych efektów w czasie rzeczywistym.

Shadery pisze się w specjalnych językach programowania, takich jak **GLSL** (OpenGL Shading Language) lub **HLSL** (High-Level Shading Language, używany w DirectX).

**Potok renderowania i rola shaderów**

Potok renderowania to sekwencja kroków, które karta graficzna wykonuje, aby przekształcić scenę 3D (złożoną z wierzchołków) w finalny obraz 2D na ekranie. Nowoczesne, programowalne potoki renderowania mają kilka etapów, w których możemy interweniować za pomocą shaderów. Dwa najważniejsze i obowiązkowe to:

**1. Vertex Shader (Shader wierzchołków)**

*   **Kiedy jest wykonywany?** Na samym początku potoku.
*   **Co robi?** Jest uruchamiany **dla każdego pojedynczego wierzchołka** modelu 3D.
*   **Główne zadania:**
    1.  **Transformacja wierzchołków:** Jego absolutnie podstawowym zadaniem jest przekształcenie pozycji wierzchołka z jego lokalnej przestrzeni (model space) do przestrzeni ekranu (screen space). Odbywa się to przez przemnożenie pozycji wierzchołka przez serię macierzy transformacji (model, view, projection).
    2.  **Przekazywanie danych:** Przygotowuje i przekazuje dane (np. współrzędne tekstury, wektor normalny, kolor wierzchołka) do następnego etapu potoku, czyli shadera fragmentów.
    3.  **Inne efekty:** Może być używany do zaawansowanych efektów modyfikujących geometrię, takich jak animacja fal na wodzie, deformacja obiektów czy symulacja wiatru na trawie.

**2. Fragment Shader (Shader fragmentów, Pixel Shader)**

*   **Kiedy jest wykonywany?** Po etapie rasteryzacji, w którym prymitywy geometryczne (trójkąty) są zamieniane na zbiór **fragmentów** (potencjalnych pikseli).
*   **Co robi?** Jest uruchamiany **dla każdego pojedynczego fragmentu (piksela)**, który ma zostać narysowany na ekranie.
*   **Główne zadania:**
    1.  **Obliczanie finalnego koloru:** To jest jego najważniejsze zadanie. Na podstawie danych otrzymanych z vertex shadera (które są interpolowane na powierzchni trójkąta), właściwości materiału (pobranych np. z tekstur) i informacji o oświetleniu, shader fragmentów oblicza ostateczny kolor piksela, który zostanie zapisany w buforze ramki.
    2.  **Implementacja modeli oświetlenia:** To tutaj implementuje się algorytmy takie jak **model oświetlenia Phonga** czy **Blinna-Phonga**, które obliczają, jak światło odbija się od powierzchni (składowa otoczenia, rozproszona i zwierciadlana).
    3.  **Teksturowanie:** Pobiera kolor z tekstury (mapy bitowej) na podstawie współrzędnych tekstury i używa go jako koloru bazowego obiektu.
    4.  **Efekty specjalne:** Implementuje efekty takie jak bump mapping (symulowanie nierówności powierzchni), przezroczystość, mgła, czy efekty post-processingu (np. bloom, rozmycie).

**Podstawowe techniki cieniowania (realizowane przez shadery)**

*   **Cieniowanie płaskie (Flat Shading):**
    *   **Jak działa:** Cały wielokąt (trójkąt) jest kolorowany jednym, jednolitym kolorem. Obliczenia oświetlenia są wykonywane tylko raz dla całego wielokąta.
    *   **Efekt:** Obiekt wygląda "kanciasto", poszczególne ściany są wyraźnie widoczne. Jest to najszybsza, ale najmniej realistyczna metoda.

*   **Cieniowanie Gourauda (Gouraud Shading):**
    *   **Jak działa:** Obliczenia oświetlenia są wykonywane **w wierzchołkach** (w vertex shaderze). Następnie kolory obliczone dla wierzchołków są **interpolowane** na całej powierzchni wielokąta (ten proces odbywa się automatycznie między vertex a fragment shaderem).
    *   **Efekt:** Daje iluzję gładkiej powierzchni, ale ma problemy z poprawnym odwzorowaniem odbić zwierciadlanych (specular highlights), które mogą wyglądać nienaturalnie.

*   **Cieniowanie Phonga (Phong Shading):**
    *   **Jak działa:** To nie to samo co model oświetlenia Phonga! W tej technice **wektory normalne** są interpolowane na powierzchni wielokąta. Następnie, **dla każdego piksela osobno** (w fragment shaderze), wykonywane są pełne obliczenia oświetlenia na podstawie zinterpolowanego wektora normalnego.
    *   **Efekt:** Daje bardzo gładkie i realistyczne rezultaty, poprawnie odwzorowując odbicia zwierciadlane. Jest to metoda najbardziej wymagająca obliczeniowo, ale jest standardem w nowoczesnej grafice czasu rzeczywistego.

| Technika | Gdzie wykonywane są obliczenia światła? | Co jest interpolowane? | Jakość | Wydajność |
|---|---|---|---|---|
| **Flat** | Raz na wielokąt | Nic | Niska | Bardzo wysoka |
| **Gouraud** | **W wierzchołkach** | **Kolor** | Średnia | Wysoka |
| **Phong** | **W każdym pikselu** | **Wektor normalny** | Wysoka | Średnia/Niska |


## 48. Metody kompresji w standardzie MPEG.

### Szczegółowe wyjaśnienie

**MPEG (Moving Picture Experts Group)** to grupa robocza, która opracowuje standardy kompresji i kodowania cyfrowego audio i wideo. Standardy te (np. MPEG-1, MPEG-2, MPEG-4) nie są pojedynczymi algorytmami, ale złożonymi zestawami narzędzi i technik, które pozwalają na drastyczne zmniejszenie rozmiaru plików multimedialnych przy zachowaniu akceptowalnej jakości. Kompresja w standardach MPEG jest **stratna**, co oznacza, że część oryginalnych informacji jest bezpowrotnie tracona, ale w sposób, który jest jak najmniej zauważalny dla ludzkiego oka i ucha.

Kluczem do skuteczności kompresji wideo MPEG jest wykorzystanie dwóch rodzajów redundancji (nadmiarowości) w sygnale wideo:

1.  **Redundancja przestrzenna (wewnątrzobrazowa):** W obrębie jednej klatki obrazu sąsiadujące piksele często mają bardzo podobny kolor. Zamiast zapisywać informację o każdym pikselu z osobna, można zapisać informację o większych blokach o podobnym kolorze.
2.  **Redundancja czasowa (międzyobrazowa):** Kolejne klatki w sekwencji wideo są do siebie bardzo podobne. Zazwyczaj zmienia się tylko niewielka część obrazu (np. poruszająca się postać na statycznym tle). Jest to najważniejszy rodzaj redundancji, którego wykorzystanie daje największe zyski kompresji.

**Główne techniki kompresji wideo w MPEG:**

**1. Kompresja wewnątrzobrazowa (Intra-frame compression)**

Ta technika redukuje redundancję przestrzenną i jest stosowana do kodowania klatek kluczowych (I-frame). Proces ten jest bardzo podobny do kompresji obrazów statycznych w standardzie **JPEG**.

*   **Podział na makrobloki:** Obraz jest dzielony na małe bloki pikseli (np. 16x16), zwane makroblokami.
*   **Transformacja DCT (Dyskretna Transformata Kosinusowa):** Każdy blok jest poddawany transformacji DCT. Przekształca ona blok pikseli z domeny przestrzennej (gdzie każdy piksel ma wartość koloru) do domeny częstotliwości. W rezultacie większość "energii" (ważnych informacji wizualnych) obrazu skupia się w kilku współczynnikach niskoczęstotliwościowych, a współczynniki wysokoczęstotliwościowe (odpowiadające za drobne detale) są bliskie zeru.
*   **Kwantyzacja:** To jest główny etap **stratny**. Współczynniki DCT są dzielone przez wartości z tablicy kwantyzacji, a następnie zaokrąglane do najbliższej liczby całkowitej. Współczynniki wysokoczęstotliwościowe, które i tak były małe, po tym procesie stają się zerami. Im wyższy stopień kwantyzacji, tym więcej informacji jest traconych, ale tym większy zysk z kompresji.
*   **Kodowanie entropijne:** Ostateczny ciąg współczynników (zawierający dużo zer) jest kompresowany bezstratnie za pomocą algorytmów takich jak kodowanie Huffmana lub kodowanie arytmetyczne.

**2. Kompresja międzyobrazowa (Inter-frame compression)**

Ta technika redukuje redundancję czasową, wykorzystując podobieństwo między kolejnymi klatkami. W tym celu standard MPEG definiuje trzy typy ramek:

*   **Ramki I (Intra-coded frames, klatki kluczowe):**
    *   Są kodowane **niezależnie** od innych ramek, wyłącznie za pomocą kompresji wewnątrzobrazowej (DCT, kwantyzacja).
    *   Są największe pod względem rozmiaru, ale służą jako **punkty odniesienia** dla innych ramek. Muszą pojawiać się co jakiś czas (tworząc tzw. **Grupę Obrazów - GOP**), aby umożliwić przewijanie filmu i naprawę błędów transmisji.

*   **Ramki P (Predicted frames, klatki przewidywane):**
    *   Są kodowane na podstawie **poprzedniej** ramki I lub P. Zamiast kodować cały obraz, koder szuka dla każdego makrobloku w ramce P najbardziej podobnego bloku w ramce odniesienia. Ten proces nazywa się **estymacją i kompensacją ruchu (motion estimation/compensation)**.
    *   Zapisywana jest tylko informacja o **wektorze ruchu** (o ile i w jakim kierunku dany blok się przesunął) oraz niewielka informacja o **błędzie predykcji** (różnicy między blokiem przewidywanym a rzeczywistym), która jest kodowana za pomocą DCT.
    *   Są znacznie mniejsze niż ramki I.

*   **Ramki B (Bi-directional predicted frames, klatki przewidywane dwukierunkowo):**
    *   Są kodowane na podstawie **zarówno poprzedniej, jak i przyszłej** ramki I lub P. Daje to jeszcze lepszą predykcję, ponieważ koder może znaleźć pasujący blok w obu kierunkach (np. dla obiektu, który był chwilowo zasłonięty).
    *   Są **najmniejsze** pod względem rozmiaru i oferują najwyższy stopień kompresji.
    *   Ich użycie wprowadza jednak większe opóźnienie w procesie kodowania i dekodowania.

Typowa sekwencja ramek (GOP) może wyglądać tak: `I B B P B B P B B I ...`

**Kompresja audio w MPEG**

Standardy MPEG definiują również formaty kompresji audio. Najbardziej znanym jest **MPEG-1 Audio Layer III**, czyli po prostu **MP3**.

*   **Zasada działania:** Kompresja audio w MPEG opiera się na **modelu psychoakustycznym** ludzkiego słuchu. Wykorzystuje fakt, że ludzkie ucho nie jest doskonałe i pewnych dźwięków nie słyszy lub słyszy je gorzej.
*   **Maskowanie częstotliwościowe:** Głośny dźwięk o pewnej częstotliwości powoduje, że cichsze dźwięki o zbliżonych częstotliwościach stają się niesłyszalne. Koder może usunąć lub mocno skompresować te "zamaskowane" dźwięki bez zauważalnej utraty jakości.
*   **Maskowanie czasowe:** Głośny dźwięk maskuje cichsze dźwięki występujące tuż przed nim i tuż po nim.

**Ewolucja standardów MPEG**

*   **MPEG-1:** Pierwszy popularny standard, używany w formacie Video CD. Zdefiniował format MP3.
*   **MPEG-2:** Standard o wyższej jakości, używany w telewizji cyfrowej (DVB), na płytach DVD i Blu-ray.
*   **MPEG-4:** Bardzo szeroki standard, który wprowadził wiele ulepszeń. Jego najważniejszą częścią jest **Part 10: Advanced Video Coding (AVC)**, znany powszechnie jako **H.264**. Jest to obecnie najpopularniejszy standard kompresji wideo, używany w streamingu internetowym (YouTube, Netflix), na płytach Blu-ray i w telewizji HD.
*   **Nowsze standardy:** Następcą H.264 jest **HEVC (High Efficiency Video Coding) / H.265**, który oferuje o około 50% lepszą kompresję przy tej samej jakości. Jest używany w wideo 4K i 8K.


## 49. Efekt aliasingu i metody jego zwalczania. Aliasing a częstotliwość próbkowania.

### Szczegółowe wyjaśnienie

**Czym jest aliasing?**

**Aliasing** to ogólne pojęcie opisujące zniekształcenia, które powstają, gdy sygnał ciągły (analogowy) jest reprezentowany przez dyskretny zbiór próbek (cyfrowy) z **niewystarczającą częstotliwością próbkowania**. W rezultacie, sygnał o wysokiej częstotliwości może zostać błędnie zinterpretowany jako sygnał o niższej częstotliwości. Nazwa "aliasing" pochodzi od tego, że jeden sygnał (o wysokiej częstotliwości) przybiera "alias" (tożsamość) innego sygnału (o niskiej częstotliwości).

Aliasing występuje w różnych dziedzinach multimediów:

*   **W grafice komputerowej:**
    *   **Aliasing przestrzenny:** Objawia się jako **"schodki" lub "ząbki" (jaggies)** na krawędziach obiektów, szczególnie na liniach ukośnych i krzywych. Wynika to z faktu, że obraz jest reprezentowany przez siatkę pikseli o skończonej rozdzielczości. Piksel może być albo w pełni włączony, albo wyłączony, co prowadzi do postrzępionych krawędzi, gdy linia przechodzi przez niego tylko częściowo.
    *   **Efekt mory (moiré pattern):** Pojawia się, gdy próbujemy odwzorować obraz zawierający bardzo drobne, regularne wzory (np. siatkę, prążki na koszuli). Jeśli częstotliwość wzoru jest zbliżona do częstotliwości próbkowania (rozdzielczości siatki pikseli), powstają nowe, fałszywe wzory, które nie istniały w oryginale.

*   **W dźwięku cyfrowym:**
    *   **Aliasing częstotliwościowy:** Jeśli sygnał audio zawiera częstotliwości wyższe niż połowa częstotliwości próbkowania, te wysokie częstotliwości "odbijają się" od połowy częstotliwości próbkowania i pojawiają się w sygnale cyfrowym jako fałszywe, niższe częstotliwości, które nie istniały w oryginalnym dźwięku. Powoduje to nieprzyjemne zniekształcenia i artefakty.

**Aliasing a częstotliwość próbkowania (Twierdzenie Nyquista-Shannona)**

Związek między aliasingiem a próbkowaniem jest precyzyjnie opisany przez **twierdzenie o próbkowaniu (twierdzenie Nyquista-Shannona)**. Mówi ono, że:

> Aby można było idealnie odtworzyć sygnał ciągły z jego próbek, częstotliwość próbkowania (`fs`) musi być co najmniej **dwa razy większa** niż najwyższa częstotliwość występująca w tym sygnale (`fmax`).

`fs >= 2 * fmax`

Ta graniczna częstotliwość (`2 * fmax`) nazywana jest **częstotliwością Nyquista**. Jeśli warunek ten nie jest spełniony, czyli próbujemy próbkować sygnał zawierający częstotliwości wyższe niż połowa częstotliwości próbkowania, **nieuchronnie wystąpi aliasing**.

**Przykład:** Ludzkie ucho słyszy dźwięki do ok. 20 kHz. Zgodnie z twierdzeniem, aby poprawnie zapisać cyfrowo wszystkie słyszalne częstotliwości, potrzebujemy częstotliwości próbkowania co najmniej 40 kHz. Dlatego standardowa częstotliwość próbkowania dla płyt CD-Audio wynosi 44.1 kHz, co daje bezpieczny margines.

**Metody zwalczania aliasingu (Antyaliasing)**

Antyaliasing to zbiór technik mających na celu redukcję lub eliminację efektu aliasingu.

**1. W grafice komputerowej:**

*   **Filtrowanie wstępne (Pre-filtering):** Teoretycznie najlepsza metoda. Polega na usunięciu z obrazu (sygnału) wszystkich częstotliwości wyższych niż częstotliwość Nyquista **przed** próbkowaniem. W praktyce jest to trudne do zrealizowania.

*   **Nadpróbkowanie (Supersampling / SSAA):**
    *   **Jak działa:** Obraz jest renderowany w **znacznie wyższej rozdzielczości** niż docelowa rozdzielczość ekranu (np. 4x większej). Następnie ten duży obraz jest skalowany w dół do rozdzielczości ekranu, a kolor każdego finalnego piksela jest uśredniany z kolorów odpowiadających mu pikseli z obrazu o wyższej rozdzielczości.
    *   **Efekt:** Daje bardzo wysoką jakość i gładkie krawędzie, ale jest **niezwykle kosztowny obliczeniowo**, ponieważ karta graficzna musi renderować wielokrotnie więcej pikseli.

*   **Wielokrotne próbkowanie (Multisampling / MSAA):**
    *   **Jak działa:** Jest to zoptymalizowana wersja supersamplingu i najpopularniejsza metoda antyaliasingu w grach. Zamiast renderować cały obraz w wyższej rozdzielczości, MSAA wykonuje kosztowny shader fragmentów tylko **raz na piksel**, ale testuje **widoczność (głębię) i pokrycie** w kilku sub-pikselowych lokalizacjach w obrębie piksela. Finalny kolor piksela jest następnie obliczany jako średnia ważona koloru obiektu i koloru tła, w zależności od tego, ile sub-próbek "trafiło" w obiekt.
    *   **Efekt:** Znacznie redukuje aliasing na krawędziach wielokątów przy znacznie niższym koszcie wydajnościowym niż SSAA. Nie wygładza jednak aliasingu wewnątrz tekstur (np. na krawędziach wynikających z przezroczystości).

*   **Antyaliasing post-processingowy (np. FXAA, SMAA):**
    *   **Jak działa:** Działa jako filtr na już wyrenderowanym obrazie. Analizuje finalną klatkę, szukając w niej postrzępionych krawędzi (kontrastowych granic pikseli), a następnie programowo je rozmywa.
    *   **Efekt:** Jest **bardzo szybki** i ma minimalny wpływ na wydajność, ale może powodować lekkie rozmycie całego obrazu. Jest często stosowany na konsolach i słabszych komputerach.

**2. W dźwięku cyfrowym:**

*   **Filtr antyaliasingowy:** Jest to **filtr dolnoprzepustowy**, który jest stosowany do sygnału analogowego **przed** przetwornikiem analogowo-cyfrowym (ADC). Filtr ten fizycznie usuwa z sygnału wszystkie częstotliwości powyżej połowy planowanej częstotliwości próbkowania, gwarantując, że warunek Nyquista jest spełniony i aliasing nie wystąpi.

## 50. Zasady interakcji człowiek-komputer: przedstaw i omów heurystyki Nielsena-Molicha.

### Szczegółowe wyjaśnienie

**Interakcja człowiek-komputer (Human-Computer Interaction - HCI)** to dziedzina nauki zajmująca się projektowaniem, ewaluacją i implementacją interaktywnych systemów komputerowych przeznaczonych dla ludzi oraz badaniem zjawisk, które im towarzyszą. Głównym celem HCI jest tworzenie systemów, które są **użyteczne, bezpieczne i przede wszystkim użyteczne (usable)** – czyli łatwe do nauczenia, efektywne w użyciu, zapamiętywalne, wolne od błędów i satysfakcjonujące dla użytkownika.

**Heurystyki Nielsena-Molicha**

**10 heurystyk użyteczności Jakoba Nielsena** (opracowanych wspólnie z Rolfem Molichem) to zbiór ogólnych, fundamentalnych zasad projektowania dobrych interfejsów użytkownika. Nie są to sztywne reguły, ale raczej "reguły kciuka", które pomagają projektantom identyfikować i rozwiązywać powszechne problemy z użytecznością. Są one podstawą **oceny heurystycznej** – metody inspekcji interfejsu, w której eksperci oceniają jego zgodność z tymi zasadami.

Oto 10 heurystyk z omówieniem:

**1. Pokazuj status systemu (Visibility of system status)**
*   **Zasada:** System powinien zawsze informować użytkownika o tym, co się dzieje, dostarczając mu odpowiednich informacji zwrotnych w rozsądnym czasie.
*   **Omówienie:** Użytkownicy muszą wiedzieć, jaki jest aktualny stan systemu, czy ich akcja została przyjęta i co się dzieje w tle. Daje im to poczucie kontroli i pozwala podejmować świadome decyzje.
*   **Przykłady:** Pasek postępu podczas pobierania pliku, animacja ładowania ("spinner"), informacja "Wiadomość została wysłana", podświetlenie aktywnego przycisku menu.

**2. Zachowaj zgodność między systemem a rzeczywistością (Match between system and the real world)**
*   **Zasada:** System powinien mówić językiem użytkownika, używając słów, fraz i pojęć znanych użytkownikowi, a nie terminologii technicznej. Informacje powinny być prezentowane w naturalnej i logicznej kolejności.
*   **Omówienie:** Interfejs powinien opierać się na metaforach i konwencjach ze świata rzeczywistego, co ułatwia jego zrozumienie i naukę.
*   **Przykłady:** Ikona kosza na śmieci do usuwania plików, ikona lupy do wyszukiwania, używanie pojęć "koszyk" i "kasa" w sklepie internetowym.

**3. Daj użytkownikowi pełną kontrolę (User control and freedom)**
*   **Zasada:** Użytkownicy często popełniają błędy. System musi zapewniać im wyraźnie oznaczone "wyjście awaryjne", aby mogli cofnąć niechciane akcje bez zbędnych problemów.
*   **Omówienie:** Użytkownik nie może czuć się uwięziony w systemie. Możliwość cofania i ponawiania akcji daje poczucie bezpieczeństwa i zachęca do eksploracji.
*   **Przykłady:** Funkcja "Cofnij" (Undo) i "Ponów" (Redo), przycisk "Anuluj" w formularzu, możliwość zamknięcia okna dialogowego w dowolnym momencie.

**4. Trzymaj się standardów i zachowaj spójność (Consistency and standards)**
*   **Zasada:** Użytkownicy nie powinni musieć się zastanawiać, czy różne słowa, sytuacje lub akcje oznaczają to samo. Należy przestrzegać konwencji danej platformy.
*   **Omówienie:** Spójność (wewnętrzna – w obrębie aplikacji, i zewnętrzna – z innymi aplikacjami) sprawia, że system jest przewidywalny i łatwiejszy do nauczenia. Użytkownik może przenieść wiedzę zdobytą w jednym miejscu na inne.
*   **Przykłady:** Używanie tej samej ikony dla tej samej akcji w całej aplikacji, umieszczanie menu nawigacyjnego zawsze w tym samym miejscu, stosowanie standardowych kontrolek systemowych.

**5. Zapobiegaj błędom (Error prevention)**
*   **Zasada:** Lepsze niż najlepsze komunikaty o błędach jest staranne projektowanie, które zapobiega wystąpieniu problemu w pierwszej kolejności.
*   **Omówienie:** System powinien aktywnie starać się eliminować warunki sprzyjające błędom lub sprawdzać je i prezentować użytkownikom opcję potwierdzenia, zanim wykonają ryzykowną akcję.
*   **Przykłady:** Wyszarzanie nieaktywnych opcji w menu, podpowiedzi w polach formularzy, pytanie "Czy na pewno chcesz usunąć ten plik?" przed jego skasowaniem, uniemożliwienie wpisania liter w polu na numer telefonu.

**6. Pozwalaj wybierać zamiast zmuszać do pamiętania (Recognition rather than recall)**
*   **Zasada:** Minimalizuj obciążenie pamięci użytkownika, czyniąc obiekty, akcje i opcje widocznymi. Użytkownik nie powinien musieć pamiętać informacji z jednej części interfejsu, aby użyć jej w innej.
*   **Omówienie:** Rozpoznawanie czegoś jest znacznie łatwiejsze poznawczo niż przypominanie sobie. Interfejs powinien być jak otwarta księga, a nie test pamięciowy.
*   **Przykłady:** Widoczne menu zamiast ukrytych komend, pokazywanie ostatnio otwieranych plików, podpowiedzi kontekstowe.

**7. Zapewnij elastyczność i efektywność (Flexibility and efficiency of use)**
*   **Zasada:** System powinien być efektywny zarówno dla początkujących, jak i zaawansowanych użytkowników. Pozwól zaawansowanym użytkownikom na dostosowanie i przyspieszenie często wykonywanych zadań.
*   **Omówienie:** Interfejs powinien oferować różne drogi do celu. Początkujący mogą korzystać z widocznych, prostych opcji, a zaawansowani – ze skrótów i zaawansowanych funkcji.
*   **Przykłady:** Skróty klawiaturowe (np. Ctrl+C, Ctrl+V), możliwość personalizacji interfejsu, gesty na ekranach dotykowych.

**8. Dbaj o estetykę i minimalistyczny design (Aesthetic and minimalist design)**
*   **Zasada:** Interfejsy nie powinny zawierać informacji, które są nieistotne lub rzadko potrzebne. Każda dodatkowa jednostka informacji w dialogu konkuruje z istotnymi jednostkami i zmniejsza ich względną widoczność.
*   **Omówienie:** Przeładowany, chaotyczny interfejs jest trudny w użyciu. Należy skupić się na tym, co najważniejsze, i usunąć wszelkie wizualne "szumy". Dobry design to nie wtedy, gdy nie ma już nic do dodania, ale gdy nie ma już nic do odjęcia.
*   **Przykłady:** Używanie dużej ilości białej przestrzeni, wyraźna hierarchia wizualna, ukrywanie zaawansowanych opcji w sekcji "Ustawienia zaawansowane".

**9. Zapewnij skuteczną obsługę błędów (Help users recognize, diagnose, and recover from errors)**
*   **Zasada:** Komunikaty o błędach powinny być wyrażone prostym językiem (bez kodów błędów), precyzyjnie wskazywać problem i konstruktywnie sugerować rozwiązanie.
*   **Omówienie:** Dobry komunikat o błędzie nie obwinia użytkownika, ale pomaga mu szybko wrócić na właściwą ścieżkę.
*   **Przykłady:** Zamiast "Błąd #2F56", komunikat "Podane hasło jest nieprawidłowe. Upewnij się, że Caps Lock nie jest włączony". Podświetlenie na czerwono pola w formularzu, które zostało źle wypełnione.

**10. Zadbaj o pomoc i dokumentację (Help and documentation)**
*   **Zasada:** Chociaż najlepiej jest, gdy system można obsługiwać bez dokumentacji, może być konieczne zapewnienie pomocy. Taka informacja powinna być łatwa do znalezienia, skoncentrowana na zadaniu użytkownika, zawierać konkretne kroki i nie być zbyt obszerna.
*   **Omówienie:** Pomoc powinna być kontekstowa i dostępna dokładnie wtedy, gdy użytkownik jej potrzebuje.
*   **Przykłady:** Ikony ze znakiem zapytania obok skomplikowanych opcji, sekcja FAQ, samouczek "tour" przy pierwszym uruchomieniu aplikacji, łatwo przeszukiwalna baza wiedzy.


---

# Odpowiedzi "to the point" na obronę

## 46. Modele barw.

Modele barw to matematyczne sposoby reprezentacji kolorów. Najważniejsze to:
*   **RGB (Red, Green, Blue):** Model **addytywny**, używany w urządzeniach emitujących światło (monitory, ekrany). Kolory powstają przez dodawanie światła, a punktem wyjścia jest czerń.
*   **CMYK (Cyan, Magenta, Yellow, Key-Black):** Model **subtraktywny**, używany w druku. Kolory powstają przez odejmowanie światła od białej powierzchni papieru.
*   **HSV/HSB (Hue, Saturation, Value/Brightness):** Model **percepcyjny**, intuicyjny dla człowieka, opisujący kolor przez jego barwę, nasycenie i jasność.

## 47. Techniki cieniowania (shadery).

**Shader** to mały program wykonywany na karcie graficznej (GPU), który oblicza finalny kolor pikseli obiektu 3D. Dwa kluczowe typy to:
*   **Vertex Shader:** Działa na każdym wierzchołku, przekształcając jego pozycję.
*   **Fragment (Pixel) Shader:** Działa na każdym pikselu, obliczając jego ostateczny kolor na podstawie oświetlenia i materiału.
Podstawowe techniki cieniowania to **Flat** (płaskie), **Gouraud** (interpolacja koloru z wierzchołków) i **Phong** (interpolacja wektorów normalnych i obliczenia per-pixel), który daje najbardziej realistyczne efekty.

## 48. Metody kompresji w standardzie MPEG.

Standardy MPEG (np. MPEG-4/H.264) używają kompresji stratnej, wykorzystując redundancję **przestrzenną** (wewnątrz jednej klatki) i **czasową** (między klatkami).
*   **Kompresja wewnątrzobrazowa (ramki I):** Działa jak JPEG – używa transformacji DCT i kwantyzacji do kompresji pojedynczych klatek kluczowych.
*   **Kompresja międzyobrazowa (ramki P i B):** Zamiast kodować całe klatki, zapisuje tylko **wektory ruchu** bloków, które się przemieściły względem klatek odniesienia. Ramki **P** są przewidywane z przeszłości, a ramki **B** dwukierunkowo (z przeszłości i przyszłości), co daje największą kompresję.

## 49. Efekt aliasingu i metody jego zwalczania. Aliasing a częstotliwość próbkowania.

**Aliasing** to zniekształcenie powstające, gdy sygnał jest próbkowany ze zbyt małą częstotliwością. W grafice objawia się jako **"ząbki" (jaggies)** na krawędziach, a w dźwięku jako fałszywe, niskie tony. Zgodnie z **twierdzeniem Nyquista-Shannona**, aby uniknąć aliasingu, częstotliwość próbkowania musi być co najmniej dwukrotnie wyższa od najwyższej częstotliwości w sygnale. Metody zwalczania (antyaliasing) w grafice to m.in. **Supersampling (SSAA)**, **Multisampling (MSAA)** oraz filtry post-processingowe jak **FXAA**.

## 50. Zasady interakcji człowiek-komputer: przedstaw i omów heurystyki Nielsena-Molicha.

To 10 ogólnych zasad projektowania użytecznych interfejsów. Najważniejsze z nich to:
1.  **Pokazuj status systemu:** Informuj użytkownika, co się dzieje (np. paskiem postępu).
2.  **Zachowaj zgodność z rzeczywistością:** Używaj zrozumiałych metafor (np. ikona kosza).
3.  **Daj użytkownikowi kontrolę:** Zapewnij funkcję "Cofnij" (Undo).
4.  **Zapobiegaj błędom:** Projektuj tak, by uniemożliwić pomyłki (np. walidacja formularzy).
5.  **Pozwalaj wybierać, nie zmuszaj do pamiętania:** Wszystkie opcje powinny być widoczne.
6.  **Dbaj o estetykę i minimalizm:** Usuń zbędne informacje, aby nie rozpraszać użytkownika.

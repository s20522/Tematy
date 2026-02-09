# Odpowiedzi na pytania do obrony pracy inżynierskiej - Matematyka

## 1. Ekstrema funkcji i gradient, zastosowania w informatyce.

### Szczegółowe wyjaśnienie

**Ekstrema funkcji**

Ekstremum funkcji to, mówiąc najprościej, jej wartość największa (maksimum) lub najmniejsza (minimum) w pewnym otoczeniu. Formalnie, dla funkcji f(x) mówimy, że w punkcie x₀ ma ona:

*   **Maksimum lokalne**, jeśli istnieje takie otoczenie punktu x₀, że dla każdego x w tym otoczeniu zachodzi f(x) ≤ f(x₀).
*   **Minimum lokalne**, jeśli istnieje takie otoczenie punktu x₀, że dla każdego x w tym otoczeniu zachodzi f(x) ≥ f(x₀).

Warunkiem koniecznym istnienia ekstremum dla funkcji różniczkowalnej jest zerowanie się jej pierwszej pochodnej w danym punkcie (f'(x₀) = 0). Punkt, w którym pochodna się zeruje, nazywamy punktem stacjonarnym. Jednak nie każdy punkt stacjonarny jest ekstremum (może to być np. punkt przegięcia). Aby sprawdzić, czy w punkcie stacjonarnym faktycznie występuje ekstremum, możemy skorzystać z drugiego warunku (warunku wystarczającego):

*   Jeśli f''(x₀) < 0, to w punkcie x₀ funkcja ma maksimum lokalne.
*   Jeśli f''(x₀) > 0, to w punkcie x₀ funkcja ma minimum lokalne.

**Gradient funkcji**

Gradient jest uogólnieniem pojęcia pochodnej na funkcje wielu zmiennych. Dla funkcji f(x₁, x₂, ..., xₙ), gradientem nazywamy wektor, którego składowymi są pochodne cząstkowe tej funkcji po każdej ze zmiennych:

∇f = [∂f/∂x₁, ∂f/∂x₂, ..., ∂f/∂xₙ]

Gradient w danym punkcie ma dwie bardzo ważne właściwości:

1.  **Wskazuje kierunek najszybszego wzrostu wartości funkcji.** Oznacza to, że poruszając się z danego punktu w kierunku wskazanym przez gradient, wartość funkcji będzie rosła najszybciej.
2.  **Jego długość (norma) informuje o szybkości tego wzrostu.** Im dłuższy wektor gradientu, tym szybszy wzrost wartości funkcji w tym kierunku.

Analogicznie, wektor przeciwny do gradientu (-∇f) wskazuje kierunek najszybszego spadku wartości funkcji.

**Zastosowania w informatyce**

Zarówno ekstrema, jak i gradient, odgrywają kluczową rolę w wielu dziedzinach informatyki, a w szczególności w **uczeniu maszynowym (machine learning)** i **sztucznej inteligencji (AI)**. Głównym celem wielu algorytmów uczenia maszynowego jest minimalizacja tzw. **funkcji kosztu (lub funkcji straty)**, która mierzy, jak bardzo przewidywania modelu różnią się od rzeczywistych danych. Im mniejsza wartość funkcji kosztu, tym lepszy jest model.

Tutaj z pomocą przychodzi **metoda spadku gradientu (gradient descent)**. Jest to iteracyjny algorytm optymalizacyjny, który stara się znaleźć minimum funkcji kosztu. Działa on w następujący sposób:

1.  Wybieramy losowy punkt startowy (czyli losowe wartości parametrów modelu).
2.  Obliczamy gradient funkcji kosztu w tym punkcie.
3.  Przesuwamy się o mały krok w kierunku przeciwnym do gradientu (czyli w kierunku najszybszego spadku).
4.  Powtarzamy kroki 2 i 3, aż dojdziemy do punktu, w którym gradient jest bliski zeru, co sugeruje, że znaleźliśmy minimum (lub minimum lokalne).

Ten prosty, a zarazem potężny mechanizm, jest podstawą trenowania większości nowoczesnych modeli uczenia maszynowego, w tym **sieci neuronowych**. W praktyce stosuje się różne warianty metody spadku gradientu, takie jak **stochastyczny spadek gradientu (Stochastic Gradient Descent - SGD)** czy **Adam**, które wprowadzają pewne modyfikacje w celu przyspieszenia i ustabilizowania procesu uczenia.

Inne zastosowania w informatyce to m.in.:

*   **Przetwarzanie obrazów:** Gradienty są używane do wykrywania krawędzi na obrazach. Duża zmiana wartości (jasności) pikseli w pewnym kierunku oznacza duży gradient, co jest charakterystyczne dla krawędzi.
*   **Grafika komputerowa:** W optymalizacji siatek (mesh optimization) i renderowaniu.
*   **Robotyka:** W planowaniu ścieżki i optymalizacji ruchów robota.


## 2. Wielomian i szereg Taylora funkcji rzeczywistej.

### Szczegółowe wyjaśnienie

**Idea aproksymacji**

Często w matematyce i informatyce spotykamy się ze skomplikowanymi funkcjami (np. sin(x), e^x, log(x)), z którymi trudno jest wykonywać operacje analityczne lub numeryczne. Idea stojąca za wielomianem i szeregiem Taylora jest genialna w swojej prostocie: **przybliżmy (aproksymujmy) te skomplikowane funkcje za pomocą prostszych funkcji, a mianowicie wielomianów.** Wielomiany są "przyjemne" w obsłudze – łatwo je różniczkować, całkować i obliczać ich wartości.

**Wielomian Taylora**

Wielomian Taylora to wielomian, który w zadanym punkcie (nazwijmy go 'a') "naśladuje" zachowanie danej funkcji. Oznacza to, że w tym punkcie 'a' wielomian ma taką samą wartość jak funkcja, taką samą wartość pierwszej pochodnej, drugiej pochodnej, i tak dalej, aż do pochodnej n-tego rzędu. Im więcej pochodnych "uzgodnimy", tym lepsze będzie przybliżenie funkcji przez wielomian w otoczeniu punktu 'a'.

Wzór na wielomian Taylora n-tego stopnia dla funkcji f(x) w otoczeniu punktu 'a' wygląda następująco:

Tₙ(x) = f(a) + (f'(a)/1!)(x-a) + (f''(a)/2!)(x-a)² + ... + (fⁿ(a)/n!)(x-a)ⁿ

Można go zapisać bardziej zwięźle jako:

Tₙ(x) = Σ (od k=0 do n) [fᵏ(a)/k!] * (x-a)ᵏ

gdzie fᵏ(a) to k-ta pochodna funkcji f w punkcie a, a k! to silnia z k.

**Szereg Taylora**

A co, jeśli pozwolimy, aby stopień wielomianu rósł w nieskończoność (n → ∞)? Otrzymamy wtedy **szereg Taylora**. Jeśli funkcja jest "wystarczająco grzeczna" (analityczna), to jej szereg Taylora będzie do niej zbieżny w pewnym przedziale zbieżności. Oznacza to, że w tym przedziale możemy traktować funkcję i jej szereg Taylora jako tożsame.

Szczególnym, ale bardzo ważnym przypadkiem szeregu Taylora jest **szereg Maclaurina**, który jest po prostu szeregiem Taylora rozwiniętym w otoczeniu punktu a = 0.

**Zastosowania w informatyce**

Szereg Taylora ma fundamentalne znaczenie w analizie numerycznej i wielu innych dziedzinach informatyki:

*   **Obliczenia numeryczne:** Komputery i kalkulatory nie przechowują wartości funkcji trygonometrycznych czy wykładniczych dla wszystkich możliwych argumentów. Zamiast tego, gdy potrzebują obliczyć np. sin(0.1), używają kilku pierwszych wyrazów szeregu Maclaurina dla funkcji sinus. Daje to bardzo dobre przybliżenie z niewielkim kosztem obliczeniowym.
*   **Analiza algorytmów:** W analizie złożoności obliczeniowej algorytmów, rozwinięcia w szereg Taylora pomagają szacować zachowanie funkcji dla dużych danych wejściowych.
*   **Fizyka i grafika komputerowa:** W symulacjach fizycznych (np. ruchu ciał) i grafice komputerowej, skomplikowane równania są często linearyzowane (przybliżane za pomocą pierwszego wyrazu szeregu Taylora), co znacznie upraszcza i przyspiesza obliczenia.
*   **Optymalizacja:** Podobnie jak gradient, szereg Taylora jest używany w bardziej zaawansowanych metodach optymalizacyjnych (np. metoda Newtona), które wykorzystują informacje z drugiej pochodnej (Hessjanu) do jeszcze szybszego znajdowania ekstremów funkcji.


## 3. Układy równań liniowych: różne metody rozwiązywania, liczba rozwiązań.

### Szczegółowe wyjaśnienie

**Czym jest układ równań liniowych?**

Układ równań liniowych to zbiór kilku równań, w których niewiadome występują tylko w pierwszej potędze. Ogólną postać układu m równań z n niewiadomymi można zapisać w postaci macierzowej jako:

**Ax = b**

Gdzie:
*   **A** to macierz współczynników przy niewiadomych (macierz główna układu).
*   **x** to wektor (kolumna) niewiadomych.
*   **b** to wektor (kolumna) wyrazów wolnych.

Rozwiązanie układu polega na znalezieniu takiego wektora **x**, który spełnia wszystkie równania jednocześnie.

**Metody rozwiązywania**

Istnieje wiele metod rozwiązywania układów równań liniowych. Można je podzielić na dwie główne kategorie:

1.  **Metody dokładne (analityczne):** Pozwalają na znalezienie dokładnego rozwiązania (o ile istnieje). Są skuteczne dla mniejszych układów.
    *   **Metoda podstawiania:** Polega na wyznaczeniu jednej niewiadomej z jednego równania i podstawieniu jej do pozostałych równań. Powtarzamy ten proces, aż dojdziemy do jednego równania z jedną niewiadomą.
    *   **Metoda przeciwnych współczynników:** Polega na takim mnożeniu równań przez liczby, aby współczynniki przy jednej z niewiadomych w dwóch różnych równaniach były liczbami przeciwnymi. Po dodaniu tych równań stronami, jedna niewiadoma się redukuje.
    *   **Metoda eliminacji Gaussa:** To bardziej systematyczna i ogólna metoda, która jest podstawą wielu algorytmów komputerowych. Polega na wykonywaniu operacji elementarnych na wierszach macierzy rozszerzonej [A|b] (macierz A uzupełniona o kolumnę b) w celu sprowadzenia jej do postaci schodkowej. Z postaci schodkowej można już łatwo odczytać rozwiązania.
    *   **Metoda Cramera (metoda wyznaczników):** Pozwala na znalezienie rozwiązania za pomocą obliczania wyznaczników. Jest elegancka teoretycznie, ale obliczeniowo bardzo kosztowna dla dużych układów (złożoność rośnie jak n!).

2.  **Metody iteracyjne (przybliżone):** Stosowane głównie w informatyce do rozwiązywania bardzo dużych układów równań (np. setki tysięcy niewiadomych), które często pojawiają się w symulacjach naukowych i inżynierskich. Metody te startują od przybliżonego rozwiązania i w kolejnych krokach (iteracjach) poprawiają je, zbliżając się do rozwiązania dokładnego.
    *   **Metoda Jacobiego**
    *   **Metoda Gaussa-Seidla**

**Liczba rozwiązań**

Kluczowe pytanie dotyczące każdego układu równań liniowych brzmi: ile ma on rozwiązań? Odpowiedź na to pytanie daje fundamentalne **twierdzenie Kroneckera-Capellego**. Mówi ono, że aby układ równań liniowych miał rozwiązanie, **rząd macierzy głównej (A) musi być równy rzędowi macierzy rozszerzonej ([A|b])**.

Rząd macierzy to, w uproszczeniu, maksymalna liczba liniowo niezależnych wierszy (lub kolumn) w tej macierzy.

Analizując rzędy obu macierzy, możemy wyróżnić trzy przypadki:

1.  **Układ sprzeczny (brak rozwiązań):** Dzieje się tak, gdy `rząd(A) < rząd([A|b])`. Oznacza to, że równania są ze sobą sprzeczne (np. x + y = 2 i x + y = 3).
2.  **Układ oznaczony (dokładnie jedno rozwiązanie):** Dzieje się tak, gdy `rząd(A) = rząd([A|b]) = n`, gdzie n to liczba niewiadomych. Wtedy istnieje dokładnie jeden wektor x, który spełnia układ.
3.  **Układ nieoznaczony (nieskończenie wiele rozwiązań):** Dzieje się tak, gdy `rząd(A) = rząd([A|b]) < n`. Oznacza to, że mamy mniej niezależnych równań niż niewiadomych. Rozwiązania zależą wtedy od pewnej liczby parametrów (dokładnie od `n - rząd(A)` parametrów).

**Zastosowania w informatyce**

Układy równań liniowych są wszechobecne w informatyce:

*   **Grafika komputerowa:** Do obliczania transformacji (obroty, skalowanie, przesunięcia), oświetlenia, cieniowania.
*   **Sieci komputerowe:** Analiza przepływu danych w sieciach.
*   **Uczenie maszynowe:** W regresji liniowej celem jest znalezienie współczynników modelu, co sprowadza się do rozwiązania układu równań.
*   **Analiza obwodów elektrycznych.**
*   **Badania operacyjne i optymalizacja.**


## 4. Wartości własne macierzy i ich zastosowanie w informatyce.

### Szczegółowe wyjaśnienie

**Intuicja geometryczna**

Wyobraźmy sobie, że macierz **A** reprezentuje pewne przekształcenie liniowe w przestrzeni (np. obrót, skalowanie, ścinanie). Działanie tej macierzy na dowolny wektor **v** daje w wyniku nowy wektor **Av**, który jest na ogół obrócony i przeskalowany względem wektora oryginalnego.

Pytanie brzmi: czy istnieją takie szczególne, **niezerowe** wektory, które po poddaniu ich temu przekształceniu **nie zmieniają swojego kierunku**? Okazuje się, że tak. Te właśnie wektory nazywamy **wektorami własnymi** macierzy **A**.

Formalnie, niezerowy wektor **v** jest wektorem własnym macierzy **A**, jeśli istnieje taka liczba **λ** (lambda), że:

**Av = λv**

Co to oznacza? Oznacza to, że działanie macierzy **A** na wektor własny **v** sprowadza się do prostego przeskalowania tego wektora przez pewną wartość **λ**. Kierunek wektora **v** pozostaje niezmieniony. Liczbę **λ** nazywamy **wartością własną** odpowiadającą wektorowi własnemu **v**.

*   Jeśli λ > 1, wektor własny jest wydłużany.
*   Jeśli 0 < λ < 1, wektor własny jest skracany.
*   Jeśli λ < 0, wektor własny zmienia zwrot na przeciwny (ale wciąż leży na tej samej prostej).

Każda macierz kwadratowa n x n ma co najwyżej n różnych wartości własnych. Znalezienie ich sprowadza się do rozwiązania tzw. **równania charakterystycznego**: `det(A - λI) = 0`, gdzie **I** to macierz jednostkowa.

**Zastosowania w informatyce**

Wartości i wektory własne są jednym z najważniejszych narzędzi algebry liniowej i mają ogromną liczbę zastosowań w informatyce, ponieważ pozwalają "zrozumieć" istotę przekształcenia reprezentowanego przez macierz – odkrywają jej niezmiennicze kierunki.

*   **Algorytm PageRank (Google):** To jedno z najsłynniejszych zastosowań. Sieć WWW można przedstawić jako gigantyczny graf, gdzie strony to wierzchołki, a linki to krawędzie. Można zbudować macierz sąsiedztwa (lub jej wariant) dla tego grafu. Okazuje się, że **wektor własny odpowiadający największej wartości własnej tej macierzy reprezentuje "ważność" każdej strony w sieci**. Komponenty tego wektora to właśnie wartości PageRank, które Google używało (i w zmodyfikowanej formie wciąż używa) do szeregowania wyników wyszukiwania.

*   **Analiza głównych składowych (Principal Component Analysis - PCA):** To fundamentalna technika w uczeniu maszynowym i statystyce, służąca do **redukcji wymiarowości** danych. Mając zbiór danych z wieloma cechami (np. tysiącami), PCA pozwala znaleźć nowe osie (kierunki) w przestrzeni tych danych, które najlepiej "wyjaśniają" wariancję w danych. Te nowe osie to nic innego jak **wektory własne macierzy kowariancji** danych. Wartości własne mówią nam, jak ważna jest każda z tych nowych osi (ile wariancji wyjaśnia). Odrzucając osie o najmniejszych wartościach własnych, możemy znacząco zredukować liczbę cech, tracąc przy tym niewiele informacji.

*   **Grafika komputerowa:** Wartości własne i wektory własne są używane do analizy tensora bezwładności, co jest kluczowe w symulacjach fizycznych i animacji brył sztywnych. Pomagają też w deformacji obiektów i analizie naprężeń.

*   **Przetwarzanie obrazów:** W rozpoznawaniu twarzy (metoda Eigenfaces), twarze są reprezentowane jako wektory. Analiza PCA na zbiorze takich wektorów pozwala wyodrębnić "twarze własne" (eigenfaces), które są podstawowymi komponentami, z których można "składać" ludzkie twarze. Każda twarz w bazie danych jest wtedy kombinacją liniową tych twarzy własnych.


## 5. Grafy i ich typy, metody reprezentacji grafów.

### Szczegółowe wyjaśnienie

**Czym jest graf?**

Graf to jedna z najbardziej fundamentalnych i uniwersalnych struktur w matematyce i informatyce. W sposób formalny, graf **G** to para **(V, E)**, gdzie:

*   **V** (od ang. *vertices*) to zbiór **wierzchołków** (nazywanych też węzłami lub punktami).
*   **E** (od ang. *edges*) to zbiór **krawędzi**, które łączą pary wierzchołków.

Grafy są niezwykle potężnym narzędziem do modelowania różnorodnych problemów, w których istotne są **relacje** i **połączenia** między obiektami. Obiektami są wierzchołki, a relacjami – krawędzie.

**Typy grafów**

Grafy można klasyfikować na wiele sposobów, w zależności od właściwości ich krawędzi i struktury:

1.  **Graf nieskierowany (prosty):** Krawędzie nie mają orientacji. Krawędź {u, v} jest tym samym co {v, u}. To najprostszy i najczęściej spotykany typ grafu. Przykład: sieć znajomych na Facebooku (jeśli A jest znajomym B, to B jest znajomym A).

2.  **Graf skierowany (digraf):** Krawędzie mają orientację (są jak strzałki). Krawędź (u, v) oznacza połączenie *od* u *do* v, co nie jest tym samym co (v, u). Przykład: sieć linków internetowych (strona A linkuje do B, ale B nie musi linkować do A).

3.  **Graf ważony:** Każdej krawędzi przypisana jest pewna wartość liczbowa, nazywana **wagą**. Waga może reprezentować koszt, odległość, czas, przepustowość itp. Przykład: mapa drogowa, gdzie wierzchołki to miasta, a wagi krawędzi to odległości między nimi.

4.  **Multigraf:** Dozwolone są **krawędzie wielokrotne** między tą samą parą wierzchołków.

5.  **Pseudograf:** Dozwolone są pętle (krawędzie łączące wierzchołek z samym sobą).

Inne ważne klasy grafów to:

*   **Graf spójny:** Z każdego wierzchołka da się dojść do każdego innego wierzchołka, poruszając się po krawędziach.
*   **Drzewo:** Graf spójny, który nie zawiera cykli. Ma fundamentalne znaczenie w informatyce (np. drzewa binarne, drzewa decyzyjne).
*   **Graf pełny:** Każdy wierzchołek jest połączony z każdym innym wierzchołkiem.
*   **Graf dwudzielny:** Zbiór wierzchołków można podzielić na dwa rozłączne podzbiory tak, że krawędzie istnieją tylko *pomiędzy* tymi podzbiorami, a nie wewnątrz nich.

**Metody reprezentacji grafów w informatyce**

Aby móc przetwarzać grafy za pomocą algorytmów, musimy je w jakiś sposób zapisać w pamięci komputera. Istnieją dwie główne metody reprezentacji:

1.  **Macierz sąsiedztwa (Adjacency Matrix):**
    *   Jest to macierz kwadratowa o wymiarach |V| x |V| (gdzie |V| to liczba wierzchołków).
    *   Jeśli istnieje krawędź między wierzchołkiem *i* a *j*, to element macierzy `A[i][j]` jest równy 1 (lub wadze krawędzi w grafie ważonym). W przeciwnym razie jest równy 0.
    *   **Zalety:** Szybkie sprawdzanie istnienia krawędzi między dwoma wierzchołkami (czas O(1)).
    *   **Wady:** Duże zużycie pamięci (|V|²), nawet dla grafów z małą liczbą krawędzi (grafów rzadkich). Iterowanie po wszystkich sąsiadach danego wierzchołka wymaga przejrzenia całego wiersza (czas O(|V|)).

2.  **Lista sąsiedztwa (Adjacency List):**
    *   Jest to tablica (lub lista) list. Dla każdego wierzchołka *u* przechowujemy listę wierzchołków, do których prowadzą krawędzie z *u*.
    *   W Pythonie można to zaimplementować jako słownik, gdzie kluczami są wierzchołki, a wartościami – listy ich sąsiadów.
    *   **Zalety:** Efektywna pamięciowo dla grafów rzadkich (zużycie pamięci proporcjonalne do |V| + |E|). Łatwe i szybkie iterowanie po wszystkich sąsiadach danego wierzchołka.
    *   **Wady:** Sprawdzanie istnienia konkretnej krawędzi (u, v) może wymagać przejrzenia całej listy sąsiadów wierzchołka *u* (czas O(stopień(u))).

**Wybór reprezentacji zależy od specyfiki problemu:** dla grafów gęstych (dużo krawędzi) macierz sąsiedztwa może być dobrym wyborem, ale w większości praktycznych zastosowań, gdzie grafy są rzadkie (np. sieć dróg, sieć społecznościowa), **lista sąsiedztwa jest znacznie bardziej efektywna** i jest standardowym wyborem.


## 6. Relacje binarne, własności i metody reprezentacji.

### Szczegółowe wyjaśnienie

**Czym jest relacja binarna?**

Relacja binarna (lub dwuargumentowa) to formalny sposób opisu powiązań między elementami. Jeśli mamy zbiór A, to relacja R na tym zbiorze jest po prostu dowolnym podzbiorem **iloczynu kartezjańskiego** A x A. 

Iloczyn kartezjański A x A to zbiór wszystkich możliwych par uporządkowanych (a, b), gdzie *a* i *b* należą do zbioru A. 

Fakt, że para (a, b) należy do relacji R, zapisujemy jako `a R b` i czytamy "a jest w relacji R z b".

**Przykłady:**
*   **Zbiór A = {1, 2, 3}.** Relacja "mniejszości" (<) to zbiór par `R = {(1, 2), (1, 3), (2, 3)}`.
*   **Zbiór A = zbiór wszystkich ludzi.** Relacja "bycia rodzeństwem" to zbiór wszystkich par (osoba1, osoba2), gdzie osoba1 jest rodzeństwem osoby2.
*   **Zbiór A = zbiór wszystkich liczb całkowitych.** Relacja "dzielenia bez reszty" to zbiór par (a, b) takich, że a jest dzielnikiem b.

**Własności relacji**

Relacje mogą mieć różne ważne właściwości, które pozwalają je klasyfikować. Dla relacji R na zbiorze A, najważniejsze własności to:

1.  **Zwrotność (refleksywność):** Relacja jest zwrotna, jeśli każdy element jest w relacji sam ze sobą.
    *   Formalnie: `∀a ∈ A: a R a`
    *   Przykład: Relacja "≤" na liczbach rzeczywistych jest zwrotna, bo każda liczba jest mniejsza lub równa samej sobie (a ≤ a).
    *   Kontrprzykład: Relacja "<" nie jest zwrotna (a < a jest fałszem).

2.  **Symetryczność:** Relacja jest symetryczna, jeśli dla dowolnych dwóch elementów, jeśli pierwszy jest w relacji z drugim, to drugi jest też w relacji z pierwszym.
    *   Formalnie: `∀a, b ∈ A: (a R b) ⇒ (b R a)`
    *   Przykład: Relacja "bycia rodzeństwem" jest symetryczna. Jeśli Jan jest bratem Anny, to Anna jest siostrą Jana.
    *   Kontrprzykład: Relacja "≤" nie jest symetryczna. 3 ≤ 5, ale 5 ≤ 3 jest fałszem.

3.  **Przechodniość (tranzytywność):** Relacja jest przechodnia, jeśli dla dowolnych trzech elementów, jeśli pierwszy jest w relacji z drugim, a drugi z trzecim, to pierwszy jest też w relacji z trzecim.
    *   Formalnie: `∀a, b, c ∈ A: (a R b ∧ b R c) ⇒ (a R c)`
    *   Przykład: Relacja "<" jest przechodnia. Jeśli a < b i b < c, to a < c.
    *   Kontrprzykład: Relacja "bycia znajomym" nie musi być przechodnia. Adam zna Basię, Basia zna Czesława, ale Adam nie musi znać Czesława.

4.  **Antysymetryczność:** Relacja jest antysymetryczna, jeśli dla dowolnych dwóch *różnych* elementów, nie może zachodzić w obie strony.
    *   Formalnie: `∀a, b ∈ A: (a R b ∧ b R a) ⇒ (a = b)`
    *   Przykład: Relacja "≤" jest antysymetryczna. Jeśli a ≤ b i b ≤ a, to musi być a = b.

Te właściwości są kluczowe, ponieważ pozwalają definiować ważne struktury matematyczne:

*   **Relacja równoważności:** To relacja, która jest jednocześnie **zwrotna, symetryczna i przechodnia**. Dzieli ona zbiór na rozłączne podzbiory, nazywane klasami abstrakcji (np. relacja "przystawania modulo n").
*   **Częściowy porządek:** To relacja, która jest **zwrotna, antysymetryczna i przechodnia**. Ustanawia ona hierarchię w zbiorze (np. relacja "≤" na liczbach, relacja zawierania się zbiorów).

**Metody reprezentacji**

Podobnie jak grafy, relacje na zbiorach skończonych możemy reprezentować w komputerze na kilka sposobów:

1.  **Macierz logiczna (macierz sąsiedztwa):** Jeśli zbiór A ma n elementów, tworzymy macierz M o wymiarach n x n. Komórka `M[i][j]` ma wartość `true` (lub 1), jeśli element *i* jest w relacji z elementem *j*, a `false` (lub 0) w przeciwnym przypadku. Ta reprezentacja jest bardzo wygodna do sprawdzania własności relacji:
    *   **Zwrotność:** Wszystkie elementy na głównej przekątnej muszą być równe 1.
    *   **Symetryczność:** Macierz musi być symetryczna względem głównej przekątnej (`M[i][j] == M[j][i]` dla wszystkich i, j).

2.  **Lista par:** Możemy po prostu przechowywać zbiór (lub listę) wszystkich par (a, b), które należą do relacji. Jest to bardziej oszczędne pamięciowo, jeśli relacja jest rzadka (mało par).

3.  **Graf skierowany:** Każdej relacji binarnej na zbiorze A odpowiada graf skierowany, którego wierzchołkami są elementy zbioru A. Krawędź skierowana od *a* do *b* istnieje wtedy i tylko wtedy, gdy `a R b`. Ta wizualna reprezentacja jest bardzo intuicyjna i pozwala łatwo "zobaczyć" własności relacji (np. pętle w każdym wierzchołku dla zwrotności, dwukierunkowe krawędzie dla symetryczności).


## 7. Zasada indukcji matematycznej.

### Szczegółowe wyjaśnienie

**Czym jest indukcja matematyczna?**

Zasada indukcji matematycznej to potężna metoda dowodzenia twierdzeń, które są prawdziwe dla wszystkich liczb naturalnych (lub dla wszystkich liczb naturalnych począwszy od pewnej liczby n₀). Jest to jedno z fundamentalnych narzędzi w matematyce, a zwłaszcza w matematyce dyskretnej i informatyce.

**Analogia kostek domina**

Najlepszym sposobem na intuicyjne zrozumienie indukcji jest wyobrażenie sobie nieskończonego rzędu kostek domina, ponumerowanych 1, 2, 3, ... . Chcemy udowodnić, że wszystkie kostki się przewrócą. Aby to zrobić, nie musimy przewracać każdej kostki z osobna. Wystarczy, że udowodnimy dwie rzeczy:

1.  **Przewrócimy pierwszą kostkę.** (To jest nasz *krok bazowy*).
2.  **Kostki są ustawione na tyle blisko siebie, że jeśli jakakolwiek kostka (nazwijmy ją *k*) się przewróci, to pociągnie za sobą następną kostkę (o numerze *k*+1).** (To jest nasz *krok indukcyjny*).

Jeśli te dwa warunki są spełnione, mamy gwarancję, że cały łańcuch reakcji zadziała: pierwsza kostka przewróci drugą, druga trzecią, trzecia czwartą, i tak dalej w nieskończoność. Wszystkie kostki się przewrócą.

**Formalny schemat dowodu indukcyjnego**

Dowód indukcyjny twierdzenia T(n) dla wszystkich liczb naturalnych n ≥ n₀ przebiega zawsze w trzech krokach:

1.  **Krok bazowy (lub baza indukcji):**
    Sprawdzamy "ręcznie", czy twierdzenie T(n) jest prawdziwe dla początkowej wartości, czyli dla n = n₀. Najczęściej n₀ = 1 lub n₀ = 0.

2.  **Założenie indukcyjne:**
    Zakładamy, że twierdzenie T(k) jest prawdziwe dla pewnej, dowolnie wybranej, ale ustalonej liczby naturalnej k ≥ n₀. Innymi słowy, zakładamy, że `T(k)` jest prawdą.

3.  **Krok indukcyjny (lub teza indukcyjna):**
    Korzystając z założenia indukcyjnego (że T(k) jest prawdziwe), musimy udowodnić, że twierdzenie jest również prawdziwe dla następnej liczby, czyli dla k+1. Musimy pokazać, że z prawdziwości `T(k)` wynika prawdziwość `T(k+1)`.

Jeśli uda nam się pomyślnie przejść przez te trzy etapy, to na mocy zasady indukcji matematycznej możemy stwierdzić, że twierdzenie T(n) jest prawdziwe dla wszystkich liczb naturalnych n ≥ n₀.

**Przykład: Suma kolejnych liczb naturalnych**

Udowodnijmy, że dla każdej liczby naturalnej n ≥ 1, suma liczb od 1 do n wynosi `n(n+1)/2`.
Twierdzenie T(n): `1 + 2 + 3 + ... + n = n(n+1)/2`

1.  **Krok bazowy (dla n=1):**
    *   Lewa strona: 1
    *   Prawa strona: `1(1+1)/2 = 2/2 = 1`
    *   L = P, więc twierdzenie jest prawdziwe dla n=1.

2.  **Założenie indukcyjne (dla n=k):**
    Zakładamy, że dla pewnego k ≥ 1, prawdą jest, że: `1 + 2 + ... + k = k(k+1)/2`

3.  **Krok indukcyjny (dla n=k+1):**
    Chcemy udowodnić, że: `1 + 2 + ... + k + (k+1) = (k+1)((k+1)+1)/2`
    Dowód:
    Zacznijmy od lewej strony tezy i skorzystajmy z założenia:
    `L = (1 + 2 + ... + k) + (k+1)`
    `L = [k(k+1)/2] + (k+1)` (tutaj użyliśmy założenia!)
    Sprowadźmy do wspólnego mianownika:
    `L = k(k+1)/2 + 2(k+1)/2`
    `L = (k(k+1) + 2(k+1))/2`
    Wyciągnijmy `(k+1)` przed nawias:
    `L = (k+1)(k+2)/2`
    `L = (k+1)((k+1)+1)/2`
    Otrzymaliśmy prawą stronę tezy. Zatem udowodniliśmy krok indukcyjny.

**Wniosek:** Ponieważ spełniony jest krok bazowy i krok indukcyjny, na mocy zasady indukcji matematycznej twierdzenie jest prawdziwe dla wszystkich n ≥ 1.

**Zastosowania w informatyce**

Indukcja jest absolutnie kluczowa w informatyce, zwłaszcza do:

*   **Dowodzenia poprawności algorytmów:** Szczególnie algorytmów rekurencyjnych i iteracyjnych (pętli). Można udowodnić, że pętla zachowuje pewien "niezmiennik" lub że algorytm rekurencyjny poprawnie rozwiązuje problem dla n, jeśli poprawnie rozwiązuje go dla n-1.
*   **Analizy złożoności obliczeniowej:** Do rozwiązywania równań rekurencyjnych, które opisują czas działania algorytmów typu "dziel i zwyciężaj".
*   **Definiowania struktur danych:** Struktury rekurencyjne, takie jak drzewa czy listy, są naturalnie definiowane i analizowane za pomocą indukcji.


## 8. Twierdzenie Bayesa.

### Szczegółowe wyjaśnienie

**Odwracanie prawdopodobieństwa warunkowego**

Twierdzenie Bayesa (nazywane też wzorem Bayesa) to fundamentalne prawo w teorii prawdopodobieństwa, które opisuje, jak zaktualizować naszą wiedzę (prawdopodobieństwo) o pewnym zdarzeniu w świetle nowych dowodów (obserwacji).

Jego istotą jest **odwracanie prawdopodobieństwa warunkowego**. Co to znaczy?

*   Często łatwo jest obliczyć `P(B|A)` - prawdopodobieństwo zajścia zdarzenia B, *pod warunkiem*, że zaszło zdarzenie A. Na przykład, łatwo jest określić prawdopodobieństwo, że test na daną chorobę da wynik pozytywny, *jeśli* pacjent jest chory.
*   Jednak w praktyce często interesuje nas coś odwrotnego: `P(A|B)` - prawdopodobieństwo, że zaszło zdarzenie A, *pod warunkiem*, że zaobserwowaliśmy zdarzenie B. Na przykład, jakie jest prawdopodobieństwo, że pacjent jest faktycznie chory, *jeśli* test dał wynik pozytywny?

Twierdzenie Bayesa pozwala nam właśnie na to przejście.

**Wzór Bayesa**

Formalny wzór Bayesa wygląda następująco:

`P(A|B) = [P(B|A) * P(A)] / P(B)`

Poszczególne składniki mają swoje nazwy w tzw. interpretacji bayesowskiej:

*   `P(A|B)` - **prawdopodobieństwo a posteriori** (ang. *posterior*). To jest to, co chcemy obliczyć – zaktualizowane prawdopodobieństwo hipotezy A po zaobserwowaniu dowodu B.
*   `P(A)` - **prawdopodobieństwo a priori** (ang. *prior*). To nasza początkowa wiedza (prawdopodobieństwo) o hipotezie A, *przed* uzyskaniem jakichkolwiek nowych dowodów.
*   `P(B|A)` - **wiarygodność** (ang. *likelihood*). Prawdopodobieństwo zaobserwowania dowodu B, przy założeniu, że hipoteza A jest prawdziwa.
*   `P(B)` - **prawdopodobieństwo brzegowe dowodu** (ang. *marginal likelihood* lub *evidence*). Całkowite prawdopodobieństwo zaobserwowania dowodu B. Jest to często najtrudniejszy do obliczenia składnik. Oblicza się go zwykle ze wzoru na prawdopodobieństwo całkowite:
    `P(B) = P(B|A) * P(A) + P(B|A') * P(A')`
    (gdzie A' to zdarzenie przeciwne do A)

**Przykład: Test medyczny**

Wyobraźmy sobie, że rzadka choroba dotyka 1% populacji. Stworzono test do jej wykrywania, który ma następującą skuteczność:
*   Jeśli ktoś jest chory, test wykrywa to w 99% przypadków (czułość).
*   Jeśli ktoś jest zdrowy, test mylnie wskazuje chorobę w 5% przypadków (1 - swoistość).

Losowa osoba poddaje się testowi i otrzymuje wynik pozytywny. Jakie jest prawdopodobieństwo, że jest faktycznie chora?

Oznaczmy:
*   A - osoba jest chora
*   A' - osoba jest zdrowa
*   B - test dał wynik pozytywny

Dane:
*   `P(A) = 0.01` (prawdopodobieństwo a priori - choroba dotyka 1% populacji)
*   `P(A') = 0.99`
*   `P(B|A) = 0.99` (wiarygodność - czułość testu)
*   `P(B|A') = 0.05` (prawdopodobieństwo wyniku fałszywie pozytywnego)

Szukamy `P(A|B)`.

Najpierw obliczmy `P(B)` ze wzoru na prawdopodobieństwo całkowite:
`P(B) = P(B|A) * P(A) + P(B|A') * P(A')`
`P(B) = (0.99 * 0.01) + (0.05 * 0.99) = 0.0099 + 0.0495 = 0.0594`

Teraz możemy użyć wzoru Bayesa:
`P(A|B) = [P(B|A) * P(A)] / P(B)`
`P(A|B) = (0.99 * 0.01) / 0.0594 = 0.0099 / 0.0594 ≈ 0.1667`

**Wniosek:** Mimo że test wydaje się bardzo dokładny, prawdopodobieństwo, że osoba z pozytywnym wynikiem jest faktycznie chora, wynosi tylko około 16.7%! Ten zaskakujący wynik pokazuje, jak ważna jest informacja a priori (w tym przypadku, jak rzadka jest choroba).

**Zastosowania w informatyce**

Twierdzenie Bayesa jest fundamentem dla ogromnej gałęzi uczenia maszynowego i sztucznej inteligencji:

*   **Filtry antyspamowe:** To klasyczne zastosowanie. Filtr uczy się, jakie jest prawdopodobieństwo wystąpienia pewnych słów (np. "Viagra", "promocja") w spamie (`P(słowo|spam)`) i w normalnych mailach (`P(słowo|nie-spam)`). Gdy przychodzi nowy mail, filtr używa twierdzenia Bayesa, aby obliczyć `P(spam|słowa w mailu)` – prawdopodobieństwo, że mail jest spamem, biorąc pod uwagę słowa, które zawiera. Algorytm ten nazywa się **naiwnym klasyfikatorem bayesowskim**.
*   **Systemy rekomendacyjne:** Pomagają oszacować prawdopodobieństwo, że użytkownik polubi dany produkt, na podstawie jego wcześniejszych ocen i ocen innych użytkowników.
*   **Rozpoznawanie mowy i przetwarzanie języka naturalnego:** Do określania najbardziej prawdopodobnego słowa lub zdania na podstawie sygnału dźwiękowego lub sekwencji znaków.
*   **Robotyka i widzenie komputerowe:** Do lokalizacji robota (gdzie jestem, biorąc pod uwagę odczyty z sensorów?) i rozpoznawania obiektów (co to za obiekt, biorąc pod uwagę jego cechy?).
*   **Sieci bayesowskie:** Graficzne modele, które reprezentują zależności probabilistyczne między zmiennymi, używane w diagnostyce, prognozowaniu i analizie ryzyka.


## 9. Testowanie hipotez statystycznych.

### Szczegółowe wyjaśnienie

**Czym jest testowanie hipotez?**

Testowanie hipotez statystycznych to formalna procedura, która pozwala nam podejmować decyzje dotyczące całej populacji na podstawie danych z losowej próby. Jest to fundament naukowego podejścia do analizy danych, pozwalający w sposób obiektywny ocenić, czy obserwowane w próbie efekty (np. różnice między grupami, zależności między zmiennymi) są "prawdziwe" i występują w całej populacji, czy też mogą być jedynie dziełem przypadku.

**Logika procesu (proces sądowy)**

Proces testowania hipotez można porównać do procesu sądowego:

1.  **Hipoteza zerowa (H₀) - "zasada domniemania niewinności":** Na początku zakładamy, że "nic ciekawego się nie dzieje". Jest to hipoteza o braku efektu, braku różnicy, braku zależności. Np. "nowy lek nie ma wpływu na czas leczenia", "średni wzrost mężczyzn i kobiet jest taki sam", "nie ma związku między paleniem a chorobami serca". **Hipoteza zerowa jest tym, co próbujemy obalić.**

2.  **Hipoteza alternatywna (H₁) - "akt oskarżenia":** To jest hipoteza, którą badacz chce udowodnić. Mówi ona, że "coś ciekawego się dzieje" - istnieje efekt, różnica lub zależność. Np. "nowy lek skraca czas leczenia", "mężczyźni są średnio wyżsi od kobiet".

3.  **Dowody (dane z próby):** Zbieramy dane z losowej próby, aby ocenić, na ile są one zgodne z hipotezą zerową.

4.  **Werdykt (decyzja statystyczna):** Na podstawie dowodów decydujemy, czy są one wystarczająco "mocne", aby odrzucić "domniemanie niewinności" (hipotezę zerową) na rzecz hipotezy alternatywnej.

**Kluczowe pojęcia**

*   **Statystyka testowa:** Jest to liczba obliczona na podstawie danych z próby, która mierzy, jak bardzo nasze dane odbiegają od tego, czego spodziewalibyśmy się, gdyby hipoteza zerowa była prawdziwa. Im dalej od zera, tym silniejsze dowody przeciwko H₀.

*   **Poziom istotności (α, alfa):** Jest to próg, który ustalamy *przed* przeprowadzeniem testu. Najczęściej α = 0.05 (czyli 5%). Reprezentuje on **maksymalne ryzyko popełnienia błędu I rodzaju, na jakie świadomie się godzimy**. Jest to próg dla "uzasadnionej wątpliwości".

*   **p-wartość (p-value):** To jest najważniejszy wynik testu. **p-wartość to prawdopodobieństwo uzyskania obserwowanej statystyki testowej (lub jeszcze bardziej ekstremalnej), przy założeniu, że hipoteza zerowa jest prawdziwa.**
    *   **Mała p-wartość (np. < 0.05):** Oznacza, że obserwowane przez nas dane są bardzo mało prawdopodobne, jeśli H₀ jest prawdziwa. To silny dowód przeciwko H₀. Można to interpretować jako: "Wow, taki wynik byłby niesamowitym zbiegiem okoliczności, gdyby nic się nie działo. Chyba jednak coś się dzieje!".
    *   **Duża p-wartość (np. > 0.05):** Oznacza, że nasze dane są całkiem zgodne z tym, czego można by się spodziewać przy prawdziwej H₀. Nie mamy podstaw, by ją odrzucić.

**Procedura testowania hipotez**

1.  Sformułuj hipotezę zerową (H₀) i alternatywną (H₁).
2.  Wybierz poziom istotności α (np. 0.05).
3.  Zbierz dane i oblicz wartość statystyki testowej (np. t, Z, chi-kwadrat).
4.  Oblicz p-wartość odpowiadającą tej statystyce.
5.  Podejmij decyzję:
    *   Jeśli **p ≤ α**, to **odrzucamy H₀** na rzecz H₁. Wynik jest **istotny statystycznie**.
    *   Jeśli **p > α**, to **nie ma podstaw do odrzucenia H₀**. Wynik jest **nieistotny statystycznie**.

**Błędy w testowaniu hipotez**

Ponieważ decyzje podejmujemy na podstawie próby, a nie całej populacji, zawsze istnieje ryzyko popełnienia błędu:

*   **Błąd I rodzaju (fałszywy alarm, α):** Odrzucenie prawdziwej hipotezy zerowej. To tak, jakby skazać niewinną osobę. Prawdopodobieństwo popełnienia tego błędu jest kontrolowane przez poziom istotności α.
*   **Błąd II rodzaju (przeoczenie, β):** Nieodrzucenie fałszywej hipotezy zerowej. To tak, jakby uniewinnić sprawcę. Prawdopodobieństwo tego błędu (β) jest związane z tzw. **mocą testu (1-β)**, która mówi o zdolności testu do wykrywania istniejących efektów.

**Zastosowania w informatyce**

*   **Testy A/B:** Fundamentalna technika w web developmencie i marketingu. Chcemy sprawdzić, czy nowa wersja strony (B) jest lepsza (np. ma wyższy współczynnik konwersji) od starej (A). H₀: "współczynnik konwersji jest taki sam dla obu wersji". H₁: "współczynnik konwersji jest wyższy dla wersji B". Testujemy, czy obserwowana różnica jest istotna statystycznie.
*   **Uczenie maszynowe:** Do oceny, czy dana cecha ma istotny wpływ na zmienną docelową, czy też jej związek jest przypadkowy. Do porównywania skuteczności różnych modeli.
*   **Bioinformatyka:** Do identyfikacji genów, których ekspresja różni się istotnie między grupą chorych a zdrowych.
*   **Badania UX (User Experience):** Do sprawdzania, czy zmiana w interfejsie istotnie skróciła czas wykonania zadania przez użytkowników.


## 10. Wyznaczanie przedziałów ufności.

### Szczegółowe wyjaśnienie

**Problem estymacji**

W statystyce rzadko kiedy mamy dostęp do danych o całej populacji (np. o wszystkich mieszkańcach Polski). Zamiast tego, badamy losową próbę i na jej podstawie staramy się wyciągać wnioski o całej populacji. Jednym z podstawowych zadań jest **estymacja (szacowanie)** nieznanych parametrów populacji, takich jak średnia (μ), wariancja (σ²) czy proporcja (p).

Możemy to robić na dwa sposoby:

1.  **Estymacja punktowa:** Obliczamy na podstawie próby jedną konkretną wartość, która ma być naszym "najlepszym strzałem" co do wartości parametru w populacji. Np. średnia z próby (x̄) jest estymatorem punktowym średniej w populacji (μ).
2.  **Estymacja przedziałowa:** Zdajemy sobie sprawę, że estymator punktowy prawie nigdy nie będzie idealnie równy prawdziwej wartości w populacji. Dlatego, zamiast podawać jedną liczbę, konstruujemy **przedział**, co do którego mamy określony poziom "ufności", że zawiera on prawdziwą, nieznaną wartość parametru. Ten przedział to właśnie **przedział ufności**.

**Czym jest przedział ufności?**

Przedział ufności to zakres wartości, obliczony na podstawie danych z próby, który z określonym prawdopodobieństwem (nazywanym **poziomem ufności**) pokrywa prawdziwą, nieznaną wartość parametru w populacji.

Najczęściej stosuje się poziom ufności 95%.

**Błędna interpretacja:** Częstym błędem jest mówienie: "istnieje 95% prawdopodobieństwa, że prawdziwa średnia populacji wpada w ten konkretny przedział [a, b]". To nie jest poprawne, ponieważ prawdziwa średnia (μ) jest stałą (choć nieznaną) wartością – ona albo w tym przedziale jest, albo jej nie ma. To przedział jest losowy, bo jest konstruowany na podstawie losowej próby.

**Poprawna interpretacja (częstościowa):** Jeśli z populacji pobralibyśmy bardzo wiele (np. 100) losowych prób i dla każdej z nich skonstruowali osobny 95% przedział ufności, to spodziewalibyśmy się, że **około 95 z tych 100 przedziałów** faktycznie pokryje prawdziwą wartość parametru populacji. Nasz jeden, konkretny przedział jest po prostu realizacją tego procesu.

**Konstrukcja przedziału ufności**

Ogólna struktura przedziału ufności jest następująca:

`Przedział ufności = (Estymator punktowy) ± (Margines błędu)`

Margines błędu zależy od trzech czynników:

1.  **Poziomu ufności:** Im wyższy poziom ufności (np. 99% zamiast 95%), tym szerszy będzie przedział. Chcąc mieć większą pewność, musimy podać szerszy zakres wartości. To wiąże się z wyborem odpowiedniej wartości krytycznej (np. z rozkładu normalnego lub t-Studenta).
2.  **Zmienności w populacji:** Im większe zróżnicowanie w populacji (mierzone odchyleniem standardowym), tym szerszy będzie przedział. Trudniej jest precyzyjnie oszacować parametr w bardzo zróżnicowanej populacji.
3.  **Wielkości próby (n):** Im większa próba, tym **węższy** będzie przedział ufności. Większa próba daje nam więcej informacji i pozwala na bardziej precyzyjne oszacowanie. To najważniejszy czynnik, na który badacz ma wpływ.

**Przykład (dla średniej, duża próba):**
95% przedział ufności dla średniej populacji (μ) ma postać:

`[x̄ - 1.96 * (σ/√n),   x̄ + 1.96 * (σ/√n)]`

Gdzie:
*   `x̄` to średnia z próby.
*   `σ` to odchylenie standardowe w populacji (jeśli nieznane, używa się odchylenia standardowego z próby `s`).
*   `n` to wielkość próby.
*   `1.96` to wartość krytyczna z rozkładu normalnego dla 95% ufności.

**Zastosowania w informatyce**

*   **Testy A/B:** Zamiast podawać tylko, że wersja B jest o 2% lepsza od A, podajemy przedział ufności dla tej różnicy, np. "Różnica w konwersji wynosi 2%, a 95% przedział ufności dla tej różnicy to [0.5%, 3.5%]". Ponieważ cały przedział jest powyżej zera, daje nam to pewność, że efekt jest realny. Gdyby przedział zawierał zero (np. [-1%, 5%]), oznaczałoby to, że różnica może być dziełem przypadku.
*   **Badania UX:** Prezentując średni czas wykonania zadania, zawsze należy podawać go wraz z przedziałem ufności, co daje pojęcie o precyzji tego oszacowania.
*   **Uczenie maszynowe:** Przy ocenie metryk wydajności modelu (np. dokładności) na zbiorze testowym, można obliczyć przedział ufności, aby oszacować, jak model prawdopodobnie zachowa się na nowych, niewidzianych danych.
*   **Monitoring systemów:** Analizując metryki wydajności (np. czas odpowiedzi serwera), przedziały ufności pomagają odróżnić normalne fluktuacje od istotnych zmian w zachowaniu systemu.


---

# Odpowiedzi "to the point" na obronę

## 1. Ekstrema funkcji i gradient, zastosowania w informatyce.

Ekstrema to lokalne minima i maksima funkcji. Dla funkcji różniczkowalnej, warunkiem koniecznym ich istnienia jest zerowanie się pierwszej pochodnej, a o ich rodzaju decyduje znak drugiej pochodnej. Gradient to wektor pochodnych cząstkowych, który wskazuje kierunek najszybszego wzrostu funkcji. Główne zastosowanie w informatyce to algorytm **spadku gradientu (gradient descent)** w uczeniu maszynowym, który minimalizuje funkcję błędu modelu poprzez iteracyjne poruszanie się w kierunku przeciwnym do gradientu, co jest podstawą trenowania np. sieci neuronowych.

## 2. Wielomian i szereg Taylora funkcji rzeczywistej.

Ideą szeregu Taylora jest aproksymacja, czyli przybliżanie skomplikowanych funkcji, jak sinus czy e^x, za pomocą prostszych funkcji, jakimi są wielomiany. Wielomian Taylora to wielomian, który w danym punkcie ma taką samą wartość i pochodne jak funkcja przybliżana. Szereg Taylora to jego rozszerzenie do nieskończonej liczby wyrazów. W informatyce używa się go głównie w obliczeniach numerycznych – np. kalkulatory używają kilku wyrazów szeregu do obliczenia wartości funkcji – oraz w grafice i fizyce do upraszczania (linearyzacji) skomplikowanych wzorów.

## 3. Układy równań liniowych: różne metody rozwiązywania, liczba rozwiązań.

Układy równań liniowych można rozwiązywać metodami dokładnymi, jak metoda eliminacji Gaussa, która jest podstawą algorytmów komputerowych, lub metodami iteracyjnymi, jak metoda Jacobiego, stosowanymi w informatyce do bardzo dużych układów. O liczbie rozwiązań decyduje **twierdzenie Kroneckera-Capellego**, które porównuje rząd macierzy głównej A i macierzy rozszerzonej. Gdy rzędy są równe i równe liczbie niewiadomych – mamy jedno rozwiązanie. Gdy rzędy są równe, ale mniejsze od liczby niewiadomych – nieskończenie wiele rozwiązań. Gdy rząd macierzy rozszerzonej jest większy – układ jest sprzeczny i nie ma rozwiązań.

## 4. Wartości własne macierzy i ich zastosowanie w informatyce.

Wektor własny macierzy to taki wektor, który po przekształceniu przez tę macierz nie zmienia swojego kierunku, a jedynie jest skalowany. Wartość własna to właśnie ten skalar. Wartości własne opisują fundamentalne właściwości przekształcenia. Główne zastosowania w informatyce to: **algorytm PageRank Google**, gdzie wektor własny macierzy sieci linków określał ranking stron, oraz **analiza głównych składowych (PCA)**, gdzie wektory własne macierzy kowariancji pozwalają na redukcję wymiarowości danych, co jest kluczowe w uczeniu maszynowym i analizie danych.

## 5. Grafy i ich typy, metody reprezentacji grafów.

Graf to struktura złożona z wierzchołków i łączących je krawędzi, służąca do modelowania relacji. Wyróżniamy grafy nieskierowane (np. sieć znajomych), skierowane (np. linki w internecie) i ważone (np. mapa dróg z odległościami). W informatyce grafy reprezentuje się na dwa główne sposoby: jako **macierz sąsiedztwa**, która jest dobra do szybkich zapytań o istnienie krawędzi, ale zajmuje dużo pamięci, oraz jako **lista sąsiedztwa**, która jest znacznie bardziej pamięciowo oszczędna dla grafów rzadkich i jest standardowym wyborem w większości zastosowań.

## 6. Relacje binarne, własności i metody reprezentacji.

Relacja binarna na zbiorze to formalny opis powiązań między jego elementami, definiowany jako podzbiór iloczynu kartezjańskiego. Kluczowe własności to **zwrotność**, **symetryczność** i **przechodniość**. Relacja, która posiada wszystkie trzy, to **relacja równoważności** i dzieli zbiór na klasy abstrakcji. Relacja zwrotna, antysymetryczna i przechodnia to **częściowy porządek**. W informatyce relacje reprezentuje się najczęściej jako macierz logiczną, gdzie łatwo sprawdzić własności, lub jako graf skierowany, co jest bardzo intuicyjne wizualnie.

## 7. Zasada indukcji matematycznej.

Indukcja matematyczna to metoda dowodzenia twierdzeń dla wszystkich liczb naturalnych. Dowód składa się z dwóch kroków, analogicznych do przewracania kostek domina. Pierwszy to **krok bazowy** – sprawdzamy twierdzenie dla pierwszej wartości, np. n=1 (przewracamy pierwszą kostkę). Drugi to **krok indukcyjny** – zakładamy, że twierdzenie jest prawdziwe dla pewnego 'k' i na tej podstawie dowodzimy, że jest prawdziwe dla 'k+1' (pokazujemy, że upadająca kostka 'k' przewraca kostkę 'k+1'). W informatyce jest to kluczowe narzędzie do dowodzenia poprawności algorytmów, zwłaszcza rekurencyjnych i pętli.

## 8. Twierdzenie Bayesa.

Twierdzenie Bayesa pozwala zaktualizować nasze przekonanie o prawdziwości hipotezy w świetle nowych dowodów. Jego istotą jest odwracanie prawdopodobieństwa warunkowego: jeśli znamy prawdopodobieństwo objawu przy danej chorobie, Bayes pozwala obliczyć prawdopodobieństwo choroby przy danym objawie. Wzór to `P(A|B) = [P(B|A) * P(A)] / P(B)`. Jest to fundament **filtrów antyspamowych**, które obliczają prawdopodobieństwo, że mail jest spamem na podstawie zawartych w nim słów, a także systemów rekomendacyjnych i diagnostyki medycznej.

## 9. Testowanie hipotez statystycznych.

Testowanie hipotez to procedura pozwalająca ocenić, czy obserwowany w próbie efekt jest rzeczywisty, czy przypadkowy. Stawiamy **hipotezę zerową (H₀)**, mówiącą o braku efektu, oraz **hipotezę alternatywną (H₁)**, którą chcemy udowodnić. Obliczamy **p-wartość**, czyli prawdopodobieństwo uzyskania naszych wyników, gdyby H₀ była prawdziwa. Jeśli p-wartość jest mniejsza od ustalonego **poziomu istotności α** (zwykle 0.05), odrzucamy H₀. Kluczowe zastosowanie w informatyce to **testy A/B**, gdzie sprawdzamy, czy zmiana na stronie internetowej istotnie poprawiła konwersję.

## 10. Wyznaczanie przedziałów ufności.

Przedział ufności to zakres wartości, który z określonym prawdopodobieństwem (np. 95%) pokrywa prawdziwą, nieznaną wartość parametru w populacji (np. średnią). Zamiast podawać jeden punktowy szacunek, podajemy przedział, co lepiej oddaje niepewność pomiaru. Jego szerokość zależy od poziomu ufności, zmienności w danych i, co najważniejsze, od wielkości próby – im większa próba, tym węższy i bardziej precyzyjny przedział. W informatyce stosuje się je np. w testach A/B, aby oszacować przedział, w jakim zawiera się rzeczywista różnica w konwersji między wersjami.

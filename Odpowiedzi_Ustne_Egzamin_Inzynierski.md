# Odpowiedzi ustne na egzamin inżynierski
## Wydział Informatyki - Wersja zwięzła

> **Format:** Odpowiedzi przygotowane w formie zwięzłej, konkretnej i "to the point" - idealne do szybkiej powtórki przed egzaminem ustnym.

---

## Spis treści

### MATEMATYKA (1-10)
1. [Ekstrema funkcji i gradient, zastosowania w informatyce](#1-ekstrema-funkcji-i-gradient-zastosowania-w-informatyce)
2. [Wielomian i szereg Taylora funkcji rzeczywistej](#2-wielomian-i-szereg-taylora-funkcji-rzeczywistej)
3. [Układy równań liniowych: różne metody rozwiązywania, liczba rozwiązań](#3-układy-równań-liniowych-różne-metody-rozwiązywania-liczba-rozwiązań)
4. [Wartości własne macierzy i ich zastosowanie w informatyce](#4-wartości-własne-macierzy-i-ich-zastosowanie-w-informatyce)
5. [Grafy i ich typy, metody reprezentacji grafów](#5-grafy-i-ich-typy-metody-reprezentacji-grafów)
6. [Relacje binarne, własności i metody reprezentacji](#6-relacje-binarne-własności-i-metody-reprezentacji)
7. [Zasada indukcji matematycznej](#7-zasada-indukcji-matematycznej)
8. [Twierdzenie Bayesa](#8-twierdzenie-bayesa)
9. [Testowanie hipotez statystycznych](#9-testowanie-hipotez-statystycznych)
10. [Wyznaczanie przedziałów ufności](#10-wyznaczanie-przedziałów-ufności)

### BAZY DANYCH (11-15)
11. [Podstawowe cechy relacyjnych baz danych](#11-podstawowe-cechy-relacyjnych-baz-danych)
12. [Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych](#12-podstawowe-elementy-i-znaczenie-diagramów-związków-encji-oraz-zasady-prawidłowego-projektowania-schematów-bazy-danych)
13. [Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych](#13-mechanizm-współbieżności-pracy-wielu-użytkowników-w-systemie-zarządzania-bazami-danych)
14. [Podstawowe obiekty, konstrukcje i znaczenie języka SQL](#14-podstawowe-obiekty-konstrukcje-i-znaczenie-języka-sql)
15. [Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych](#15-podstawowe-zasady-optymalizacji-zapytań-w-tym-rodzaje-i-znaczenie-indeksów-w-bazie-danych)

### TECHNIKI I ARCHITEKTURA KOMPUTERÓW (16-20)
16. [Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce](#16-model-architekturalny-komputera-wg-von-neumanna-a-model-obliczeniowy-komputera-na-podstawie-maszyny-turinga-i-ich-rola-w-informatyce)
17. [Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów](#17-logika-boolowska-i-jej-zastosowania-w-warstwie-sprzętowej-komputerów)
18. [Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa](#18-zapis-binarny-liczb-całkowitych-zapis-zmiennoprzecinkowy-liczb-rzeczywistych-arytmetyka-komputerowa)
19. [Miary wydajności procesorów, pamięci i systemów obliczeniowych](#19-miary-wydajności-procesorów-pamięci-i-systemów-obliczeniowych)
20. [Podstawowe elementy i znaczenie systemów wbudowanych](#20-podstawowe-elementy-i-znaczenie-systemów-wbudowanych)

### SYSTEMY OPERACYJNE (21-25)
21. [Rola i zadania systemu operacyjnego, podstawowe elementy i rodzaje systemów operacyjnych](#21-rola-i-zadania-systemu-operacyjnego-podstawowe-elementy-i-rodzaje-systemów-operacyjnych)
22. [Pojęcie procesu i wątku, stany procesu/wątku, przełączanie kontekstu, algorytmy szeregowania procesów](#22-pojęcie-procesu-i-wątku-stany-procesuwątku-przełączanie-kontekstu-algorytmy-szeregowania-procesów)
23. [Problem wzajemnego wykluczania i jego rozwiązania, synchronizacja procesów i wątków, problem zakleszczenia](#23-problem-wzajemnego-wykluczania-i-jego-rozwiązania-synchronizacja-procesów-i-wątków-problem-zakleszczenia)
24. [Zarządzanie pamięcią operacyjną, pojęcie pamięci wirtualnej, segmentacja i stronicowanie pamięci](#24-zarządzanie-pamięcią-operacyjną-pojęcie-pamięci-wirtualnej-segmentacja-i-stronicowanie-pamięci)
25. [System plików, organizacja i implementacja, metody dostępu do plików](#25-system-plików-organizacja-i-implementacja-metody-dostępu-do-plików)

### SIECI KOMPUTEROWE (26-30)
26. [Model warstwowy ISO/OSI i TCP/IP, protokoły i ich rola w komunikacji sieciowej](#26-model-warstwowy-isoosi-i-tcpip-protokoły-i-ich-rola-w-komunikacji-sieciowej)
27. [Adresacja w sieciach komputerowych: adresy fizyczne, logiczne i porty, rola i zadania protokołów ARP, DNS, DHCP](#27-adresacja-w-sieciach-komputerowych-adresy-fizyczne-logiczne-i-porty-rola-i-zadania-protokołów-arp-dns-dhcp)
28. [Podstawowe urządzenia sieciowe i ich rola w przesyle danych: koncentrator, przełącznik, router](#28-podstawowe-urządzenia-sieciowe-i-ich-rola-w-przesyle-danych-koncentrator-przełącznik-router)
29. [Rola i zadania wybranych protokołów warstwy aplikacji: HTTP, FTP, SMTP, DNS](#29-rola-i-zadania-wybranych-protokołów-warstwy-aplikacji-http-ftp-smtp-dns)
30. [Podstawowe zagadnienia bezpieczeństwa sieci komputerowych: zagrożenia, metody ochrony, kryptografia](#30-podstawowe-zagadnienia-bezpieczeństwa-sieci-komputerowych-zagrożenia-metody-ochrony-kryptografia)

### ALGORYTMY I PROGRAMOWANIE (31-39)
31. [Cykl życia oprogramowania i jego modele (modele wytwarzania oprogramowania)](#31-cykl-życia-oprogramowania-i-jego-modele-modele-wytwarzania-oprogramowania)
32. [Analiza i projektowanie algorytmów, złożoność obliczeniowa, notacja asymptotyczna](#32-analiza-i-projektowanie-algorytmów-złożoność-obliczeniowa-notacja-asymptotyczna)
33. [Paradygmaty programowania: imperatywny, obiektowy, funkcyjny, deklaratywny](#33-paradygmaty-programowania-imperatywny-obiektowy-funkcyjny-deklaratywny)
34. [Programowanie obiektowe: klasy, obiekty, dziedziczenie, polimorfizm](#34-programowanie-obiektowe-klasy-obiekty-dziedziczenie-polimorfizm)
35. [Podstawowe struktury danych: tablica, lista, stos, kolejka, drzewo, graf](#35-podstawowe-struktury-danych-tablica-lista-stos-kolejka-drzewo-graf)
36. [Algorytmy sortowania: bąbelkowe, przez wstawianie, przez wybór, szybkie, przez scalanie](#36-algorytmy-sortowania-bąbelkowe-przez-wstawianie-przez-wybór-szybkie-przez-scalanie)
37. [Algorytmy wyszukiwania: liniowe, binarne](#37-algorytmy-wyszukiwania-liniowe-binarne)
38. [Algorytmy grafowe: przeszukiwanie wszerz i w głąb, algorytm Dijkstry, algorytmy Kruskala i Prima](#38-algorytmy-grafowe-przeszukiwanie-wszerz-i-w-głąb-algorytm-dijkstry-algorytmy-kruskala-i-prima)
39. [Klasy złożoności P i NP, problemy NP-zupełne](#39-klasy-złożoności-p-i-np-problemy-np-zupełne)

### GRAFIKA I INTERFEJSY (40-41)
40. [Grafika rastrowa i wektorowa, modele barw](#40-grafika-rastrowa-i-wektorowa-modele-barw)
41. [Interfejsy użytkownika, interakcja człowiek-komputer, podstawowe zasady projektowania interfejsów](#41-interfejsy-użytkownika-interakcja-człowiek-komputer-podstawowe-zasady-projektowania-interfejsów)

### INŻYNIERIA OPROGRAMOWANIA (42-48)
42. [Inżynieria wymagań: proces, wymagania funkcjonalne i niefunkcjonalne](#42-inżynieria-wymagań-proces-wymagania-funkcjonalne-i-niefunkcjonalne)
43. [Wzorce projektowe: kreacyjne, strukturalne i behawioralne (pojęcia i przykłady)](#43-wzorce-projektowe-kreacyjne-strukturalne-i-behawioralne-pojęcia-i-przykłady)
44. [Testowanie oprogramowania: poziomy testów, techniki czarno- i białoskrzynkowe](#44-testowanie-oprogramowania-poziomy-testów-techniki-czarno--i-białoskrzynkowe)
45. [Systemy kontroli wersji, Git, GitHub](#45-systemy-kontroli-wersji-git-github)
46. [Konteneryzacja, Docker](#46-konteneryzacja-docker)
47. [Metodyki zwinne (Agile), Scrum, Kanban](#47-metodyki-zwinne-agile-scrum-kanban)
48. [Ciągła integracja i ciągłe dostarczanie (CI/CD), Jenkins, GitHub Actions](#48-ciągła-integracja-i-ciągłe-dostarczanie-cicd-jenkins-github-actions)

### INTERNET I BEZPIECZEŃSTWO (49-52)
49. [Architektura i usługi sieci Internet](#49-architektura-i-usługi-sieci-internet)
50. [Podstawowe pojęcia z zakresu bezpieczeństwa IT: zagrożenie, podatność, ryzyko, polityka bezpieczeństwa](#50-podstawowe-pojęcia-z-zakresu-bezpieczeństwa-it-zagrożenie-podatność-ryzyko-polityka-bezpieczeństwa)
51. [Kryptografia symetryczna i asymetryczna, klucz publiczny i prywatny, podpis cyfrowy](#51-kryptografia-symetryczna-i-asymetryczna-klucz-publiczny-i-prywatny-podpis-cyfrowy)
52. [Złośliwe oprogramowanie i ataki sieciowe](#52-złośliwe-oprogramowanie-i-ataki-sieciowe)

### ETYKA I PRAWO (53-54)
53. [Etyka w informatyce, kodeksy etyczne](#53-etyka-w-informatyce-kodeksy-etyczne)
54. [Prawne aspekty oprogramowania: prawa autorskie, patenty, licencje](#54-prawne-aspekty-oprogramowania-prawa-autorskie-patenty-licencje)

### TECHNOLOGIE ZAAWANSOWANE (55-60)
55. [Chmura obliczeniowa: modele usług (IaaS, PaaS, SaaS) i wdrożenia (prywatna, publiczna, hybrydowa)](#55-chmura-obliczeniowa-modele-usług-iaas-paas-saas-i-wdrożenia-prywatna-publiczna-hybrydowa)
56. [Uczenie maszynowe: uczenie nadzorowane, nienadzorowane i ze wzmocnieniem](#56-uczenie-maszynowe-uczenie-nadzorowane-nienadzorowane-i-ze-wzmocnieniem)
57. [Sztuczne sieci neuronowe, głębokie uczenie (deep learning)](#57-sztuczne-sieci-neuronowe-głębokie-uczenie-deep-learning)
58. [Przetwarzanie języka naturalnego (NLP)](#58-przetwarzanie-języka-naturalnego-nlp)
59. [Systemy rozproszone, Big Data](#59-systemy-rozproszone-big-data)
60. [Internet Rzeczy (Internet of Things - IoT)](#60-internet-rzeczy-internet-of-things---iot)

---

# 1. Ekstrema funkcji i gradient, zastosowania w informatyce

**1. Czym są ekstrema funkcji?**

Ekstrema to wartości minimalne i maksymalne funkcji. Dzielimy je na:
*   **Lokalne:** Największa lub najmniejsza wartość w pewnym otoczeniu punktu.
*   **Globalne:** Największa lub najmniejsza wartość w całej dziedzinie funkcji.

**2. Jak znajdujemy ekstrema?**

Używamy do tego pochodnych:
*   **Warunek konieczny:** Pierwsza pochodna musi być równa zero ($f'(x) = 0$). Punkt, który to spełnia, nazywamy punktem stacjonarnym.
*   **Warunek wystarczający:** Analizujemy drugą pochodną w punkcie stacjonarnym:
    *   Jeśli $f''(x_0) > 0$, mamy **minimum** lokalne.
    *   Jeśli $f''(x_0) < 0$, mamy **maksimum** lokalne.

**3. Czym jest gradient?**

Gradient to uogólnienie pochodnej na funkcje wielu zmiennych. Jest to **wektor**, który składa się z pochodnych cząstkowych funkcji.

Kluczowa własność: **Gradient zawsze wskazuje kierunek najszybszego wzrostu wartości funkcji**, a wektor przeciwny do gradientu ($- \nabla f$) wskazuje kierunek najszybszego spadku.

**4. Główne zastosowanie w informatyce?**

**Uczenie maszynowe**, a konkretnie **optymalizacja modeli** za pomocą algorytmu **metody gradientu prostego (Gradient Descent)**.

*   **Cel:** Znaleźć takie parametry modelu, które minimalizują funkcję błędu (kosztu).
*   **Jak to działa?** Algorytm startuje w losowym punkcie i iteracyjnie przesuwa się "w dół" po powierzchni błędu, podążając za kierunkiem przeciwnym do gradientu, aż dotrze do minimum. Jest to fundament trenowania niemal wszystkich sieci neuronowych.

Inne zastosowania to **grafika komputerowa** (np. wykrywanie krawędzi na obrazach) i **robotyka** (planowanie ścieżki).

---

# 2. Wielomian i szereg Taylora funkcji rzeczywistej

**1. Czym jest wielomian Taylora?**

To wielomian, który służy do **przybliżania (aproksymacji) dowolnej, dostatecznie gładkiej funkcji** w otoczeniu wybranego punktu. Im wyższy stopień wielomianu, tym lepsze przybliżenie funkcji w tym otoczeniu.

**2. Czym jest szereg Taylora?**

To **nieskończone rozszerzenie wielomianu Taylora**. Jeśli funkcja jest analityczna, jej szereg Taylora jest z nią tożsamy, czyli idealnie ją odwzorowuje. Jest to reprezentacja funkcji w postaci nieskończonej sumy potęgowej.

**3. Jaki jest cel stosowania szeregu Taylora?**

Celem jest zastąpienie skomplikowanej funkcji (np. $sin(x)$, $e^x$, $log(x)$) **prostym wielomianem**, na którym znacznie łatwiej jest wykonywać operacje, takie jak obliczanie wartości, różniczkowanie czy całkowanie.

**4. Główne zastosowania w informatyce?**

*   **Obliczanie wartości funkcji transcendentalnych:** Komputery i kalkulatory nie przechowują tabel z wartościami sinusa czy logarytmu. Zamiast tego, gdy potrzebują obliczyć np. $sin(0.1)$, wykorzystują kilka pierwszych wyrazów szeregu Taylora, aby uzyskać przybliżenie z wymaganą dokładnością.
*   **Optymalizacja:** W algorytmach optymalizacyjnych (np. metoda Newtona) szereg Taylora jest używany do lokalnego przybliżania funkcji kwadratową, co pozwala efektywnie znajdować jej ekstrema.
*   **Fizyka i symulacje komputerowe:** Upraszczanie skomplikowanych równań fizycznych do postaci wielomianowej, która jest łatwiejsza do rozwiązania numerycznego.

---

# 3. Układy równań liniowych: różne metody rozwiązywania, liczba rozwiązań

**1. Czym jest układ równań liniowych?**

To zbiór kilku równań liniowych z tym samym zestawem niewiadomych. Celem jest znalezienie wartości niewiadomych, które spełniają wszystkie równania jednocześnie.

**2. Jakie są metody rozwiązywania?**

Dzielimy je na dwie główne grupy:

*   **Metody dokładne (algebraiczne):** Dają precyzyjne rozwiązanie. Są skuteczne dla małych i średnich układów.
    *   **Metoda eliminacji Gaussa:** To fundamentalna i najczęściej stosowana metoda. Polega na przekształceniu macierzy rozszerzonej układu do postaci schodkowej za pomocą operacji elementarnych, co pozwala łatwo wyznaczyć rozwiązania.
    *   **Wzory Cramera:** Wykorzystują wyznaczniki. Metoda jest ważna teoretycznie, ale w praktyce bardzo nieefektywna obliczeniowo dla układów większych niż 3x3.

*   **Metody iteracyjne (przybliżone):** Stosowane dla bardzo dużych układów równań, gdzie metody dokładne są zbyt wolne. Zaczynają od przybliżonego rozwiązania i w kolejnych krokach (iteracjach) zbliżają się do właściwego wyniku.
    *   Przykłady: Metoda Jacobiego, Metoda Gaussa-Seidla.

**3. Jak określić liczbę rozwiązań bez rozwiązywania układu?**

Używamy do tego **Twierdzenia Kroneckera-Capellego**. Porównuje ono rząd macierzy współczynników (A) z rzędem macierzy rozszerzonej (U).

*   **Rząd(A) < Rząd(U):** Układ jest sprzeczny, **brak rozwiązań**.
*   **Rząd(A) = Rząd(U) = n** (gdzie 'n' to liczba niewiadomych): Układ jest oznaczony, ma **dokładnie jedno rozwiązanie**.
*   **Rząd(A) = Rząd(U) < n:** Układ jest nieoznaczony, ma **nieskończenie wiele rozwiązań** zależnych od `n - Rząd(A)` parametrów.

**4. Zastosowania w informatyce?**

Układy równań liniowych są wszechobecne:
*   **Grafika komputerowa:** Obliczanie transformacji geometrycznych, oświetlenia, cieni.
*   **Uczenie maszynowe:** W regresji liniowej do znajdowania parametrów modelu.
*   **Analiza sieci:** Obliczanie przepływów w sieciach komputerowych lub transportowych.
*   **Symulacje inżynierskie:** Metoda elementów skończonych (MES) do analizy naprężeń w konstrukcjach sprowadza się do rozwiązania gigantycznych układów równań liniowych.

---

# 4. Wartości własne macierzy i ich zastosowanie w informatyce

**1. Czym są wartości i wektory własne?**

Macierz reprezentuje przekształcenie liniowe (np. obrót, skalowanie). 

*   **Wektor własny** to taki szczególny, niezerowy wektor, który po tym przekształceniu **nie zmienia swojego kierunku**, a jedynie swoją długość.
*   **Wartość własna** to liczba (skalar), która mówi, **jak bardzo** wektor własny został przeskalowany (wydłużony lub skrócony) podczas tego przekształcenia.

Formalnie, dla macierzy A, wektora x i wartości własnej λ zachodzi równanie: **Ax = λx**.

**2. Jak je obliczamy?**

Rozwiązujemy tzw. **równanie charakterystyczne**: `det(A - λI) = 0`, gdzie 'det' to wyznacznik, A to nasza macierz, λ to szukana wartość własna, a I to macierz jednostkowa. Rozwiązania tego równania dają nam wartości własne.

**3. Jaka jest ich interpretacja?**

Wektory własne wyznaczają **osie lub kierunki**, wzdłuż których przekształcenie działa w najprostszy możliwy sposób – jak czyste skalowanie. Mówią nam o "wewnętrznej strukturze" i "preferowanych kierunkach" danego przekształcenia.

**4. Główne zastosowania w informatyce?**

*   **Analiza głównych składowych (PCA - Principal Component Analysis):** To fundamentalna technika w uczeniu maszynowym i statystyce służąca do **redukcji wymiarowości danych**. Wektory własne macierzy kowariancji danych wskazują kierunki największej wariancji (największego zróżnicowania informacji). PCA pozwala odrzucić mniej istotne wymiary i zachować te najważniejsze, co upraszcza dane i przyspiesza obliczenia.

*   **Algorytm PageRank (Google):** To algorytm, który zrewolucjonizował wyszukiwarki internetowe. Sieć internetową można przedstawić jako gigantyczną macierz. Wektor własny tej macierzy odpowiadający największej wartości własnej określa "ważność" (ranking) każdej strony w sieci. Strona jest tym ważniejsza, im więcej ważnych stron do niej linkuje.

*   **Grafika komputerowa:** Wartości własne są używane do analizy i upraszczania przekształceń geometrycznych oraz w technikach deformacji obiektów ów 3D.

---

# 5. Grafy i ich typy, metody reprezentacji grafów

**1. Czym jest graf?**

Graf to abstrakcyjna struktura matematyczna służąca do modelowania **relacji** między obiektami. Składa się z dwóch zbiorów:
*   **Wierzchołków (V):** Reprezentują obiekty.
*   **Krawędzi (E):** Reprezentują połączenia (relacje) między wierzchołkami.

**2. Jakie są podstawowe typy grafów?**

*   **Graf nieskierowany:** Krawędzie nie mają orientacji (np. relacja "bycia w przyjaźni" na Facebooku – jest obustronna).
*   **Graf skierowany (digraf):** Krawędzie mają określony kierunek (np. relacja "obserwowania" na Twitterze – może być jednostronna).
*   **Graf ważony:** Każda krawędź ma przypisaną wartość (wagę), która może reprezentować np. koszt, odległość, czas (np. mapa drogowa, gdzie wagi to długości dróg).
*   **Graf prosty:** Nie ma pętli (krawędzi z wierzchołka do samego siebie) ani krawędzi wielokrotnych między tymi samymi wierzchołkami.
*   **Drzewo:** Szczególny typ grafu – spójny i acykliczny (nie zawiera cykli).

**3. Jak reprezentujemy grafy w pamięci komputera?**

Istnieją dwie główne metody:

*   **Macierz sąsiedztwa:**
    *   **Jak działa?** Tworzymy macierz kwadratową o wymiarach V x V. Komórka `M[i][j] = 1` oznacza, że istnieje krawędź od wierzchołka `i` do `j`. Dla grafów ważonych wpisujemy wagę krawędzi.
    *   **Zalety:** Szybkie sprawdzanie istnienia krawędzi (czas stały O(1)).
    *   **Wady:** Duże zużycie pamięci (O(V²)), nawet dla grafów rzadkich (z małą liczbą krawędzi).

*   **Lista sąsiedztwa:**
    *   **Jak działa?** Dla każdego wierzchołka tworzymy listę wierzchołków, z którymi jest on połączony.
    *   **Zalety:** Efektywna pamięciowo dla grafów rzadkich (zużycie pamięci O(V+E)).
    *   **Wady:** Wolniejsze sprawdzanie istnienia krawędzi (w najgorszym przypadku O(V)).

**4. Wybór reprezentacji:**

*   Dla **grafów gęstych** (dużo krawędzi) lepsza jest **macierz sąsiedztwa**.
*   Dla **grafów rzadkich** (mało krawędzi), które są najczęstsze w praktyce, zdecydowanie lepsza jest **lista sąsiedztwa**.

---

# 6. Relacje binarne, własności i metody reprezentacji

**1. Czym jest relacja binarna?**

Relacja binarna (dwuargumentowa) na zbiorze A to dowolny podzbiór iloczynu kartezjańskiego A x A. Mówiąc prościej, jest to zbiór par uporządkowanych (a, b), gdzie a i b należą do zbioru A. Jeśli para (a, b) należy do relacji, mówimy, że "a jest w relacji z b".

**2. Jakie są kluczowe własności relacji?**

*   **Zwrotność:** Każdy element jest w relacji sam z sobą. (dla każdego a, (a, a) należy do relacji). Przykład: relacja "mniejszy lub równy" (≤).
*   **Przeciwzwrotność:** Żaden element nie jest w relacji sam z sobą. Przykład: relacja "mniejszy" (<).
*   **Symetryczność:** Jeśli a jest w relacji z b, to b jest w relacji z a. Przykład: relacja "bycia rodzeństwem".
*   **Antysymetryczność:** Jeśli a jest w relacji z b i b jest w relacji z a, to a musi być równe b. Przykład: relacja "mniejszy lub równy" (≤).
*   **Przechodniość:** Jeśli a jest w relacji z b i b jest w relacji z c, to a jest w relacji z c. Przykład: relacja "bycia przodkiem".

**3. Czym jest relacja równoważności?**

To relacja, która jest jednocześnie **zwrotna, symetryczna i przechodnia**. Dzieli ona zbiór na rozłączne podzbiory, zwane klasami abstrakcji. Przykład: relacja "mieć ten sam kolor".

**4. Czym jest relacja częściowego porządku?**

To relacja, która jest jednocześnie **zwrotna, antysymetryczna i przechodnia**. Porządkuje ona elementy zbioru, ale niekoniecznie wszystkie pary da się porównać. Przykład: relacja "bycia podzbiorem" (⊆).

**5. Jak reprezentujemy relacje?**

*   **Macierz sąsiedztwa:** Podobnie jak w grafach, tworzymy macierz, gdzie 1 w komórce (i, j) oznacza, że element i jest w relacji z j.
*   **Graf:** Relację można przedstawić jako graf skierowany, gdzie wierzchołki to elementy zbioru, a krawędzie reprezentują pary należące do relacji.

---

# 7. Zasada indukcji matematycznej

**1. Czym jest zasada indukcji matematycznej?**

To fundamentalna metoda **dowodzenia twierdzeń** dotyczących liczb naturalnych. Pozwala ona udowodnić, że pewna własność jest prawdziwa dla **wszystkich** liczb naturalnych (lub od pewnego progu w górę).

**2. Na czym polega ta metoda?**

Dowód indukcyjny składa się z dwóch obowiązkowych kroków:

*   **Krok bazowy (Baza indukcji):**
    *   Sprawdzamy, czy twierdzenie jest prawdziwe dla **pierwszej, najmniejszej liczby naturalnej**, dla której ma być ono prawdziwe (zazwyczaj dla n=0 lub n=1).

*   **Krok indukcyjny:**
    1.  **Założenie indukcyjne:** Zakładamy, że twierdzenie jest prawdziwe dla pewnej **dowolnej, ale ustalonej** liczby naturalnej `k`.
    2.  **Teza indukcyjna:** Korzystając z tego założenia, musimy udowodnić, że twierdzenie jest również prawdziwe dla **następnej liczby**, czyli `k+1`.

**3. Jaka jest intuicja za tą zasadą?**

Można to porównać do **efektu domina**. 
*   Krok bazowy to **przewrócenie pierwszej kostki**.
*   Krok indukcyjny to dowód, że **jeśli jakakolwiek kostka (k) się przewróci, to pociągnie za sobą następną (k+1)**.

Jeśli oba te warunki są spełnione, to mamy pewność, że wszystkie kostki domina się przewrócą. Analogicznie, jeśli spełnione są oba kroki indukcji, twierdzenie jest prawdziwe dla wszystkich liczb naturalnych.

**4. Główne zastosowania w informatyce?**

*   **Analiza poprawności algorytmów:** Indukcja jest kluczowym narzędziem do dowodzenia, że algorytmy, zwłaszcza **rekurencyjne**, działają poprawnie dla każdego możliwego wejścia. Dowodzimy, że jeśli algorytm działa dla problemu o rozmiarze `k`, to zadziała też dla problemu o rozmiarze `k+1`.
*   **Analiza złożoności obliczeniowej:** Służy do rozwiązywania równań rekurencyjnych, które opisują czas działania algorytmów typu "dziel i zwyciężaj" (np. sortowanie przez scalanie).
*   **Dowodzenie własności struktur danych:** Np. dowodzenie, że drzewo binarne o `n` węzłach ma `n-1` krawędzi.

---

# 8. Twierdzenie Bayesa

**1. Czym jest twierdzenie Bayesa?**

To fundamentalne twierdzenie rachunku prawdopodobieństwa, które pozwala na **aktualizację naszej wiedzy (prawdopodobieństwa) o pewnym zdarzeniu w świetle nowych dowodów (informacji)**.

**2. Co ono opisuje?**

Twierdzenie Bayesa łączy **prawdopodobieństwo warunkowe** zdarzenia A pod warunkiem B z prawdopodobieństwem warunkowym zdarzenia B pod warunkiem A. Wzór ma postać:

`P(A|B) = [P(B|A) * P(A)] / P(B)`

*   `P(A|B)` - **prawdopodobieństwo a posteriori**: to, co chcemy obliczyć. Prawdopodobieństwo, że zaszło zdarzenie A, jeśli wiemy, że zaszło zdarzenie B.
*   `P(B|A)` - **wiarygodność (likelihood)**: prawdopodobieństwo zaobserwowania dowodu B, jeśli założymy, że zdarzenie A jest prawdziwe.
*   `P(A)` - **prawdopodobieństwo a priori**: nasza początkowa wiedza o prawdopodobieństwie zdarzenia A, zanim uzyskaliśmy dowód B.
*   `P(B)` - **prawdopodobieństwo brzegowe**: całkowite prawdopodobieństwo zaobserwowania dowodu B.

**3. Jaka jest intuicja?**

Twierdzenie Bayesa formalizuje proces uczenia się na podstawie doświadczeń. Pozwala nam odpowiedzieć na pytanie: "Jak bardzo powinienem zmienić swoje przekonanie o czymś, gdy otrzymam nową informację?".

**4. Główne zastosowania w informatyce?**

*   **Filtry antyspamowe:** To klasyczny przykład. 
    *   **A priori:** Jakie jest ogólne prawdopodobieństwo, że dowolny e-mail to spam?
    *   **Dowód:** E-mail zawiera słowo "wygrałeś".
    *   **Twierdzenie Bayesa pozwala obliczyć:** Jakie jest prawdopodobieństwo, że ten e-mail to spam, SKORO zawiera słowo "wygrałeś"? Filtry uczą się na podstawie tysięcy przykładów, jakie słowa najczęściej występują w spamie.

*   **Diagnostyka medyczna:** Obliczanie prawdopodobieństwa, że pacjent ma daną chorobę, na podstawie wyników testu (który nie jest w 100% pewny).

*   **Uczenie maszynowe:** Twierdzenie Bayesa jest podstawą całej gałęzi uczenia maszynowego zwanej **statystyką bayesowską** oraz algorytmów takich jak **Naiwny Klasyfikator Bayesowski**.

*   **Rozpoznawanie mowy i NLP:** Modele językowe używają podejścia bayesowskiego do przewidywania najbardziej prawdopodobnego słowa lub zdania.

---

# 9. Testowanie hipotez statystycznych

**1. Czym jest testowanie hipotez?**

To formalna procedura statystyczna, która pozwala na podstawie **próby losowej** podjąć decyzję o **prawdziwości pewnego założenia dotyczącego całej populacji**.

**2. Jakie są kluczowe pojęcia?**

*   **Hipoteza zerowa (H0):** To standardowe, domyślne założenie, które próbujemy **obalić**. Zazwyczaj mówi o "braku efektu" lub "braku różnicy" (np. "średni wzrost mężczyzn i kobiet jest taki sam").
*   **Hipoteza alternatywna (H1):** To zaprzeczenie hipotezy zerowej. Mówi o istnieniu efektu lub różnicy (np. "średni wzrost mężczyzn i kobiet jest różny").
*   **Poziom istotności (α):** Małe prawdopodobieństwo (zwykle 0.05 lub 0.01), które ustalamy przed testem. Jest to próg naszej tolerancji na błąd – maksymalne ryzyko odrzucenia prawdziwej hipotezy zerowej, na jakie się godzimy.
*   **Wartość p (p-value):** To **wynik testu**. Jest to prawdopodobieństwo uzyskania obserwowanej w próbie zależności (lub jeszcze silniejszej), przy założeniu, że hipoteza zerowa jest prawdziwa.

**3. Jak przebiega proces testowania?**

1.  Sformułuj hipotezę zerową (H0) i alternatywną (H1).
2.  Wybierz poziom istotności (α).
3.  Zbierz dane (próbę losową).
4.  Oblicz statystykę testową i odpowiadającą jej **wartość p**.
5.  Podejmij decyzję:
    *   Jeśli **p ≤ α**: Wynik jest **istotny statystycznie**. Odrzucamy hipotezę zerową na rzecz alternatywnej. Mamy podstawy sądzić, że obserwowany efekt nie jest dziełem przypadku.
    *   Jeśli **p > α**: Wynik jest **nieistotny statystycznie**. Nie ma podstaw do odrzucenia hipotezy zerowej.

**4. Główne zastosowania w informatyce?**

*   **Testy A/B:** To kluczowe narzędzie w rozwoju oprogramowania i marketingu. Chcemy sprawdzić, czy nowa wersja strony internetowej (np. z innym kolorem przycisku) jest lepsza od starej. 
    *   H0: "Konwersja na obu wersjach strony jest taka sama".
    *   H1: "Konwersja jest różna".
    *   Testowanie hipotez pozwala stwierdzić, czy zaobserwowana różnica w konwersji jest rzeczywistym efektem zmiany, czy tylko przypadkową fluktuacją.

*   **Uczenie maszynowe:** Do oceny, czy różnica w skuteczności dwóch modeli jest statystycznie istotna, czy też może wynikać z losowości w danych testowych.

*   **Analiza danych:** Do weryfikacji, czy istnieje statystycznie istotna korelacja między dwiema zmiennymi w zbiorze danych.

---

# 10. Wyznaczanie przedziałów ufności

**1. Czym jest przedział ufności?**

Przedział ufności to **zakres wartości**, który z określonym, wysokim prawdopodobieństwem (zwanym **poziomem ufności**) **zawiera prawdziwą, nieznaną wartość parametru w całej populacji**.

**2. Jaka jest różnica między estymacją punktową a przedziałową?**

*   **Estymacja punktowa:** Obliczamy na podstawie próby **jedną konkretną wartość**, która ma być naszym najlepszym "strzałem" co do wartości parametru w populacji (np. średnia z próby jako estymator średniej w populacji).
*   **Estymacja przedziałowa (przedział ufności):** Zamiast jednej liczby, podajemy **przedział**, który z pewnym prawdopodobieństwem pokrywa prawdziwą wartość. Jest to bardziej informatywne, bo uwzględnia niepewność wynikającą z losowości próby.

**3. Jak interpretować przedział ufności?**

Jeśli wyznaczamy 95% przedział ufności, to **nie oznacza to**, że istnieje 95% szans, że prawdziwa wartość parametru leży w *tym konkretnym* przedziale.

Prawidłowa interpretacja jest następująca: "Gdybyśmy wielokrotnie powtarzali proces losowania próby i dla każdej z nich budowali 95% przedział ufności, to **95% tak skonstruowanych przedziałów zawierałoby prawdziwą wartość parametru populacji**."

**4. Od czego zależy szerokość przedziału ufności?**

*   **Poziom ufności:** Im wyższy poziom ufności (np. 99% zamiast 95%), tym **szerszy** przedział (potrzebujemy szerszej "siatki", by z większą pewnością złapać prawdziwą wartość).
*   **Wielkość próby:** Im większa próba, tym **węższy** przedział (większa próba daje nam więcej informacji i zmniejsza niepewność).
*   **Zmienność w populacji:** Im większe zróżnicowanie (odchylenie standardowe) w populacji, tym **szerszy** przedział.

**5. Zastosowania w informatyce?**

*   **Analiza wyników testów A/B:** Zamiast mówić, że nowa wersja strony zwiększyła konwersję o 2%, podajemy przedział ufności, np. "z 95% ufnością, zmiana konwersji leży w przedziale od 0.5% do 3.5%". Daje to znacznie pełniejszy obraz niepewności pomiaru.
*   **Uczenie maszynowe:** Do oceny niepewności predykcji modeli. Zamiast prognozować, że sprzedaż wyniesie 1000 sztuk, model może podać 95% przedział ufności [950, 1050].
*   **Pomiary wydajności:** Do prezentacji wyników benchmarków. Zamiast podawać, że średni czas odpowiedzi serwera to 50ms, podajemy przedział ufności, np. [48ms, 52ms].

---

# 11. Podstawowe cechy relacyjnych baz danych

**1. Czym jest relacyjna baza danych?**

To baza danych oparta na **modelu relacyjnym**, w którym dane są zorganizowane w **tabelach** (zwanych relacjami). Tabele składają się z wierszy (rekordów, zwanych krotkami) i kolumn (pól, zwanych atrybutami).

**2. Jakie są jej kluczowe cechy?**

*   **Struktura oparta na tabelach:** Wszystkie dane przechowywane są w prostych, dwuwymiarowych tabelach.
*   **Integralność danych:** System wymusza spójność danych za pomocą więzów integralności:
    *   **Klucz podstawowy (Primary Key):** Unikalnie identyfikuje każdy wiersz w tabeli. Nie może zawierać wartości NULL.
    *   **Klucz obcy (Foreign Key):** Kolumna (lub zestaw kolumn), która łączy dwie tabele. Wartości w kluczu obcym muszą odpowiadać wartościom klucza podstawowego w innej tabeli, co zapewnia spójność referencyjną.
*   **Język SQL:** Standardowy język zapytań (Structured Query Language) służący do definiowania, manipulowania i odpytywania danych.
*   **Transakcyjność i właściwości ACID:** Relacyjne bazy danych gwarantują niezawodność operacji dzięki transakcjom, które spełniają właściwości ACID:
    *   **Atomicity (Atomowość):** Transakcja jest niepodzielna – albo wszystkie jej operacje zostaną wykonane poprawnie, albo żadna.
    *   **Consistency (Spójność):** Transakcja przeprowadza bazę danych z jednego spójnego stanu w drugi.
    *   **Isolation (Izolacja):** Transakcje wykonywane współbieżnie nie wpływają na siebie nawzajem. Z perspektywy jednej transakcji, inne wyglądają tak, jakby wykonywały się szeregowo.
    *   **Durability (Trwałość):** Po zatwierdzeniu transakcji, jej wyniki są trwale zapisane i odporne na awarie.

**3. Przykłady systemów:**

PostgreSQL, MySQL, Oracle Database, Microsoft SQL Server.

---

# 12. Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych

**1. Czym jest diagram związków encji (ERD)?**

To **graficzne narzędzie** do modelowania danych na poziomie konceptualnym. Służy do wizualizacji struktury bazy danych przed jej fizycznym utworzeniem. Pokazuje, jakie **obiekty (encje)** będą w bazie i jakie **związki** między nimi zachodzą.

**2. Jakie są jego podstawowe elementy?**

*   **Encja:** Reprezentuje obiekt ze świata rzeczywistego, o którym chcemy przechowywać informacje (np. `Student`, `Kurs`). Na diagramie przedstawiana jako **prostokąt**.
*   **Atrybut:** Właściwość lub cecha opisująca encję (np. dla studenta: `imie`, `nazwisko`). Na diagramie jako **elipsa**.
*   **Związek (Relacja):** Opisuje powiązanie między dwiema lub więcej encjami (np. student `zapisuje się na` kurs). Na diagramie jako **romb**.
*   **Liczność (Krotność):** Określa, ile instancji jednej encji może być powiązanych z instancjami drugiej. Najczęstsze typy to:
    *   **Jeden do jednego (1:1):** (np. Mąż - Żona)
    *   **Jeden do wielu (1:N):** (np. Wykładowca - Studenci)
    *   **Wiele do wielu (N:M):** (np. Student - Kurs)

**3. Jakie są zasady prawidłowego projektowania schematów?**

Celem jest stworzenie struktury, która jest wydajna, elastyczna i zapobiega anomaliom danych. Kluczową techniką jest **normalizacja**.

*   **Normalizacja:** Proces organizowania kolumn i tabel w bazie danych w celu **zminimalizowania redundancji (powtarzania się) danych**. Odbywa się poprzez rozbijanie dużych tabel na mniejsze, dobrze ustrukturyzowane tabele.
*   **Postacie normalne:**
    *   **Pierwsza postać normalna (1NF):** Każda komórka tabeli musi zawierać pojedynczą, niepodzielną (atomową) wartość. Tabela nie może zawierać grup powtarzających się.
    *   **Druga postać normalna (2NF):** Musi być w 1NF. Dodatkowo, wszystkie atrybuty niekluczowe muszą być w pełni zależne od **całego** klucza głównego (dotyczy kluczy złożonych).
    *   **Trzecia postać normalna (3NF):** Musi być w 2NF. Dodatkowo, wszystkie atrybuty muszą zależeć **tylko** od klucza głównego, a nie od innych atrybutów niekluczowych (brak zależności przechodnich).

**Zasada ogólna:** Każdy atrybut w tabeli powinien opisywać **klucz, cały klucz i tylko klucz**.

---

# 13. Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych

**1. Na czym polega problem współbieżności?**

Problem pojawia się, gdy **wielu użytkowników (transakcji) próbuje w tym samym czasie odczytywać i modyfikować te same dane**. Bez odpowiednich mechanizmów kontroli, może to prowadzić do utraty danych i niespójności bazy. Nazywamy to **anomaliami współbieżności**.

**2. Jakie są typowe anomalie?**

*   **Utracona modyfikacja (Lost Update):** Dwie transakcje odczytują tę samą wartość, obie ją modyfikują, ale ostatni zapis nadpisuje i unieważnia zapis pierwszej transakcji.
*   **Brudny odczyt (Dirty Read):** Jedna transakcja odczytuje dane zmodyfikowane przez drugą transakcję, która **jeszcze się nie zakończyła (nie została zatwierdzona)**. Jeśli ta druga transakcja zostanie wycofana, pierwsza będzie operować na nieaktualnych, "brudnych" danych.
*   **Niepowtarzalny odczyt (Non-repeatable Read):** Transakcja dwukrotnie odczytuje ten sam rekord i za każdym razem otrzymuje inną wartość, ponieważ w międzyczasie inna transakcja zdążyła go zmodyfikować i zatwierdzić.

**3. Jak systemy bazodanowe radzą sobie z tym problemem?**

Kluczowym mechanizmem jest **blokowanie (locking)**.

*   **Jak działa?** Gdy transakcja chce zmodyfikować dane, zakłada na nie **blokadę (zamek)**. Inne transakcje, które chcą uzyskać dostęp do tych samych danych, muszą poczekać, aż blokada zostanie zwolniona (co następuje po zakończeniu pierwszej transakcji).
*   **Rodzaje blokad:**
    *   **Blokada na zapis (wyłączna, exclusive lock):** Zakładana podczas operacji zapisu (UPDATE, DELETE). Tylko jedna transakcja może ją trzymać. Blokuje inne blokady na zapis i odczyt.
    *   **Blokada na odczyt (dzielona, shared lock):** Zakładana podczas operacji odczytu (SELECT). Wiele transakcji może jednocześnie trzymać blokadę na odczyt dla tych samych danych. Blokuje tylko blokady na zapis.

**4. Czym są poziomy izolacji transakcji?**

Systemy bazodanowe pozwalają na zdefiniowanie, jak bardzo transakcje mają być od siebie odizolowane. Jest to kompromis między spójnością danych a wydajnością systemu. Standard SQL definiuje cztery poziomy:

1.  **Read Uncommitted:** Najniższy poziom, pozwala na brudne odczyty. Najszybszy, ale najmniej bezpieczny.
2.  **Read Committed:** Domyślny w wielu bazach. Zapobiega brudnym odczytom, ale wciąż możliwe są niepowtarzalne odczyty.
3.  **Repeatable Read:** Zapobiega brudnym i niepowtarzalnym odczytom.
4.  **Serializable:** Najwyższy, najbardziej restrykcyjny poziom. Gwarantuje pełną izolację, tak jakby transakcje wykonywały się jedna po drugiej. Eliminuje wszystkie anomalie, ale jest najwolniejszy.

---

# 14. Podstawowe obiekty, konstrukcje i znaczenie języka SQL

**1. Czym jest SQL?**

SQL (Structured Query Language) to **deklaratywny język** służący do zarządzania i przetwarzania danych w relacyjnych bazach danych. Mówimy w nim **co** chcemy uzyskać, a nie **jak** system ma to zrobić.

**2. Jakie są podjęzyki SQL?**

SQL dzieli się na kilka grup poleceń:

*   **DDL (Data Definition Language):** Służy do **definiowania struktury** bazy danych.
    *   `CREATE`: Tworzenie obiektów (np. `CREATE TABLE`, `CREATE VIEW`).
    *   `ALTER`: Modyfikacja obiektów (np. `ALTER TABLE`).
    *   `DROP`: Usuwanie obiektów (np. `DROP TABLE`).

*   **DML (Data Manipulation Language):** Służy do **manipulowania danymi** w tabelach.
    *   `SELECT`: Pobieranie danych.
    *   `INSERT`: Wstawianie nowych danych.
    *   `UPDATE`: Aktualizacja istniejących danych.
    *   `DELETE`: Usuwanie danych.

*   **DCL (Data Control Language):** Służy do **zarządzania uprawnieniami** użytkowników.
    *   `GRANT`: Nadawanie uprawnień.
    *   `REVOKE`: Odbieranie uprawnień.

*   **TCL (Transaction Control Language):** Służy do **zarządzania transakcjami**.
    *   `COMMIT`: Zatwierdzenie transakcji.
    *   `ROLLBACK`: Wycofanie transakcji.

**3. Jakie są podstawowe obiekty w bazie danych?**

*   **Tabela (TABLE):** Podstawowy obiekt przechowujący dane w formie wierszy i kolumn.
*   **Widok (VIEW):** Wirtualna tabela, która jest wynikiem zapytania `SELECT`. Nie przechowuje fizycznie danych, ale upraszcza skomplikowane zapytania i pozwala na ograniczenie dostępu do danych.
*   **Indeks (INDEX):** Struktura danych, która przyspiesza operacje wyszukiwania w tabeli. Działa jak skorowidz w książce.
*   **Procedura składowana (STORED PROCEDURE):** Zbiór poleceń SQL zapisany w bazie danych pod jedną nazwą, który można wielokrotnie wywoływać.

**4. Jakie są kluczowe konstrukcje w zapytaniu `SELECT`?**

*   `SELECT [kolumny]`: Wybiera kolumny, które chcemy zobaczyć.
*   `FROM [tabela]`: Określa tabelę, z której pobieramy dane.
*   `WHERE [warunek]`: Filtruje wiersze, zwracając tylko te, które spełniają warunek.
*   `GROUP BY [kolumna]`: Grupuje wiersze na podstawie wartości w kolumnie, co pozwala na użycie funkcji agregujących (np. `COUNT`, `SUM`, `AVG`).
*   `HAVING [warunek]`: Filtruje grupy utworzone przez `GROUP BY`.
*   `ORDER BY [kolumna]`: Sortuje wyniki.
*   `JOIN`: Służy do łączenia wierszy z dwóch lub więcej tabel na podstawie powiązanych kolumn (np. `INNER JOIN`, `LEFT JOIN`).

---

# 15. Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych

**1. Na czym polega optymalizacja zapytań?**

To proces modyfikacji zapytania SQL lub struktury bazy danych w celu **jak najszybszego uzyskania wyniku** przy jak najmniejszym zużyciu zasobów (CPU, I/O).

**2. Kto odpowiada za optymalizację?**

Każdy system bazodanowy ma wbudowany **optymalizator zapytań**. Jest to komponent, który analizuje zapytanie SQL i tworzy **plan wykonania** – czyli sekwencję kroków, jakie baza musi podjąć, aby zwrócić wynik. Optymalizator stara się wybrać najefektywniejszy plan, ale możemy mu w tym pomóc.

**3. Jakie jest najważniejsze narzędzie optymalizacji?**

**Indeksy.**

*   **Czym jest indeks?** To specjalna struktura danych (najczęściej B-drzewo), która przechowuje posortowane wartości z jednej lub więcej kolumn tabeli oraz wskaźniki do odpowiadających im wierszy. Działa jak **skorowidz w książce** – zamiast przeglądać całą książkę (tabelę), by znaleźć temat, zaglądamy do skorowidza i od razu przechodzimy do właściwej strony (wiersza).

*   **Kiedy stosować indeksy?**
    *   Na kolumnach, które są **często używane w klauzuli `WHERE`** do filtrowania danych.
    *   Na kolumnach używanych do **łączenia tabel (`JOIN`)**.
    *   Na kolumnach, po których często **sortujemy dane (`ORDER BY`)**.

*   **Rodzaje indeksów:**
    *   **Klastrowany:** Fizycznie porządkuje wiersze w tabeli na dysku zgodnie z kolejnością indeksu. Może być **tylko jeden** na tabelę (zazwyczaj zakładany na kluczu głównym).
    *   **Nieklastrowany:** Tworzy osobną strukturę, która zawiera wartości z indeksowanych kolumn i wskaźniki do oryginalnych wierszy. Może być **wiele** takich indeksów na tabelę.

**4. Jakie są inne zasady optymalizacji?**

*   **Unikaj `SELECT *`:** Zawsze wybieraj tylko te kolumny, których naprawdę potrzebujesz. Zmniejsza to ilość przesyłanych danych.
*   **Używaj `WHERE` do filtrowania jak najwcześniej:** Im mniej wierszy trzeba przetwarzać w kolejnych krokach (np. grupowanie, sortowanie), tym lepiej.
*   **Uważaj na funkcje w klauzuli `WHERE`:** Użycie funkcji na indeksowanej kolumnie (np. `WHERE YEAR(data_zamowienia) = 2023`) często **uniemożliwia użycie indeksu**. Lepiej przekształcić warunek: `WHERE data_zamowienia >= '2023-01-01' AND data_zamowienia < '2024-01-01'`.
*   **Zrozum plan wykonania:** Używaj polecenia `EXPLAIN` (lub `EXPLAIN ANALYZE`), aby zobaczyć, jak baza danych zamierza wykonać Twoje zapytanie. Szukaj operacji typu "Full Table Scan", które wskazują na brak użycia indeksu i są potencjalnym wąskim gardłem.

---

# 16. Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce

**1. Czym jest maszyna Turinga?**

To **abstrakcyjny model matematyczny** stworzony przez Alana Turinga, który formalizuje pojęcie **algorytmu**. Składa się z nieskończonej taśmy, głowicy oraz tablicy stanów. Maszyna Turinga potrafi wykonywać proste operacje (odczyt, zapis, przesunięcie głowicy), ale mimo to jest w stanie obliczyć wszystko, co jest obliczalne. Jest to **teoretyczny model obliczeń**, a nie projekt komputera.

**2. Czym jest architektura von Neumanna?**

To **praktyczny model architektury komputera**, który jest podstawą budowy niemal wszystkich współczesnych komputerów. Jej kluczową cechą jest koncepcja **wspólnej pamięci dla danych i instrukcji**.

**3. Jakie są główne komponenty architektury von Neumanna?**

*   **Jednostka centralna (CPU):** Mózg komputera, składający się z:
    *   **Jednostki arytmetyczno-logicznej (ALU):** Wykonuje operacje matematyczne i logiczne.
    *   **Jednostki sterującej (CU):** Kieruje przepływem danych i instrukcji, interpretuje polecenia.
*   **Pamięć operacyjna (RAM):** Przechowuje zarówno **program (instrukcje)**, jak i **dane**, na których ten program operuje.
*   **Urządzenia wejścia/wyjścia (I/O):** Umożliwiają komunikację z użytkownikiem i innymi urządzeniami (klawiatura, monitor, dysk twardy).
*   **Magistrala (Bus):** System szyn komunikacyjnych łączący wszystkie powyższe komponenty.

**4. Jaka jest relacja między tymi dwoma modelami?**

*   **Maszyna Turinga** odpowiada na pytanie: **"Co teoretycznie można obliczyć?"**. Definiuje granice obliczalności.
*   **Architektura von Neumanna** odpowiada na pytanie: **"Jak praktycznie zbudować maszynę, która będzie to obliczać?"**. Jest to fizyczna realizacja uniwersalnej maszyny Turinga.

**5. Czym jest "wąskie gardło von Neumanna"?**

To fundamentalne ograniczenie tej architektury. Procesor jest znacznie szybszy niż pamięć. Oznacza to, że CPU często musi **czekać** na dane i instrukcje pobierane z pamięci przez magistralę. Ta magistrala staje się "wąskim gardłem", które ogranicza ogólną wydajność systemu. Problem ten łagodzi się poprzez stosowanie szybkich pamięci podręcznych (cache) umieszczonych blisko procesora.

---

# 17. Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów

**1. Czym jest logika boolowska (algebra Boole'a)?**

To dział matematyki i logiki zajmujący się operacjami na **wartościach logicznych**: **prawda (1)** i **fałsz (0)**. Jest to fundament cyfrowego świata.

**2. Jakie są podstawowe operacje (funktory) logiczne?**

*   **Koniunkcja (AND, I):** Zwraca prawdę (1) tylko wtedy, gdy **oba** argumenty są prawdziwe.
*   **Alternatywa (OR, LUB):** Zwraca prawdę (1), gdy **co najmniej jeden** z argumentów jest prawdziwy.
*   **Negacja (NOT, NIE):** Zmienia wartość logiczną na przeciwną (1 na 0, 0 na 1).

Z tych trzech podstawowych operacji można zbudować wszystkie inne, np. NAND (negacja AND), NOR (negacja OR), XOR (alternatywa wykluczająca).

**3. Jak logika Boole'a jest realizowana w sprzęcie?**

Operacje logiczne są fizycznie realizowane za pomocą **bramek logicznych**. Bramki logiczne to podstawowe układy elektroniczne (zbudowane z tranzystorów), które przyjmują na wejściu sygnały elektryczne (reprezentujące 0 i 1) i na podstawie określonej funkcji logicznej generują sygnał wyjściowy.

*   Wysoki poziom napięcia reprezentuje **1** (prawdę).
*   Niski poziom napięcia reprezentuje **0** (fałsz).

**4. Jakie jest znaczenie logiki Boole'a w architekturze komputerów?**

Jest absolutnie fundamentalne. Z prostych bramek logicznych, jak z klocków LEGO, buduje się coraz bardziej złożone układy cyfrowe:

*   **Sumatory (Adders):** Układy do dodawania liczb binarnych.
*   **Przerzutniki (Flip-flops):** Układy zdolne do przechowywania jednego bitu informacji, stanowiące podstawę pamięci statycznej (SRAM).
*   **Rejestry:** Zbiory przerzutników do przechowywania słów maszynowych.
*   **Multipleksery i demultipleksery:** Układy do wybierania i przesyłania sygnałów.

Z tych z kolei buduje się całe komponenty komputera, takie jak **jednostka arytmetyczno-logiczna (ALU)**, **pamięć podręczna (cache)** i **jednostka sterująca (CU)**. Ostatecznie, cały procesor jest gigantycznym, złożonym układem bramek logicznych realizujących operacje zdefiniowane przez algebrę Boole'a.

---

# 18. Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa

**1. Jak komputery zapisują liczby całkowite?**

Używają **systemu binarnego (dwójkowego)**. Najpopularniejszym standardem jest **kod uzupełnień do dwóch (U2)**.

*   **Liczby dodatnie:** Zapisywane standardowo, np. `5` to `0101`.
*   **Liczby ujemne:** Aby zapisać np. `-5`, bierzemy zapis `5` (`0101`), negujemy wszystkie bity (`1010`) i dodajemy 1 (`1011`).
*   **Zaleta:** Arytmetyka (dodawanie, odejmowanie) jest taka sama dla liczb dodatnich i ujemnych. Odejmowanie `A - B` to po prostu dodawanie `A + (-B)`.

**2. Jak komputery zapisują liczby rzeczywiste?**

Używają **zapisu zmiennoprzecinkowego**, zdefiniowanego w standardzie **IEEE 754**. Liczba jest reprezentowana w postaci "naukowej":

`liczba = znak * mantysa * 2 ^ cecha`

Bitowy zapis liczby jest podzielony na trzy pola:
*   **Znak (S):** 1 bit (0 dla dodatniej, 1 dla ujemnej).
*   **Cecha (wykładnik, E):** Określa rząd wielkości liczby (potęgę dwójki). Jest zapisana z przesunięciem (bias), aby móc reprezentować zarówno duże, jak i małe wartości.
*   **Mantysa (M):** Określa precyzję (cyfry znaczące) liczby. Jest to liczba ułamkowa z przedziału [1, 2).

**3. Jakie są konsekwencje zapisu zmiennoprzecinkowego?**

*   **Ograniczona precyzja:** Nie wszystkie liczby dziesiętne da się dokładnie zapisać w systemie binarnym (np. `0.1`). Prowadzi to do **błędów zaokrągleń**.
*   **Porównywanie:** Porównywanie liczb zmiennoprzecinkowych za pomocą `==` jest niebezpieczne. Zamiast tego, należy sprawdzać, czy ich różnica jest mniejsza od pewnej małej wartości (epsilon).

**4. Czym jest arytmetyka komputerowa?**

To sposób, w jaki komputer wykonuje operacje arytmetyczne na liczbach binarnych. Kluczowe operacje realizowane są przez układy logiczne w **ALU (Jednostce Arytmetyczno-Logicznej)**.

*   **Dodawanie:** Realizowane przez sumatory (półsumatory i pełne sumatory).
*   **Odejmowanie:** Sprowadza się do dodawania liczby przeciwnej w kodzie U2.
*   **Mnożenie i dzielenie:** Realizowane przez bardziej złożone układy, często za pomocą sekwencji dodawań i przesunięć bitowych.

Arytmetyka komputerowa musi radzić sobie z ograniczeniami reprezentacji liczb, takimi jak **nadmiar (overflow)**, który występuje, gdy wynik operacji jest zbyt duży, by zmieścić się w dostępnej liczbie bitów.

---

# 19. Miary wydajności procesorów, pamięci i systemów obliczeniowych

**1. Jak mierzymy wydajność procesora (CPU)?**

*   **Taktowanie zegara (GHz):** Mówi, ile cykli zegara procesor wykonuje na sekundę. Wyższe taktowanie generalnie oznacza wyższą wydajność, ale to **nie jest jedyny czynnik**. Nowoczesne procesory mogą wykonywać więcej pracy w jednym cyklu.

*   **IPC (Instructions Per Cycle):** Liczba instrukcji wykonywanych średnio w jednym cyklu zegara. Jest to miara **efektywności architektury** procesora.

*   **FLOPS (Floating Point Operations Per Second):** Liczba operacji zmiennoprzecinkowych na sekundę. Kluczowa miara w obliczeniach naukowych i grafice (często podawana w GFLOPS lub TFLOPS).

*   **Benchmarki:** Najbardziej praktyczna miara. Są to standardowe programy (np. SPEC, Cinebench) lub gry, które mierzą, jak szybko procesor wykonuje realne zadania.

**2. Jak mierzymy wydajność pamięci (RAM)?**

*   **Przepustowość (Bandwidth):** Mierzona w GB/s. Określa, jak szybko dane mogą być odczytywane z pamięci i zapisywane do niej. Zależy od taktowania pamięci i szerokości magistrali.

*   **Opóźnienie (Latency, CAS Latency):** Mierzone w nanosekundach lub cyklach zegara. Określa, ile czasu upływa od momentu zażądania danych przez procesor do momentu, gdy są one dostępne. **Niższe opóźnienie jest lepsze**.

**3. Jak mierzymy wydajność całego systemu obliczeniowego?**

Wydajność systemu to nie tylko suma wydajności jego komponentów. Ważne są też inne czynniki:

*   **Czas odpowiedzi (Response Time):** Czas, jaki upływa od rozpoczęcia do zakończenia zadania. Ważny z perspektywy pojedynczego użytkownika.

*   **Przepustowość systemu (Throughput):** Liczba zadań, jakie system może wykonać w jednostce czasu. Ważna w systemach serwerowych obsługujących wielu użytkowników.

*   **Prawo Amdahla:** Mówi o tym, jak bardzo można przyspieszyć program, optymalizując tylko jego część. Jeśli program w 90% działa sekwencyjnie, a tylko w 10% równolegle, to nawet nieskończona liczba procesorów przyspieszy go co najwyżej o około 10%. Pokazuje to, że wąskie gardła decydują o ogólnej wydajności.

*   **Benchmarki systemowe:** Programy takie jak PCMark czy SYSmark, które symulują typowe zadania użytkownika (przeglądanie internetu, praca biurowa) i oceniają ogólną responsywność systemu.

---

# 20. Podstawowe elementy i znaczenie systemów wbudowanych

**1. Czym jest system wbudowany (embedded)?**

To **wyspecjalizowany system komputerowy**, który jest integralną częścią większego urządzenia i jest zaprojektowany do wykonywania **jednej, konkretnej funkcji** lub niewielkiego zestawu zadań. Działa w tle i często nie ma tradycyjnego interfejsu użytkownika.

**2. Jakie są jego kluczowe cechy?**

*   **Zorientowanie na zadanie:** Wykonuje precyzyjnie zdefiniowane zadania (np. sterowanie hamulcami w samochodzie, odczyt temperatury w termostacie).
*   **Ograniczenia zasobów:** Zazwyczaj ma ograniczoną moc obliczeniową, pamięć i zasilanie.
*   **Niezawodność i praca w czasie rzeczywistym:** Wiele systemów wbudowanych (np. w medycynie, motoryzacji) musi działać niezawodnie i reagować na zdarzenia w ściśle określonym czasie (systemy czasu rzeczywistego).
*   **Brak standardowego interfejsu:** Interakcja z użytkownikiem jest często ograniczona do kilku przycisków, diod LED lub jest całkowicie nieobecna.

**3. Z jakich elementów się składa?**

*   **Mikrokontroler (MCU):** To "serce" systemu. Jest to mały układ scalony, który zawiera w sobie procesor, pamięć (RAM i Flash) oraz peryferia (porty I/O, timery, przetworniki A/C) – wszystko w jednej obudowie.
*   **Czujniki (Sensors):** Zbierają dane ze świata fizycznego (np. temperatura, ciśnienie, światło).
*   **Elementy wykonawcze (Actuators):** Wpływają na świat fizyczny (np. silniki, diody, przekaźniki).
*   **Oprogramowanie (Firmware):** Specjalistyczne oprogramowanie zapisane na stałe w pamięci mikrokontrolera, które steruje jego działaniem.

**4. Jakie jest znaczenie i gdzie je spotykamy?**

Systemy wbudowane są **wszechobecne** i stanowią ukrytą podstawę nowoczesnego świata. Znajdziemy je w:

*   **Elektronice konsumenckiej:** Pralki, lodówki, telewizory, smartwatche.
*   **Motoryzacji:** Sterowniki silnika (ECU), systemy ABS, poduszki powietrzne, systemy inforozrywki.
*   **Przemyśle (IIoT):** Sterowniki PLC, roboty przemysłowe, systemy monitorowania maszyn.
*   **Medycynie:** Rozruszniki serca, pompy insulinowe, sprzęt diagnostyczny.
*   **Lotnictwie i wojsku:** Awionika, systemy naprowadzania.

Systemy wbudowane są kluczowym elementem **Internetu Rzeczy (IoT)**, gdzie łączą świat fizyczny z cyfrowym.

---

# 21. Rola i zadania systemu operacyjnego, podstawowe elementy i rodzaje systemów operacyjnych

**1. Czym jest system operacyjny (OS)?**

To **oprogramowanie pośredniczące** między użytkownikiem a sprzętem komputerowym. Zarządza zasobami komputera i tworzy środowisko, w którym użytkownik może uruchamiać aplikacje.

**2. Jakie są jego główne zadania?**

*   **Zarządzanie procesami:** Przydzielanie czasu procesora (CPU) poszczególnym zadaniom i przełączanie się między nimi.
*   **Zarządzanie pamięcią:** Alokowanie i zwalnianie pamięci operacyjnej (RAM) dla procesów, zarządzanie pamięcią wirtualną.
*   **Zarządzanie systemem plików:** Organizacja danych na dyskach, kontrola dostępu do plików i katalogów.
*   **Zarządzanie urządzeniami wejścia/wyjścia (I/O):** Obsługa komunikacji z urządzeniami takimi jak klawiatura, mysz, drukarka, dyski.
*   **Zapewnienie interfejsu użytkownika:** Umożliwia interakcję z komputerem, np. poprzez wiersz poleceń (CLI) lub interfejs graficzny (GUI).

**3. Jakie są podstawowe elementy (komponenty) systemu operacyjnego?**

*   **Jądro (Kernel):** To serce systemu operacyjnego. Działa w trybie uprzywilejowanym, ma bezpośredni dostęp do sprzętu i zarządza wszystkimi kluczowymi funkcjami systemu. Jest to pierwsza część OS ładowana do pamięci.
*   **Powłoka (Shell):** Interfejs użytkownika, który tłumaczy polecenia użytkownika na wywołania systemowe zrozumiałe dla jądra. Może być tekstowa (np. Bash w Linuksie) lub graficzna (np. Eksplorator w Windows).
*   **System plików:** Struktura logiczna do organizacji i przechowywania plików na dysku.

**4. Jakie są rodzaje systemów operacyjnych?**

*   **Ze względu na zastosowanie:**
    *   **Systemy dla komputerów osobistych:** Windows, macOS, Linux.
    *   **Systemy serwerowe:** Windows Server, Linux (np. Ubuntu Server, Red Hat).
    *   **Systemy mobilne:** Android, iOS.
    *   **Systemy wbudowane i czasu rzeczywistego (RTOS):** Specjalistyczne systemy do urządzeń embedded, gdzie kluczowy jest czas reakcji (np. QNX, FreeRTOS).
*   **Ze względu na architekturę jądra:**
    *   **Jądro monolityczne:** Wszystkie kluczowe funkcje (zarządzanie procesami, pamięcią, sterowniki) działają w jednej, dużej przestrzeni adresowej jądra. Jest szybkie, ale awaria jednego komponentu może zawiesić cały system. (Przykład: Linux).
    *   **Mikrojądro:** Jądro zawiera tylko absolutne minimum funkcji (komunikacja międzyprocesowa, podstawowe zarządzanie pamięcią). Reszta usług (system plików, sterowniki) działa jako osobne procesy w przestrzeni użytkownika. Jest bardziej bezpieczne i modułowe, ale wolniejsze z powodu narzutu komunikacyjnego. (Przykład: QNX).

---

# 22. Pojęcie procesu i wątku, stany procesu/wątku, przełączanie kontekstu, algorytmy szeregowania procesów

**1. Czym jest proces?**

Proces to **instancja uruchomionego programu**. Jest to podstawowa jednostka, której system operacyjny przydziela zasoby, takie jak czas procesora i własna, izolowana przestrzeń adresowa w pamięci.

**2. Czym jest wątek?**

Wątek to **jednostka wykonania wewnątrz procesu**. Jeden proces może składać się z wielu wątków, które współdzielą tę samą przestrzeň adresową i zasoby (np. otwarte pliki). Wątki pozwalają na wykonywanie kilku zadań "jednocześnie" w ramach jednej aplikacji (np. jeden wątek obsługuje interfejs użytkownika, a drugi w tle zapisuje plik).

**3. Jakie są stany procesu/wątku?**

*   **Nowy (New):** Proces został utworzony, ale nie jest jeszcze gotowy do wykonania.
*   **Gotowy (Ready):** Proces czeka na przydział czasu procesora.
*   **Wykonywany (Running):** Proces aktualnie wykonuje instrukcje na procesorze.
*   **Oczekujący / Zablokowany (Waiting / Blocked):** Proces czeka na jakieś zdarzenie, np. zakończenie operacji I/O lub zwolnienie zasobu.
*   **Zakończony (Terminated):** Proces zakończył swoje działanie.

**4. Na czym polega przełączanie kontekstu?**

To mechanizm, za pomocą którego system operacyjny **przełącza procesor z wykonywania jednego procesu na drugi**. Polega na:
1.  **Zapisaniu stanu bieżącego procesu** (rejestrów CPU, licznika rozkazów) w jego bloku kontrolnym (PCB).
2.  **Wczytaniu stanu nowego procesu** z jego PCB do rejestrów CPU.

Przełączanie kontekstu jest **kosztowną operacją**, ponieważ zajmuje czas, w którym procesor nie wykonuje użytecznej pracy. Przełączanie między wątkami w obrębie tego samego procesu jest znacznie "tańsze" niż między procesami, bo nie wymaga zmiany przestrzeni adresowej.

**5. Czym są algorytmy szeregowania (scheduling)?**

To algorytmy, których używa system operacyjny, aby zdecydować, **który z procesów w stanie "Gotowy" ma jako następny otrzymać czas procesora**. Celem jest zapewnienie sprawiedliwości, wydajności i responsywności systemu.

*   **FCFS (First-Come, First-Served):** Prosta kolejka – proces, który przyszedł pierwszy, jest obsługiwany jako pierwszy. Sprawiedliwy, ale nieoptymalny.
*   **SJF (Shortest Job First):** Wybierany jest proces, który potrzebuje najmniej czasu procesora. Optymalny pod względem średniego czasu oczekiwania, ale trudny do zaimplementowania (skąd wiedzieć, ile czasu potrzebuje proces?).
*   **Szeregowanie rotacyjne (Round Robin):** Każdy proces otrzymuje mały, stały kwant czasu procesora. Jeśli go nie skończy, wraca na koniec kolejki. Zapewnia dobrą responsywność w systemach interaktywnych.

---

# 23. Problem wzajemnego wykluczania i jego rozwiązania, synchronizacja procesów i wątków, problem zakleszczenia

**1. Na czym polega problem wzajemnego wykluczania (mutual exclusion)?**

Problem ten pojawia się, gdy wiele procesów lub wątków chce uzyskać dostęp do **współdzielonego zasobu** (np. zmiennej, pliku, drukarki), który nie może być używany przez kilka z nich jednocześnie. **Sekcja krytyczna** to fragment kodu, w którym proces uzyskuje dostęp do takiego zasobu. Wzajemne wykluczanie to zapewnienie, że **w danym momencie co najwyżej jeden proces może znajdować się w swojej sekcji krytycznej**.

**2. Jakie są rozwiązania tego problemu (mechanizmy synchronizacji)?**

*   **Semafor:** To specjalna zmienna całkowita, na której można wykonywać tylko dwie niepodzielne (atomowe) operacje: `wait()` (dekrementacja, P) i `signal()` (inkrementacja, V). Jeśli semafor ma wartość 0, proces próbujący wykonać `wait()` zostaje zablokowany, aż inny proces zwolni zasób za pomocą `signal()`. Semafor, który przyjmuje tylko wartości 0 i 1, nazywamy **semaforem binarnym** lub **muteksem**.

*   **Muteks (Mutex - MUTual EXclusion):** To prostsza forma semafora, działająca jak zamek. Może być w jednym z dwóch stanów: **zamknięty** lub **otwarty**. Proces przed wejściem do sekcji krytycznej musi "zamknąć" muteks. Jeśli jest już zamknięty, proces czeka. Po wyjściu z sekcji krytycznej, proces "otwiera" muteks. **Ważne:** tylko ten wątek, który zamknął muteks, może go otworzyć.

*   **Monitor:** To konstrukcja programistyczna wysokiego poziomu (obecna w językach jak Java czy C#), która hermetyzuje współdzielone dane i procedury operujące na nich, automatycznie zapewniając wzajemne wykluczanie. Tylko jeden wątek może być w danym momencie "aktywny" wewnątrz monitora.

**3. Czym jest problem zakleszczenia (deadlock)?**

Zakleszczenie to sytuacja, w której **dwa lub więcej procesów czeka na siebie nawzajem**, blokując się bez końca. Każdy z nich trzyma zasób, którego potrzebuje inny, i czeka na zasób, który ten inny trzyma.

**4. Jakie warunki muszą być spełnione, aby doszło do zakleszczenia?**

Muszą wystąpić **jednocześnie** cztery warunki (warunki Coffmana):
1.  **Wzajemne wykluczanie:** Zasoby nie mogą być współdzielone.
2.  **Trzymanie i oczekiwanie (Hold and Wait):** Proces trzymający co najmniej jeden zasób, czeka na przydział kolejnego.
3.  **Brak wywłaszczania (No Preemption):** Zasób nie może być siłą odebrany procesowi, który go trzyma.
4.  **Cykliczne oczekiwanie (Circular Wait):** Istnieje cykl procesów, w którym każdy czeka na zasób trzymany przez następny proces w cyklu.

Zapobieganie zakleszczeniom polega na wyeliminowaniu co najmniej jednego z tych czterech warunków.

---

# 24. Zarządzanie pamięcią operacyjną, pojęcie pamięci wirtualnej, segmentacja i stronicowanie pamięci

**1. Na czym polega zarządzanie pamięcią operacyjną?**

To jedno z kluczowych zadań systemu operacyjnego. Polega na **alokowaniu (przydzielaniu) i zwalnianiu bloków pamięci RAM** dla procesów, tak aby mogły one być wykonywane, a jednocześnie nie wchodziły sobie w drogę.

**2. Czym jest pamięć wirtualna?**

To mechanizm, który daje każdemu procesowi **iluzję posiadania własnej, ciągłej i dużej przestrzeni adresowej**, niezależnie od fizycznej ilości i organizacji pamięci RAM. Pozwala to na:
*   **Uruchamianie programów większych niż fizyczna pamięć RAM:** Tylko potrzebne fragmenty programu są w danym momencie trzymane w RAM, reszta znajduje się na dysku twardym (w tzw. pliku wymiany lub partycji swap).
*   **Izolację procesów:** Każdy proces działa we własnej, odizolowanej przestrzeni adresowej, co zapobiega wzajemnemu zakłócaniu się.

**3. Jak implementuje się pamięć wirtualną?**

Kluczową rolę odgrywa tu sprzętowy komponent zwany **MMU (Memory Management Unit)**, który tłumaczy adresy wirtualne (używane przez proces) na adresy fizyczne (w pamięci RAM).

Dwie główne techniki implementacji to **stronicowanie** i **segmentacja**.

**4. Na czym polega stronicowanie (paging)?**

*   **Idea:** Pamięć wirtualna procesu i pamięć fizyczna są dzielone na małe bloki o **stałym rozmiarze**, zwane odpowiednio **stronami** (pages) i **ramkami** (frames).
*   **Działanie:** System operacyjny utrzymuje dla każdego procesu **tablicę stron**, która mapuje strony wirtualne na ramki fizyczne. Gdy proces odwołuje się do adresu, MMU używa tablicy stron, aby znaleźć odpowiednią ramkę w RAM.
*   **Błąd strony (Page Fault):** Jeśli strona, do której odwołuje się proces, nie znajduje się aktualnie w pamięci RAM, MMU generuje przerwanie zwane błędem strony. System operacyjny wstrzymuje proces, wczytuje brakującą stronę z dysku do wolnej ramki, aktualizuje tablicę stron i wznawia proces.

**5. Na czym polega segmentacja (segmentation)?**

*   **Idea:** Pamięć wirtualna procesu jest dzielona na **logiczne segmenty o zmiennej długości**, które odpowiadają strukturze programu (np. segment kodu, segment danych, segment stosu).
*   **Działanie:** Adres wirtualny składa się z numeru segmentu i przesunięcia wewnątrz tego segmentu. System operacyjny utrzymuje tablicę segmentów, która przechowuje fizyczny adres bazowy i rozmiar każdego segmentu.
*   **Zalety:** Ułatwia współdzielenie kodu i ochronę pamięci (można nadać różne uprawnienia różnym segmentom, np. segment kodu tylko do odczytu).

**Współczesne systemy (np. Linux, Windows) używają kombinacji obu technik – segmentacji ze stronicowaniem.**

---

# 25. System plików, organizacja i implementacja, metody dostępu do plików

**1. Czym jest system plików?**

To część systemu operacyjnego, która odpowiada za **organizację, przechowywanie i zarządzanie plikami na nośnikach danych** (np. dyskach twardych, SSD). Zapewnia on logiczną, hierarchiczną strukturę (drzewo katalogów), ukrywając przed użytkownikiem fizyczną lokalizację danych na dysku.

**2. Jakie są jego główne zadania?**

*   Tworzenie, usuwanie i modyfikowanie plików i katalogów.
*   Mapowanie logicznej struktury plików na fizyczne bloki na dysku.
*   Zarządzanie wolnym miejscem.
*   Kontrola dostępu i ochrona danych.

**3. Jak wygląda typowa organizacja i implementacja?**

*   **Bloki:** Dysk jest podzielony na logiczne bloki o stałym rozmiarze, które są najmniejszą jednostką alokacji.
*   **Metadane:** System plików przechowuje informacje o plikach (metadane), takie jak nazwa, rozmiar, data modyfikacji, uprawnienia i, co najważniejsze, **wskaźniki do bloków danych**, które składają się na plik. Te metadane są przechowywane w specjalnej strukturze, np. **i-węźle (inode)** w systemach uniksowych (Linux, macOS) lub w **Master File Table (MFT)** w systemie NTFS (Windows).
*   **Alokacja plików:**
    *   **Alokacja ciągła:** Plik zajmuje ciągły obszar bloków na dysku. Szybki dostęp, ale powoduje fragmentację zewnętrzną.
    *   **Alokacja listowa (łańcuchowa):** Bloki pliku są rozproszone po dysku. Każdy blok zawiera wskaźnik do następnego bloku. Eliminuje fragmentację, ale uniemożliwia szybki dostęp swobodny (trzeba przejść całą listę).
    *   **Alokacja indeksowa (np. i-węzły):** Metadane pliku (i-węzeł) zawierają listę wskaźników do wszystkich bloków danych tego pliku. Jest to rozwiązanie elastyczne i wydajne, stosowane w większości nowoczesnych systemów plików.

**4. Jakie są metody dostępu do plików?**

*   **Dostęp sekwencyjny (Sequential Access):** Dane są odczytywane lub zapisywane po kolei, jeden rekord po drugim. Jest to najprostsza i najczęstsza metoda, używana np. przy odczycie plików tekstowych.

*   **Dostęp swobodny (Direct/Random Access):** Pozwala na odczyt lub zapis dowolnego bloku pliku bezpośrednio, bez konieczności przetwarzania poprzednich. Kluczowy dla aplikacji bazodanowych, które muszą szybko uzyskiwać dostęp do konkretnych rekordów.

---

# 26. Model warstwowy ISO/OSI i TCP/IP, protokoły i ich rola w komunikacji sieciowej

**1. Czym jest model warstwowy i jaki jest jego cel?**

To **koncepcyjny schemat**, który dzieli złożony proces komunikacji sieciowej na mniejsze, zarządzalne części zwane **warstwami**. Każda warstwa ma ściśle zdefiniowane zadania i komunikuje się tylko z warstwami bezpośrednio powyżej i poniżej niej. Celem jest **uproszczenie projektowania, standaryzacja i umożliwienie interoperacyjności** (współdziałania) urządzeń różnych producentów.

**2. Jakie są dwa główne modele warstwowe?**

*   **Model referencyjny ISO/OSI:** Model teoretyczny, składający się z **siedmiu warstw**. Jest ważny dla zrozumienia teorii sieci, ale rzadko implementowany w czystej postaci.
    *   7. Aplikacji (np. HTTP, FTP)
    *   6. Prezentacji
    *   5. Sesji
    *   4. Transportu (np. TCP, UDP)
    *   3. Sieci (np. IP)
    *   2. Łącza danych (np. Ethernet)
    *   1. Fizyczna

*   **Model TCP/IP (Model internetowy):** Model praktyczny, na którym opiera się działanie internetu. Składa się z **czterech warstw**.
    *   4. Aplikacji (odpowiada warstwom 5-7 z OSI)
    *   3. Transportu
    *   2. Internetu (odpowiada warstwie 3 z OSI)
    *   1. Dostępu do sieci (odpowiada warstwom 1-2 z OSI)

**3. Czym jest protokół sieciowy?**

To **zbiór reguł i procedur**, które określają, w jaki sposób urządzenia sieciowe mają się ze sobą komunikować. Definiuje format, kolejność i znaczenie przesyłanych komunikatów. Każda warstwa modelu używa własnych protokołów do realizacji swoich zadań.

**4. Jak dane podróżują przez warstwy (enkapsulacja i dekapsulacja)?**

*   **Enkapsulacja (u nadawcy):** Dane z warstwy wyższej są "pakowane" w jednostkę danych warstwy niższej. Każda warstwa dodaje do danych swój własny **nagłówek** (zawierający informacje sterujące), tworząc nową jednostkę danych (PDU - Protocol Data Unit).
    *   Dane w warstwie aplikacji -> Segment w warstwie transportu -> Pakiet w warstwie sieci -> Ramka w warstwie łącza danych -> Bity w warstwie fizycznej.

*   **Dekapsulacja (u odbiorcy):** Proces odwrotny. Każda warstwa odczytuje i usuwa swój nagłówek, a resztę danych przekazuje do warstwy wyższej, aż do momentu, gdy aplikacja odbiorcy otrzyma oryginalne dane.

---

# 27. Adresacja w sieciach komputerowych: adresy fizyczne, logiczne i porty, rola i zadania protokołów ARP, DNS, DHCP

**1. Jakie są rodzaje adresów w sieciach?**

*   **Adres fizyczny (MAC - Media Access Control):**
    *   **Czym jest?** Unikalny, 48-bitowy identyfikator "wypalony" na stałe w karcie sieciowej (NIC) przez producenta.
    *   **Gdzie działa?** W warstwie łącza danych (L2). Używany do komunikacji **w obrębie tej samej sieci lokalnej (LAN)**.

*   **Adres logiczny (IP - Internet Protocol):**
    *   **Czym jest?** 32-bitowy (IPv4) lub 128-bitowy (IPv6) adres, który jest logicznie przypisywany do urządzenia. Może być stały lub dynamiczny.
    *   **Gdzie działa?** W warstwie sieci (L3). Używany do komunikacji **między różnymi sieciami** (w internecie).

*   **Port:**
    *   **Czym jest?** 16-bitowy numer, który identyfikuje **konkretną aplikację lub usługę** działającą na komputerze.
    *   **Gdzie działa?** W warstwie transportu (L4). Para (Adres IP : Port) tworzy tzw. **gniazdo (socket)**, które jednoznacznie identyfikuje proces na danym hoście w całej sieci.

**2. Jak te adresy współpracują?**

Komputer, chcąc wysłać pakiet do innego komputera w tej samej sieci lokalnej, zna jego adres IP, ale do wysłania ramki potrzebuje jego adresu MAC. Tu z pomocą przychodzą specjalne protokoły.

**3. Jaką rolę pełnią protokoły ARP, DNS i DHCP?**

*   **ARP (Address Resolution Protocol):**
    *   **Zadanie:** Tłumaczenie **adresów IP na adresy MAC** w sieci lokalnej.
    *   **Jak działa?** Komputer wysyła w sieć lokalną zapytanie rozgłoszeniowe (broadcast) o treści: "Kto ma adres IP 192.168.1.10?". Komputer o tym adresie IP odpowiada, podając swój adres MAC.

*   **DNS (Domain Name System):**
    *   **Zadanie:** Tłumaczenie **nazw domenowych** (łatwych do zapamiętania dla ludzi, np. `www.google.com`) na **adresy IP** (zrozumiałe dla maszyn).
    *   **Jak działa?** Działa jak rozproszona książka telefoniczna dla internetu. Przeglądarka, zanim połączy się ze stroną, pyta serwer DNS o jej adres IP.

*   **DHCP (Dynamic Host Configuration Protocol):**
    *   **Zadanie:** **Automatyczne przydzielanie adresów IP** i innych parametrów konfiguracyjnych (maska podsieci, brama domyślna, adresy serwerów DNS) urządzeniom w sieci.
    *   **Jak działa?** Gdy urządzenie podłącza się do sieci, wysyła zapytanie o konfigurację. Serwer DHCP (często wbudowany w router) odpowiada, "wypożyczając" mu wolny adres IP na określony czas.

---

# 28. Podstawowe urządzenia sieciowe i ich rola w przesyle danych: koncentrator, przełącznik, router

**1. Koncentrator (Hub):**

*   **Warstwa działania:** Warstwa 1 (Fizyczna).
*   **Jak działa?** Jest to proste urządzenie, które działa jak "elektryczny przedłużacz". Sygnał otrzymany na jednym porcie jest **kopiowany i rozsyłany na wszystkie pozostałe porty**, bez żadnej analizy danych.
*   **Rola:** Łączenie komputerów w sieć o topologii gwiazdy.
*   **Wady:** Bardzo nieefektywny. Tworzy jedną, dużą **domenę kolizyjną** – jeśli dwa komputery nadają w tym samym czasie, dochodzi do kolizji i transmisja musi być powtórzona. Dziś jest to urządzenie historyczne.

**2. Przełącznik (Switch):**

*   **Warstwa działania:** Warstwa 2 (Łącza danych).
*   **Jak działa?** Jest to inteligentne urządzenie. Analizuje przychodzące **ramki**, odczytuje **adres MAC** odbiorcy i przesyła ramkę **tylko do tego portu**, do którego podłączony jest docelowy komputer. Uczy się adresów MAC urządzeń podłączonych do jego portów i przechowuje je w tablicy MAC.
*   **Rola:** Łączenie komputerów w sieć lokalną (LAN) w sposób wydajny.
*   **Zalety:** Każdy port stanowi osobną **domenę kolizyjną**, co eliminuje problem kolizji i znacznie zwiększa wydajność sieci w porównaniu do koncentratora.

**3. Router:**

*   **Warstwa działania:** Warstwa 3 (Sieci).
*   **Jak działa?** Jest to najbardziej zaawansowane z tych urządzeń. Analizuje przychodzące **pakiety**, odczytuje **adres IP** odbiorcy i na podstawie swojej **tablicy routingu** podejmuje decyzję, którędy (którym interfejsem) wysłać pakiet dalej, aby dotarł on do celu.
*   **Rola:** Jego głównym zadaniem jest **łączenie różnych sieci komputerowych** i **wyznaczanie najlepszej trasy** dla pakietów w internecie. Każdy port routera tworzy osobną **domenę rozgłoszeniową** (broadcastową).

| Cecha | Koncentrator (Hub) | Przełącznik (Switch) | Router |
| :--- | :--- | :--- | :--- |
| **Warstwa** | 1 (Fizyczna) | 2 (Łącza Danych) | 3 (Sieci) |
| **Adresy** | Nie używa | MAC | IP |
| **Jednostka danych**| Bity | Ramki | Pakiety |
| **Decyzja** | Brak (kopiuje wszędzie) | Przesyła do konkretnego portu | Wybiera najlepszą trasę |
| **Zastosowanie** | Przestarzały | Sieć lokalna (LAN) | Łączenie sieci (Internet) |

_No response_

---

# 29. Rola i zadania wybranych protokołów warstwy aplikacji: HTTP, FTP, SMTP, DNS

**1. HTTP (HyperText Transfer Protocol):**

*   **Rola:** Podstawa komunikacji w World Wide Web. Służy do przesyłania stron internetowych (dokumentów HTML), obrazków i innych zasobów między serwerem WWW a przeglądarką klienta.
*   **Jak działa?** Działa w modelu "żądanie-odpowiedź". Klient (przeglądarka) wysyła żądanie (np. `GET /index.html`), a serwer odpowiada, przesyłając żądany zasób lub kod błędu.
*   **Wersje:** HTTP/1.1 jest wciąż popularny, ale nowszy **HTTPS** (HTTP Secure) szyfruje całą komunikację, zapewniając bezpieczeństwo.

**2. FTP (File Transfer Protocol):**

*   **Rola:** Służy do przesyłania plików między komputerami w sieci.
*   **Jak działa?** Używa dwóch osobnych połączeń: **kanału sterującego** do przesyłania poleceń (np. `LIST`, `GET`) i **kanału danych** do właściwego transferu plików. Jest to protokół "stanowy" - serwer pamięta stan sesji klienta.

**3. SMTP (Simple Mail Transfer Protocol):**

*   **Rola:** Służy do **wysyłania i przesyłania poczty elektronicznej** między serwerami pocztowymi. Twój klient pocztowy używa SMTP, aby wysłać e-mail do Twojego serwera, a serwery używają SMTP do przekazywania go dalej.
*   **Uwaga:** Do **odbierania** poczty używa się innych protokołów, takich jak **POP3** lub **IMAP**.

**4. DNS (Domain Name System):**

*   **Rola:** Działa jak **książka telefoniczna internetu**. Tłumaczy łatwe do zapamiętania dla ludzi **nazwy domenowe** (np. `www.example.com`) na zrozumiałe dla maszyn **adresy IP** (np. `93.184.216.34`).
*   **Jak działa?** Jest to globalny, rozproszony system baz danych. Gdy wpisujesz adres w przeglądarce, Twój komputer wysyła zapytanie do serwera DNS, aby uzyskać adres IP docelowej strony.

---

# 30. Podstawowe zagadnienia bezpieczeństwa sieci komputerowych: zagrożenia, metody ochrony, kryptografia

**1. Jakie są główne zagrożenia w sieciach?**

*   **Podsłuchiwanie (Eavesdropping):** Nieautoryzowane przechwytywanie danych przesyłanych w sieci.
*   **Ataki Man-in-the-Middle (MITM):** Atakujący potajemnie pośredniczy w komunikacji między dwiema stronami, mogąc podsłuchiwać i modyfikować przesyłane dane.
*   **Ataki DoS/DDoS (Denial of Service):** Próba zablokowania działania usługi sieciowej poprzez zalanie jej ogromną liczbą zapytań, co prowadzi do wyczerpania jej zasobów.
*   **Malware:** Złośliwe oprogramowanie (wirusy, robaki, trojany, ransomware) rozprzestrzeniające się przez sieć.
*   **Phishing:** Próba wyłudzenia poufnych informacji (np. haseł, danych karty kredytowej) poprzez podszywanie się pod zaufaną instytucję (np. fałszywa strona banku).

**2. Jakie są podstawowe metody ochrony?**

*   **Firewall (Zapora sieciowa):** Działa jak filtr na granicy sieci. Analizuje ruch przychodzący i wychodzący i na podstawie zdefiniowanych reguł decyduje, czy go przepuścić, czy zablokować.
*   **Systemy wykrywania i zapobiegania włamaniom (IDS/IPS):** Monitorują ruch sieciowy w poszukiwaniu wzorców wskazujących na atak. IDS tylko alarmuje, a IPS potrafi również aktywnie blokować podejrzany ruch.
*   **Wirtualne Sieci Prywatne (VPN):** Tworzą szyfrowany "tunel" przez publiczną sieć (internet), zapewniając poufność i integralność komunikacji, tak jakby odbywała się w sieci prywatnej.
*   **Uwierzytelnianie i autoryzacja:** Weryfikacja tożsamości użytkowników (np. hasła, certyfikaty, 2FA) i nadawanie im odpowiednich uprawnień.

**3. Jaką rolę odgrywa kryptografia?**

Jest **fundamentalna** dla bezpieczeństwa sieci. Zapewnia trzy kluczowe usługi:

*   **Poufność:** Szyfrowanie danych sprawia, że są one nieczytelne dla osób nieuprawnionych, nawet jeśli zostaną podsłuchane. (Realizowane przez szyfry symetryczne i asymetryczne).
*   **Integralność:** Funkcje skrótu (haszujące) pozwalają zweryfikować, czy dane nie zostały zmienione podczas przesyłu.
*   **Uwierzytelnienie i niezaprzeczalność:** Podpisy cyfrowe pozwalają zweryfikować tożsamość nadawcy i uniemożliwiają mu wyparcie się autorstwa wiadomości.

---

# 31. Cykl życia oprogramowania i jego modele (modele wytwarzania oprogramowania)

**1. Czym jest cykl życia oprogramowania (SDLC)?**

To **ustrukturyzowany proces**, który dzieli proces tworzenia oprogramowania na kolejne, dobrze zdefiniowane fazy. Celem jest poprawa jakości oprogramowania i kontrola nad całym procesem, od pomysłu do wycofania produktu.

**2. Jakie są typowe fazy cyklu życia?**

1.  **Planowanie i analiza wymagań:** Zrozumienie, co system ma robić, zebranie wymagań od klienta.
2.  **Projektowanie:** Stworzenie architektury systemu i szczegółowego projektu technicznego.
3.  **Implementacja (Kodowanie):** Pisanie kodu źródłowego.
4.  **Testowanie:** Weryfikacja, czy oprogramowanie działa zgodnie z wymaganiami i jest wolne od błędów.
5.  **Wdrożenie (Deployment):** Instalacja oprogramowania w środowisku produkcyjnym.
6.  **Utrzymanie:** Poprawianie błędów, dodawanie nowych funkcji i adaptacja do zmieniających się warunków po wdrożeniu.

**3. Jakie są główne modele wytwarzania oprogramowania?**

*   **Model kaskadowy (Waterfall):**
    *   **Idea:** Proces jest liniowy i sekwencyjny. Każda faza musi się w pełni zakończyć, zanim rozpocznie się następna. Nie ma powrotu do wcześniejszych etapów.
    *   **Zalety:** Prosty i łatwy do zarządzania.
    *   **Wady:** Bardzo nieelastyczny. Nie nadaje się do projektów, gdzie wymagania mogą się zmieniać. Błędy wykryte na późnym etapie są bardzo kosztowne w naprawie.

*   **Model iteracyjno-przyrostowy:**
    *   **Idea:** Oprogramowanie jest tworzone w kolejnych **iteracjach (cyklach)**. W każdej iteracji przechodzi się przez wszystkie fazy (analiza, projekt, kod, test) i dostarcza **przyrost** funkcjonalności – mały, ale działający fragment systemu.
    *   **Zalety:** Elastyczność, możliwość wczesnego uzyskania informacji zwrotnej od klienta, mniejsze ryzyko.

*   **Metodyki zwinne (Agile):**
    *   **Idea:** To rozwinięcie modelu iteracyjnego, które kładzie nacisk na **adaptacyjność, bliską współpracę z klientem i szybkie dostarczanie wartości**. Praca jest zorganizowana w krótkie cykle (sprinty), a wymagania mogą ewoluować w trakcie projektu.
    *   **Przykłady:** Scrum, Kanban.

*   **Model spiralny:**
    *   **Idea:** Łączy cechy modelu iteracyjnego z systematycznym podejściem modelu kaskadowego, dodając na każdym etapie **analizę ryzyka**. Stosowany w dużych, złożonych i ryzykownych projektach.

---

# 32. Analiza i projektowanie algorytmów, złożoność obliczeniowa, notacja asymptotyczna

**1. Czym jest analiza i projektowanie algorytmów?**

*   **Projektowanie algorytmów:** To proces tworzenia krok-po-kroku przepisu na rozwiązanie danego problemu obliczeniowego.
*   **Analiza algorytmów:** To proces oceny, jak **wydajny** jest dany algorytm. Interesuje nas głównie, jak zapotrzebowanie algorytmu na zasoby (czas i pamięć) rośnie wraz ze wzrostem rozmiaru danych wejściowych.

**2. Czym jest złożoność obliczeniowa?**

To formalna miara zasobów (głównie czasu) potrzebnych algorytmowi do rozwiązania problemu w zależności od rozmiaru danych wejściowych (n).

*   **Złożoność czasowa:** Mówi, jak liczba operacji elementarnych wykonywanych przez algorytm zależy od `n`.
*   **Złożoność pamięciowa:** Mówi, jak ilość pamięci zajmowanej przez algorytm zależy od `n`.

**3. Czym jest notacja asymptotyczna (notacja O)?**

To matematyczny zapis służący do opisywania **tempa wzrostu** funkcji, a w informatyce – do klasyfikowania algorytmów pod względem ich złożoności. Ignoruje ona stałe i czynniki niższego rzędu, skupiając się na tym, co dominuje, gdy `n` dąży do nieskończoności.

*   **O(1) – złożoność stała:** Czas wykonania jest niezależny od rozmiaru danych (np. dostęp do elementu tablicy).
*   **O(log n) – złożoność logarytmiczna:** Czas rośnie bardzo wolno. Typowa dla algorytmów, które w każdym kroku redukują problem o stały czynnik (np. wyszukiwanie binarne).
*   **O(n) – złożoność liniowa:** Czas rośnie proporcjonalnie do rozmiaru danych (np. wyszukiwanie elementu w nieposortowanej liście).
*   **O(n log n) – złożoność liniowo-logarytmiczna:** Typowa dla efektywnych algorytmów sortowania (np. sortowanie przez scalanie, quicksort).
*   **O(n²) – złożoność kwadratowa:** Czas rośnie proporcjonalnie do kwadratu rozmiaru danych. Typowa dla prostych algorytmów sortowania (np. sortowanie bąbelkowe) lub operacji na parach elementów.
*   **O(2^n) – złożoność wykładnicza:** Czas rośnie bardzo gwałtownie. Algorytmy o tej złożoności są praktycznie bezużyteczne już dla niewielkich `n` (np. problem komiwojażera rozwiązywany metodą siłową).

**Cel:** Zawsze dążymy do projektowania algorytmów o jak najniższej złożoności obliczeniowej.

---

# 33. Paradygmaty programowania: imperatywny, obiektowy, funkcyjny, deklaratywny

**1. Czym jest paradygmat programowania?**

To **styl lub sposób myślenia** o programowaniu i strukturyzowaniu kodu. Definiuje, jak programista postrzega problem i jakimi narzędziami koncepcyjnymi się posługuje do jego rozwiązania.

**2. Paradygmat imperatywny:**

*   **Idea:** Program to **sekwencja instrukcji**, które krok po kroku **zmieniają stan programu** (wartości zmiennych). Programista opisuje **jak** komputer ma wykonać zadanie.
*   **Kluczowe pojęcia:** Zmienne, przypisania, pętle, instrukcje warunkowe.
*   **Przykład:** Języki C, Pascal, Fortran.

**3. Paradygmat obiektowy (OOP - Object-Oriented Programming):**

*   **Idea:** To rozszerzenie paradygmatu imperatywnego. Program jest postrzegany jako **zbiór współpracujących ze sobą obiektów**. Obiekt hermetyzuje w sobie **dane (stan)** i **operacje (zachowanie)**, które można na tych danych wykonać.
*   **Kluczowe pojęcia:** Klasa, obiekt, dziedziczenie, polimorfizm, enkapsulacja.
*   **Cel:** Lepsza organizacja kodu, modularyzacja, ponowne wykorzystanie kodu.
*   **Przykład:** Java, C++, C#, Python.

**4. Paradygmat funkcyjny (FP - Functional Programming):**

*   **Idea:** Programowanie polega na **komponowaniu i stosowaniu funkcji matematycznych**. Kładzie nacisk na unikanie **stanu i danych mutowalnych (zmiennych)**. Funkcje dla tych samych argumentów zawsze zwracają ten sam wynik (są deterministyczne).
*   **Kluczowe pojęcia:** Funkcje wyższego rzędu, niemutowalność, czyste funkcje, rekurencja.
*   **Cel:** Pisanie bardziej przewidywalnego, łatwiejszego do testowania i zrównoleglania kodu.
*   **Przykład:** Haskell, Lisp, F#, a także elementy funkcyjne w JavaScript i Pythonie.

**5. Paradygmat deklaratywny:**

*   **Idea:** To ogólna kategoria, do której zalicza się m.in. programowanie funkcyjne i logiczne. Programista opisuje **co** chce osiągnąć, a nie **jak** to zrobić. System sam znajduje sposób na osiągnięcie celu.
*   **Przykład:**
    *   **SQL:** `SELECT name FROM users WHERE country = 'Poland';` (Mówimy co chcemy, nie jak baza ma to znaleźć).
    *   **HTML:** Opisujemy strukturę strony, a nie jak przeglądarka ma ją rysować krok po kroku.
    *   **Prolog:** Język programowania logicznego.

---

# 34. Programowanie obiektowe: klasy, obiekty, dziedziczenie, polimorfizm

**1. Czym jest klasa i obiekt?**

*   **Klasa:** To **szablon lub przepis**, na podstawie którego tworzone są obiekty. Definiuje ona **właściwości (pola, atrybuty)**, które będą miały obiekty danej klasy, oraz **metody (funkcje)**, czyli operacje, które będzie można na nich wykonać.
*   **Obiekt:** To **konkretna instancja** klasy. Jest to byt istniejący w pamięci komputera, posiadający swój własny stan (wartości pól) i zachowanie (zdefiniowane przez metody klasy).

*Przykład:* Klasa `Samochod` definiuje, że każdy samochód ma `kolor` i `predkosc` oraz potrafi `przyspieszac()`. Obiekt `mojeCzerwoneFerrari` jest konkretną instancją tej klasy, z `kolor = 

'czerwony'` i `predkosc = 50`.

**2. Czym jest dziedziczenie?**

*   **Idea:** Mechanizm, który pozwala tworzyć nową klasę (**klasa pochodna**) na bazie już istniejącej (**klasa bazowa**). Klasa pochodna **dziedziczy** wszystkie pola i metody klasy bazowej, a dodatkowo może dodawać własne lub modyfikować (przesłaniać) odziedziczone.
*   **Cel:** Ponowne wykorzystanie kodu i tworzenie hierarchii klas (np. `Pojazd` -> `Samochod` -> `SamochodElektryczny`).

**3. Czym jest polimorfizm?**

*   **Idea:** Z greckiego "wielopostaciowość". Oznacza, że obiekty różnych klas, ale należące do tej samej hierarchii dziedziczenia, mogą być traktowane w jednolity sposób. Ta sama operacja (wywołanie tej samej metody) może zachowywać się inaczej w zależności od tego, na jakim konkretnie obiekcie jest wywoływana.
*   **Przykład:** Mamy klasę bazową `Zwierze` z metodą `wydajDzwiek()`. Klasy pochodne `Pies` i `Kot` przesłaniają tę metodę. Jeśli mamy tablicę zwierząt, możemy w pętli wywołać `zwierze.wydajDzwiek()` dla każdego elementu, a w zależności od tego, czy dany obiekt jest Psem czy Kotem, usłyszymy "Hau!" lub "Miau!".

**4. Czym jest enkapsulacja (hermetyzacja)?**

*   **Idea:** Ukrywanie szczegółów implementacyjnych obiektu przed światem zewnętrznym. Stan obiektu (jego pola) jest prywatny i dostęp do niego jest możliwy tylko poprzez publiczne metody (tzw. gettery i settery).
*   **Cel:** Ochrona danych przed nieautoryzowanymi modyfikacjami, zwiększenie modularności i ułatwienie zmian w implementacji bez wpływu na resztę systemu.

---

# 35. Podstawowe struktury danych: tablica, lista, stos, kolejka, drzewo, graf

*   **Tablica (Array):** Kolekcja elementów tego samego typu, przechowywana w ciągłym bloku pamięci. Umożliwia bardzo szybki dostęp do dowolnego elementu przez jego indeks (złożoność O(1)). Jej rozmiar jest zazwyczaj stały.

*   **Lista (List):** Sekwencja elementów, gdzie każdy element (węzeł) przechowuje wskaźnik do następnego (lista jednokierunkowa) lub też do poprzedniego (lista dwukierunkowa). Umożliwia łatwe dodawanie i usuwanie elementów w dowolnym miejscu (O(1)), ale dostęp do konkretnego elementu wymaga przejścia przez listę (O(n)).

*   **Stos (Stack):** Struktura działająca w trybie **LIFO (Last-In, First-Out)** – ostatni element dodany jest zdejmowany jako pierwszy. Działa jak stos talerzy. Dwie podstawowe operacje to `push` (połóż na stosie) i `pop` (zdejmij ze stosu).

*   **Kolejka (Queue):** Struktura działająca w trybie **FIFO (First-In, First-Out)** – pierwszy element dodany jest obsługiwany jako pierwszy. Działa jak kolejka w sklepie. Dwie podstawowe operacje to `enqueue` (dodaj na koniec) i `dequeue` (pobierz z początku).

*   **Drzewo (Tree):** Hierarchiczna struktura danych składająca się z węzłów połączonych krawędziami. Ma jeden wyróżniony węzeł (korzeń) i każdy węzeł (oprócz korzenia) ma dokładnie jednego rodzica. Szczególnym przypadkiem jest **drzewo binarne**, gdzie każdy węzeł ma co najwyżej dwoje dzieci.

*   **Graf (Graph):** Uogólnienie drzewa. Zbiór wierzchołków połączonych krawędziami. W przeciwieństwie do drzewa, nie ma wyróżnionego korzenia i może zawierać cykle.

---

# 36. Algorytmy sortowania: bąbelkowe, przez wstawianie, przez wybór, szybkie, przez scalanie

**1. Sortowanie Bąbelkowe (Bubble Sort):**

*   **Złożoność:** O(n²)
*   **Idea:** Wielokrotnie przechodzi przez listę, porównując sąsiednie elementy i zamieniając je miejscami, jeśli są w złej kolejności. "Cięższe" elementy "opadają" na koniec, a "lżejsze" "wypływają" na początek. Prosty, ale bardzo niewydajny.

**2. Sortowanie przez Wstawianie (Insertion Sort):**

*   **Złożoność:** O(n²)
*   **Idea:** Dzieli listę na część posortowaną i nieposortowaną. Bierze kolejne elementy z części nieposortowanej i wstawia je w odpowiednie miejsce w części posortowanej. Efektywny dla małych i częściowo posortowanych zbiorów.

**3. Sortowanie przez Wybór (Selection Sort):**

*   **Złożoność:** O(n²)
*   **Idea:** Wielokrotnie przechodzi przez nieposortowaną część listy, znajduje najmniejszy element i zamienia go z pierwszym elementem tej części. Prosty, ale niewydajny.

**4. Sortowanie Szybkie (Quicksort):**

*   **Złożoność:** Średnio O(n log n), najgorszy przypadek O(n²)
*   **Idea:** Działa na zasadzie "dziel i zwyciężaj". Wybiera element zwany **pivotem**, a następnie dzieli resztę elementów na dwie grupy: mniejsze od pivota i większe od pivota. Następnie rekurencyjnie sortuje obie grupy. Jeden z najszybszych algorytmów sortowania w praktyce.

**5. Sortowanie przez Scalanie (Merge Sort):**

*   **Złożoność:** Zawsze O(n log n)
*   **Idea:** Również działa na zasadzie "dziel i zwyciężaj". Rekurencyjnie dzieli listę na pół, aż do uzyskania jednoelementowych list. Następnie scala posortowane połówki w jedną, większą posortowaną listę. Jest stabilny i ma gwarantowaną złożoność, ale wymaga dodatkowej pamięci.

---

# 37. Algorytmy wyszukiwania: liniowe, binarne

**1. Wyszukiwanie Liniowe (Linear Search):**

*   **Złożoność:** O(n)
*   **Wymagania:** Brak – działa na **nieposortowanych** danych.
*   **Idea:** Najprostszy możliwy algorytm. Polega na sprawdzaniu kolejno każdego elementu w kolekcji, aż do znalezienia szukanego elementu lub do końca kolekcji.

**2. Wyszukiwanie Binarne (Binary Search):**

*   **Złożoność:** O(log n)
*   **Wymagania:** Dane **muszą być posortowane**.
*   **Idea:** Działa na zasadzie "dziel i zwyciężaj". Porównuje szukany element z elementem środkowym w kolekcji.
    *   Jeśli są równe – element znaleziony.
    *   Jeśli szukany element jest mniejszy – odrzuca prawą połowę kolekcji i kontynuuje wyszukiwanie w lewej.
    *   Jeśli szukany element jest większy – odrzuca lewą połowę i kontynuuje w prawej.
*   Jest to znacznie wydajniejszy algorytm niż wyszukiwanie liniowe, ale wymaga uprzedniego posortowania danych.

---

# 38. Algorytmy grafowe: przeszukiwanie wszerz i w głąb, algorytm Dijkstry, algorytmy Kruskala i Prima

**1. Przeszukiwanie Wszerz (BFS - Breadth-First Search):**

*   **Idea:** Zaczyna od wierzchołka startowego i eksploruje graf "warstwami". Najpierw odwiedza wszystkich sąsiadów wierzchołka startowego, potem sąsiadów tych sąsiadów, i tak dalej. Używa **kolejki** do przechowywania wierzchołków do odwiedzenia.
*   **Zastosowanie:** Znajdowanie najkrótszej ścieżki w grafie nieważonym.

**2. Przeszukiwanie w Głąb (DFS - Depth-First Search):**

*   **Idea:** Zaczyna od wierzchołka startowego i eksploruje graf, idąc tak daleko, jak to możliwe wzdłuż jednej ścieżki, zanim zawróci. Używa **stosu** (często niejawnie, poprzez rekurencję) do przechowywania wierzchołków.
*   **Zastosowanie:** Wykrywanie cykli w grafie, sortowanie topologiczne.

**3. Algorytm Dijkstry:**

*   **Cel:** Znajdowanie **najkrótszej ścieżki** od jednego wierzchołka startowego do wszystkich pozostałych w **grafie ważonym z nieujemnymi wagami**.
*   **Idea:** Działa zachłannie. Utrzymuje zbiór wierzchołków, do których zna już najkrótszą ścieżkę. W każdym kroku wybiera wierzchołek spoza tego zbioru, do którego prowadzi najkrótsza znana ścieżka, i dodaje go do zbioru, aktualizując odległości do jego sąsiadów.

**4. Algorytmy Kruskala i Prima:**

*   **Cel:** Znajdowanie **Minimalnego Drzewa Rozpinającego (MST)** w spójnym, nieważonym grafie nieskierowanym. MST to podgraf, który łączy wszystkie wierzchołki, nie zawiera cykli i ma minimalną możliwą sumę wag krawędzi.
*   **Algorytm Prima:** Działa podobnie do Dijkstry. Zaczyna od jednego wierzchołka i w każdym kroku "dokleja" do rosnącego drzewa najtańszą krawędź prowadzącą do wierzchołka spoza drzewa.
*   **Algorytm Kruskala:** Sortuje wszystkie krawędzie w grafie od najtańszej do najdroższej. Następnie przechodzi przez posortowane krawędzie i dodaje każdą do drzewa, pod warunkiem, że nie tworzy ona cyklu.

---

# 39. Klasy złożoności P i NP, problemy NP-zupełne

**1. Klasa P (Polynomial):**

*   **Definicja:** Zbiór **problemów decyzyjnych** (odpowiedź TAK/NIE), które można rozwiązać za pomocą deterministycznej maszyny Turinga w **czasie wielomianowym** (np. O(n), O(n²), O(n³)).
*   **Intuicja:** Są to problemy "łatwe" lub "obliczalnie trakcyjne", dla których znamy **efektywne algorytmy**.
*   **Przykłady:** Sortowanie, wyszukiwanie binarne, znajdowanie najkrótszej ścieżki.

**2. Klasa NP (Nondeterministic Polynomial):**

*   **Definicja:** Zbiór problemów decyzyjnych, dla których **weryfikacja** proponowanego rozwiązania (certyfikatu) może być wykonana w czasie wielomianowym.
*   **Intuicja:** Jeśli ktoś da nam rozwiązanie problemu z klasy NP, jesteśmy w stanie **szybko sprawdzić, czy jest ono poprawne**. Nie oznacza to jednak, że potrafimy to rozwiązanie szybko znaleźć.
*   **Przykłady:** Problem komiwojażera (wersja decyzyjna: "Czy istnieje trasa o długości mniejszej niż X?"), problem kolorowania grafu.

**3. Problem P vs NP:**

*   To najważniejszy nierozwiązany problem w informatyce. Pytanie brzmi: **Czy P = NP?**
*   Wiadomo, że **P ⊆ NP** (każdy problem, który da się szybko rozwiązać, da się też szybko zweryfikować).
*   Pytanie brzmi, czy istnieje jakikolwiek problem w NP, który nie należy do P. Powszechnie uważa się, że **P ≠ NP**, ale nikt nie potrafi tego udowodnić.

**4. Problemy NP-zupełne (NP-Complete):**

*   **Definicja:** To **najtrudniejsze problemy w klasie NP**. Mają dwie właściwości:
    1.  Należą do klasy NP.
    2.  Każdy inny problem z klasy NP można do nich **zredukować** w czasie wielomianowym (czyli sprowadzić do ich postaci).
*   **Znaczenie:** Jeśli ktoś znalazłby efektywny (wielomianowy) algorytm dla **jakiegokolwiek** problemu NP-zupełnego, oznaczałoby to, że potrafimy efektywnie rozwiązać **wszystkie** problemy z klasy NP, a co za tym idzie, że P = NP.
*   **Przykłady:** Problem komiwojażera (TSP), problem spełnialności formuł logicznych (SAT), problem plecakowy.

---

# 40. Grafika rastrowa i wektorowa, modele barw

**1. Grafika Rastrowa (Bitmapowa):**

*   **Idea:** Obraz jest reprezentowany jako **siatka pikseli** (prostokątna tablica punktów). Każdy piksel ma przypisany konkretny kolor.
*   **Cechy:**
    *   **Skalowanie:** Słabo się skaluje. Powiększanie obrazu prowadzi do utraty jakości i widocznej "pikselozy".
    *   **Rozmiar pliku:** Zależy od wymiarów obrazu i głębi kolorów, a nie od jego zawartości. Duże obrazy zajmują dużo miejsca.
*   **Zastosowanie:** Fotografie, skomplikowane obrazy z płynnymi przejściami tonalnymi.
*   **Formaty:** JPG, PNG, GIF, BMP.

**2. Grafika Wektorowa:**

*   **Idea:** Obraz jest opisywany za pomocą **obiektów geometrycznych** (linii, krzywych, wielokątów) zdefiniowanych przez wzory matematyczne.
*   **Cechy:**
    *   **Skalowanie:** Doskonale się skaluje. Obraz można dowolnie powiększać i pomniejszać bez żadnej utraty jakości.
    *   **Rozmiar pliku:** Zależy od złożoności obrazu (liczby obiektów), a nie od jego wymiarów.
*   **Zastosowanie:** Logotypy, ikony, diagramy, ilustracje, czcionki.
*   **Formaty:** SVG, AI, EPS, PDF.

**3. Modele Barw:**

To matematyczne sposoby reprezentacji kolorów za pomocą liczb.

*   **Model RGB (Red, Green, Blue):**
    *   **Typ:** Addytywny (dodawanie światła).
    *   **Idea:** Kolor powstaje przez mieszanie trzech podstawowych barw światła: czerwonej, zielonej i niebieskiej. (0,0,0) to czerń, (255,255,255) to biel.
    *   **Zastosowanie:** Wyświetlacze cyfrowe (monitory, telewizory, ekrany smartfonów).

*   **Model CMYK (Cyan, Magenta, Yellow, Key/Black):**
    *   **Typ:** Subtraktywny (odejmowanie światła).
    *   **Idea:** Kolor powstaje przez mieszanie farb (pigmentów), które pochłaniają (odejmują) pewne składowe światła białego. Teoretycznie mieszanina C, M, Y powinna dać czerń, ale w praktyce daje brudny brąz, dlatego dodaje się czarny pigment (K).
    *   **Zastosowanie:** Druk.

---

# 41. Interfejsy użytkownika, interakcja człowiek-komputer, podstawowe zasady projektowania interfejsów

**1. Czym jest interfejs użytkownika (UI - User Interface)?**

To **punkt styku** między człowiekiem a maszyną (komputerem, aplikacją). Jest to wszystko, co użytkownik widzi, słyszy i z czym może wejść w interakcję, aby osiągnąć swój cel.

*   **Rodzaje UI:**
    *   **CLI (Command-Line Interface):** Interfejs tekstowy, oparty na poleceniach (np. terminal w Linuksie).
    *   **GUI (Graphical User Interface):** Interfejs graficzny, oparty na elementach wizualnych, takich jak okna, ikony, menu, przyciski (np. Windows, macOS).
    *   **VUI (Voice User Interface):** Interfejs głosowy (np. Siri, Alexa).

**2. Czym jest interakcja człowiek-komputer (HCI - Human-Computer Interaction)?**

To **dziedzina nauki**, która bada, projektuje i ocenia interfejsy użytkownika. Celem HCI jest tworzenie systemów, które są **użyteczne, bezpieczne i satysfakcjonujące** w użyciu. HCI łączy w sobie informatykę, psychologię, projektowanie i socjologię.

**3. Czym jest User Experience (UX)?**

To **całkowite doświadczenie i odczucia** użytkownika podczas interakcji z produktem lub usługą. UI jest tylko częścią UX. UX obejmuje również użyteczność, dostępność, wydajność, a nawet emocje, jakie produkt wywołuje.

**4. Jakie są podstawowe zasady projektowania interfejsów (Heurystyki Nielsena)?**

To 10 ogólnych zasad, które pomagają tworzyć dobre interfejsy:

1.  **Pokazuj status systemu:** Użytkownik zawsze powinien wiedzieć, co się dzieje (np. pasek postępu).
2.  **Zachowaj zgodność między systemem a rzeczywistością:** Używaj języka i pojęć zrozumiałych dla użytkownika.
3.  **Daj użytkownikowi pełną kontrolę:** Zawsze powinna być możliwość cofnięcia operacji ("wyjście awaryjne").
4.  **Trzymaj się standardów i konwencji:** Elementy, które wyglądają tak samo, powinny działać tak samo.
5.  **Zapobiegaj błędom:** Lepiej jest zaprojektować interfejs tak, aby błędy były trudne do popełnienia, niż tworzyć dobre komunikaty o błędach.
6.  **Pozwalaj wybierać zamiast zmuszać do pamiętania:** Elementy i opcje powinny być widoczne.
7.  **Zapewnij elastyczność i efektywność:** Zapewnij skróty klawiszowe dla zaawansowanych użytkowników.
8.  **Dbaj o estetykę i minimalizm:** Interfejs nie powinien zawierać zbędnych informacji.
9.  **Zapewnij zrozumiałe komunikaty o błędach:** Komunikat powinien jasno mówić, co się stało i jak rozwiązać problem.
10. **Zapewnij pomoc i dokumentację:** Pomoc powinna być łatwa do znalezienia i przeszukiwania.

---

# 42. Inżynieria wymagań: proces, wymagania funkcjonalne i niefunkcjonalne

**1. Czym jest inżynieria wymagań?**

To **systematyczny proces** definiowania, dokumentowania i zarządzania wymaganiami dla systemu oprogramowania. Jest to kluczowy etap w cyklu życia oprogramowania, ponieważ błędy popełnione na tym etapie są najdroższe w naprawie.

**2. Jakie są etapy procesu inżynierii wymagań?**

1.  **Pozyskiwanie (Elicitation):** Zbieranie wymagań od interesariuszy (klientów, użytkowników) za pomocą wywiadów, warsztatów, ankiet, obserwacji.
2.  **Analiza:** Zrozumienie zebranych wymagań, rozwiązywanie konfliktów między nimi, negocjowanie priorytetów.
3.  **Specyfikacja:** Precyzyjne i jednoznaczne udokumentowanie wymagań w dokumencie (np. SRS - Software Requirements Specification).
4.  **Walidacja:** Sprawdzenie, czy udokumentowane wymagania rzeczywiście odpowiadają potrzebom klienta i czy są spójne i kompletne.
5.  **Zarządzanie:** Kontrolowanie zmian w wymaganiach w trakcie trwania projektu.

**3. Czym są wymagania funkcjonalne?**

Opisują, **co system ma robić**. Definiują **funkcje, zadania i zachowania** systemu.

*   **Przykłady:**
    *   "System musi pozwalać użytkownikowi na zalogowanie się za pomocą adresu e-mail i hasła."
    *   "Użytkownik musi mieć możliwość dodania produktu do koszyka."
    *   "System powinien generować raport sprzedaży w formacie PDF."

**4. Czym są wymagania niefunkcjonalne?**

Opisują, **jak system ma coś robić**. Definiują **jakość, atrybuty i ograniczenia** systemu. Nie dotyczą konkretnych funkcji, ale ogólnych właściwości.

*   **Kategorie i przykłady:**
    *   **Wydajność:** "Strona główna musi załadować się w czasie poniżej 2 sekund."
    *   **Niezawodność:** "System musi być dostępny przez 99.9% czasu."
    *   **Bezpieczeństwo:** "Hasła użytkowników muszą być haszowane za pomocą algorytmu bcrypt."
    *   **Użyteczność:** "Nowy użytkownik powinien być w stanie dokonać zakupu w czasie poniżej 5 minut bez szkolenia."
    *   **Przenośność:** "Aplikacja musi działać na systemach Windows 10 i macOS."

---

# 43. Wzorce projektowe: kreacyjne, strukturalne i behawioralne (pojęcia i przykłady)

**1. Czym jest wzorzec projektowy?**

To **sprawdzone, powtarzalne rozwiązanie** typowego problemu projektowego w oprogramowaniu. To nie jest gotowy kod, ale **opis lub szablon**, który można dostosować do konkretnej sytuacji. Wzorce dostarczają wspólnego języka dla programistów.

**2. Wzorce Kreacyjne:**

*   **Cel:** Zajmują się **procesem tworzenia obiektów**. Pozwalają uniezależnić system od tego, jak jego obiekty są tworzone, komponowane i reprezentowane.
*   **Przykłady:**
    *   **Singleton:** Gwarantuje, że klasa ma **tylko jedną instancję** i zapewnia globalny punkt dostępu do niej (np. obiekt połączenia z bazą danych, menedżer logowania).
    *   **Fabryka (Factory Method):** Definiuje interfejs do tworzenia obiektu, ale pozwala podklasom decydować, którą konkretnie klasę utworzyć. Przenosi odpowiedzialność za tworzenie obiektów do podklas.
    *   **Budowniczy (Builder):** Pozwala na konstruowanie złożonych obiektów krok po kroku. Umożliwia tworzenie różnych reprezentacji tego samego obiektu przy użyciu tego samego procesu budowania (np. budowanie różnych konfiguracji komputera).

**3. Wzorce Strukturalne:**

*   **Cel:** Zajmują się **kompozycją klas i obiektów** w większe struktury. Ułatwiają projektowanie, identyfikując proste sposoby realizacji relacji między obiektami.
*   **Przykłady:**
    *   **Adapter:** Pozwala na współpracę obiektów o **niekompatybilnych interfejsach**. Działa jak przejściówka, tłumacząc wywołania z jednego interfejsu na drugi.
    *   **Dekorator:** Pozwala na **dynamiczne dodawanie nowych funkcjonalności** do obiektu bez modyfikowania jego klasy. "Owijamy" obiekt w kolejne warstwy dekoratorów, z których każda dodaje coś od siebie.
    *   **Fasada:** Dostarcza **uproszczony interfejs** do złożonego podsystemu. Ukrywa skomplikowane zależności i logikę, udostępniając prostą "fasadę", z którą klient może pracować.

**4. Wzorce Behawioralne (Czynnościowe):**

*   **Cel:** Zajmują się **algorytmami i podziałem odpowiedzialności** między obiektami. Opisują wzorce komunikacji między obiektami.
*   **Przykłady:**
    *   **Strategia:** Definiuje rodzinę algorytmów, umieszcza każdy z nich w osobnej klasie i sprawia, że stają się one wymienialne. Pozwala klientowi wybrać, którego algorytmu chce użyć w czasie działania programu (np. różne strategie sortowania, różne metody płatności).
    *   **Obserwator (Observer):** Definiuje relację "jeden do wielu" między obiektami. Gdy stan jednego obiektu (obserwowanego) się zmienia, wszystkie zależne od niego obiekty (obserwatorzy) są automatycznie powiadamiane i aktualizowane.
    *   **Polecenie (Command):** Zamienia żądanie w samodzielny obiekt, który zawiera wszystkie informacje o tym żądaniu. Pozwala na parametryzację obiektów żądaniami, kolejkowanie operacji, a także implementację mechanizmu `undo`.

---

# 44. Testowanie oprogramowania: poziomy testów, techniki czarno- i białoskrzynkowe

**1. Czym jest testowanie oprogramowania?**

To proces **weryfikacji i walidacji** oprogramowania, którego celem jest znalezienie błędów i ocena, czy system spełnia zdefiniowane wymagania. Testowanie nie może udowodnić braku błędów, a jedynie ich istnienie.

**2. Jakie są poziomy testów?**

Testy można podzielić na poziomy w zależności od tego, jak dużą część systemu obejmują (od najmniejszej do największej):

*   **Testy jednostkowe (Unit Tests):**
    *   **Co testują?** Najmniejsze, izolowane fragmenty kodu – pojedyncze funkcje, metody lub klasy.
    *   **Kto pisze?** Zazwyczaj programiści.

*   **Testy integracyjne (Integration Tests):**
    *   **Co testują?** Współpracę między kilkoma modułami lub komponentami systemu. Sprawdzają, czy połączone ze sobą jednostki działają poprawnie.

*   **Testy systemowe (System Tests):**
    *   **Co testują?** Cały, zintegrowany system jako całość. Weryfikują, czy system spełnia wymagania funkcjonalne i niefunkcjonalne.

*   **Testy akceptacyjne (Acceptance Tests):**
    *   **Co testują?** Sprawdzają, czy system spełnia potrzeby biznesowe klienta i czy jest gotowy do wdrożenia. Często wykonywane przez klienta lub użytkowników końcowych (UAT - User Acceptance Testing).

**3. Czym są techniki czarnoskrzynkowe (black-box)?**

*   **Idea:** Tester traktuje oprogramowanie jak "czarną skrzynkę". **Nie zna wewnętrznej struktury ani kodu** programu. Testy są projektowane wyłącznie na podstawie **specyfikacji i wymagań**.
*   **Cel:** Sprawdzenie, **czy** system robi to, co miał robić.
*   **Techniki:**
    *   **Partycjonowanie równoważności:** Dzielenie danych wejściowych na klasy (partycje), z których wszystkie dane powinny być traktowane tak samo. Testuje się po jednym reprezentancie z każdej klasy.
    *   **Analiza wartości brzegowych:** Testowanie na krawędziach partycji, ponieważ tam najczęściej występują błędy (np. dla zakresu [1, 100] testujemy 0, 1, 100, 101).

**4. Czym są techniki białoskrzynkowe (white-box)?**

*   **Idea:** Tester **zna wewnętrzną strukturę i kod** programu. Testy są projektowane tak, aby sprawdzić logikę i ścieżki wykonania w kodzie.
*   **Cel:** Sprawdzenie, **jak** system coś robi i czy robi to poprawnie.
*   **Techniki:**
    *   **Pokrycie instrukcji:** Zaprojektowanie testów tak, aby każda linia kodu została wykonana co najmniej raz.
    *   **Pokrycie decyzji/gałęzi:** Zaprojektowanie testów tak, aby każdy możliwy wynik instrukcji warunkowej (prawda/fałsz) został sprawdzony co najmniej raz.

---

# 45. Systemy kontroli wersji, Git, GitHub

**1. Czym jest system kontroli wersji (VCS - Version Control System)?**

To oprogramowanie, które **śledzi i zarządza zmianami w kodzie źródłowym** w czasie. Pozwala wielu programistom na jednoczesną pracę nad tym samym projektem bez wchodzenia sobie w drogę.

**2. Jakie są jego główne korzyści?**

*   **Historia zmian:** Rejestruje każdą zmianę, kto ją wprowadził, kiedy i dlaczego. Pozwala to na powrót do dowolnej poprzedniej wersji projektu.
*   **Praca zespołowa:** Umożliwia łączenie (merge) zmian wprowadzonych przez różnych programistów.
*   **Rozgałęzianie (Branching):** Pozwala na tworzenie osobnych "gałęzi" deweloperskich do pracy nad nowymi funkcjami lub eksperymentami, bez wpływu na główną, stabilną wersję kodu.

**3. Czym jest Git?**

*   To **rozproszony system kontroli wersji (DVCS)**. Jest to obecnie najpopularniejszy VCS na świecie.
*   **Rozproszony** oznacza, że każdy programista ma na swoim komputerze **pełną kopię całego repozytorium**, włącznie z całą jego historią. Pozwala to na pracę w trybie offline i jest bardziej odporne na awarie centralnego serwera.
*   **Podstawowe polecenia:** `git clone`, `git add`, `git commit`, `git push`, `git pull`, `git branch`, `git merge`.

**4. Czym jest GitHub?**

*   To **platforma internetowa**, która świadczy usługę **hostingu repozytoriów Git**. To nie jest to samo co Git!
*   **Git** to narzędzie działające lokalnie na komputerze.
*   **GitHub** to serwis w chmurze, który przechowuje te repozytoria i dodaje do nich wiele funkcji ułatwiających współpracę:
    *   **Pull Requests:** Mechanizm proponowania zmian w projekcie i prowadzenia dyskusji (code review) na ich temat przed włączeniem ich do głównej gałęzi.
    *   **Issues:** System do śledzenia zadań, błędów i pomysłów.
    *   **GitHub Actions:** Narzędzie do automatyzacji procesów (CI/CD).
    *   **Funkcje społecznościowe:** Obserwowanie projektów, forkowanie (tworzenie własnej kopii) repozytoriów.
*   **Alternatywy dla GitHuba:** GitLab, Bitbucket.

---

# 46. Konteneryzacja, Docker

**1. Czym jest konteneryzacja?**

To technologia wirtualizacji na poziomie **systemu operacyjnego**, która pozwala na uruchamianie aplikacji i ich zależności w **izolowanych środowiskach zwanych kontenerami**. Wszystkie kontenery działają na tym samym jądrze systemu operacyjnego gospodarza.

**2. Czym różni się od maszyn wirtualnych (VM)?**

*   **Maszyna wirtualna:** Wirtualizuje **cały sprzęt**. Każda VM ma swój własny, pełny system operacyjny (guest OS). Są ciężkie, wolno się uruchamiają i zużywają dużo zasobów.
*   **Kontener:** Wirtualizuje **system operacyjny**. Kontenery współdzielą jądro systemu gospodarza. Są lekkie, szybkie i zużywają znacznie mniej zasobów.

**3. Czym jest Docker?**

To **platforma do konteneryzacji**, która spopularyzowała tę technologię. Upraszcza ona proces tworzenia, uruchamiania i zarządzania kontenerami.

**4. Jakie są kluczowe pojęcia w Dockerze?**

*   **Obraz (Image):** To **szablon tylko do odczytu**, który zawiera wszystko, co jest potrzebne do uruchomienia aplikacji: kod, biblioteki, zależności, zmienne środowiskowe. Obrazy są budowane na podstawie pliku tekstowego zwanego `Dockerfile`.

*   **Kontener (Container):** To **uruchomiona instancja obrazu**. Jest to lekkie, izolowane środowisko, w którym działa aplikacja. Można tworzyć, uruchamiać, zatrzymywać i usuwać wiele kontenerów z tego samego obrazu.

*   **Dockerfile:** To **plik tekstowy z instrukcjami**, który opisuje, jak zbudować obraz Dockera krok po kroku (np. z jakiego obrazu bazowego skorzystać, jakie pliki skopiować, jakie polecenia wykonać).

*   **Docker Hub / Registry:** To **repozytorium obrazów**. Docker Hub to publiczne, centralne repozytorium, z którego można pobierać gotowe obrazy (np. `ubuntu`, `python`, `postgres`).

**5. Jakie są główne korzyści z konteneryzacji?**

*   **Przenośność:** Kontener działa tak samo na laptopie dewelopera, na serwerze testowym i w chmurze produkcyjnej ("działa na moim komputerze" przestaje być problemem).
*   **Spójność środowiska:** Zapewnia, że środowisko deweloperskie i produkcyjne są identyczne.
*   **Szybkość i wydajność:** Kontenery uruchamiają się w ułamku sekundy i mają minimalny narzut wydajnościowy.
*   **Izolacja:** Aplikacje działające w kontenerach są od siebie odizolowane.
*   **Mikroserwisy:** Konteneryzacja jest idealną technologią do budowania i wdrażania aplikacji opartych na architekturze mikroserwisów.

---

# 47. Metodyki zwinne (Agile), Scrum, Kanban

**1. Czym są metodyki zwinne (Agile)?**

To **grupa iteracyjnych i przyrostowych metodyk** wytwarzania oprogramowania, które kładą nacisk na **elastyczność, współpracę i szybkie dostarczanie wartości**. Są one odpowiedzią na ograniczenia tradycyjnych, sztywnych modeli (jak model kaskadowy). Agile to bardziej **filozofia i zbiór zasad** (opisanych w Manifeście Agile) niż jedna konkretna metodyka.

**2. Jakie są kluczowe zasady Agile?**

*   Ludzie i interakcje ponad procesy i narzędzia.
*   Działające oprogramowanie ponad obszerną dokumentację.
*   Współpraca z klientem ponad formalne negocjacje.
*   Reagowanie na zmiany ponad podążanie za planem.

**3. Czym jest Scrum?**

To **framework (szkielet procesowy)** do zarządzania projektami, który implementuje zasady Agile. Jest to obecnie najpopularniejsza metodyka zwinna.

*   **Kluczowe elementy Scruma:**
    *   **Role:**
        *   **Product Owner:** Odpowiada za wizję produktu i zarządzanie backlogiem produktu. Reprezentuje interesy klienta.
        *   **Scrum Master:** Dba o to, by zespół przestrzegał zasad Scruma, usuwa przeszkody i facylituje proces.
        *   **Development Team:** Samoorganizujący się zespół, który realizuje pracę.
    *   **Artefakty:**
        *   **Product Backlog:** Uporządkowana lista wszystkiego, co ma być zrobione w produkcie.
        *   **Sprint Backlog:** Zbiór zadań z backlogu produktu wybranych do realizacji w danym sprincie.
    *   **Wydarzenia (Ceremonie):**
        *   **Sprint:** Krótki, stały okres (zwykle 2-4 tygodnie), w którym zespół tworzy działający przyrost produktu.
        *   **Sprint Planning:** Planowanie pracy na nadchodzący sprint.
        *   **Daily Scrum:** Codzienne, 15-minutowe spotkanie zespołu w celu synchronizacji pracy.
        *   **Sprint Review:** Prezentacja działającego przyrostu produktu interesariuszom.
        *   **Sprint Retrospective:** Spotkanie zespołu w celu inspekcji i adaptacji procesu pracy.

**4. Czym jest Kanban?**

To inna metodyka zwinna, która koncentruje się na **wizualizacji przepływu pracy i ograniczaniu pracy w toku (WIP - Work In Progress)**.

*   **Kluczowe elementy Kanbana:**
    *   **Tablica Kanban:** Wizualna reprezentacja przepływu pracy, podzielona na kolumny odpowiadające kolejnym etapom (np. `Do zrobienia`, `W trakcie`, `Zrobione`). Zadania są reprezentowane przez karteczki, które przesuwają się po tablicy.
    *   **Limity WIP:** Każda kolumna (oprócz pierwszej i ostatniej) ma nałożony limit, ile zadań może się w niej jednocześnie znajdować. Zmusza to zespół do kończenia rozpoczętej pracy, zanim zacznie nową, co eliminuje wąskie gardła i poprawia przepływ.
*   **Różnica w stosunku do Scruma:** Kanban jest bardziej elastyczny. Nie ma w nim zdefiniowanych ról ani stałych iteracji (sprintów). Jest to proces ciągły, zorientowany na przepływ.

---

# 48. Ciągła integracja i ciągłe dostarczanie (CI/CD), Jenkins, GitHub Actions

**1. Czym jest Ciągła Integracja (CI - Continuous Integration)?**

To praktyka deweloperska polegająca na tym, że programiści **często (przynajmniej raz dziennie) integrują swoje zmiany w kodzie** do wspólnego repozytorium. Każda taka integracja jest **automatycznie weryfikowana** przez proces budowania i uruchamiania testów jednostkowych.

*   **Cel:** Wczesne wykrywanie błędów integracyjnych, poprawa jakości kodu i unikanie problemów związanych z łączeniem dużych zmian na późnym etapie.

**2. Czym jest Ciągłe Dostarczanie (CD - Continuous Delivery)?**

To rozszerzenie Ciągłej Integracji. Polega na tym, że każda zmiana, która pomyślnie przejdzie przez proces CI, jest **automatycznie przygotowywana do wdrożenia na produkcję**. Oznacza to, że kod jest budowany, testowany (na różnych poziomach) i pakowany w taki sposób, że jest **gotowy do wdrożenia w każdej chwili za naciśnięciem jednego przycisku**.

**3. Czym jest Ciągłe Wdrażanie (CD - Continuous Deployment)?**

To kolejny krok po Ciągłym Dostarczaniu. Polega na tym, że każda zmiana, która pomyślnie przejdzie wszystkie etapy testów, jest **automatycznie wdrażana na produkcję bez żadnej ręcznej interwencji**.

**4. Jak wygląda typowy potok (pipeline) CI/CD?**

1.  **Commit:** Programista wysyła zmiany do repozytorium (np. `git push`).
2.  **Build:** Serwer CI automatycznie pobiera kod i go kompiluje/buduje.
3.  **Test:** Uruchamiane są automatyczne testy (jednostkowe, integracyjne).
4.  **Deploy (to Staging):** Jeśli testy przejdą pomyślnie, aplikacja jest wdrażana na środowisko testowe (staging).
5.  **Further Testing:** Uruchamiane są kolejne testy (np. systemowe, akceptacyjne).
6.  **Deploy (to Production):** Po pomyślnym przejściu wszystkich testów, zmiana jest wdrażana na produkcję (ręcznie w Continuous Delivery, automatycznie w Continuous Deployment).

**5. Jakie narzędzia to realizują?**

*   **Jenkins:** To bardzo popularny, open-source'owy serwer automatyzacji, który działa jako silnik CI/CD. Jest bardzo elastyczny i ma ogromną liczbę wtyczek, ale jego konfiguracja może być skomplikowana.

*   **GitHub Actions:** To narzędzie CI/CD wbudowane bezpośrednio w platformę GitHub. Pozwala na definiowanie potoków automatyzacji za pomocą plików YAML bezpośrednio w repozytorium. Jest łatwiejszy w użyciu i dobrze zintegrowany z ekosystemem GitHuba.

---

# 49. Architektura i usługi sieci Internet

**1. Jaka jest architektura Internetu?**

Internet to **globalna sieć sieci** ("internetwork"), która łączy miliony sieci prywatnych, publicznych, akademickich i rządowych. Jest to sieć **zdecentralizowana**, bez centralnego punktu zarządzania.

*   **Architektura oparta na przełączaniu pakietów:** Dane są dzielone na małe części zwane **pakietami**. Każdy pakiet jest przesyłany przez sieć niezależnie i może podążać inną trasą. Routery po drodze decydują, którędy przesłać dany pakiet.
*   **Model warstwowy TCP/IP:** Komunikacja opiera się na zestawie protokołów TCP/IP, który definiuje cztery warstwy (Aplikacji, Transportu, Internetu, Dostępu do sieci).

**2. Jakie są kluczowe protokoły?**

*   **IP (Internet Protocol):** Działa w warstwie Internetu. Odpowiada za **adresowanie logiczne** i **routing** pakietów między sieciami. Jest protokołem "zawodnym" i "bezpołączeniowym" – nie gwarantuje, że pakiety dotrą do celu, ani w jakiej kolejności.
*   **TCP (Transmission Control Protocol):** Działa w warstwie Transportu. Zapewnia **niezawodną, połączeniową** transmisję danych. Gwarantuje, że wszystkie pakiety dotrą do celu w odpowiedniej kolejności i bez błędów. Używany tam, gdzie liczy się niezawodność (np. przeglądanie stron WWW, e-mail).
*   **UDP (User Datagram Protocol):** Działa w warstwie Transportu. Zapewnia **szybką, bezpołączeniową** transmisję. Nie gwarantuje dostarczenia ani kolejności pakietów. Używany tam, gdzie liczy się szybkość, a nie niezawodność (np. streaming wideo, gry online, DNS).

**3. Jakie są podstawowe usługi sieci Internet?**

Usługi to aplikacje działające na bazie tej architektury, z których korzystają użytkownicy.

*   **World Wide Web (WWW):** System połączonych ze sobą dokumentów hipertekstowych (stron internetowych), dostępnych za pomocą protokołu HTTP/HTTPS.
*   **Poczta elektroniczna (E-mail):** Usługa przesyłania wiadomości, oparta na protokołach SMTP, POP3 i IMAP.
*   **System nazw domenowych (DNS):** Usługa tłumacząca nazwy domenowe na adresy IP.
*   **Transfer plików (FTP):** Usługa przesyłania plików.
*   **Usługi czasu rzeczywistego:** Telefonia internetowa (VoIP), wideokonferencje, gry online.

---

# 50. Podstawowe pojęcia z zakresu bezpieczeństwa IT: zagrożenie, podatność, ryzyko, polityka bezpieczeństwa

**1. Zagrożenie (Threat):**

*   **Definicja:** Potencjalne zdarzenie lub okoliczność, która może spowodować szkodę w systemie lub organizacji (np. utratę danych, przerwę w działaniu).
*   **Przykłady:** Atak hakera, wirus komputerowy, awaria sprzętu, błąd ludzki, pożar.

**2. Podatność (Vulnerability):**

*   **Definicja:** **Słabość** w systemie, procesie lub zabezpieczeniach, która może zostać wykorzystana przez zagrożenie do wyrządzenia szkody.
*   **Przykłady:** Niezałataną dziura w oprogramowaniu, słabe hasło, brak firewalla, nieprzeszkolony pracownik.

**3. Ryzyko (Risk):**

*   **Definicja:** **Prawdopodobieństwo**, że dane zagrożenie wykorzysta daną podatność i spowoduje określoną szkodę. Ryzyko łączy w sobie pojęcie zagrożenia, podatności i wpływu (konsekwencji).
*   **Wzór:** `Ryzyko = Zagrożenie * Podatność * Wpływ`
*   **Przykład:** Ryzyko utraty danych klientów w wyniku ataku ransomware wykorzystującego podatność w nieaktualnym oprogramowaniu serwera.

**4. Zarządzanie ryzykiem:**

To proces identyfikacji, oceny i reagowania na ryzyko. Możliwe reakcje to:
*   **Akceptacja:** Świadome zaakceptowanie ryzyka (gdy koszt przeciwdziałania jest zbyt wysoki).
*   **Unikanie:** Zrezygnowanie z działania, które generuje ryzyko.
*   **Transfer:** Przeniesienie ryzyka na inny podmiot (np. wykupienie ubezpieczenia).
*   **Mitygacja:** Wprowadzenie zabezpieczeń w celu zmniejszenia prawdopodobieństwa lub wpływu ryzyka.

**5. Polityka bezpieczeństwa:**

*   **Definicja:** To **formalny dokument**, który określa **cele, zasady i procedury** dotyczące bezpieczeństwa informacji w organizacji. Jest to dokument wysokiego poziomu, który stanowi podstawę do wdrażania konkretnych zabezpieczeń technicznych i organizacyjnych.
*   **Cel:** Zapewnienie, że wszyscy pracownicy rozumieją swoją rolę w ochronie zasobów firmy i postępują zgodnie z ustalonymi regułami.
*   **Przykładowe zapisy:** Polityka haseł, polityka czystego biurka, zasady korzystania z poczty elektronicznej, procedura reagowania na incydenty.

---

# 51. Kryptografia symetryczna i asymetryczna, klucz publiczny i prywatny, podpis cyfrowy

**1. Kryptografia Symetryczna (z kluczem tajnym):**

*   **Idea:** Do **szyfrowania i deszyfrowania** danych używany jest **ten sam, jeden klucz**. Klucz ten musi być tajny i znany obu stronom komunikacji.
*   **Zalety:** Bardzo **szybka** i wydajna.
*   **Wady:** **Problem dystrybucji klucza**. Jak bezpiecznie przekazać tajny klucz drugiej stronie? Jeśli ktoś przechwyci klucz, może odszyfrować całą komunikację.
*   **Algorytmy:** AES (Advanced Encryption Standard - obecny standard), DES, 3DES.
*   **Zastosowanie:** Szyfrowanie dużych ilości danych (np. plików na dysku, transmisji danych), gdy klucz został już bezpiecznie wymieniony.

**2. Kryptografia Asymetryczna (z kluczem publicznym):**

*   **Idea:** Używana jest **para kluczy**: **klucz publiczny** i **klucz prywatny**. Są one ze sobą matematycznie powiązane.
    *   **Klucz publiczny:** Może być swobodnie rozpowszechniany. Służy do **szyfrowania** danych i **weryfikacji podpisu cyfrowego**.
    *   **Klucz prywatny:** Musi być trzymany w ścisłej tajemnicy przez właściciela. Służy do **deszyfrowania** danych i **tworzenia podpisu cyfrowego**.
*   **Zalety:** Rozwiązuje problem dystrybucji klucza. Nie trzeba bezpiecznie przesyłać tajnego klucza.
*   **Wady:** Znacznie **wolniejsza** od kryptografii symetrycznej.
*   **Algorytmy:** RSA, ECC (kryptografia krzywych eliptycznych).

**3. Jak działają razem w praktyce (szyfrowanie hybrydowe)?**

Kryptografia asymetryczna jest używana do bezpiecznej wymiany klucza symetrycznego, a następnie reszta komunikacji jest szyfrowana za pomocą szybkiej kryptografii symetrycznej. Tak działa np. protokół **TLS/SSL** (kłódka w przeglądarce).

**4. Czym jest podpis cyfrowy?**

To mechanizm, który zapewnia **uwierzytelnienie, integralność i niezaprzeczalność** danych. Jest to kryptograficzny odpowiednik odręcznego podpisu.

*   **Jak działa tworzenie podpisu?**
    1.  Nadawca oblicza **skrót (hash)** z wiadomości, którą chce wysłać.
    2.  Następnie **szyfruje ten skrót za pomocą swojego klucza PRYWATNEGO**.
    3.  Zaszyfrowany skrót to właśnie podpis cyfrowy, który jest dołączany do wiadomości.

*   **Jak działa weryfikacja podpisu?**
    1.  Odbiorca otrzymuje wiadomość i podpis.
    2.  **Deszyfruje podpis za pomocą klucza PUBLICZNEGO nadawcy**, otrzymując oryginalny skrót (Skrót A).
    3.  Samodzielnie oblicza skrót z otrzymanej wiadomości (Skrót B).
    4.  Jeśli **Skrót A == Skrót B**, oznacza to, że:
        *   Wiadomość pochodzi od właściwej osoby (bo tylko ona mogła zaszyfrować skrót swoim kluczem prywatnym) - **uwierzytelnienie**.
        *   Wiadomość nie została zmieniona po drodze - **integralność**.

---

# 52. Złośliwe oprogramowanie i ataki sieciowe

**1. Złośliwe oprogramowanie (Malware):**

To ogólna nazwa na wszelkie oprogramowanie stworzone w celu szkodzenia lub kradzieży danych.

*   **Wirus:** Fragment kodu, który **dołącza się do istniejącego programu** i rozprzestrzenia się, gdy ten program jest uruchamiany. Potrzebuje "nosiciela".
*   **Robak (Worm):** **Samodzielny program**, który potrafi sam się replikować i rozprzestrzeniać przez sieć, wykorzystując luki w zabezpieczeniach. Nie potrzebuje nosiciela.
*   **Trojan (Koń trojański):** Program, który **udaje pożyteczną aplikację**, ale w tle wykonuje szkodliwe działania (np. kradnie hasła, instaluje backdoora).
*   **Ransomware:** Oprogramowanie, które **szyfruje pliki na dysku** użytkownika, a następnie żąda okupu za ich odszyfrowanie.
*   **Spyware:** Oprogramowanie szpiegujące, które potajemnie zbiera informacje o użytkowniku (np. historia przeglądania, wciśnięte klawisze - keylogger).
*   **Adware:** Oprogramowanie, które automatycznie wyświetla niechciane reklamy.

**2. Ataki sieciowe:**

*   **Ataki DoS/DDoS (Denial of Service / Distributed Denial of Service):**
    *   **Cel:** Uniemożliwienie działania usługi sieciowej (np. serwera WWW) poprzez zalanie jej ogromną ilością fałszywego ruchu. W ataku DDoS ruch pochodzi z wielu, rozproszonych komputerów (często zainfekowanych botnetem), co utrudnia obronę.

*   **Atak Man-in-the-Middle (MITM):**
    *   **Cel:** Podsłuchiwanie i modyfikowanie komunikacji między dwiema stronami.
    *   **Jak działa?** Atakujący umieszcza się "pośrodku" komunikacji, np. tworząc fałszywy hotspot Wi-Fi. Ofiary myślą, że komunikują się bezpośrednio ze sobą, a w rzeczywistości cała komunikacja przechodzi przez atakującego.

*   **Phishing:**
    *   **Cel:** Wyłudzenie poufnych informacji (danych logowania, numerów kart kredytowych).
    *   **Jak działa?** Jest to atak socjotechniczny. Atakujący wysyła fałszywą wiadomość e-mail lub SMS, która wygląda jak autentyczna komunikacja z banku, portalu społecznościowego itp. Wiadomość zawiera link do fałszywej strony, która do złudzenia przypomina prawdziwą. Użytkownik, wpisując tam swoje dane, przekazuje je atakującemu.

*   **SQL Injection:**
    *   **Cel:** Atak na aplikację webową połączoną z bazą danych.
    *   **Jak działa?** Atakujący wstrzykuje fragment złośliwego kodu SQL w dane wejściowe przesyłane do aplikacji (np. w polu formularza logowania). Jeśli aplikacja jest podatna, może to pozwolić atakującemu na wykonanie dowolnych zapytań do bazy danych (np. odczytanie wszystkich haseł, usunięcie danych).

---

# 53. Etyka w informatyce, kodeksy etyczne

**1. Czym jest etyka w informatyce?**

To dziedzina zajmująca się **analizą moralnych i społecznych skutków** wykorzystania technologii informatycznych. Dotyczy ona dylematów i problemów, przed którymi stają profesjonaliści IT w swojej pracy.

**2. Jakie są główne obszary problemowe?**

*   **Prywatność:** Gromadzenie, analiza i wykorzystywanie danych osobowych przez firmy i rządy. Kto ma prawo do naszych danych?
*   **Własność intelektualna:** Piractwo oprogramowania, prawa autorskie, patenty na algorytmy.
*   **Bezpieczeństwo:** Odpowiedzialność za tworzenie bezpiecznego oprogramowania i ochrona systemów przed atakami.
*   **Niezawodność i odpowiedzialność:** Kto ponosi odpowiedzialność za błędy w oprogramowaniu, które powodują straty finansowe lub zagrażają życiu (np. w systemach medycznych, autonomicznych pojazdach)?
*   **Sztuczna inteligencja i automatyzacja:** Wpływ AI na rynek pracy, problem stronniczości (bias) w algorytmach, etyka autonomicznej broni.
*   **Dostęp cyfrowy (Digital Divide):** Nierówności w dostępie do technologii między różnymi grupami społecznymi.

**3. Czym są kodeksy etyczne?**

To **zbiory zasad i wytycznych**, które mają pomagać informatykom w podejmowaniu etycznych decyzji. Są one tworzone przez organizacje zawodowe, aby promować odpowiedzialne i profesjonalne zachowania.

**4. Jakie są przykłady i kluczowe zasady z kodeksów etycznych (np. ACM/IEEE)?**

Najbardziej znanym jest **Kodeks Etyczny ACM (Association for Computing Machinery)**. Jego ogólne zasady moralne to:

1.  **Przyczyniaj się do rozwoju społeczeństwa i ludzkiego dobrobytu.** (Technologia ma służyć ludziom).
2.  **Unikaj wyrządzania krzywdy.** (Nadrzędna zasada - bezpieczeństwo i dobrostan publiczny są najważniejsze).
3.  **Bądź uczciwy i godny zaufania.**
4.  **Bądź sprawiedliwy i podejmuj działania, aby nie dyskryminować.** (Twórz systemy dostępne i sprawiedliwe dla wszystkich).
5.  **Szanuj pracę potrzebną do wytworzenia nowych pomysłów, wynalazków i dzieł.** (Respektuj prawa autorskie i patenty).
6.  **Szanuj prywatność.**
7.  **Szanuj poufność.**

Kodeksy te podkreślają, że odpowiedzialność informatyka wykracza poza czysto techniczne aspekty pracy i obejmuje również jej wpływ na społeczeństwo.

---

# 54. Prawne aspekty oprogramowania: prawa autorskie, patenty, licencje

**1. Prawo autorskie (Copyright):**

*   **Co chroni?** **Wyrażenie idei**, a nie samą ideę. W kontekście oprogramowania chroni **kod źródłowy i wynikowy**, a także dokumentację i elementy graficzne. Nie chroni algorytmu czy funkcjonalności jako takiej.
*   **Jak działa?** Ochrona powstaje **automatycznie** z chwilą stworzenia utworu (napisania kodu). Nie wymaga rejestracji. Daje autorowi wyłączne prawo do kopiowania, modyfikowania i rozpowszechniania swojego dzieła.
*   **Ograniczenia:** Prawo autorskie jest ograniczone w czasie (w Polsce 70 lat po śmierci autora).

**2. Patent:**

*   **Co chroni?** **Wynalazek** – czyli konkretne, nowe i nieoczywiste rozwiązanie problemu technicznego. W kontekście oprogramowania można opatentować **algorytm lub metodę działania**, jeśli są one częścią szerszego, technicznego rozwiązania.
*   **Jak działa?** Ochrona **wymaga rejestracji** w urzędzie patentowym. Jest to proces długi i kosztowny. Daje właścicielowi monopol na korzystanie z wynalazku przez określony czas (zwykle 20 lat).
*   **Kontrowersje:** Patenty na oprogramowanie są kontrowersyjne, ponieważ istnieje obawa, że hamują innowacyjność, blokując użycie fundamentalnych algorytmów.

**3. Licencja na oprogramowanie:**

*   **Czym jest?** To **umowa prawna** między właścicielem praw autorskich a użytkownikiem, która określa **warunki, na jakich użytkownik może korzystać z oprogramowania**.
*   **Rodzaje licencji:**
    *   **Licencje własnościowe (Proprietary):** Użytkownik zazwyczaj kupuje prawo do używania oprogramowania, ale nie otrzymuje dostępu do kodu źródłowego. Zabronione jest kopiowanie, modyfikowanie i redystrybucja. (Przykład: licencja na system Windows, Microsoft Office).
    *   **Licencje Wolnego i Otwartego Oprogramowania (FOSS - Free and Open Source Software):** Dają użytkownikowi cztery podstawowe wolności: uruchamiania, analizowania (dostęp do kodu źródłowego), modyfikowania i redystrybucji (zarówno w wersji oryginalnej, jak i zmodyfikowanej).
        *   **Licencje permisywne (np. MIT, BSD):** Bardzo liberalne. Pozwalają na niemal dowolne wykorzystanie kodu, w tym włączenie go do oprogramowania własnościowego. Wymagają jedynie zachowania informacji o autorze.
        *   **Licencje typu copyleft (np. GPL):** Wymagają, aby wszelkie programy pochodne (modyfikacje lub programy wykorzystujące kod na licencji GPL) były również udostępniane na tej samej licencji GPL. Zapewnia to, że oprogramowanie pozostanie "wolne".

---

# 55. Chmura obliczeniowa: modele usług (IaaS, PaaS, SaaS) i wdrożenia (prywatna, publiczna, hybrydowa)

**1. Czym jest chmura obliczeniowa (Cloud Computing)?**

To model dostarczania zasobów obliczeniowych (serwerów, pamięci masowej, baz danych, oprogramowania) **przez internet na żądanie**, w modelu "pay-as-you-go" (płacisz za to, czego używasz). Zamiast kupować i utrzymywać własną infrastrukturę, firmy mogą wynajmować ją od dostawcy chmury.

**2. Jakie są modele usług?**

Modele te różnią się poziomem abstrakcji i zakresem odpowiedzialności między klientem a dostawcą.

*   **IaaS (Infrastructure as a Service - Infrastruktura jako usługa):**
    *   **Co dostajesz?** Dostęp do **podstawowych zasobów infrastruktury**: wirtualnych serwerów, pamięci masowej, sieci. To jak wynajęcie pustego serwera.
    *   **Twoja odpowiedzialność:** Instalacja i zarządzanie systemem operacyjnym, oprogramowaniem pośredniczącym (middleware) i aplikacjami.
    *   **Przykład:** Amazon Web Services (AWS EC2), Microsoft Azure (Virtual Machines), Google Cloud (Compute Engine).

*   **PaaS (Platform as a Service - Platforma jako usługa):**
    *   **Co dostajesz?** Kompletne **środowisko do tworzenia i wdrażania aplikacji**, bez martwienia się o infrastrukturę. Dostawca zarządza systemem operacyjnym, serwerami, sieciami.
    *   **Twoja odpowiedzialność:** Zarządzanie własną aplikacją i jej danymi.
    *   **Przykład:** Heroku, AWS Elastic Beanstalk, Google App Engine.

*   **SaaS (Software as a Service - Oprogramowanie jako usługa):**
    *   **Co dostajesz?** Dostęp do **gotowej aplikacji** przez przeglądarkę internetową. Nie martwisz się o nic – ani o infrastrukturę, ani o aplikację.
    *   **Twoja odpowiedzialność:** Korzystanie z aplikacji i zarządzanie swoimi danymi w jej obrębie.
    *   **Przykład:** Google Workspace (Gmail, Docs), Microsoft 365, Salesforce, Dropbox.

**3. Jakie są modele wdrożenia?**

*   **Chmura publiczna:** Infrastruktura należy do dostawcy (np. AWS, Google, Microsoft) i jest udostępniana wielu klientom przez publiczny internet. Najbardziej popularny model.
*   **Chmura prywatna:** Infrastruktura jest dedykowana **jednej organizacji**. Może być zlokalizowana w jej własnym centrum danych lub hostowana przez zewnętrznego dostawcę. Daje większą kontrolę i bezpieczeństwo, ale jest droższa.
*   **Chmura hybrydowa:** Połączenie chmury publicznej i prywatnej. Pozwala na przenoszenie danych i aplikacji między nimi. Umożliwia np. przechowywanie wrażliwych danych w chmurze prywatnej, a mniej krytycznych aplikacji w chmurze publicznej.

---

# 56. Uczenie maszynowe: uczenie nadzorowane, nienadzorowane i ze wzmocnieniem

**1. Czym jest uczenie maszynowe (Machine Learning - ML)?**

To dziedzina sztucznej inteligencji, która polega na tworzeniu algorytmów, które potrafią **uczyć się na podstawie danych** i podejmować decyzje lub robić predykcje, bez bycia jawnie zaprogramowanymi do wykonania konkretnego zadania.

**2. Uczenie nadzorowane (Supervised Learning):**

*   **Idea:** Algorytm uczy się na **danych opatrzonych etykietami**. Oznacza to, że dla każdego przykładu w danych treningowych znamy poprawną odpowiedź.
*   **Cel:** Nauczenie się mapowania z danych wejściowych na wyjściowe, aby móc przewidywać odpowiedzi dla nowych, nieznanych danych.
*   **Typy problemów:**
    *   **Klasyfikacja:** Przewidywanie **kategorii** (etykiety dyskretnej). Przykłady: klasyfikacja e-maili jako spam/nie-spam, rozpoznawanie cyfr na obrazkach, diagnoza medyczna (chory/zdrowy).
    *   **Regresja:** Przewidywanie **wartości ciągłej**. Przykłady: prognozowanie ceny domu, przewidywanie temperatury, szacowanie kursu akcji.

**3. Uczenie nienadzorowane (Unsupervised Learning):**

*   **Idea:** Algorytm uczy się na **danych nieopatrzonych etykietami**. Nie znamy poprawnych odpowiedzi.
*   **Cel:** Odkrywanie **ukrytej struktury, wzorców i zależności** w danych.
*   **Typy problemów:**
    *   **Klastrowanie (Grupowanie):** Dzielenie danych na grupy (klastry) w taki sposób, aby obiekty w tej samej grupie były do siebie bardziej podobne niż do obiektów z innych grup. Przykład: segmentacja klientów na podstawie ich zachowań zakupowych.
    *   **Redukcja wymiarowości:** Zmniejszanie liczby zmiennych w danych przy jednoczesnym zachowaniu jak największej ilości informacji (np. PCA).
    *   **Asocjacja:** Odkrywanie reguł współwystępowania (np. "klienci, którzy kupili chleb, często kupują też masło").

**4. Uczenie ze wzmocnieniem (Reinforcement Learning):**

*   **Idea:** Algorytm (zwany **agentem**) uczy się poprzez **interakcję ze środowiskiem**. Agent podejmuje akcje, a środowisko w odpowiedzi zmienia swój stan i daje agentowi **nagrodę lub karę**.
*   **Cel:** Nauczenie się takiej **strategii (polityki)** podejmowania akcji, która maksymalizuje sumę otrzymanych nagród w długim okresie.
*   **Przykłady:** Uczenie programów do gry w szachy lub Go (AlphaGo), sterowanie robotami, optymalizacja systemów rekomendacyjnych, autonomiczna jazda.

---

# 57. Sztuczne sieci neuronowe, głębokie uczenie (deep learning)

**1. Czym jest sztuczna sieć neuronowa (ANN - Artificial Neural Network)?**

To model obliczeniowy inspirowany **strukturą i działaniem ludzkiego mózgu**. Składa się z połączonych ze sobą prostych jednostek przetwarzających zwanych **sztucznymi neuronami**, zorganizowanych w **warstwy**.

*   **Struktura:** Typowa sieć składa się z **warstwy wejściowej**, jednej lub więcej **warstw ukrytych** i **warstwy wyjściowej**.
*   **Działanie:** Każdy neuron w warstwie otrzymuje sygnały z neuronów w warstwie poprzedniej. Oblicza on sumę ważoną tych sygnałów, dodaje stałą (bias) i przepuszcza wynik przez **funkcję aktywacji**, która decyduje o sygnale wyjściowym tego neuronu.
*   **Uczenie:** Proces uczenia polega na **dostosowywaniu wag** połączeń między neuronami tak, aby sieć dla danych wejściowych generowała pożądane wyniki. Odbywa się to najczęściej za pomocą algorytmu **propagacji wstecznej błędu (backpropagation)**, który jest formą metody gradientu prostego.

**2. Czym jest głębokie uczenie (Deep Learning)?**

To poddziedzina uczenia maszynowego, która wykorzystuje **głębokie sieci neuronowe (DNN - Deep Neural Networks)** – czyli sieci neuronowe z **wieloma warstwami ukrytymi** (często dziesiątkami lub setkami).

*   **Idea:** Wiele warstw pozwala sieci na uczenie się **hierarchii cech** o rosnącym poziomie abstrakcji. Pierwsze warstwy uczą się prostych cech (np. krawędzie, kolory), a kolejne składają je w bardziej złożone koncepty (np. oczy, nos, twarze).

**3. Jakie są kluczowe architektury sieci głębokich?**

*   **Konwolucyjne Sieci Neuronowe (CNN - Convolutional Neural Networks):**
    *   **Specjalizacja:** Przetwarzanie danych o strukturze siatki, głównie **obrazów**.
    *   **Kluczowa idea:** Używają specjalnych warstw **konwolucyjnych**, które działają jak filtry przesuwające się po obrazie i wykrywające lokalne wzorce (krawędzie, tekstury). Są bardzo efektywne w zadaniach takich jak rozpoznawanie obiektów na zdjęciach.

*   **Rekurencyjne Sieci Neuronowe (RNN - Recurrent Neural Networks):**
    *   **Specjalizacja:** Przetwarzanie **danych sekwencyjnych**, takich jak tekst, szeregi czasowe, mowa.
    *   **Kluczowa idea:** Posiadają **pętle (połączenia zwrotne)**, które pozwalają na utrzymywanie "pamięci" o poprzednich elementach sekwencji. Nowsze, bardziej zaawansowane warianty to **LSTM (Long Short-Term Memory)** i **GRU**, które lepiej radzą sobie z długimi zależnościami.

**4. Zastosowania:**

Rozpoznawanie obrazów i mowy, przetwarzanie języka naturalnego (tłumaczenia maszynowe, chatboty), autonomiczne pojazdy, diagnostyka medyczna.

---

# 58. Przetwarzanie języka naturalnego (NLP)

**1. Czym jest przetwarzanie języka naturalnego (NLP - Natural Language Processing)?**

To dziedzina sztucznej inteligencji i informatyki, która zajmuje się **umożliwieniem komputerom rozumienia, interpretowania i generowania ludzkiego języka** (zarówno w formie tekstu, jak i mowy).

**2. Jakie są główne zadania NLP?**

*   **Analiza sentymentu:** Określanie emocjonalnego zabarwienia tekstu (pozytywny, negatywny, neutralny). Używane do analizy opinii o produktach, recenzji, komentarzy w mediach społecznościowych.
*   **Rozpoznawanie nazwanych encji (NER - Named Entity Recognition):** Identyfikowanie i klasyfikowanie kluczowych informacji w tekście, takich jak imiona i nazwiska, nazwy organizacji, lokalizacje, daty.
*   **Tłumaczenie maszynowe:** Automatyczne tłumaczenie tekstu z jednego języka na drugi (np. Tłumacz Google).
*   **Odpowiadanie na pytania (Question Answering):** Systemy, które potrafią odpowiedzieć na pytania zadane w języku naturalnym (np. chatboty, asystenci głosowi).
*   **Generowanie tekstu:** Tworzenie spójnego i sensownego tekstu (np. podsumowania artykułów, opisy produktów, a nawet poezja).
*   **Modelowanie tematyczne:** Odkrywanie głównych tematów poruszanych w dużym zbiorze dokumentów.

**3. Jakie techniki są stosowane w NLP?**

Tradycyjne NLP opierało się na regułach lingwistycznych i modelach statystycznych. Współczesne NLP jest zdominowane przez **głębokie uczenie**.

*   **Tokenizacja:** Dzielenie tekstu na mniejsze jednostki – słowa lub zdania (tokeny).
*   **Embeddingi słów (Word Embeddings):** Technika reprezentowania słów jako **wektorów liczb** w przestrzeni wielowymiarowej. Słowa o podobnym znaczeniu mają podobne wektory (np. wektory dla "król" i "królowa" są blisko siebie). Pozwala to sieciom neuronowym rozumieć semantyczne relacje między słowami. (Przykłady: Word2Vec, GloVe).
*   **Modele rekurencyjne (RNN/LSTM):** Były standardem w przetwarzaniu sekwencji tekstowych.
*   **Architektura Transformer i mechanizm uwagi (Attention):** To **rewolucja w NLP**. Modele oparte na tej architekturze (takie jak **BERT** czy **GPT**) potrafią analizować relacje między wszystkimi słowami w tekście jednocześnie, a nie tylko sekwencyjnie. Pozwoliło to na osiągnięcie przełomowych wyników w niemal wszystkich zadaniach NLP.

---

# 59. Systemy rozproszone, Big Data

**1. Czym jest system rozproszony?**

To system, w którym **wiele niezależnych komputerów (węzłów) współpracuje ze sobą**, komunikując się przez sieć, aby osiągnąć wspólny cel. Z perspektywy użytkownika, system ten wygląda jak jeden, spójny system.

*   **Kluczowe cechy:**
    *   **Współbieżność:** Wiele komponentów działa jednocześnie.
    *   **Brak globalnego zegara:** Każdy węzeł ma własny zegar, co utrudnia koordynację.
    *   **Niezależne awarie:** Awaria jednego węzła nie powinna powodować awarii całego systemu.

**2. Jakie są zalety i wady systemów rozproszonych?**

*   **Zalety:**
    *   **Skalowalność:** Możliwość zwiększania mocy obliczeniowej przez dodawanie kolejnych węzłów (skalowalność horyzontalna).
    *   **Niezawodność i wysoka dostępność:** Awaria pojedynczych węzłów nie zatrzymuje działania całego systemu (redundancja).
*   **Wady:**
    *   **Złożoność:** Są znacznie trudniejsze do zaprojektowania, zaimplementowania i debugowania niż systemy scentralizowane.
    *   **Problemy z bezpieczeństwem i spójnością danych.**

**3. Czym jest Big Data?**

To termin opisujący **ogromne i złożone zbiory danych**, których przetwarzanie za pomocą tradycyjnych narzędzi bazodanowych jest niemożliwe lub niepraktyczne. Big Data charakteryzuje się tzw. **"3V" (lub więcej)**:

*   **Volume (Objętość):** Ogromna ilość danych (terabajty, petabajty).
*   **Velocity (Szybkość):** Wysoka szybkość napływania i przetwarzania danych (np. dane z mediów społecznościowych, czujników IoT).
*   **Variety (Różnorodność):** Dane pochodzą z różnych źródeł i mają różne formaty – od ustrukturyzowanych (bazy danych), przez częściowo ustrukturyzowane (JSON, XML), po nieustrukturyzowane (tekst, wideo, audio).

**4. Jak przetwarza się Big Data?**

Do przetwarzania Big Data używa się **systemów rozproszonych** i specjalnych frameworków. Kluczowym paradygmatem jest **MapReduce**.

*   **MapReduce:** To model programowania do przetwarzania dużych zbiorów danych w sposób rozproszony.
    *   **Faza Map:** Dzieli duży problem na mniejsze podproblemy. Główny węzeł rozsyła fragmenty danych do wielu węzłów roboczych, z których każdy wykonuje na swoich danych tę samą operację (mapowanie).
    *   **Faza Reduce:** Zbiera i agreguje wyniki z fazy Map, aby uzyskać końcowy rezultat.
*   **Apache Hadoop:** To najpopularniejszy, open-source'owy framework do implementacji MapReduce. Składa się z rozproszonego systemu plików **HDFS** (do przechowywania danych) i silnika **MapReduce** (do ich przetwarzania).
*   **Apache Spark:** Nowocześniejszy i znacznie szybszy następca Hadoopa. Przetwarza dane głównie w pamięci RAM, co czyni go idealnym do iteracyjnych algorytmów uczenia maszynowego i analizy danych w czasie rzeczywistym.

---

# 60. Internet Rzeczy (Internet of Things - IoT)

**1. Czym jest Internet Rzeczy (IoT)?**

To koncepcja, w której **przedmioty codziennego użytku** są wyposażone w czujniki, oprogramowanie i łączność z internetem, co pozwala im **zbierać i wymieniać dane** oraz autonomicznie podejmować działania. Jest to połączenie świata fizycznego ze światem cyfrowym.

**2. Jaka jest typowa architektura IoT?**

Składa się z czterech warstw:

1.  **Warstwa percepcji / urządzeń:** Fizyczne "rzeczy" – **czujniki** (zbierają dane, np. temperaturę, ruch) i **aktuatory** (wykonują akcje, np. włączają światło).
2.  **Warstwa sieci / łączności:** Odpowiada za przesyłanie danych z urządzeń do chmury. Wykorzystuje technologie takie jak Wi-Fi, Bluetooth, LoRaWAN, 5G.
3.  **Warstwa przetwarzania / platformy:** Zazwyczaj **platforma chmurowa**, która odbiera, przechowuje i analizuje ogromne ilości danych. To tutaj działają algorytmy i podejmowane są decyzje.
4.  **Warstwa aplikacji / interfejsu:** To, z czym interaguje użytkownik – **aplikacja mobilna** lub **panel sterowania (dashboard)**, który pozwala na monitorowanie i zarządzanie systemem.

**3. Jakie są przykłady zastosowań?**

*   **Inteligentny dom (Smart Home):** Inteligentne termostaty, oświetlenie, zamki, sprzęt AGD.
*   **Urządzenia noszone (Wearables):** Smartwatche, opaski fitness monitorujące aktywność i zdrowie.
*   **Inteligentne miasto (Smart City):** Inteligentne zarządzanie ruchem, oświetleniem ulicznym, gospodarką odpadami.
*   **Przemysłowy Internet Rzeczy (IIoT):** Monitorowanie maszyn w fabrykach w celu przewidywania awarii (konserwacja predykcyjna).
*   **Inteligentne rolnictwo:** Czujniki wilgotności gleby, drony monitorujące uprawy.

**4. Jakie są największe wyzwania i zagrożenia?**

*   **Bezpieczeństwo:** Wiele urządzeń IoT ma bardzo słabe zabezpieczenia, co czyni je łatwym celem dla hakerów. Przejęte urządzenia mogą być wykorzystane do tworzenia **botnetów** (np. Mirai) lub do ataków na prywatność (np. przejęcie kontroli nad kamerą w domu).
*   **Prywatność:** Urządzenia te zbierają ogromne ilości danych o naszych nawykach i zachowaniach. Istnieje ryzyko, że dane te mogą być wykorzystane w niepożądany sposób lub skradzione.
*   **Interoperacyjność:** Brak jednolitych standardów komunikacji między urządzeniami różnych producentów.

# Opracowanie zagadnień na egzamin inżynierski
## Wydział Informatyki

---

## Spis treści

### MATEMATYKA
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

### BAZY DANYCH
11. [Podstawowe cechy relacyjnych baz danych](#11-podstawowe-cechy-relacyjnych-baz-danych)
12. [Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych](#12-podstawowe-elementy-i-znaczenie-diagramów-związków-encji-oraz-zasady-prawidłowego-projektowania-schematów-bazy-danych)
13. [Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych](#13-mechanizm-współbieżności-pracy-wielu-użytkowników-w-systemie-zarządzania-bazami-danych)
14. [Podstawowe obiekty, konstrukcje i znaczenie języka SQL](#14-podstawowe-obiekty-konstrukcje-i-znaczenie-języka-sql)
15. [Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych](#15-podstawowe-zasady-optymalizacji-zapytań-w-tym-rodzaje-i-znaczenie-indeksów-w-bazie-danych)

### TECHNIKI I ARCHITEKTURA KOMPUTERÓW
16. [Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce](#16-model-architekturalny-komputera-wg-von-neumanna-a-model-obliczeniowy-komputera-na-podstawie-maszyny-turinga-i-ich-rola-w-informatyce)
17. [Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów](#17-logika-boolowska-i-jej-zastosowania-w-warstwie-sprzętowej-komputerów)
18. [Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa](#18-zapis-binarny-liczb-całkowitych-zapis-zmiennoprzecinkowy-liczb-rzeczywistych-arytmetyka-komputerowa)
19. [Miary wydajności procesorów, pamięci i systemów obliczeniowych](#19-miary-wydajności-procesorów-pamięci-i-systemów-obliczeniowych)
20. [Podstawowe elementy i znaczenie systemów wbudowanych](#20-podstawowe-elementy-i-znaczenie-systemów-wbudowanych)

### SYSTEMY OPERACYJNE
21. [Rola i zadania systemu operacyjnego, podstawowe elementy i rodzaje systemów operacyjnych](#21-rola-i-zadania-systemu-operacyjnego-podstawowe-elementy-i-rodzaje-systemów-operacyjnych)
22. [Pojęcie procesu i wątku, stany procesu/wątku, przełączanie kontekstu, algorytmy szeregowania procesów](#22-pojęcie-procesu-i-wątku-stany-procesuwątku-przełączanie-kontekstu-algorytmy-szeregowania-procesów)
23. [Problem wzajemnego wykluczania i jego rozwiązania, synchronizacja procesów i wątków, problem zakleszczenia](#23-problem-wzajemnego-wykluczania-i-jego-rozwiązania-synchronizacja-procesów-i-wątków-problem-zakleszczenia)
24. [Zarządzanie pamięcią operacyjną, pojęcie pamięci wirtualnej, segmentacja i stronicowanie pamięci](#24-zarządzanie-pamięcią-operacyjną-pojęcie-pamięci-wirtualnej-segmentacja-i-stronicowanie-pamięci)
25. [System plików, organizacja i implementacja, metody dostępu do plików](#25-system-plików-organizacja-i-implementacja-metody-dostępu-do-plików)

### SIECI KOMPUTEROWE
26. [Model warstwowy ISO/OSI i TCP/IP, protokoły i ich rola w komunikacji sieciowej](#26-model-warstwowy-isoosi-i-tcpip-protokoły-i-ich-rola-w-komunikacji-sieciowej)
27. [Adresacja w sieciach komputerowych: adresy fizyczne, logiczne i porty, rola i zadania protokołów ARP, DNS, DHCP](#27-adresacja-w-sieciach-komputerowych-adresy-fizyczne-logiczne-i-porty-rola-i-zadania-protokołów-arp-dns-dhcp)
28. [Podstawowe urządzenia sieciowe i ich rola w przesyle danych: koncentrator, przełącznik, router](#28-podstawowe-urządzenia-sieciowe-i-ich-rola-w-przesyle-danych-koncentrator-przełącznik-router)
29. [Rola i zadania wybranych protokołów warstwy aplikacji: HTTP, FTP, SMTP, DNS](#29-rola-i-zadania-wybranych-protokołów-warstwy-aplikacji-http-ftp-smtp-dns)
30. [Podstawowe zagadnienia bezpieczeństwa sieci komputerowych: zagrożenia, metody ochrony, kryptografia](#30-podstawowe-zagadnienia-bezpieczeństwa-sieci-komputerowych-zagrożenia-metody-ochrony-kryptografia)

### ALGORYTMY I PROGRAMOWANIE
31. [Cykl życia oprogramowania i jego modele (modele wytwarzania oprogramowania)](#31-cykl-życia-oprogramowania-i-jego-modele-modele-wytwarzania-oprogramowania)
32. [Analiza i projektowanie algorytmów, złożoność obliczeniowa, notacja asymptotyczna](#32-analiza-i-projektowanie-algorytmów-złożoność-obliczeniowa-notacja-asymptotyczna)
33. [Paradygmaty programowania: imperatywny, obiektowy, funkcyjny, deklaratywny](#33-paradygmaty-programowania-imperatywny-obiektowy-funkcyjny-deklaratywny)
34. [Programowanie obiektowe: klasy, obiekty, dziedziczenie, polimorfizm](#34-programowanie-obiektowe-klasy-obiekty-dziedziczenie-polimorfizm)
35. [Podstawowe struktury danych: tablica, lista, stos, kolejka, drzewo, graf](#35-podstawowe-struktury-danych-tablica-lista-stos-kolejka-drzewo-graf)
36. [Algorytmy sortowania: bąbelkowe, przez wstawianie, przez wybór, szybkie, przez scalanie](#36-algorytmy-sortowania-bąbelkowe-przez-wstawianie-przez-wybór-szybkie-przez-scalanie)
37. [Algorytmy wyszukiwania: liniowe, binarne](#37-algorytmy-wyszukiwania-liniowe-binarne)
38. [Algorytmy grafowe: przeszukiwanie wszerz i w głąb, algorytm Dijkstry, algorytmy Kruskala i Prima](#38-algorytmy-grafowe-przeszukiwanie-wszerz-i-w-głąb-algorytm-dijkstry-algorytmy-kruskala-i-prima)
39. [Klasy złożoności P i NP, problemy NP-zupełne](#39-klasy-złożoności-p-i-np-problemy-np-zupełne)

### GRAFIKA I INTERFEJSY
40. [Grafika rastrowa i wektorowa, modele barw](#40-grafika-rastrowa-i-wektorowa-modele-barw)
41. [Interfejsy użytkownika, interakcja człowiek-komputer, podstawowe zasady projektowania interfejsów](#41-interfejsy-użytkownika-interakcja-człowiek-komputer-podstawowe-zasady-projektowania-interfejsów)

### INŻYNIERIA OPROGRAMOWANIA
42. [Inżynieria wymagań: proces, wymagania funkcjonalne i niefunkcjonalne](#42-inżynieria-wymagań-proces-wymagania-funkcjonalne-i-niefunkcjonalne)
43. [Wzorce projektowe: kreacyjne, strukturalne i behawioralne (pojęcia i przykłady)](#43-wzorce-projektowe-kreacyjne-strukturalne-i-behawioralne-pojęcia-i-przykłady)
44. [Testowanie oprogramowania: poziomy testów, techniki czarno- i białoskrzynkowe](#44-testowanie-oprogramowania-poziomy-testów-techniki-czarno--i-białoskrzynkowe)
45. [Systemy kontroli wersji, Git, GitHub](#45-systemy-kontroli-wersji-git-github)
46. [Konteneryzacja, Docker](#46-konteneryzacja-docker)
47. [Metodyki zwinne (Agile), Scrum, Kanban](#47-metodyki-zwinne-agile-scrum-kanban)
48. [Ciągła integracja i ciągłe dostarczanie (CI/CD), Jenkins, GitHub Actions](#48-ciągła-integracja-i-ciągłe-dostarczanie-cicd-jenkins-github-actions)

### INTERNET I BEZPIECZEŃSTWO
49. [Architektura i usługi sieci Internet](#49-architektura-i-usługi-sieci-internet)
50. [Podstawowe pojęcia z zakresu bezpieczeństwa IT: zagrożenie, podatność, ryzyko, polityka bezpieczeństwa](#50-podstawowe-pojęcia-z-zakresu-bezpieczeństwa-it-zagrożenie-podatność-ryzyko-polityka-bezpieczeństwa)
51. [Kryptografia symetryczna i asymetryczna, klucz publiczny i prywatny, podpis cyfrowy](#51-kryptografia-symetryczna-i-asymetryczna-klucz-publiczny-i-prywatny-podpis-cyfrowy)
52. [Złośliwe oprogramowanie i ataki sieciowe](#52-złośliwe-oprogramowanie-i-ataki-sieciowe)

### ETYKA I PRAWO
53. [Etyka w informatyce, kodeksy etyczne](#53-etyka-w-informatyce-kodeksy-etyczne)
54. [Prawne aspekty oprogramowania: prawa autorskie, patenty, licencje](#54-prawne-aspekty-oprogramowania-prawa-autorskie-patenty-licencje)

### TECHNOLOGIE ZAAWANSOWANE
55. [Chmura obliczeniowa: modele usług (IaaS, PaaS, SaaS) i wdrożenia (prywatna, publiczna, hybrydowa)](#55-chmura-obliczeniowa-modele-usług-iaas-paas-saas-i-wdrożenia-prywatna-publiczna-hybrydowa)
56. [Uczenie maszynowe: uczenie nadzorowane, nienadzorowane i ze wzmocnieniem](#56-uczenie-maszynowe-uczenie-nadzorowane-nienadzorowane-i-ze-wzmocnieniem)
57. [Sztuczne sieci neuronowe, głębokie uczenie (deep learning)](#57-sztuczne-sieci-neuronowe-głębokie-uczenie-deep-learning)
58. [Przetwarzanie języka naturalnego (NLP)](#58-przetwarzanie-języka-naturalnego-nlp)
59. [Systemy rozproszone, Big Data](#59-systemy-rozproszone-big-data)
60. [Internet Rzeczy (Internet of Things - IoT)](#60-internet-rzeczy-internet-of-things---iot)

---

# 1. Ekstrema funkcji i gradient, zastosowania w informatyce

#### Wprowadzenie

Zagadnienie ekstremów funkcji oraz pojęcie gradientu stanowią fundamentalne narzędzia analizy matematycznej, które znajdują szerokie i kluczowe zastosowania w różnych dziedzinach informatyki. Od optymalizacji algorytmów, przez uczenie maszynowe, po grafikę komputerową – umiejętność znajdowania maksymalnych i minimalnych wartości funkcji oraz rozumienie, jak zmieniają się one w przestrzeni, jest niezbędna do rozwiązywania złożonych problemów obliczeniowych. W tym rozdziale przyjrzymy się formalnym definicjom, metodom analitycznym i numerycznym wyznaczania ekstremów, a także praktycznym przykładom ich implementacji w kontekście informatycznym.

#### Szczegółowe wyjaśnienie

**Ekstrema funkcji**

Ekstremum funkcji to, najprościej mówiąc, jej wartość maksymalna lub minimalna. Rozróżniamy dwa podstawowe rodzaje ekstremów:

*   **Ekstremum globalne:** Jest to największa (maksimum globalne) lub najmniejsza (minimum globalne) wartość, jaką funkcja przyjmuje w całej swojej dziedzinie.
*   **Ekstremum lokalne:** Jest to wartość największa (maksimum lokalne) lub najmniejsza (minimum lokalne) w pewnym otoczeniu (sąsiedztwie) danego punktu.

Formalnie, funkcja $f(x)$ ma w punkcie $x_0$ **maksimum lokalne**, jeśli istnieje takie otoczenie tego punktu, że dla każdego $x$ z tego otoczenia zachodzi nierówność $f(x) \le f(x_0)$. Analogicznie, ma **minimum lokalne**, jeśli $f(x) \ge f(x_0)$.

**Warunki konieczne i wystarczające istnienia ekstremum**

Do znajdowania ekstremów funkcji różniczkowalnych wykorzystujemy rachunek pochodnych.

1.  **Warunek konieczny (Fermata):** Jeśli funkcja $f(x)$ ma w punkcie $x_0$ ekstremum lokalne i jest w tym punkcie różniczkowalna, to jej pochodna w tym punkcie musi być równa zeru: $f'(x_0) = 0$. Punkty, w których pochodna się zeruje, nazywamy **punktami stacjonarnymi** lub krytycznymi.

2.  **Warunek wystarczający (dla funkcji jednej zmiennej):**
    *   **Z wykorzystaniem pierwszej pochodnej:** Jeśli funkcja $f(x)$ jest ciągła w punkcie $x_0$ i różniczkowalna w jego otoczeniu, a jej pochodna $f'(x)$ zmienia w tym punkcie znak z dodatniego na ujemny, to w $x_0$ jest maksimum lokalne. Jeśli zmiana znaku jest z ujemnego na dodatni – minimum lokalne.
    *   **Z wykorzystaniem drugiej pochodnej:** Jeśli $f'(x_0) = 0$ oraz druga pochodna $f''(x_0)$ istnieje i jest różna od zera, to:
        *   Gdy $f''(x_0) < 0$, funkcja ma w $x_0$ maksimum lokalne.
        *   Gdy $f''(x_0) > 0$, funkcja ma w $x_0$ minimum lokalne.

**Gradient funkcji**

Gradient jest uogólnieniem pojęcia pochodnej na funkcje wielu zmiennych (pola skalarne). Dla funkcji $f(x_1, x_2, ..., x_n)$ gradient jest wektorem, którego składowe to pochodne cząstkowe tej funkcji względem poszczególnych zmiennych.

$$ \nabla f = \left[ \frac{\partial f}{\partial x_1}, \frac{\partial f}{\partial x_2}, ..., \frac{\partial f}{\partial x_n} \right] $$

**Kluczowe własności gradientu:**

*   **Kierunek najszybszego wzrostu:** Gradient w danym punkcie wskazuje kierunek, w którym wartość funkcji rośnie najszybciej.
*   **Kierunek najszybszego spadku:** Wektor przeciwny do gradientu ($- \nabla f$) wskazuje kierunek najszybszego spadku wartości funkcji.
*   **Ortogonalność do poziomic:** Gradient jest prostopadły do linii (lub powierzchni) stałej wartości funkcji (poziomic).

**Ekstrema funkcji wielu zmiennych**

Podobnie jak dla funkcji jednej zmiennej, warunkiem koniecznym istnienia ekstremum w punkcie jest zerowanie się gradientu: $\nabla f(x_1, ..., x_n) = 0$. Oznacza to, że wszystkie pochodne cząstkowe muszą być równe zeru.

Warunek wystarczający opiera się na analizie **macierzy Hessego** (hesjanu), czyli macierzy drugich pochodnych cząstkowych:

$$ H_f = \begin{bmatrix} \frac{\partial^2 f}{\partial x_1^2} & \frac{\partial^2 f}{\partial x_1 \partial x_2} & \cdots & \frac{\partial^2 f}{\partial x_1 \partial x_n} \\ \frac{\partial^2 f}{\partial x_2 \partial x_1} & \frac{\partial^2 f}{\partial x_2^2} & \cdots & \frac{\partial^2 f}{\partial x_2 \partial x_n} \\ \vdots & \vdots & \ddots & \vdots \\ \frac{\partial^2 f}{\partial x_n \partial x_1} & \frac{\partial^2 f}{\partial x_n \partial x_2} & \cdots & \frac{\partial^2 f}{\partial x_n^2} \end{bmatrix} $$

Analiza określoności tej macierzy w punkcie stacjonarnym pozwala stwierdzić, czy mamy do czynienia z ekstremum:

*   Jeśli hesjan jest **dodatnio określony** (wszystkie jego wartości własne są dodatnie), w punkcie jest minimum lokalne.
*   Jeśli hesjan jest **ujemnie określony** (wszystkie jego wartości własne są ujemne), w punkcie jest maksimum lokalne.
*   Jeśli hesjan jest **nieokreślony** (ma zarówno dodatnie, jak i ujemne wartości własne), w punkcie jest tzw. **punkt siodłowy** (nie ma ekstremum).

#### Praktyczne zastosowania w informatyce

Koncepcje ekstremów i gradientu są wszechobecne w informatyce, stanowiąc podstawę dla wielu kluczowych algorytmów i technik.

**1. Uczenie maszynowe (Machine Learning)**

Najważniejszym zastosowaniem jest tutaj **optymalizacja funkcji kosztu (lub straty)**. Modele uczenia maszynowego, takie jak sieci neuronowe czy regresja liniowa, uczą się poprzez minimalizację błędu, który jest opisany przez funkcję kosztu. Celem jest znalezienie takich parametrów modelu (wag), które minimalizują tę funkcję.

*   **Metoda gradientu prostego (Gradient Descent):** Jest to iteracyjny algorytm optymalizacyjny służący do znajdowania minimum funkcji. Działa on w następujący sposób:
    1.  Wybierz losowy punkt startowy (początkowe wagi modelu).
    2.  Oblicz gradient funkcji kosztu w tym punkcie.
    3.  Przesuń się o mały krok w kierunku przeciwnym do gradientu (kierunku najszybszego spadku).
    4.  Powtarzaj kroki 2 i 3, aż do osiągnięcia minimum (gradient bliski zeru) lub wykonania określonej liczby iteracji.

    Wzór na aktualizację wag w każdej iteracji wygląda następująco:
    $$ w_{new} = w_{old} - \eta \nabla f(w_{old}) $$
    gdzie $\eta$ (eta) to **współczynnik uczenia (learning rate)**, mała stała kontrolująca wielkość kroku.

    Warianty tej metody, takie jak **stochastyczny spadek gradientu (SGD)** czy **Adam**, są podstawą treningu niemal wszystkich nowoczesnych modeli głębokiego uczenia.

**2. Grafika komputerowa i przetwarzanie obrazów**

*   **Wykrywanie krawędzi:** Gradient obrazu (który jest funkcją 2D, gdzie wartością jest intensywność piksela) wskazuje kierunek i siłę największej zmiany koloru. Miejsca, gdzie gradient ma dużą magnitudę, odpowiadają krawędziom na obrazie. Algorytmy takie jak **operator Sobela** czy **Canny'ego** wykorzystują tę właściwość.
*   **Cieniowanie i oświetlenie:** W grafice 3D gradienty (a konkretnie wektory normalne do powierzchni, które są z nimi powiązane) są kluczowe do obliczania, jak światło odbija się od obiektów, co decyduje o ich wyglądzie i cieniowaniu (np. cieniowanie Phonga).

**3. Sieci komputerowe**

*   **Algorytmy routingu:** Chociaż nie jest to bezpośrednie zastosowanie gradientu w sensie matematycznym, koncepcja "najszybszego spadku" jest analogiczna do znajdowania najkrótszej ścieżki w grafie. Algorytmy takie jak **Dijkstry** czy **A*** można interpretować jako proces minimalizacji funkcji kosztu (długości ścieżki).

#### Przykłady

**Przykład 1: Znajdowanie minimum funkcji jednej zmiennej**

Niech dana będzie funkcja $f(x) = x^2 - 4x + 5$.

1.  **Warunek konieczny:** Obliczamy pierwszą pochodną i przyrównujemy do zera.
    $f'(x) = 2x - 4$
    $2x - 4 = 0 \implies x = 2$. Mamy jeden punkt stacjonarny.

2.  **Warunek wystarczający:** Obliczamy drugą pochodną.
    $f''(x) = 2$
    Ponieważ $f''(2) = 2 > 0$, funkcja ma w punkcie $x=2$ **minimum lokalne**.
    Wartość minimum wynosi $f(2) = 2^2 - 4(2) + 5 = 4 - 8 + 5 = 1$.

**Przykład 2: Ilustracja kroku metody gradientu prostego**

Chcemy zminimalizować funkcję $f(w) = w^2$ za pomocą metody gradientu prostego. Niech współczynnik uczenia $\eta = 0.1$, a punkt startowy $w_0 = 5$.

1.  **Obliczamy gradient (pochodną):** $\nabla f(w) = f'(w) = 2w$.
2.  **Iteracja 1:**
    *   Oblicz gradient w punkcie $w_0=5$: $\nabla f(5) = 2 * 5 = 10$.
    *   Zaktualizuj wagę: $w_1 = w_0 - \eta \nabla f(w_0) = 5 - 0.1 * 10 = 5 - 1 = 4$.
3.  **Iteracja 2:**
    *   Oblicz gradient w punkcie $w_1=4$: $\nabla f(4) = 2 * 4 = 8$.
    *   Zaktualizuj wagę: $w_2 = w_1 - \eta \nabla f(w_1) = 4 - 0.1 * 8 = 4 - 0.8 = 3.2$.

Jak widać, z każdą iteracją zbliżamy się do minimum funkcji, które znajduje się w punkcie $w=0$.

**Przykład 3: Ekstrema funkcji dwóch zmiennych**

Znajdź ekstrema funkcji $f(x, y) = x^2 + y^2 - 2x + 4y + 8$.

1.  **Obliczamy gradient i przyrównujemy do zera:**
    $\frac{\partial f}{\partial x} = 2x - 2 = 0 \implies x = 1$
    $\frac{\partial f}{\partial y} = 2y + 4 = 0 \implies y = -2$
    Punkt stacjonarny to $(1, -2)$.

2.  **Obliczamy macierz Hessego:**
    $\frac{\partial^2 f}{\partial x^2} = 2$
    $\frac{\partial^2 f}{\partial y^2} = 2$
    $\frac{\partial^2 f}{\partial x \partial y} = 0$

    $H_f = \begin{bmatrix} 2 & 0 \\ 0 & 2 \end{bmatrix}$

3.  **Analizujemy hesjan:** Wyznacznik hesjanu $det(H_f) = 2*2 - 0*0 = 4 > 0$. Ponieważ element w lewym górnym rogu jest dodatni ($2 > 0$), macierz jest dodatnio określona. Zatem w punkcie $(1, -2)$ funkcja ma **minimum lokalne**.

#### Podsumowanie

*   **Ekstrema** to maksymalne lub minimalne wartości funkcji, kluczowe w problemach optymalizacyjnych.
*   **Gradient** to wektor pochodnych cząstkowych, który wskazuje kierunek najszybszego wzrostu funkcji.
*   Warunkiem koniecznym istnienia ekstremum funkcji różniczkowalnej jest **zerowanie się pochodnej (lub gradientu)**.
*   Warunek wystarczający opiera się na **znaku drugiej pochodnej** (dla jednej zmiennej) lub **określoności macierzy Hessego** (dla wielu zmiennych).
*   W informatyce, gradient jest fundamentem **metody gradientu prostego**, podstawowego algorytmu optymalizacyjnego w **uczeniu maszynowym**.
*   Inne zastosowania to m.in. **przetwarzanie obrazów** (wykrywanie krawędzi) i **grafika komputerowa** (cieniowanie).

**Typowe pytania egzaminacyjne:**
*   Proszę podać warunek konieczny i wystarczający istnienia ekstremum funkcji jednej/dwóch zmiennych.
*   Czym jest gradient i jaka jest jego geometryczna interpretacja?
*   Jak działa metoda gradientu prostego? Proszę opisać jej zastosowanie w uczeniu maszynowym.
*   Proszę znaleźć ekstrema podanej funkcji $f(x,y)$.

---

# 2. Wielomian i szereg Taylora funkcji rzeczywistej

#### Wprowadzenie

Wielomian i szereg Taylora to jedne z najpotężniejszych narzędzi analizy matematycznej, pozwalające na przybliżanie (aproksymację) skomplikowanych funkcji za pomocą prostszych w obsłudze wielomianów. Idea polega na skonstruowaniu wielomianu, który w otoczeniu pewnego punktu "naśladuje" zachowanie danej funkcji tak dobrze, jak to tylko możliwe. W informatyce, gdzie często operuje się na funkcjach, których obliczenie jest kosztowne lub niemożliwe w sposób analityczny (np. funkcje trygonometryczne, logarytmiczne), rozwinięcie w szereg Taylora stanowi podstawę wielu algorytmów numerycznych, silników fizycznych w grach i metod optymalizacyjnych.

#### Szczegółowe wyjaśnienie

**Idea aproksymacji wielomianowej**

Załóżmy, że mamy funkcję $f(x)$, która jest wielokrotnie różniczkowalna w punkcie $x_0$. Chcemy znaleźć wielomian $W(x)$, który będzie jak najlepszym przybliżeniem funkcji $f(x)$ w pobliżu tego punktu. Aby to osiągnąć, żądamy, aby wielomian i jego pochodne w punkcie $x_0$ miały takie same wartości, jak funkcja $f(x)$ i jej odpowiednie pochodne w tym samym punkcie.

**Wielomian Taylora**

Wielomian Taylora stopnia $n$ dla funkcji $f(x)$ w punkcie $x_0$ jest zdefiniowany jako:

$$ T_n(x) = f(x_0) + \frac{f'(x_0)}{1!}(x-x_0) + \frac{f''(x_0)}{2!}(x-x_0)^2 + \dots + \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n $$

Można go zapisać w bardziej zwartej formie za pomocą symbolu sumy:

$$ T_n(x) = \sum_{k=0}^{n} \frac{f^{(k)}(x_0)}{k!}(x-x_0)^k $$

gdzie $f^{(k)}(x_0)$ oznacza $k$-tą pochodną funkcji $f$ obliczoną w punkcie $x_0$, a $0!$ przyjmujemy jako 1.

*   **Wielomian Maclaurina:** Jest to szczególny przypadek wielomianu Taylora, gdy punkt rozwinięcia $x_0 = 0$.

**Reszta we wzorze Taylora**

Wielomian Taylora jest tylko przybliżeniem. Różnicę między prawdziwą wartością funkcji a wartością wielomianu nazywamy **resztą** i oznaczamy jako $R_n(x)$:

$$ f(x) = T_n(x) + R_n(x) $$

Najczęściej używaną postacią reszty jest **postać Lagrange'a**:

$$ R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1} $$

gdzie $c$ jest pewnym punktem leżącym pomiędzy $x_0$ a $x$. Reszta ta pozwala oszacować błąd aproksymacji. Im wyższy stopień wielomianu $n$, tym zazwyczaj mniejszy błąd.

**Szereg Taylora**

Jeśli funkcja jest nieskończenie wiele razy różniczkowalna w punkcie $x_0$, możemy rozszerzyć wielomian Taylora do nieskończoności, tworząc **szereg Taylora**:

$$ f(x) = \sum_{k=0}^{\infty} \frac{f^{(k)}(x_0)}{k!}(x-x_0)^k $$

Jeśli reszta $R_n(x)$ dąży do zera, gdy $n$ dąży do nieskończoności ($lim_{n \to \infty} R_n(x) = 0$), to szereg Taylora jest zbieżny do funkcji $f(x)$ w pewnym przedziale zbieżności wokół $x_0$. Oznacza to, że w tym przedziale funkcja jest **równa** swojemu szeregowi Taylora.

#### Praktyczne zastosowania w informatyce

**1. Obliczenia numeryczne i biblioteki standardowe**

Kalkulatory i komputery nie przechowują wartości funkcji takich jak $sin(x)$, $cos(x)$, $e^x$ czy $ln(x)$ dla wszystkich możliwych argumentów. Zamiast tego, gdy potrzebna jest wartość takiej funkcji, jest ona obliczana w locie za pomocą aproksymacji wielomianowej, najczęściej opartej na szeregu Maclaurina. Używa się kilku pierwszych wyrazów szeregu, aby uzyskać wymaganą precyzję.

*   **Przykład:** Aby obliczyć $sin(0.1)$, komputer może użyć rozwinięcia Maclaurina dla $sin(x)$: $x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots$. Już dwa pierwsze wyrazy dają $0.1 - \frac{0.001}{6} \approx 0.099833$, co jest bardzo bliskie prawdziwej wartości.

**2. Silniki fizyczne w grach komputerowych**

W symulacjach fizycznych często trzeba rozwiązywać złożone równania różniczkowe opisujące ruch, kolizje czy deformacje obiektów. Rozwiązania analityczne są rzadko dostępne. Zamiast tego, stosuje się metody numeryczne (np. **metoda Eulera**), które w swojej istocie są rozwinięciem Taylora pierwszego rzędu. Pozwala to na przybliżenie stanu systemu (pozycji, prędkości) w następnej, małej klatce czasowej na podstawie stanu obecnego.

**3. Optymalizacja i uczenie maszynowe**

Rozwinięcie Taylora jest teoretyczną podstawą dla zaawansowanych metod optymalizacyjnych, takich jak **metoda Newtona** do znajdowania minimów funkcji. Metoda ta wykorzystuje przybliżenie funkcji za pomocą wielomianu Taylora drugiego stopnia (aproksymacja kwadratowa), co pozwala na szybsze zbieganie do minimum niż w metodzie gradientu prostego (która używa aproksymacji liniowej - pierwszego rzędu).

**4. Przetwarzanie sygnałów i analiza błędów**

W analizie błędów pomiarowych i propagacji niepewności, wzór Taylora pozwala na linearyzację skomplikowanych zależności i oszacowanie, jak małe błędy na wejściu wpływają na błąd wyniku końcowego.

#### Przykłady

**Przykład 1: Wielomian Maclaurina dla funkcji $e^x$**

Chcemy znaleźć wielomian Maclaurina (czyli Taylora dla $x_0=0$) stopnia 3 dla funkcji $f(x) = e^x$.

1.  **Obliczamy pochodne w punkcie $x_0=0$:**
    *   $f(x) = e^x \implies f(0) = e^0 = 1$
    *   $f'(x) = e^x \implies f'(0) = 1$
    *   $f''(x) = e^x \implies f''(0) = 1$
    *   $f'''(x) = e^x \implies f'''(0) = 1$

2.  **Wstawiamy do wzoru na wielomian Taylora:**
    $T_3(x) = f(0) + \frac{f'(0)}{1!}x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3$
    $T_3(x) = 1 + \frac{1}{1}x + \frac{1}{2}x^2 + \frac{1}{6}x^3 = 1 + x + \frac{x^2}{2} + \frac{x^3}{6}$

Ten wielomian jest dobrym przybliżeniem $e^x$ dla $x$ bliskich zeru.

**Przykład 2: Szereg Maclaurina dla $cos(x)$**

Znajdźmy ogólny wzór na szereg Maclaurina dla $f(x) = cos(x)$.

1.  **Pochodne w $x_0=0$:**
    *   $f(x) = cos(x) \implies f(0) = 1$
    *   $f'(x) = -sin(x) \implies f'(0) = 0$
    *   $f''(x) = -cos(x) \implies f''(0) = -1$
    *   $f'''(x) = sin(x) \implies f'''(0) = 0$
    *   $f^{(4)}(x) = cos(x) \implies f^{(4)}(0) = 1$
    Wartości pochodnych cyklicznie powtarzają się: $(1, 0, -1, 0, 1, ...)$.

2.  **Zapisujemy szereg:**
    $cos(x) = \frac{1}{0!}x^0 + \frac{0}{1!}x^1 + \frac{-1}{2!}x^2 + \frac{0}{3!}x^3 + \frac{1}{4!}x^4 + \dots$
    $cos(x) = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \dots = \sum_{k=0}^{\infty} (-1)^k \frac{x^{2k}}{(2k)!}$

Ten szereg jest zbieżny dla wszystkich liczb rzeczywistych $x$.

#### Podsumowanie

*   **Wielomian Taylora** to wielomian stopnia $n$, który przybliża funkcję $f(x)$ w otoczeniu punktu $x_0$, mając w tym punkcie takie same wartości pochodnych do rzędu $n$ co funkcja.
*   **Szereg Taylora** to nieskończona suma, która (jeśli jest zbieżna) jest równa funkcji.
*   **Szereg Maclaurina** to szczególny przypadek szeregu Taylora dla $x_0=0$.
*   **Reszta** we wzorze Taylora określa błąd aproksymacji.
*   W informatyce szeregi Taylora są używane do **obliczania wartości funkcji** (np. w bibliotekach matematycznych), w **symulacjach fizycznych**, **algorytmach optymalizacyjnych** i **analizie błędów**.

**Typowe pytania egzaminacyjne:**
*   Proszę podać wzór na wielomian Taylora stopnia $n$.
*   Czym różni się wielomian Taylora od szeregu Taylora?
*   Proszę znaleźć rozwinięcie w szereg Maclaurina dla funkcji $sin(x)$ lub $e^x$.
*   Jakie jest praktyczne zastosowanie szeregu Taylora w informatyce? Proszę podać i omówić przykład.

---

# 3. Układy równań liniowych: różne metody rozwiązywania, liczba rozwiązań

#### Wprowadzenie

Układy równań liniowych stanowią jeden z fundamentalnych problemów algebry liniowej i są wszechobecne w niemal każdej dziedzinie nauki i inżynierii, w tym w informatyce. Opisują one zależności między wieloma zmiennymi w sposób liniowy, co pozwala modelować szeroką gamę zjawisk – od analizy obwodów elektrycznych, przez grafikę komputerową, aż po optymalizację i uczenie maszynowe. Zrozumienie, kiedy układ ma rozwiązanie, ile tych rozwiązań istnieje oraz jak je efektywnie znaleźć, jest kluczową umiejętnością analityczną.

#### Szczegółowe wyjaśnienie

Układ $m$ równań liniowych z $n$ niewiadomymi ma postać:

$$ \begin{cases} a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1 \\ a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b_2 \\ \vdots \\ a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m \end{cases} $$

Można go zapisać w zwartej formie macierzowej jako $AX = B$, gdzie:

*   $A$ – macierz współczynników o wymiarach $m \times n$.
*   $X$ – wektor (kolumna) niewiadomych o wymiarach $n \times 1$.
*   $B$ – wektor (kolumna) wyrazów wolnych o wymiarach $m \times 1$.

**Liczba rozwiązań – Twierdzenie Kroneckera-Capellego**

To fundamentalne twierdzenie pozwala określić liczbę rozwiązań układu bez potrzeby jego rozwiązywania. Wymaga ono porównania rzędu dwóch macierzy:

1.  **Macierzy głównej (A):** Macierz współczynników przy niewiadomych.
2.  **Macierzy uzupełnionej (rozszerzonej) [A|B]:** Macierz A, do której dołączono kolumnę wyrazów wolnych B.

**Rząd macierzy** (ozn. $rz(A)$ lub $rank(A)$) to wymiar największej podmacierzy kwadratowej o niezerowym wyznaczniku lub, równoważnie, maksymalna liczba liniowo niezależnych wektorów (kolumn lub wierszy) tej macierzy.

Twierdzenie Kroneckera-Capellego mówi, że:

1.  Układ równań ma rozwiązanie (jest **niesprzeczny**) wtedy i tylko wtedy, gdy rząd macierzy głównej jest równy rzędowi macierzy uzupełnionej:
    $$ rz(A) = rz([A|B]) $$
2.  Jeśli ten warunek jest spełniony, to:
    *   Układ ma **dokładnie jedno rozwiązanie** (jest **oznaczony**), gdy rząd macierzy jest równy liczbie niewiadomych:
        $$ rz(A) = rz([A|B]) = n $$
    *   Układ ma **nieskończenie wiele rozwiązań** (jest **nieoznaczony**), gdy rząd macierzy jest mniejszy od liczby niewiadomych:
        $$ rz(A) = rz([A|B]) < n $$
        Liczba tzw. **parametrów**, czyli zmiennych, które możemy wybrać dowolnie, wynosi $n - rz(A)$.
3.  Jeśli $rz(A) \neq rz([A|B])$, układ jest **sprzeczny** i nie ma rozwiązań.

#### Metody rozwiązywania

**1. Metoda eliminacji Gaussa**

Jest to najbardziej uniwersalna i efektywna algorytmicznie metoda, stosowana powszechnie w obliczeniach komputerowych. Polega na przekształceniu macierzy uzupełnionej $[A|B]$ do postaci schodkowej (lub schodkowej zredukowanej) za pomocą operacji elementarnych na wierszach, które nie zmieniają rozwiązania układu:

*   Zamiana dwóch wierszy miejscami.
*   Pomnożenie wiersza przez dowolną stałą różną od zera.
*   Dodanie do jednego wiersza innego wiersza pomnożonego przez stałą.

**Kroki algorytmu:**
1.  Utwórz macierz uzupełnioną $[A|B]$.
2.  Za pomocą operacji elementarnych wyzeruj elementy pod główną przekątną w kolejnych kolumnach, sprowadzając macierz do **postaci schodkowej**.
3.  Po uzyskaniu postaci schodkowej, układ równań można łatwo rozwiązać, zaczynając od ostatniego równania i wykonując podstawienia wstecz (tzw. **back substitution**).

**2. Metoda wyznaczników (wzory Cramera)**

Metoda ta ma głównie znaczenie teoretyczne i jest wygodna tylko dla małych układów (2x2, 3x3). Można ją stosować **tylko wtedy, gdy macierz A jest kwadratowa ($m=n$) i jej wyznacznik jest różny od zera** (co, zgodnie z tw. Kroneckera-Capellego, gwarantuje istnienie dokładnie jednego rozwiązania).

**Kroki algorytmu:**
1.  Oblicz wyznacznik główny $W = det(A)$. Jeśli $W=0$, metody nie można stosować.
2.  Dla każdej niewiadomej $x_i$ oblicz wyznacznik $W_i = det(A_i)$, gdzie macierz $A_i$ powstaje przez zastąpienie $i$-tej kolumny macierzy $A$ kolumną wyrazów wolnych $B$.
3.  Rozwiązaniem jest:
    $$ x_1 = \frac{W_1}{W}, \quad x_2 = \frac{W_2}{W}, \quad \dots, \quad x_n = \frac{W_n}{W} $$

**3. Metoda macierzy odwrotnej**

Podobnie jak wzory Cramera, metoda ta działa tylko dla układów z macierzą kwadratową $A$ o niezerowym wyznaczniku. Polega na znalezieniu macierzy odwrotnej $A^{-1}$ i pomnożeniu przez nią obustronnie równania $AX=B$:

$$ A^{-1}AX = A^{-1}B \implies IX = A^{-1}B \implies X = A^{-1}B $$

Rozwiązanie otrzymujemy przez proste mnożenie macierzy. Problemem jest jednak koszt obliczeniowy znalezienia macierzy odwrotnej, który jest znacznie wyższy niż koszt eliminacji Gaussa.

#### Praktyczne zastosowania w informatyce

1.  **Grafika komputerowa:** Układy równań liniowych są używane do obliczania transformacji geometrycznych (obroty, skalowanie, przesunięcia), znajdowania przecięć promieni z obiektami (ray tracing), a także w zaawansowanych technikach renderowania i animacji.
2.  **Uczenie maszynowe:** W regresji liniowej celem jest znalezienie prostej (lub hiperpłaszczyzny), która najlepiej pasuje do danych. Współczynniki tej prostej są rozwiązaniem układu równań liniowych (tzw. równań normalnych).
3.  **Analiza sieci i obwodów:** W analizie obwodów elektrycznych (prawo Kirchhoffa) czy przepływów w sieciach, zależności między prądami i napięciami tworzą układy równań liniowych.
4.  **Robotyka i widzenie komputerowe:** Do kalibracji kamer, triangulacji punktów w przestrzeni 3D czy planowania ruchu manipulatorów robotów.
5.  **Kryptografia:** Niektóre historyczne i prostsze szyfry (np. szyfr Hilla) opierają swoje działanie na operacjach macierzowych i rozwiązywaniu układów równań w ciałach skończonych.

#### Przykłady

**Przykład 1: Rozwiązanie układu metodą eliminacji Gaussa**

Rozwiąż układ: $\begin{cases} x + y + z = 6 \\ x - 2y + 2z = 3 \\ 2x + y - z = 1 \end{cases}$

1.  **Macierz uzupełniona:** $\left[ \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 1 & -2 & 2 & 3 \\ 2 & 1 & -1 & 1 \end{array} \right]$
2.  **Eliminacja:**
    *   $w_2 - w_1$, $w_3 - 2w_1$: $\left[ \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & -3 & 1 & -3 \\ 0 & -1 & -3 & -11 \end{array} \right]$
    *   $w_3 - \frac{1}{3}w_2$: $\left[ \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & -3 & 1 & -3 \\ 0 & 0 & -\frac{10}{3} & -10 \end{array} \right]$
3.  **Podstawienie wstecz:**
    *   Z ostatniego wiersza: $-\frac{10}{3}z = -10 \implies z = 3$.
    *   Z drugiego wiersza: $-3y + z = -3 \implies -3y + 3 = -3 \implies -3y = -6 \implies y = 2$.
    *   Z pierwszego wiersza: $x + y + z = 6 \implies x + 2 + 3 = 6 \implies x = 1$.
    Rozwiązanie: $x=1, y=2, z=3$.

**Przykład 2: Analiza liczby rozwiązań (tw. Kroneckera-Capellego)**

Zbadaj liczbę rozwiązań układu: $\begin{cases} x + 2y = 3 \\ 2x + 4y = 5 \end{cases}$

1.  $A = \begin{bmatrix} 1 & 2 \\ 2 & 4 \end{bmatrix}$, $[A|B] = \left[ \begin{array}{cc|c} 1 & 2 & 3 \\ 2 & 4 & 5 \end{array} \right]$
2.  **Rząd A:** $det(A) = 1*4 - 2*2 = 0$. Rząd nie jest 2. Ponieważ są niezerowe elementy, $rz(A)=1$.
3.  **Rząd [A|B]:** Sprowadzamy do postaci schodkowej: $w_2 - 2w_1 \implies \left[ \begin{array}{cc|c} 1 & 2 & 3 \\ 0 & 0 & -1 \end{array} \right]$. Mamy dwa liniowo niezależne wiersze, więc $rz([A|B])=2$.
4.  **Wniosek:** Ponieważ $rz(A) = 1 \neq rz([A|B]) = 2$, układ jest **sprzeczny**.

#### Podsumowanie

*   Układy równań liniowych można zapisać w postaci macierzowej $AX=B$.
*   **Twierdzenie Kroneckera-Capellego** pozwala określić liczbę rozwiązań przez porównanie rzędu macierzy głównej i uzupełnionej.
*   Układ może być **oznaczony** (1 rozwiązanie), **nieoznaczony** (nieskończenie wiele rozwiązań) lub **sprzeczny** (brak rozwiązań).
*   Główną metodą rozwiązywania jest **eliminacja Gaussa**, która jest uniwersalna i wydajna obliczeniowo.
*   **Wzory Cramera** i **metoda macierzy odwrotnej** mają zastosowanie tylko w szczególnych przypadkach (macierz kwadratowa, nieosobliwa) i są mniej efektywne dla dużych układów.
*   Zastosowania w informatyce obejmują m.in. **grafikę komputerową, uczenie maszynowe i robotykę**.

**Typowe pytania egzaminacyjne:**
*   Proszę sformułować twierdzenie Kroneckera-Capellego.
*   Jakie są metody rozwiązywania układów równań liniowych? Proszę omówić jedną z nich.
*   Kiedy można stosować wzory Cramera i na czym one polegają?
*   Proszę rozwiązać podany układ równań lub zbadać liczbę jego rozwiązań.

---

# 4. Wartości własne macierzy i ich zastosowanie w informatyce

#### Wprowadzenie

Wartości i wektory własne to jedne z najważniejszych pojęć algebry liniowej, które pozwalają na głębsze zrozumienie natury i właściwości przekształceń liniowych reprezentowanych przez macierze. Zamiast opisywać, jak macierz transformuje dowolny wektor, analiza własna koncentruje się na znalezieniu szczególnych, "wyróżnionych" kierunków w przestrzeni, wzdłuż których działanie macierzy sprowadza się do prostego skalowania. Te "niezmiennicze" kierunki (wektory własne) i odpowiadające im skale (wartości własne) ujawniają fundamentalną strukturę macierzy i mają ogromne znaczenie praktyczne w informatyce, od redukcji wymiarowości danych, przez analizę grafów, po mechanikę kwantową.

#### Szczegółowe wyjaśnienie

**Definicja wartości i wektora własnego**

Niech $A$ będzie macierzą kwadratową o wymiarach $n \times n$. **Wektorem własnym** tej macierzy nazywamy taki **niezerowy** wektor $v$, który po pomnożeniu przez macierz $A$ daje w wyniku ten sam wektor $v$ pomnożony przez pewną stałą (skalar) $\lambda$.

$$ Av = \lambda v $$

Skalar $\lambda$ nazywamy **wartością własną** macierzy $A$ odpowiadającą wektorowi własnemu $v$.

**Interpretacja geometryczna:** Działanie macierzy $A$ na jej wektor własny $v$ nie zmienia jego kierunku – wektor wynikowy $Av$ jest jedynie rozciągany lub ściskany (a jeśli $\lambda < 0$, również odwracany) wzdłuż tej samej linii, którą wyznacza $v$.

**Jak znaleźć wartości i wektory własne?**

Równanie definicyjne $Av = \lambda v$ można przekształcić:

$$ Av - \lambda v = 0 \\ Av - \lambda I v = 0 \\ (A - \lambda I)v = 0 $$

gdzie $I$ to macierz jednostkowa. Szukamy niezerowego wektora $v$ spełniającego to równanie. Taki niezerowy wektor istnieje wtedy i tylko wtedy, gdy macierz $(A - \lambda I)$ jest **osobliwa**, czyli jej wyznacznik jest równy zero.

$$ det(A - \lambda I) = 0 $$

To równanie nazywamy **równaniem charakterystycznym** macierzy $A$. Jest to wielomian stopnia $n$ zmiennej $\lambda$, a jego pierwiastki są właśnie **wartościami własnymi** macierzy $A$.

**Procedura obliczeniowa:**

1.  **Znajdowanie wartości własnych:** Utwórz macierz $(A - \lambda I)$ i oblicz jej wyznacznik. Rozwiąż równanie charakterystyczne $det(A - \lambda I) = 0$, aby znaleźć wartości własne $\lambda_1, \lambda_2, \dots, \lambda_n$.
2.  **Znajdowanie wektorów własnych:** Dla każdej znalezionej wartości własnej $\lambda_i$ rozwiąż układ równań liniowych $(A - \lambda_i I)v = 0$. Każde niezerowe rozwiązanie $v$ tego układu jest wektorem własnym odpowiadającym wartości własnej $\lambda_i$.

**Ważne właściwości:**

*   Suma wartości własnych macierzy jest równa jej **śladowi** (sumie elementów na głównej przekątnej): $\sum \lambda_i = Tr(A)$.
*   Iloczyn wartości własnych jest równy jej **wyznacznikowi**: $\prod \lambda_i = det(A)$.
*   Dla macierzy symetrycznych (takich, że $A = A^T$), wartości własne są zawsze rzeczywiste, a wektory własne odpowiadające różnym wartościom własnym są do siebie ortogonalne.

#### Praktyczne zastosowania w informatyce

**1. Analiza głównych składowych (Principal Component Analysis - PCA)**

PCA to jedna z najważniejszych technik **redukcji wymiarowości** w uczeniu maszynowym i analizie danych. Służy do przekształcania zbioru danych o dużej liczbie skorelowanych zmiennych w nowy zbiór o mniejszej liczbie nieskorelowanych zmiennych, zwanych **głównymi składowymi**, przy jak najmniejszej utracie informacji.

*   **Jak to działa?** PCA znajduje wartości i wektory własne **macierzy kowariancji** danych. Wektory własne (tzw. **principal components**) wskazują kierunki największej wariancji w danych, a odpowiadające im wartości własne mówią, jak duża jest ta wariancja. Pierwsza główna składowa (wektor własny o największej wartości własnej) to kierunek, w którym dane są najbardziej "rozstrzelone".
*   **Zastosowanie:** Przez rzutowanie danych na podprzestrzeń rozpiętą przez kilka pierwszych wektorów własnych (o największych wartościach własnych) można znacząco zredukować liczbę wymiarów, zachowując jednocześnie większość informacji (wariancji). Używane w kompresji obrazów, wizualizacji danych i jako krok wstępny przed zastosowaniem innych algorytmów uczenia maszynowego.

**2. Algorytm PageRank (Google)**

PageRank to algorytm, który był podstawą sukcesu wyszukiwarki Google. Służy do oceny "ważności" stron internetowych w sieci. Sieć WWW jest modelowana jako graf skierowany, gdzie strony to wierzchołki, a linki to krawędzie.

*   **Jak to działa?** PageRank definiuje ważność strony jako prawdopodobieństwo, że losowy internauta, klikający w linki, znajdzie się na tej stronie. Okazuje się, że wektor tych prawdopodobieństw (wektor PageRank) jest **wektorem własnym** macierzy przejść tego grafu (odpowiednio zmodyfikowanej), odpowiadającym **wartości własnej równej 1**.
*   **Znaczenie:** Znalezienie dominującego wektora własnego macierzy reprezentującej całą sieć WWW pozwala uszeregować strony według ich ważności.

**3. Grafika komputerowa i deformacje**

Wektory własne macierzy transformacji (np. macierzy odkształceń) wskazują kierunki, w których obiekt jest rozciągany lub ściskany w najprostszy sposób, bez ścinania (shear). Analiza własna pozwala zrozumieć i kontrolować deformacje obiektów 3D.

**4. Mechanika kwantowa i chemia obliczeniowa**

W mechanice kwantowej stany stacjonarne systemu (np. poziomy energetyczne elektronu w atomie) są opisywane przez wektory własne operatora Hamiltona, a odpowiadające im wartości własne to właśnie te poziomy energetyczne.

#### Przykłady

**Przykład 1: Znajdowanie wartości i wektorów własnych**

Znajdź wartości i wektory własne macierzy $A = \begin{bmatrix} 4 & 1 \\ 2 & 3 \end{bmatrix}$.

1.  **Równanie charakterystyczne:**
    $det(A - \lambda I) = det(\begin{bmatrix} 4-\lambda & 1 \\ 2 & 3-\lambda \end{bmatrix}) = (4-\lambda)(3-\lambda) - 1*2 = 0$
    $12 - 4\lambda - 3\lambda + \lambda^2 - 2 = 0$
    $\lambda^2 - 7\lambda + 10 = 0$
    $(\lambda - 5)(\lambda - 2) = 0$
    Wartości własne: $\lambda_1 = 5$, $\lambda_2 = 2$.

2.  **Wektory własne:**
    *   **Dla $\lambda_1 = 5$:**
        $(A - 5I)v = 0 \implies \begin{bmatrix} -1 & 1 \\ 2 & -2 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}$
        $-x + y = 0 \implies y = x$. Wektor własny ma postać $v_1 = \begin{bmatrix} x \\ x \end{bmatrix} = x \begin{bmatrix} 1 \\ 1 \end{bmatrix}$. Przyjmujemy np. $v_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$.
    *   **Dla $\lambda_2 = 2$:**
        $(A - 2I)v = 0 \implies \begin{bmatrix} 2 & 1 \\ 2 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}$
        $2x + y = 0 \implies y = -2x$. Wektor własny ma postać $v_2 = \begin{bmatrix} x \\ -2x \end{bmatrix} = x \begin{bmatrix} 1 \\ -2 \end{bmatrix}$. Przyjmujemy np. $v_2 = \begin{bmatrix} 1 \\ -2 \end{bmatrix}$.

#### Podsumowanie

*   **Wektor własny** macierzy $A$ to niezerowy wektor $v$, którego kierunek nie zmienia się pod wpływem transformacji $A$ ($Av = \lambda v$).
*   **Wartość własna** $\lambda$ to skalar, o który wektor własny jest mnożony.
*   Wartości własne znajdujemy jako pierwiastki **równania charakterystycznego** $det(A - \lambda I) = 0$.
*   Wektory własne znajdujemy, rozwiązując układ równań $(A - \lambda I)v = 0$ dla każdej wartości własnej.
*   Kluczowe zastosowania w informatyce to **PCA** (redukcja wymiarowości przez znalezienie kierunków największej wariancji), **algorytm PageRank** (ranking stron WWW przez znalezienie dominującego wektora własnego macierzy grafu) oraz **grafika komputerowa**.

**Typowe pytania egzaminacyjne:**
*   Co to jest wartość własna i wektor własny macierzy? Proszę podać definicję i interpretację geometryczną.
*   Jak wyznacza się wartości i wektory własne macierzy?
*   Proszę omówić zastosowanie wartości własnych w informatyce na wybranym przykładzie (np. PCA lub PageRank).
*   Proszę znaleźć wartości i wektory własne podanej macierzy 2x2.

---

# 5. Grafy i ich typy, metody reprezentacji grafów

#### Wprowadzenie

Teoria grafów to dziedzina matematyki i informatyki, która zajmuje się badaniem grafów – abstrakcyjnych struktur służących do modelowania relacji między obiektami. Grafy stanowią jeden z najbardziej uniwersalnych i fundamentalnych modeli w informatyce, pozwalając w jednolity sposób opisywać i analizować tak różnorodne problemy, jak sieci komputerowe, połączenia lotnicze, zależności między zadaniami, media społecznościowe czy struktura stron internetowych. Zrozumienie typów grafów oraz efektywnych sposobów ich reprezentacji w pamięci komputera jest kluczowe dla projektowania i implementacji algorytmów grafowych.

#### Szczegółowe wyjaśnienie

Formalnie, graf $G$ to para $(V, E)$, gdzie:

*   $V$ (ang. *vertices*) to zbiór **wierzchołków** (nazywanych też węzłami).
*   $E$ (ang. *edges*) to zbiór **krawędzi**, które łączą pary wierzchołków.

**Typy grafów**

Grafy można klasyfikować na wiele sposobów, w zależności od właściwości ich krawędzi i struktury.

1.  **Graf nieskierowany (Undirected Graph):** Krawędzie nie mają orientacji. Jeśli istnieje krawędź między wierzchołkami A i B, to relacja jest symetryczna (można przejść z A do B i z B do A). Przykład: sieć znajomych na Facebooku.

2.  **Graf skierowany (Directed Graph, Digraph):** Każda krawędź ma określony kierunek (jest parą uporządkowaną $(u, v)$). Krawędź z A do B nie implikuje istnienia krawędzi z B do A. Przykład: sieć obserwowanych na Twitterze, zależności w projekcie.

3.  **Graf ważony (Weighted Graph):** Każdej krawędzi przypisana jest liczba (waga lub koszt), która może reprezentować odległość, czas, przepustowość itp. Przykład: mapa drogowa z odległościami między miastami.

4.  **Graf prosty (Simple Graph):** Graf, w którym między dowolną parą wierzchołków istnieje co najwyżej jedna krawędź i nie ma pętli (krawędzi łączących wierzchołek z samym sobą).

5.  **Multigraf:** Graf, w którym dopuszczalne są wielokrotne krawędzie między tymi samymi wierzchołkami oraz pętle.

6.  **Graf pełny (Complete Graph):** Graf prosty, w którym każda para różnych wierzchołków jest połączona krawędzią. Oznaczany jako $K_n$ dla grafu o $n$ wierzchołkach.

7.  **Graf dwudzielny (Bipartite Graph):** Graf, którego zbiór wierzchołków można podzielić na dwa rozłączne podzbiory, $U$ i $W$, tak że każda krawędź łączy wierzchołek z $U$ z wierzchołkiem z $W$. Przykład: modelowanie dopasowań (np. pracownicy do zadań).

8.  **Drzewo (Tree):** Spójny graf acykliczny (niezawierający cykli). Jest to szczególny, ale bardzo ważny typ grafu.

#### Metody reprezentacji grafów

Aby przetwarzać grafy za pomocą komputera, musimy je zapisać w pamięci. Dwie najpopularniejsze metody to macierz sąsiedztwa i listy sąsiedztwa.

**1. Macierz sąsiedztwa (Adjacency Matrix)**

Jest to macierz kwadratowa $M$ o wymiarach $n \times n$, gdzie $n$ to liczba wierzchołków. Element $M[i][j]$ opisuje krawędź między wierzchołkiem $i$ a $j$:

*   **Dla grafu nieważonego:**
    $M[i][j] = 1$, jeśli istnieje krawędź między $i$ a $j$.
    $M[i][j] = 0$, w przeciwnym razie.
*   **Dla grafu ważonego:**
    $M[i][j] = waga$, jeśli istnieje krawędź o wadze $w$ między $i$ a $j$.
    $M[i][j] = 0$ lub $\infty$, jeśli krawędź nie istnieje.

Dla grafów nieskierowanych macierz sąsiedztwa jest symetryczna ($M[i][j] = M[j][i]$).

**2. Listy sąsiedztwa (Adjacency Lists)**

Ta reprezentacja składa się z tablicy (lub listy) list. Dla każdego wierzchołka $u$ przechowujemy listę wierzchołków, do których prowadzą krawędzie z $u$. Innymi słowy, dla każdego wierzchołka tworzymy listę jego sąsiadów.

*   **Dla grafu nieważonego:** Tablica, gdzie `adj[i]` zawiera listę numerów wierzchołków sąsiadujących z wierzchołkiem `i`.
*   **Dla grafu ważonego:** `adj[i]` zawiera listę par `(sąsiad, waga)`. 

**Porównanie metod reprezentacji**

Niech $n$ będzie liczbą wierzchołków, a $m$ liczbą krawędzi.

| Operacja | Macierz Sąsiedztwa | Listy Sąsiedztwa |
|---|---|---|
| **Złożoność pamięciowa** | $O(n^2)$ | $O(n+m)$ |
| **Sprawdzenie istnienia krawędzi (i, j)** | $O(1)$ | $O(deg(i))$ * |
| **Pobranie wszystkich sąsiadów wierzchołka i** | $O(n)$ | $O(deg(i))$ * |
| **Dodanie/usunięcie krawędzi** | $O(1)$ | $O(deg(i))$ * |

* $deg(i)$ to stopień wierzchołka $i$ (liczba jego sąsiadów).

**Wybór reprezentacji:**

*   **Macierz sąsiedztwa** jest lepsza dla **grafów gęstych**, gdzie liczba krawędzi $m$ jest bliska $n^2$. Sprawdzanie istnienia krawędzi jest błyskawiczne.
*   **Listy sąsiedztwa** są znacznie lepsze dla **grafów rzadkich** (większość grafów spotykanych w praktyce, np. sieci społeczne), gdzie $m$ jest znacznie mniejsze od $n^2$. Są o wiele bardziej oszczędne pamięciowo, a iterowanie po sąsiadach jest bardzo wydajne.

#### Praktyczne zastosowania

*   **Sieci społecznościowe:** Wierzchołki to użytkownicy, krawędzie to znajomości/obserwacje. Analiza grafu pozwala na rekomendowanie znajomych, identyfikację społeczności.
*   **Systemy nawigacji (GPS):** Wierzchołki to skrzyżowania, krawędzie to drogi z wagami (długość, czas przejazdu). Algorytmy grafowe (np. Dijkstry) znajdują najkrótszą trasę.
*   **Internet:** Wierzchołki to strony WWW, krawędzie to hiperłącza. Algorytmy takie jak PageRank używają struktury grafu do oceny ważności stron.
*   **Zarządzanie zależnościami:** Wierzchołki to zadania lub pakiety oprogramowania, krawędzie to zależności. Sortowanie topologiczne pozwala ustalić prawidłową kolejność wykonania.
*   **Kompilatory:** Grafy przepływu sterowania i grafy zależności danych są używane do analizy i optymalizacji kodu.

#### Przykład

Rozważmy prosty, nieskierowany i nieważony graf:

*   $V = \{1, 2, 3, 4\}$
*   $E = \{(1,2), (1,3), (2,3), (2,4), (3,4)\}$

**Reprezentacja macierzą sąsiedztwa:**

$$ M = \begin{bmatrix} 0 & 1 & 1 & 0 \\ 1 & 0 & 1 & 1 \\ 1 & 1 & 0 & 1 \\ 0 & 1 & 1 & 0 \end{bmatrix} $$

**Reprezentacja listami sąsiedztwa:**

*   `1: [2, 3]`
*   `2: [1, 3, 4]`
*   `3: [1, 2, 4]`
*   `4: [2, 3]`

#### Podsumowanie

*   **Graf** to struktura składająca się z wierzchołków i krawędzi, modelująca relacje między obiektami.
*   Wyróżniamy wiele **typów grafów**, m.in. skierowane/nieskierowane, ważone/nieważone, proste/multigrafy.
*   Dwie główne metody **reprezentacji grafów** w pamięci komputera to **macierz sąsiedztwa** i **listy sąsiedztwa**.
*   **Macierz sąsiedztwa** ($O(n^2)$ pamięci) jest dobra dla grafów gęstych i szybkiego sprawdzania krawędzi.
*   **Listy sąsiedztwa** ($O(n+m)$ pamięci) są standardowym wyborem dla grafów rzadkich ze względu na oszczędność pamięci i wydajne iterowanie po sąsiadach.
*   Grafy mają fundamentalne znaczenie w modelowaniu problemów z dziedziny **sieci, logistyki, mediów społecznościowych i wielu innych**.

**Typowe pytania egzaminacyjne:**
*   Co to jest graf? Proszę podać formalną definicję.
*   Proszę wymienić i krótko scharakteryzować znane typy grafów.
*   Jakie są metody reprezentacji grafów w pamięci komputera? Proszę je opisać.
*   Proszę porównać macierz sąsiedztwa i listy sąsiedztwa, podając ich wady i zalety oraz złożoność pamięciową.
*   Dla jakiego typu grafów (gęstych/rzadkich) lepsza jest macierz sąsiedztwa, a dla jakich listy sąsiedztwa? Proszę uzasadnić.

---

# 6. Relacje binarne, własności i metody reprezentacji

#### Wprowadzenie

Relacje binarne (dwuargumentowe) są fundamentalnym pojęciem matematycznym, które formalizuje ideę powiązania między elementami. W informatyce stanowią one podstawę teoretyczną dla wielu kluczowych struktur i koncepcji, takich jak relacyjne bazy danych, teoria grafów, czy analiza porządku zadań. Relacja opisuje, czy pewien związek zachodzi między dwoma obiektami. Zrozumienie własności relacji, takich jak zwrotność, symetria czy przechodniość, pozwala na ich klasyfikację i wykorzystanie ich specyficznej struktury do rozwiązywania problemów.

#### Szczegółowe wyjaśnienie

**Definicja relacji binarnej**

Formalnie, relacja binarna $R$ ze zbioru $A$ do zbioru $B$ to dowolny podzbiór **iloczynu kartezjańskiego** $A \times B$. Iloczyn kartezjański $A \times B$ to zbiór wszystkich możliwych par uporządkowanych $(a, b)$, gdzie $a \in A$ i $b \in B$.

$$ R \subseteq A \times B $$

Jeśli para $(a, b)$ należy do relacji $R$, mówimy, że element $a$ jest w relacji z elementem $b$, i zapisujemy to jako $aRb$. Jeśli zbiory $A$ i $B$ są takie same ($A=B$), mówimy o **relacji na zbiorze A**.

**Własności relacji na zbiorze A**

Analiza własności relacji jest kluczowa dla ich zrozumienia i klasyfikacji. Najważniejsze z nich to:

1.  **Zwrotność (Reflexivity):** Relacja jest zwrotna, jeśli każdy element jest w relacji sam z sobą.
    $$ \forall a \in A: aRa $$
    *Przykład: Relacja "mniejszy lub równy" ($\le$) na zbiorze liczb rzeczywistych jest zwrotna, bo każda liczba jest mniejsza lub równa samej sobie ($a \le a$).*

2.  **Symetryczność (Symmetry):** Relacja jest symetryczna, jeśli dla dowolnych dwóch elementów, fakt, że pierwszy jest w relacji z drugim, implikuje, że drugi jest w relacji z pierwszym.
    $$ \forall a, b \in A: (aRb \implies bRa) $$
    *Przykład: Relacja "bycia w tym samym wieku" jest symetryczna. Jeśli Ania jest w tym samym wieku co Bartek, to Bartek jest w tym samym wieku co Ania.*

3.  **Przechodniość (Transitivity):** Relacja jest przechodnia, jeśli dla dowolnych trzech elementów, fakt, że pierwszy jest w relacji z drugim, a drugi z trzecim, implikuje, że pierwszy jest w relacji z trzecim.
    $$ \forall a, b, c \in A: (aRb \land bRc \implies aRc) $$
    *Przykład: Relacja "bycia przodkiem" jest przechodnia. Jeśli X jest przodkiem Y, a Y jest przodkiem Z, to X jest przodkiem Z.*

4.  **Antysymetria (Antisymmetry):** Relacja jest antysymetryczna, jeśli dla dowolnych dwóch różnych elementów nie mogą one być jednocześnie w relacji w obie strony. Formalnie, jeśli element jest w relacji z drugim, a drugi z pierwszym, to muszą to być te same elementy.
    $$ \forall a, b \in A: (aRb \land bRa \implies a=b) $$
    *Przykład: Relacja "mniejszy lub równy" ($\le$) jest antysymetryczna. Jeśli $a \le b$ i $b \le a$, to musi zachodzić $a=b$.*

**Szczególne typy relacji**

Kombinacje powyższych własności definiują ważne klasy relacji:

*   **Relacja równoważności (Equivalence Relation):** To relacja, która jest **zwrotna, symetryczna i przechodnia**. Dzieli ona zbiór na rozłączne podzbiory, zwane **klasami abstrakcji**, gdzie wszystkie elementy w jednej klasie są ze sobą w relacji. Przykład: relacja przystawania modulo n.

*   **Częściowy porządek (Partial Order):** To relacja, która jest **zwrotna, antysymetryczna i przechodnia**. Umożliwia ona porównywanie niektórych (ale niekoniecznie wszystkich) par elementów. Przykład: relacja zawierania się zbiorów ($\subseteq$).

#### Metody reprezentacji relacji

Relacje binarne można reprezentować na kilka sposobów, z których każdy ma swoje zalety.

1.  **Zbiór par uporządkowanych:** To podstawowa, formalna reprezentacja. Relację $R$ na zbiorze $A = \{1, 2, 3\}$ można zapisać jako $R = \{(1,1), (1,2), (2,3), (3,1)\}$.

2.  **Macierz relacji (Macierz sąsiedztwa):** Dla relacji na zbiorze $A$ o $n$ elementach, tworzymy macierz $M$ o wymiarach $n \times n$. Element $M[i][j] = 1$, jeśli $i$-ty element jest w relacji z $j$-tym, i $0$ w przeciwnym razie. Jest to ta sama koncepcja co macierz sąsiedztwa dla grafu.

3.  **Graf relacji (Digraf):** Relację na zbiorze $A$ można przedstawić jako graf skierowany, gdzie wierzchołkami są elementy zbioru $A$. Krawędź skierowana od $a$ do $b$ istnieje wtedy i tylko wtedy, gdy $aRb$. Pętla w wierzchołku $a$ oznacza, że $aRa$.

**Własności w reprezentacjach:**

| Własność | W reprezentacji macierzowej | W reprezentacji grafowej |
|---|---|---|
| **Zwrotność** | Wszystkie elementy na głównej przekątnej są równe 1. | Każdy wierzchołek ma pętlę. |
| **Symetria** | Macierz jest symetryczna ($M = M^T$). | Jeśli istnieje krawędź z $a$ do $b$, to istnieje też z $b$ do $a$. |
| **Antysymetria** | Jeśli $M[i][j]=1$ i $i \neq j$, to $M[j][i]=0$. | Jeśli istnieje krawędź z $a$ do $b$ ($a \neq b$), to nie ma krawędzi z $b$ do $a$. |
| **Przechodniość** | Jeśli $M[i][j]=1$ i $M[j][k]=1$, to $M[i][k]=1$. | Jeśli istnieje ścieżka z $a$ do $b$ i z $b$ do $c$, to istnieje krawędź z $a$ do $c$. |

#### Praktyczne zastosowania

*   **Relacyjne bazy danych:** Cały model relacyjny opiera się na matematycznym pojęciu relacji. Tabela w bazie danych jest reprezentacją relacji, a wiersze to krotki należące do tej relacji.
*   **Teoria grafów:** Każdy graf skierowany jest wizualną reprezentacją relacji binarnej. Własności relacji przekładają się na właściwości strukturalne grafu.
*   **Kompilatory i analiza programów:** Relacje zależności między zmiennymi lub instrukcjami programu są kluczowe dla optymalizacji kodu.
*   **Sztuczna inteligencja:** Sieci semantyczne i ontologie, używane do reprezentacji wiedzy, modelują związki między pojęciami za pomocą relacji.

#### Przykład

Niech dany będzie zbiór $A = \{1, 2, 3\}$ i relacja $R$ zdefiniowana jako $aRb \iff a \le b$.

*   **Zbiór par:** $R = \{(1,1), (1,2), (1,3), (2,2), (2,3), (3,3)\}$
*   **Macierz relacji:**
    $$ M_R = \begin{bmatrix} 1 & 1 & 1 \\ 0 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix} $$
*   **Graf relacji:** Graf z trzema wierzchołkami, pętlami na każdym z nich i krawędziami $(1,2), (1,3), (2,3)$.

**Analiza własności:**
*   **Zwrotna:** Tak, bo $a \le a$ (na przekątnej są same jedynki).
*   **Symetryczna:** Nie, bo $1R2$, ale nieprawda, że $2R1$.
*   **Antysymetryczna:** Tak, bo jeśli $a \le b$ i $b \le a$, to $a=b$.
*   **Przechodnia:** Tak, bo jeśli $a \le b$ i $b \le c$, to $a \le c$.

Ponieważ relacja jest zwrotna, antysymetryczna i przechodnia, jest to **częściowy porządek**.

#### Podsumowanie

*   **Relacja binarna** to zbiór par uporządkowanych, formalizujący związek między elementami.
*   Kluczowe **własności** relacji to **zwrotność, symetria, antysymetria i przechodniość**.
*   Kombinacje tych własności definiują ważne struktury, takie jak **relacje równoważności** i **częściowe porządki**.
*   Relacje można **reprezentować** jako zbiór par, **macierz relacji** lub **graf skierowany**.
*   Relacje są teoretyczną podstawą **relacyjnych baz danych**, **teorii grafów** i wielu innych dziedzin informatyki.

**Typowe pytania egzaminacyjne:**
*   Co to jest relacja binarna? Proszę podać definicję.
*   Proszę zdefiniować zwrotność, symetrię i przechodniość relacji.
*   Czym charakteryzuje się relacja równoważności, a czym częściowy porządek?
*   Jakie są metody reprezentacji relacji? Proszę je omówić.
*   Dla podanej relacji (np. w postaci grafu lub macierzy) proszę zbadać jej własności.

---

# 7. Zasada indukcji matematycznej

#### Wprowadzenie

Zasada indukcji matematycznej to jedna z najważniejszych i najpotężniejszych metod dowodzenia twierdzeń dotyczących liczb naturalnych (lub, ogólniej, dowolnych zbiorów o podobnej, "schodkowej" strukturze). Pozwala ona udowodnić, że pewna własność jest prawdziwa dla nieskończonej liczby przypadków, wykonując jedynie dwa skończone kroki. W informatyce indukcja jest absolutnie fundamentalnym narzędziem, używanym przede wszystkim do dowodzenia poprawności algorytmów (zarówno iteracyjnych, jak i rekurencyjnych) oraz do analizy ich złożoności. Można ją przyrównać do efektu domina: jeśli potrafimy przewrócić pierwszy klocek i udowodnimy, że każdy przewracający się klocek pociąga za sobą następny, to mamy pewność, że wszystkie klocki się przewrócą.

#### Szczegółowe wyjaśnienie

**Zasada Indukcji Matematycznej**

Niech $T(n)$ będzie pewnym twierdzeniem (zdaniem logicznym) zależnym od liczby naturalnej $n$. Aby udowodnić, że $T(n)$ jest prawdziwe dla wszystkich liczb naturalnych $n$ począwszy od pewnej wartości $n_0$, należy wykonać dwa kroki:

1.  **Krok bazowy (Base Case):** Udowodnić, że twierdzenie $T(n_0)$ jest prawdziwe. Najczęściej $n_0=0$ lub $n_0=1$. To jest nasz "pierwszy klocek domina".

2.  **Krok indukcyjny (Inductive Step):** Udowodnić, że dla dowolnej liczby naturalnej $k \ge n_0$, jeśli założymy, że $T(k)$ jest prawdziwe (**założenie indukcyjne**), to z tego założenia wynika, że $T(k+1)$ również jest prawdziwe. Formalnie, dowodzimy implikacji:
    $$ \forall k \ge n_0: (T(k) \implies T(k+1)) $$
    To jest dowód, że "każdy klocek przewraca następny".

Jeśli oba te kroki zostaną pomyślnie przeprowadzone, to na mocy zasady indukcji matematycznej możemy stwierdzić, że twierdzenie $T(n)$ jest prawdziwe dla wszystkich liczb naturalnych $n \ge n_0$.

**Logika działania:** Krok bazowy daje nam pewny start ($T(n_0)$ jest prawdą). Krok indukcyjny to "silnik", który przenosi prawdziwość na kolejne liczby. Skoro $T(n_0)$ jest prawdą, to z kroku indukcyjnego (dla $k=n_0$) wynika, że $T(n_0+1)$ jest prawdą. Skoro teraz wiemy, że $T(n_0+1)$ jest prawdą, to z kroku indukcyjnego (dla $k=n_0+1$) wynika, że $T(n_0+2)$ jest prawdą, i tak w nieskończoność.

#### Praktyczne zastosowania w informatyce

**1. Dowodzenie poprawności algorytmów**

To najważniejsze zastosowanie indukcji w informatyce. Pozwala formalnie udowodnić, że dany fragment kodu działa zgodnie ze specyfikacją dla wszystkich dopuszczalnych danych wejściowych.

*   **Algorytmy rekurencyjne:** Dowodzenie poprawności funkcji rekurencyjnych jest naturalnym zastosowaniem indukcji.
    *   **Krok bazowy:** Dowodzimy, że funkcja zwraca poprawny wynik dla bazowego przypadku rekurencji (np. dla n=0 w funkcji obliczającej silnię).
    *   **Krok indukcyjny:** Zakładamy (założenie indukcyjne), że funkcja działa poprawnie dla mniejszych wartości (np. dla $k$), i używamy tego faktu, aby udowodnić, że zadziała poprawnie dla wartości $k+1$.

*   **Algorytmy iteracyjne (pętle):** Poprawność pętli dowodzi się za pomocą tzw. **niezmienników pętli (loop invariants)**. Niezmiennik to warunek, który:
    1.  Jest prawdziwy przed pierwszym wykonaniem pętli (krok bazowy).
    2.  Jeśli jest prawdziwy przed kolejną iteracją (założenie indukcyjne), to pozostaje prawdziwy po jej zakończeniu (krok indukcyjny).

    Jeśli potrafimy znaleźć taki niezmiennik, który po zakończeniu pętli (gdy warunek pętli staje się fałszywy) wraz z tym warunkiem implikuje poprawność wyniku, to udowodniliśmy poprawność algorytmu.

**2. Analiza złożoności obliczeniowej**

Indukcja jest często używana do dowodzenia wzorów na złożoność czasową lub pamięciową algorytmów, zwłaszcza rekurencyjnych. Na przykład, można indukcyjnie udowodnić, że rozwiązaniem pewnego równania rekurencyjnego opisującego złożoność algorytmu "dziel i zwyciężaj" jest $O(n \log n)$.

**3. Dowodzenie własności struktur danych**

Można użyć indukcji do dowodzenia twierdzeń o strukturach danych. Na przykład, można udowodnić, że pełne drzewo binarne o wysokości $h$ ma dokładnie $2^{h+1}-1$ wierzchołków.

#### Przykłady

**Przykład 1: Dowód wzoru na sumę liczb**

Udowodnijmy, że dla każdego $n \ge 1$ zachodzi: $T(n): 1 + 2 + 3 + \dots + n = \frac{n(n+1)}{2}$.

1.  **Krok bazowy (dla n=1):**
    Lewa strona: $1$.
    Prawa strona: $\frac{1(1+1)}{2} = \frac{2}{2} = 1$.
    $L=P$, więc $T(1)$ jest prawdziwe.

2.  **Krok indukcyjny:**
    **Założenie indukcyjne:** Zakładamy, że $T(k)$ jest prawdziwe dla pewnego $k \ge 1$, czyli:
    $1 + 2 + \dots + k = \frac{k(k+1)}{2}$.
    **Teza indukcyjna:** Chcemy udowodnić, że $T(k+1)$ jest prawdziwe, czyli:
    $1 + 2 + \dots + k + (k+1) = \frac{(k+1)((k+1)+1)}{2} = \frac{(k+1)(k+2)}{2}$.

    **Dowód tezy:** Zaczynamy od lewej strony tezy i korzystamy z założenia:
    $L = (1 + 2 + \dots + k) + (k+1)$
    Na mocy założenia indukcyjnego, zastępujemy sumę w nawiasie:
    $L = \frac{k(k+1)}{2} + (k+1)$
    Sprowadzamy do wspólnego mianownika:
    $L = \frac{k(k+1) + 2(k+1)}{2} = \frac{(k+1)(k+2)}{2} = P$.
    Udało nam się przekształcić lewą stronę tezy w prawą, co kończy dowód kroku indukcyjnego.

Na mocy zasady indukcji matematycznej, wzór jest prawdziwy dla wszystkich $n \ge 1$.

**Przykład 2: Poprawność funkcji rekurencyjnej (silnia)**

Rozważmy funkcję `factorial(n)`:
`if n == 0: return 1`
`else: return n * factorial(n-1)`

Udowodnijmy, że `factorial(n)` oblicza $n!$ dla wszystkich $n \ge 0$.

1.  **Krok bazowy (dla n=0):**
    Funkcja zwraca `1`. Z definicji $0! = 1$. Zgadza się.

2.  **Krok indukcyjny:**
    **Założenie indukcyjne:** Zakładamy, że dla pewnego $k \ge 0$, `factorial(k)` poprawnie oblicza $k!$.
    **Teza indukcyjna:** Chcemy udowodnić, że `factorial(k+1)` poprawnie oblicza $(k+1)!$.

    **Dowód tezy:** Dla $n=k+1$ (które jest $>0$), funkcja wykonuje `return (k+1) * factorial(k)`. Z założenia indukcyjnego wiemy, że `factorial(k)` zwróci $k!$. Zatem całe wyrażenie zwróci $(k+1) * k!$. Z definicji silni, $(k+1) * k! = (k+1)!$. To jest dokładnie wartość, którą miała obliczyć funkcja `factorial(k+1)`. Dowód zakończony.

#### Podsumowanie

*   **Zasada indukcji matematycznej** to metoda dowodzenia twierdzeń dla wszystkich liczb naturalnych od pewnego punktu startowego.
*   Składa się z dwóch kroków: **kroku bazowego** (dowód dla pierwszego elementu) i **kroku indukcyjnego** (dowód implikacji $T(k) \implies T(k+1)$).
*   W informatyce jest to kluczowe narzędzie do **dowodzenia poprawności algorytmów** (rekurencyjnych i iteracyjnych przez niezmienniki pętli) oraz do **analizy ich złożoności**.
*   Pozwala na formalne i rygorystyczne upewnienie się, że kod działa zgodnie z oczekiwaniami dla nieskończonej liczby przypadków.

**Typowe pytania egzaminacyjne:**
*   Na czym polega zasada indukcji matematycznej? Proszę opisać jej kroki.
*   Proszę udowodnić za pomocą indukcji matematycznej podany wzór (np. na sumę kwadratów, sumę szeregu geometrycznego).
*   Jakie jest zastosowanie indukcji matematycznej w informatyce? Proszę omówić na przykładzie dowodzenia poprawności algorytmu.
*   Co to jest niezmiennik pętli i jaki ma związek z indukcją matematyczną?

---

# 8. Twierdzenie Bayesa

#### Wprowadzenie

Twierdzenie Bayesa to fundamentalne prawo teorii prawdopodobieństwa, które opisuje, jak zaktualizować naszą wiarę (prawdopodobieństwo) w prawdziwość hipotezy w świetle nowych dowodów. Pozwala ono formalnie połączyć prawdopodobieństwo początkowe (to, co wiemy przed uzyskaniem dowodu) z prawdopodobieństwem warunkowym (informacją, jaką niesie dowód), aby uzyskać zaktualizowane prawdopodobieństwo końcowe. W informatyce twierdzenie to jest kamieniem węgielnym dla całej gałęzi uczenia maszynowego zwanej statystyką bayesowską, a jego zastosowania sięgają od filtrowania spamu, przez systemy diagnostyki medycznej, po autonomiczne pojazdy.

#### Szczegółowe wyjaśnienie

**Prawdopodobieństwo warunkowe**

Zanim przejdziemy do twierdzenia Bayesa, musimy zrozumieć **prawdopodobieństwo warunkowe**, oznaczane jako $P(A|B)$. Jest to prawdopodobieństwo zajścia zdarzenia $A$, pod warunkiem, że zaszło zdarzenie $B$. Oblicza się je ze wzoru:

$$ P(A|B) = \frac{P(A \cap B)}{P(B)} $$

gdzie $P(A \cap B)$ to prawdopodobieństwo, że zajdą oba zdarzenia naraz.

**Twierdzenie Bayesa**

Twierdzenie Bayesa w swojej najprostszej formie pozwala "odwrócić" prawdopodobieństwo warunkowe. Jeśli znamy $P(B|A)$, możemy obliczyć $P(A|B)$. Wzór ma postać:

$$ P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)} $$

**Interpretacja składników wzoru:**

*   $P(A|B)$ – **prawdopodobieństwo a posteriori** (końcowe). Jest to prawdopodobieństwo hipotezy $A$ po uwzględnieniu dowodu $B$. To jest to, co chcemy obliczyć.
*   $P(B|A)$ – **wiarygodność (likelihood)**. Jest to prawdopodobieństwo zaobserwowania dowodu $B$, przy założeniu, że hipoteza $A$ jest prawdziwa.
*   $P(A)$ – **prawdopodobieństwo a priori** (początkowe). Jest to nasza początkowa wiara w prawdziwość hipotezy $A$, zanim uzyskaliśmy jakikolwiek dowód.
*   $P(B)$ – **prawdopodobieństwo brzegowe (marginal likelihood)**. Jest to całkowite prawdopodobieństwo zaobserwowania dowodu $B$, niezależnie od hipotezy. Często oblicza się je za pomocą wzoru na prawdopodobieństwo całkowite:
    $P(B) = P(B|A)P(A) + P(B|\neg A)P(\neg A)$, gdzie $\neg A$ to hipoteza przeciwna do $A$.

**Wersja rozszerzona (dla wielu hipotez)**

Jeśli mamy zbiór wykluczających się i wyczerpujących wszystkich możliwości hipotez $H_1, H_2, \dots, H_n$, to prawdopodobieństwo hipotezy $H_i$ w świetle dowodu $E$ wynosi:

$$ P(H_i|E) = \frac{P(E|H_i) \cdot P(H_i)}{\sum_{j=1}^{n} P(E|H_j) \cdot P(H_j)} $$

#### Praktyczne zastosowania w informatyce

**1. Filtry antyspamowe (Klasyfikator Naiwny Bayesa)**

To klasyczne i jedno z pierwszych skutecznych zastosowań twierdzenia Bayesa. Celem jest obliczenie prawdopodobieństwa, że dany e-mail jest spamem, biorąc pod uwagę słowa, które zawiera.

*   **Hipoteza:** E-mail jest spamem ($S$) lub nie jest spamem ($\neg S$).
*   **Dowód:** E-mail zawiera określone słowa ($W_1, W_2, \dots, W_n$).
*   **Cel:** Obliczyć $P(S | W_1, W_2, \dots, W_n)$.

**Klasyfikator Naiwny Bayesa** (ang. *Naive Bayes Classifier*) upraszcza problem, przyjmując "naiwne" założenie, że wystąpienia słów w e-mailu są od siebie niezależne. Mimo że to założenie jest w rzeczywistości fałszywe (słowa często występują razem), klasyfikator działa zaskakująco dobrze w praktyce. Oblicza on "wynik spamowości" na podstawie częstości występowania poszczególnych słów w historycznych danych (e-mailach oznaczonych jako spam i nie-spam).

**2. Diagnostyka medyczna i systemy eksperckie**

Systemy wspomagające diagnozę mogą używać twierdzenia Bayesa do obliczenia prawdopodobieństwa, że pacjent cierpi na daną chorobę, na podstawie wyników testów i obserwowanych objawów.

*   **Hipoteza:** Pacjent ma chorobę $Ch$.
*   **Dowód:** Wynik testu jest pozytywny ($T+$).
*   **Cel:** Obliczyć $P(Ch | T+)$.

Twierdzenie Bayesa pozwala tu uwzględnić niedoskonałość testów (ich czułość i specyficzność) oraz bazowe prawdopodobieństwo występowania choroby w populacji.

**3. Rozpoznawanie mowy i przetwarzanie języka naturalnego (NLP)**

Modele językowe często muszą odgadnąć, jakie jest najbardziej prawdopodobne słowo lub zdanie, biorąc pod uwagę usłyszany sygnał akustyczny lub poprzedzający kontekst. Sieci bayesowskie, będące uogólnieniem twierdzenia Bayesa na wiele zmiennych, są tu potężnym narzędziem.

**4. Uczenie maszynowe i sieci bayesowskie**

Cała dziedzina uczenia bayesowskiego opiera się na tej koncepcji. Zamiast szukać jednej, "najlepszej" wartości parametrów modelu, metody bayesowskie starają się znaleźć cały rozkład prawdopodobieństwa dla tych parametrów, co pozwala na lepsze kwantyfikowanie niepewności modelu.

#### Przykład

Załóżmy, że pewna choroba występuje u 1% populacji. Stworzono test do jej wykrywania, który ma następujące właściwości:

*   Jeśli osoba jest chora, test daje wynik pozytywny w 99% przypadków (czułość).
*   Jeśli osoba jest zdrowa, test daje wynik pozytywny w 2% przypadków (fałszywe alarmy, 1 - specyficzność).

Pacjent otrzymuje pozytywny wynik testu. Jakie jest prawdopodobieństwo, że jest on faktycznie chory?

**Oznaczenia:**
*   $Ch$ – zdarzenie "pacjent jest chory".
*   $Z$ – zdarzenie "pacjent jest zdrowy".
*   $T+$ – zdarzenie "test dał wynik pozytywny".

**Dane:**
*   $P(Ch) = 0.01$ (prawdopodobieństwo a priori)
*   $P(Z) = 1 - P(Ch) = 0.99$
*   $P(T+|Ch) = 0.99$ (czułość)
*   $P(T+|Z) = 0.02$ (fałszywe alarmy)

**Cel:** Obliczyć $P(Ch|T+)$.

**Używamy twierdzenia Bayesa:**

$$ P(Ch|T+) = \frac{P(T+|Ch) \cdot P(Ch)}{P(T+)} $$

Najpierw obliczamy mianownik, czyli całkowite prawdopodobieństwo pozytywnego wyniku testu, $P(T+)$:

$P(T+) = P(T+|Ch)P(Ch) + P(T+|Z)P(Z)$
$P(T+) = (0.99 \cdot 0.01) + (0.02 \cdot 0.99) = 0.0099 + 0.0198 = 0.0297$

Teraz możemy obliczyć prawdopodobieństwo a posteriori:

$P(Ch|T+) = \frac{0.99 \cdot 0.01}{0.0297} = \frac{0.0099}{0.0297} = \frac{1}{3} \approx 33.3\%$

**Wniosek:** Mimo bardzo czułego testu i pozytywnego wyniku, prawdopodobieństwo, że pacjent jest faktycznie chory, wynosi tylko 33.3%. Intuicyjnie wydaje się to mało, ale wynika to z faktu, że choroba jest bardzo rzadka, a fałszywe alarmy, choć rzadkie procentowo, generują w liczbach bezwzględnych znacznie więcej pozytywnych wyników niż prawdziwe przypadki choroby.

#### Podsumowanie

*   **Twierdzenie Bayesa** to matematyczny wzór pozwalający na **aktualizację prawdopodobieństwa hipotezy w świetle nowych dowodów**.
*   Wzór: $P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$.
*   Łączy ono prawdopodobieństwo **a priori** (początkowe) z **wiarygodnością** dowodu, dając w wyniku prawdopodobieństwo **a posteriori** (końcowe).
*   Jest podstawą **statystyki bayesowskiej** i ma kluczowe zastosowania w informatyce, w tym w **klasyfikatorach naiwnych Bayesa** (np. filtry spamu), **diagnostyce medycznej** i ogólnie w **uczeniu maszynowym**.
*   Pozwala na formalne rozumowanie w warunkach niepewności i efektywne wykorzystanie dostępnych danych.

**Typowe pytania egzaminacyjne:**
*   Proszę podać i wyjaśnić wzór Bayesa.
*   Jakie jest zastosowanie twierdzenia Bayesa w informatyce? Proszę omówić na przykładzie filtrowania spamu.
*   Proszę rozwiązać zadanie z prawdopodobieństwa warunkowego z użyciem twierdzenia Bayesa (podobne do przykładu z testem medycznym).
*   Co oznaczają terminy: prawdopodobieństwo a priori, a posteriori i wiarygodność?

---

# 9. Testowanie hipotez statystycznych

#### Wprowadzenie

Testowanie hipotez statystycznych to formalna procedura, która pozwala na podejmowanie decyzji i wyciąganie wniosków na temat całej populacji na podstawie danych z losowej próby. Jest to jedno z kluczowych narzędzi wnioskowania statystycznego, które pozwala w sposób obiektywny i ilościowy ocenić, czy zaobserwowane w próbie efekty (np. różnice między grupami, korelacje) są rzeczywiste i występują w całej populacji, czy też mogą być jedynie wynikiem losowej zmienności. W informatyce testowanie hipotez jest fundamentem dla **testów A/B**, analizy wyników eksperymentów, oceny wydajności systemów czy weryfikacji, czy zmiana w algorytmie przyniosła statystycznie istotną poprawę.

#### Szczegółowe wyjaśnienie

Procedura testowania hipotez opiera się na konfrontacji dwóch przeciwstawnych stwierdzeń:

1.  **Hipoteza zerowa ($H_0$):** Jest to hipoteza, którą staramy się obalić. Zazwyczaj reprezentuje ona status quo, brak efektu, brak różnicy lub brak zależności. Przykłady: "średni czas spędzony na stronie jest taki sam dla obu wersji interfejsu", "nowy algorytm nie jest szybszy od starego".

2.  **Hipoteza alternatywna ($H_1$ lub $H_a$):** Jest to hipoteza, którą przyjmiemy, jeśli uda nam się odrzucić hipotezę zerową. Reprezentuje ona to, co badacz chce wykazać. Przykłady: "średni czas spędzony na stronie jest różny dla obu wersji", "nowy algorytm jest szybszy od starego".

**Logika testowania:**

Cała procedura opiera się na założeniu, że **hipoteza zerowa jest prawdziwa**, i obliczeniu, jak bardzo prawdopodobne jest uzyskanie naszych wyników (lub jeszcze bardziej ekstremalnych) przy tym założeniu. Jeśli to prawdopodobieństwo jest bardzo małe, dochodzimy do wniosku, że nasze początkowe założenie ($H_0$) było prawdopodobnie błędne i odrzucamy je na rzecz hipotezy alternatywnej.

**Kluczowe pojęcia:**

*   **Statystyka testowa:** Wartość obliczona na podstawie danych z próby, która mierzy, jak bardzo nasze wyniki odbiegają od tego, czego spodziewalibyśmy się przy prawdziwości $H_0$. Przykłady: statystyka t w teście t-Studenta, statystyka chi-kwadrat.

*   **Poziom istotności ($\alpha$):** Próg prawdopodobieństwa, ustalany *przed* przeprowadzeniem testu, poniżej którego uznajemy wyniki za "statystycznie istotne". Jest to prawdopodobieństwo popełnienia **błędu I rodzaju**. Najczęściej przyjmuje się $\alpha = 0.05$ (czyli 5%).

*   **p-wartość (p-value):** Najważniejszy wynik testu. Jest to obliczone prawdopodobieństwo uzyskania wyników co najmniej tak ekstremalnych, jak te zaobserwowane w próbie, przy założeniu, że hipoteza zerowa jest prawdziwa. **Uwaga:** p-wartość *nie jest* prawdopodobieństwem, że hipoteza zerowa jest prawdziwa!

**Procedura decyzyjna:**

Po obliczeniu p-wartości porównujemy ją z ustalonym poziomem istotności $\alpha$:

*   Jeśli **p-wartość $\le \alpha$**: Odrzucamy hipotezę zerową ($H_0$). Wynik jest **statystycznie istotny**. Mamy podstawy, by sądzić, że obserwowany efekt nie jest dziełem przypadku.
*   Jeśli **p-wartość $> \alpha$**: Nie ma podstaw do odrzucenia hipotezy zerowej ($H_0$). Wynik jest **statystycznie nieistotny**. Nie oznacza to, że $H_0$ jest prawdziwa, a jedynie, że nie udało nam się jej obalić na podstawie zebranych danych.

**Błędy w testowaniu hipotez:**

| Decyzja | $H_0$ jest prawdziwa | $H_0$ jest fałszywa |
|---|---|---|
| **Odrzuć $H_0$** | **Błąd I rodzaju** (fałszywy alarm) | Decyzja poprawna |
| **Nie odrzucaj $H_0$** | Decyzja poprawna | **Błąd II rodzaju** (przeoczenie) |

*   **Błąd I rodzaju ($\alpha$):** Odrzucenie prawdziwej hipotezy zerowej. Uznajemy, że istnieje efekt, podczas gdy go nie ma. Prawdopodobieństwo jego popełnienia kontrolujemy, ustalając poziom istotności $\alpha$.
*   **Błąd II rodzaju ($\beta$):** Nieodrzucenie fałszywej hipotezy zerowej. Przeoczamy istniejący efekt. Prawdopodobieństwo jego popełnienia zależy m.in. od wielkości próby i siły efektu.

#### Praktyczne zastosowania w informatyce

**1. Testy A/B (A/B Testing)**

To fundamentalna technika używana w rozwoju oprogramowania, e-commerce i marketingu cyfrowym do porównywania dwóch wersji produktu (np. strony internetowej, aplikacji, kampanii e-mailowej) w celu określenia, która z nich lepiej realizuje dany cel (np. wyższy współczynnik konwersji, dłuższy czas spędzony na stronie).

*   **Jak to działa?** Użytkownicy są losowo dzieleni na dwie grupy. Grupa A widzi wersję kontrolną (starą), a grupa B widzi wersję testową (nową). Po zebraniu wystarczającej ilości danych przeprowadza się test statystyczny (np. test t-Studenta dla średnich, test chi-kwadrat dla proporcji).
*   **Hipotezy:**
    *   $H_0$: Metryka (np. współczynnik konwersji) jest taka sama dla obu wersji.
    *   $H_1$: Metryka jest różna (lub wyższa) dla wersji B.
*   **Decyzja:** Jeśli p-wartość jest poniżej $\alpha$, odrzucamy $H_0$ i wdrażamy nową wersję, mając statystyczne dowody na jej wyższość.

**2. Ocena wydajności systemów**

Testowanie hipotez pozwala sprawdzić, czy zmiana w kodzie, konfiguracji serwera czy architekturze systemu przyniosła statystycznie istotną poprawę wydajności (np. skrócenie czasu odpowiedzi).

*   **Hipotezy:**
    *   $H_0$: Średni czas odpowiedzi jest taki sam przed i po zmianie.
    *   $H_1$: Średni czas odpowiedzi po zmianie jest niższy.

**3. Weryfikacja modeli uczenia maszynowego**

Po wytrenowaniu nowego modelu klasyfikacyjnego chcemy sprawdzić, czy jest on faktycznie lepszy od modelu bazowego. Można przeprowadzić test statystyczny (np. test McNemara) porównujący trafność obu modeli na tym samym zbiorze testowym, aby sprawdzić, czy różnica w ich wynikach jest istotna statystycznie.

#### Przykład

Firma prowadząca sklep internetowy chce sprawdzić, czy zmiana koloru przycisku "Kup teraz" z niebieskiego na zielony zwiększy współczynnik konwersji. Przeprowadzono test A/B.

*   **Grupa A (kontrolna, niebieski przycisk):** 1000 użytkowników, 100 dokonało zakupu. Konwersja: $p_A = 100/1000 = 10\%$.
*   **Grupa B (testowa, zielony przycisk):** 1000 użytkowników, 125 dokonało zakupu. Konwersja: $p_B = 125/1000 = 12.5\%$.

**Procedura testowa:**
1.  **Hipotezy:**
    *   $H_0: p_A = p_B$ (kolor przycisku nie ma wpływu na konwersję).
    *   $H_1: p_A < p_B$ (zielony przycisk ma wyższą konwersję).
2.  **Poziom istotności:** Ustalamy $\alpha = 0.05$.
3.  **Test statystyczny:** Używamy testu dla dwóch proporcji. Obliczamy statystykę testową $z$ (która dla tych danych wynosi ok. 1.98).
4.  **Obliczenie p-wartości:** Dla statystyki $z=1.98$ i hipotezy jednostronnej, p-wartość wynosi ok. 0.024.
5.  **Decyzja:** Ponieważ **p-wartość (0.024) $\le \alpha$ (0.05)**, odrzucamy hipotezę zerową.

**Wniosek:** Mamy statystycznie istotne dowody na to, że zielony przycisk prowadzi do wyższego współczynnika konwersji. Firma powinna wdrożyć zmianę.

#### Podsumowanie

*   **Testowanie hipotez statystycznych** to metoda wnioskowania o populacji na podstawie danych z próby.
*   Polega na konfrontacji **hipotezy zerowej ($H_0$)** z **hipotezą alternatywną ($H_1$)**.
*   Kluczowe pojęcia to **poziom istotności ($\alpha$)** i **p-wartość**.
*   Decyzję podejmujemy, porównując p-wartość z $\alpha$: jeśli $p \le \alpha$, odrzucamy $H_0$.
*   Możemy popełnić dwa rodzaje błędów: **błąd I rodzaju** (odrzucenie prawdziwej $H_0$) i **błąd II rodzaju** (nieodrzucenie fałszywej $H_0$).
*   W informatyce jest to podstawa **testów A/B**, oceny wydajności i weryfikacji modeli.

**Typowe pytania egzaminacyjne:**
*   Na czym polega testowanie hipotez statystycznych?
*   Co to jest hipoteza zerowa i alternatywna? Proszę podać przykłady.
*   Proszę wyjaśnić pojęcia: poziom istotności, p-wartość, błąd I i II rodzaju.
*   Jak interpretujemy wynik testu, gdy p-wartość jest mniejsza od poziomu istotności?
*   Proszę opisać zastosowanie testowania hipotez w informatyce na przykładzie testów A/B.

---

# 10. Wyznaczanie przedziałów ufności

#### Wprowadzenie

Wyznaczanie przedziałów ufności to, obok testowania hipotez, drugie fundamentalne narzędzie wnioskowania statystycznego. Podczas gdy testowanie hipotez daje zero-jedynkową odpowiedź na pytanie "czy istnieje efekt?", przedziały ufności dostarczają znacznie bogatszej informacji: określają **zakres prawdopodobnych wartości dla nieznanego parametru populacji** (np. średniej, proporcji) na podstawie danych z próby. Zamiast mówić tylko, że nowa wersja strony jest "lepsza", przedział ufności może nam powiedzieć, że "jesteśmy w 95% pewni, że wzrost konwersji wynosi od 1.5% do 3.5%". Daje to nie tylko informację o istnieniu efektu, ale także o jego **wielkości i precyzji naszego oszacowania**, co jest niezwykle cenne w podejmowaniu decyzji biznesowych i inżynierskich.

#### Szczegółowe wyjaśnienie

**Czym jest przedział ufności?**

Przedział ufności to zakres wartości, który z pewnym wysokim prawdopodobieństwem, zwanym **poziomem ufności**, zawiera prawdziwą, nieznaną wartość parametru w populacji. Najczęściej stosuje się poziom ufności 95%.

**Błędna, ale popularna interpretacja:** "Istnieje 95% prawdopodobieństwa, że prawdziwa średnia populacji wpada w ten konkretny przedział (np. od 10.2 do 11.8)".

**Poprawna interpretacja (częstościowa):** "Jeśli wielokrotnie powtarzalibyśmy nasz eksperyment (pobierali losowe próby i dla każdej z nich budowali 95% przedział ufności), to 95% tak skonstruowanych przedziałów zawierałoby prawdziwą wartość parametru populacji".

Innymi słowy, to nie parametr populacji jest losowy, ale nasz przedział, który zależy od losowej próby. Poziom ufności 95% oznacza, że mamy 95% zaufania do *procedury*, której użyliśmy do skonstruowania przedziału.

**Struktura przedziału ufności:**

Przedział ufności jest zazwyczaj symetryczny wokół estymatora punktowego (wartości z próby) i ma postać:

$$ \text{Estymator punktowy} \pm \text{Margines błędu} $$

*   **Estymator punktowy:** Najlepsze pojedyncze oszacowanie parametru na podstawie próby (np. średnia z próby $\bar{x}$ jako estymator średniej populacji $\mu$).
*   **Margines błędu:** Określa "szerokość" przedziału. Zależy on od trzech czynników:
    1.  **Poziomu ufności:** Im wyższy poziom ufności (np. 99% vs 95%), tym szerszy przedział (potrzebujemy szerszej "siatki", by mieć większą pewność złapania parametru).
    2.  **Zmienności w danych:** Im większe odchylenie standardowe w próbie, tym szerszy przedział (większa niepewność).
    3.  **Wielkości próby:** Im większa próba, tym węższy przedział (więcej danych prowadzi do bardziej precyzyjnych oszacowań).

**Wyznaczanie przedziału ufności dla średniej (duża próba lub znane odchylenie standardowe populacji):**

$$ \bar{x} \pm z_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}} $$

*   $\bar{x}$ – średnia z próby.
*   $\sigma$ – odchylenie standardowe populacji (jeśli nieznane, dla dużych prób, $n>30$, można przybliżyć odchyleniem standardowym z próby $s$).
*   $n$ – wielkość próby.
*   $z_{\alpha/2}$ – **wartość krytyczna** z rozkładu normalnego, zależna od poziomu ufności. Dla 95% poziomu ufności, $z_{\alpha/2} \approx 1.96$.

#### Praktyczne zastosowania w informatyce

**1. Analiza wyników testów A/B**

Przedziały ufności są potężnym uzupełnieniem p-wartości w testach A/B. Test A/B może dać p-wartość 0.04 i pozwolić odrzucić hipotezę zerową, ale to nie mówi nic o skali sukcesu.

*   **Przykład:** Porównujemy dwie wersje przycisku. Obliczamy różnicę we współczynnikach konwersji i dla tej różnicy budujemy 95% przedział ufności. Możliwe wyniki:
    *   **Przedział [0.5%, 1.5%]:** Jesteśmy w 95% pewni, że nowa wersja jest lepsza o wartość z tego przedziału. Wynik jest pozytywny i precyzyjny. Wdrażamy.
    *   **Przedział [0.1%, 8.0%]:** Wynik jest statystycznie istotny (przedział nie zawiera zera), ale bardzo nieprecyzyjny. Efekt może być znikomy (0.1%) lub ogromny (8.0%). Może to być sygnał, że potrzebujemy więcej danych, aby zawęzić przedział.
    *   **Przedział [-0.5%, 2.0%]:** Wynik jest nieistotny statystycznie (zawiera zero). Nie możemy być pewni, czy nowa wersja jest lepsza, gorsza, czy taka sama. Nie wdrażamy.

**2. Monitorowanie wydajności i jakości usług (SLA)**

Podczas pomiaru kluczowych metryk systemu, takich jak średni czas odpowiedzi serwera czy uptime, pojedyncza wartość (np. średnia z ostatniej godziny) może być myląca. Podanie 95% przedziału ufności dla tej średniej daje znacznie lepszy obraz sytuacji.

*   **Przykład:** Zamiast raportować "średni czas odpowiedzi to 120ms", raportujemy "jesteśmy w 95% pewni, że prawdziwy średni czas odpowiedzi mieści się w przedziale [110ms, 130ms]". Pozwala to ocenić stabilność i przewidywalność systemu.

**3. Szacowanie w zarządzaniu projektami**

W metodykach zwinnych (Agile), zamiast podawać pojedyncze estymaty czasowe dla zadań, zespoły mogą podawać przedziały ufności (np. "jesteśmy w 90% pewni, że to zadanie zajmie od 3 do 5 dni"), co lepiej odzwierciedla niepewność związaną z pracą deweloperską.

#### Przykład

Chcemy oszacować średni czas, jaki użytkownicy spędzają na nowej stronie głównej. Z losowej próby 100 użytkowników ($n=100$) uzyskaliśmy średni czas $\bar{x} = 85$ sekund, a odchylenie standardowe z próby wyniosło $s = 20$ sekund.

Wyznaczmy 95% przedział ufności dla prawdziwego średniego czasu w całej populacji.

1.  **Poziom ufności:** 95%, co oznacza $\alpha = 0.05$.
2.  **Wartość krytyczna:** Dla 95% ufności, $z_{\alpha/2} = 1.96$.
3.  **Błąd standardowy średniej:** $SE = \frac{s}{\sqrt{n}} = \frac{20}{\sqrt{100}} = \frac{20}{10} = 2$.
4.  **Margines błędu:** $ME = z_{\alpha/2} \cdot SE = 1.96 \cdot 2 = 3.92$.
5.  **Przedział ufności:**
    $\bar{x} \pm ME = 85 \pm 3.92$
    Przedział wynosi **[81.08, 88.92]**.

**Wniosek:** Na podstawie zebranych danych, z 95% ufnością możemy stwierdzić, że prawdziwy średni czas spędzany przez wszystkich użytkowników na stronie głównej mieści się w przedziale od 81.08 do 88.92 sekund.

#### Podsumowanie

*   **Przedział ufności** to zakres wartości, który z określonym wysokim prawdopodobieństwem (poziomem ufności) zawiera nieznaną wartość parametru populacji.
*   Dostarcza informacji nie tylko o **istnieniu efektu**, ale także o jego **wielkości i precyzji oszacowania**.
*   Jego szerokość zależy od **poziomu ufności**, **zmienności w danych** i **wielkości próby**.
*   Poprawna interpretacja jest **częstościowa**: 95% przedziałów skonstruowanych tą metodą będzie zawierać prawdziwy parametr.
*   W informatyce są kluczowe w **analizie wyników testów A/B**, **monitorowaniu wydajności** i **szacowaniu**.

**Typowe pytania egzaminacyjne:**
*   Co to jest przedział ufności i jak go interpretujemy?
*   Czym różni się poziom ufności od przedziału ufności?
*   Od jakich czynników zależy szerokość przedziału ufności?
*   Proszę wyznaczyć przedział ufności dla średniej na podstawie podanych danych.
*   Jakie jest praktyczne znaczenie przedziałów ufności w testach A/B?

---

# 11. Podstawowe cechy relacyjnych baz danych

#### Wprowadzenie

Relacyjne bazy danych, oparte na modelu relacyjnym zaproponowanym przez Edgara F. Codda w 1970 roku, stanowią dominujący paradygmat przechowywania i zarządzania danymi od dziesięcioleci. Ich sukces wynika z prostoty, solidnych podstaw teoretycznych (opartych na matematycznej teorii zbiorów i logice predykatów) oraz elastyczności. Model relacyjny organizuje dane w prostych, dwuwymiarowych tabelach, co jest intuicyjne dla użytkowników, a jednocześnie pozwala na wykonywanie złożonych zapytań i zapewnienie integralności danych. Zrozumienie kluczowych cech tego modelu jest niezbędne dla każdego, kto pracuje z danymi w nowoczesnej informatyce.

#### Szczegółowe wyjaśnienie

Podstawowe cechy relacyjnych baz danych można podzielić na kilka kluczowych obszarów: struktura, integralność, manipulacja danymi oraz gwarancje transakcyjne.

**1. Struktura oparta na relacjach (tabelach)**

Podstawowym budulcem relacyjnej bazy danych jest **relacja**, która w praktyce jest reprezentowana jako **tabela**.

*   **Tabela (Relacja):** Składa się z wierszy i kolumn.
*   **Wiersz (Krotka/Rekord):** Reprezentuje pojedynczy obiekt lub zdarzenie (np. jednego klienta, jedno zamówienie).
*   **Kolumna (Atrybut):** Opisuje jedną cechę obiektów w tabeli (np. imię klienta, data zamówienia). Każda kolumna ma określoną **dziedzinę**, czyli zbiór dopuszczalnych wartości (np. tekst, liczba całkowita, data).
*   **Klucz podstawowy (Primary Key):** Jedna lub więcej kolumn, których wartość jednoznacznie identyfikuje każdy wiersz w tabeli. Wartość klucza podstawowego nie może być pusta (NULL) i musi być unikalna.

**2. Integralność danych**

Systemy zarządzania relacyjnymi bazami danych (RDBMS) wymuszają zbiór reguł zapewniających spójność i poprawność danych.

*   **Integralność encji (Entity Integrity):** Gwarantuje, że każdy wiersz w tabeli jest unikalny. Wymusza ją klucz podstawowy – żaden element klucza podstawowego nie może przyjmować wartości NULL.
*   **Integralność referencyjna (Referential Integrity):** Zapewnia spójność między powiązanymi tabelami. Jest realizowana za pomocą **kluczy obcych (Foreign Keys)**. Klucz obcy w jednej tabeli wskazuje na klucz podstawowy w innej tabeli. Integralność referencyjna gwarantuje, że nie można utworzyć wiersza z kluczem obcym, który nie istnieje w tabeli nadrzędnej, ani usunąć wiersza z tabeli nadrzędnej, jeśli istnieją do niego odwołania.
*   **Integralność dziedziny (Domain Integrity):** Zapewnia, że wszystkie wartości w danej kolumnie są zgodne z jej zdefiniowanym typem danych, formatem i zakresem (np. kolumna "wiek" nie może zawierać wartości ujemnych).

**3. Język zapytań SQL**

Standardowym językiem do komunikacji z relacyjnymi bazami danych jest **SQL (Structured Query Language)**. Jest to język deklaratywny, co oznacza, że użytkownik określa, *jakie* dane chce uzyskać, a nie *jak* system ma je pobrać. RDBMS sam decyduje o optymalnej ścieżce dostępu do danych. SQL służy do definiowania struktur (tworzenie tabel), manipulowania danymi (wstawianie, aktualizacja, usuwanie) i odpytywania bazy (pobieranie danych).

**4. Gwarancje transakcyjne ACID**

Transakcja to logiczna jednostka pracy, składająca się z jednej lub więcej operacji na bazie danych. Relacyjne bazy danych gwarantują, że transakcje posiadają cztery kluczowe właściwości, znane pod akronimem **ACID**.

*   **Atomowość (Atomicity):** Transakcja jest niepodzielna – albo wszystkie jej operacje zostaną wykonane poprawnie, albo żadna z nich. Jeśli w trakcie transakcji wystąpi błąd, system wycofa wszystkie dotychczasowe zmiany (rollback), przywracając bazę do stanu sprzed transakcji.
*   **Spójność (Consistency):** Transakcja przeprowadza bazę danych z jednego spójnego stanu w drugi spójny stan. Oznacza to, że po zakończeniu transakcji wszystkie reguły integralności (klucze, ograniczenia) muszą być spełnione.
*   **Izolacja (Isolation):** Równocześnie wykonywane transakcje nie powinny na siebie wpływać. Z perspektywy jednej transakcji wygląda to tak, jakby była ona jedyną operującą na bazie danych. Systemy RDBMS realizują to za pomocą mechanizmów blokad (locking).
*   **Trwałość (Durability):** Zmiany wprowadzone przez pomyślnie zakończoną (zatwierdzoną) transakcję są trwałe i nie zostaną utracone nawet w przypadku awarii systemu (np. awarii zasilania).

#### Praktyczne zastosowania

Relacyjne bazy danych są podstawą ogromnej większości systemów informatycznych, w tym:

*   **Systemy bankowe i finansowe:** Gdzie gwarancje ACID są absolutnie krytyczne.
*   **Systemy rezerwacji:** (lotnicze, hotelowe) wymagające spójnego zarządzania dostępnością.
*   **Sklepy internetowe (e-commerce):** Zarządzanie produktami, zamówieniami i klientami.
*   **Systemy zarządzania zasobami przedsiębiorstwa (ERP) i relacjami z klientami (CRM).**
*   **Większość aplikacji webowych i mobilnych**, które wymagają trwałego przechowywania danych o użytkownikach, treściach itp.

#### Przykład

Rozważmy dwie tabele w bazie danych sklepu:

**Klienci**
| ID_Klienta (PK) | Imię | Nazwisko |
|---|---|---|
| 1 | Jan | Kowalski |
| 2 | Anna | Nowak |

**Zamówienia**
| ID_Zamówienia (PK) | Data | ID_Klienta (FK) | Kwota |
|---|---|---|---|
| 101 | 2023-10-26 | 1 | 150.00 |
| 102 | 2023-10-27 | 2 | 200.00 |

**Cechy modelu relacyjnego w tym przykładzie:**
*   **Struktura:** Dane są w tabelach z wierszami i kolumnami.
*   **Integralność encji:** `ID_Klienta` i `ID_Zamówienia` jednoznacznie identyfikują każdy wiersz w swoich tabelach.
*   **Integralność referencyjna:** Kolumna `ID_Klienta` w tabeli `Zamówienia` jest kluczem obcym wskazującym na `ID_Klienta` w tabeli `Klienci`. Baza danych nie pozwoli na dodanie zamówienia z `ID_Klienta = 3`, dopóki taki klient nie zostanie dodany do tabeli `Klienci`.
*   **Transakcja ACID:** Gdy klient składa zamówienie, operacje takie jak zmniejszenie stanu magazynowego produktu i zapisanie nowego zamówienia muszą być wykonane w ramach jednej transakcji. Jeśli zabraknie produktu, cała operacja zostanie wycofana, a zamówienie nie powstanie.

#### Podsumowanie

*   Model relacyjny organizuje dane w **tabelach** (relacjach) składających się z wierszy (krotek) i kolumn (atrybutów).
*   **Klucze podstawowe** zapewniają unikalność każdego rekordu w tabeli.
*   **Reguły integralności** (encji, referencyjna, dziedziny) gwarantują spójność i poprawność danych.
*   Standardowym językiem do pracy z relacyjnymi bazami danych jest **SQL**.
*   Kluczową cechą, gwarantującą niezawodność, jest obsługa **transakcji ACID** (Atomowość, Spójność, Izolacja, Trwałość).
*   Mimo pojawienia się baz NoSQL, model relacyjny pozostaje standardem w zastosowaniach wymagających silnych gwarancji spójności i transakcyjności.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i krótko scharakteryzować podstawowe cechy relacyjnych baz danych.
*   Co to są właściwości ACID i co każda z nich oznacza? Proszę podać przykład transakcji.
*   Na czym polega integralność referencyjna i jak jest realizowana w relacyjnych bazach danych?
*   Jakie są podstawowe elementy składowe modelu relacyjnego (tabela, wiersz, kolumna, klucz)?

---

# 12. Podstawowe elementy i znaczenie diagramów związków encji oraz zasady prawidłowego projektowania schematów bazy danych

#### Wprowadzenie

Zanim powstanie działająca baza danych, musi zostać starannie zaprojektowana. Proces projektowania to kluczowy etap, który decyduje o wydajności, skalowalności i łatwości utrzymania przyszłego systemu. Jednym z najważniejszych narzędzi na tym etapie jest **Diagram Związków Encji (ERD - Entity-Relationship Diagram)**. Jest to graficzny, konceptualny model danych, który pozwala analitykom i projektantom wizualizować obiekty (encje), ich cechy (atrybuty) oraz wzajemne powiązania (związki) w sposób niezależny od konkretnego systemu bazodanowego. Prawidłowo stworzony ERD jest fundamentem dla dobrze zaprojektowanego schematu bazy danych, który z kolei jest planem implementacji bazy w postaci tabel, kluczy i relacji.

#### Podstawowe elementy Diagramu Związków Encji (ERD)

Diagram ERD składa się z trzech podstawowych typów obiektów:

1.  **Encja (Entity):**
    *   **Definicja:** Obiekt, osoba, miejsce, zdarzenie lub pojęcie, o którym chcemy przechowywać informacje. Jest to odpowiednik przyszłej tabeli w bazie danych.
    *   **Notacja graficzna:** Prostokąt z nazwą encji w środku (np. `Student`, `Kurs`, `Zamówienie`).

2.  **Atrybut (Attribute):**
    *   **Definicja:** Właściwość lub cecha opisująca daną encję. Odpowiada przyszłej kolumnie w tabeli.
    *   **Notacja graficzna:** Elipsa połączona z encją. Atrybut, który jest **identyfikatorem** (kluczem głównym), jest zazwyczaj podkreślony (np. `ID_Studenta`).

3.  **Związek (Relationship):**
    *   **Definicja:** Powiązanie lub interakcja między dwiema (lub więcej) encjami. Odpowiada przyszłej relacji między tabelami, często realizowanej przez klucze obce.
    *   **Notacja graficzna:** Romb łączący powiązane encje, z opisem związku w środku (np. `zapisuje się na`).

**Liczebność (krotność) związku (Cardinality):**

Kluczowym elementem opisu związku jest jego liczebność, która określa, ile instancji jednej encji może być powiązanych z ile instancjami drugiej encji. Wyróżniamy trzy podstawowe typy liczebności:

*   **Jeden do jednego (1:1):** Każdej instancji encji A odpowiada co najwyżej jedna instancja encji B, i na odwrót. *Przykład: `Mąż` - `ma` - `Żona` (w systemie monogamicznym).* Jest to rzadko spotykany typ związku.
*   **Jeden do wielu (1:N):** Jednej instancji encji A może odpowiadać wiele instancji encji B, ale każdej instancji B odpowiada dokładnie jedna instancja A. *Przykład: `Wykładowca` - `prowadzi` - `Kursy`. Jeden wykładowca może prowadzić wiele kursów, ale jeden kurs jest prowadzony przez jednego wykładowcę.*
*   **Wiele do wielu (M:N):** Jednej instancji encji A może odpowiadać wiele instancji encji B, i na odwrót. *Przykład: `Student` - `zapisuje się na` - `Kurs`. Jeden student może być zapisany na wiele kursów, a na jeden kurs może być zapisanych wielu studentów.*

#### Zasady prawidłowego projektowania schematów bazy danych

Po stworzeniu modelu konceptualnego (ERD) następuje projektowanie logiczne, czyli tworzenie schematu bazy danych. Celem jest stworzenie struktury, która będzie wydajna, wolna od anomalii i łatwa w utrzymaniu. Kluczową rolę odgrywa tu proces **normalizacji**.

**Normalizacja** to proces organizowania kolumn i tabel w relacyjnej bazie danych w celu zminimalizowania **redundancji danych** (powtarzania tych samych informacji w wielu miejscach). Redundancja prowadzi do tzw. **anomalii**, czyli problemów podczas modyfikacji danych:

*   **Anomalia wstawiania:** Nie można dodać informacji o jednym obiekcie bez jednoczesnego dodania informacji o innym (np. nie można dodać nowego kursu, dopóki nie zapisze się na niego żaden student).
*   **Anomalia usuwania:** Usunięcie jednego rekordu powoduje niezamierzoną utratę innych informacji (np. usunięcie ostatniego studenta z kursu powoduje usunięcie informacji o samym kursie).
*   **Anomalia modyfikacji:** Zmiana jednej informacji wymaga jej aktualizacji w wielu miejscach, co grozi niespójnością danych.

Normalizacja polega na dekompozycji (rozbijaniu) dużych tabel na mniejsze, dobrze ustrukturyzowane tabele i definiowaniu między nimi relacji. Proces ten opisują **postacie normalne (NF - Normal Form)**.

**Podstawowe postacie normalne:**

1.  **Pierwsza postać normalna (1NF):**
    *   **Zasada:** Wszystkie atrybuty (kolumny) muszą być **atomowe**, czyli zawierać niepodzielne wartości. W tabeli nie mogą istnieć grupy powtarzających się kolumn ani kolumny przechowujące wiele wartości (np. lista w jednej komórce).
    *   **Cel:** Usunięcie grup powtarzających się.

2.  **Druga postać normalna (2NF):**
    *   **Warunek:** Tabela musi być w 1NF.
    *   **Zasada:** Każdy atrybut niebędący częścią klucza głównego musi być w **pełni funkcyjnie zależny** od *całego* klucza głównego. Ta postać ma znaczenie tylko dla tabel z kluczami głównymi złożonymi z wielu kolumn.
    *   **Cel:** Usunięcie częściowych zależności. Jeśli atrybut zależy tylko od części klucza złożonego, należy go przenieść do osobnej tabeli.

3.  **Trzecia postać normalna (3NF):**
    *   **Warunek:** Tabela musi być w 2NF.
    *   **Zasada:** Żaden atrybut niekluczowy nie może zależeć od innego atrybutu niekluczowego. Muszą istnieć tylko zależności od klucza głównego.
    *   **Cel:** Usunięcie **zależności przechodnich**. Jeśli atrybut C zależy od atrybutu B, a atrybut B zależy od klucza głównego A, to zależność A -> C jest przechodnia i należy ją wyeliminować, tworząc nową tabelę.

**Praktyczna zasada dla 3NF:** "Każdy atrybut niekluczowy musi dostarczać informacji o kluczu, całym kluczu i tylko o kluczu".

#### Przykład

**Problem:** Projektujemy bazę do obsługi zapisów na kursy. Początkowa, nieznormalizowana tabela mogłaby wyglądać tak:

| ID_Studenta | Nazwisko_Stud | ID_Kursu | Nazwa_Kursu | Nazwisko_Wykładowcy |
|---|---|---|---|---|
| 101 | Kowalski | CS101 | Wprowadzenie do C++ | prof. Nowak |
| 101 | Kowalski | CS102 | Bazy Danych | prof. Iksiński |
| 102 | Wiśniewski | CS101 | Wprowadzenie do C++ | prof. Nowak |

**Problemy (anomalie):**
*   **Redundancja:** Nazwisko studenta, nazwa kursu i nazwisko wykładowcy powtarzają się.
*   **Anomalia modyfikacji:** Jeśli prof. Nowak zmieni nazwisko, trzeba to zaktualizować w wielu wierszach.
*   **Anomalia usuwania:** Jeśli student Kowalski wypisze się z kursu CS102, stracimy informację, że prof. Iksiński prowadzi ten kurs.

**Rozwiązanie (Normalizacja do 3NF):**

1.  **Tabela `Studenci`:**
    | ID_Studenta (PK) | Nazwisko_Stud |
    |---|---|
    | 101 | Kowalski |
    | 102 | Wiśniewski |

2.  **Tabela `Kursy`:**
    | ID_Kursu (PK) | Nazwa_Kursu | Nazwisko_Wykładowcy |
    |---|---|---|
    | CS101 | Wprowadzenie do C++ | prof. Nowak |
    | CS102 | Bazy Danych | prof. Iksiński |

3.  **Tabela `Zapisy` (tabela łącząca dla relacji M:N):**
    | ID_Zapisu (PK) | ID_Studenta (FK) | ID_Kursu (FK) |
    |---|---|---|
    | 1 | 101 | CS101 |
    | 2 | 101 | CS102 |
    | 3 | 102 | CS101 |

Ten znormalizowany schemat eliminuje wszystkie anomalie i redundancję.

#### Podsumowanie

*   **Diagram Związków Encji (ERD)** to graficzny model konceptualny używany na wczesnym etapie projektowania baz danych.
*   Jego podstawowe elementy to **encje** (tabele), **atrybuty** (kolumny) i **związki** (relacje).
*   Kluczowym elementem opisu związku jest jego **liczebność** (1:1, 1:N, M:N).
*   **Normalizacja** to proces projektowania schematu bazy danych w celu minimalizacji redundancji i eliminacji anomalii (wstawiania, usuwania, modyfikacji).
*   Podstawowe postacie normalne to **1NF** (atomowe wartości), **2NF** (brak częściowych zależności od klucza) i **3NF** (brak zależności przechodnich).
*   Dobrze zaprojektowany i znormalizowany schemat jest fundamentem wydajnej, spójnej i łatwej w utrzymaniu bazy danych.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać podstawowe elementy diagramu związków encji.
*   Co to jest liczebność związku? Proszę podać przykłady związków 1:N i M:N.
*   Na czym polega proces normalizacji baz danych i jaki jest jego cel?
*   Proszę opisać pierwszą, drugą i trzecią postać normalną.
*   Dla podanej nieznormalizowanej tabeli proszę wskazać występujące anomalie i zaproponować schemat znormalizowany do 3NF.

---

# 13. Mechanizm współbieżności pracy wielu użytkowników w systemie zarządzania bazami danych

#### Wprowadzenie

Nowoczesne systemy bazodanowe muszą obsługiwać jednoczesny dostęp do danych przez wielu użytkowników i wiele aplikacji. Ta zdolność do równoległego przetwarzania wielu transakcji nazywana jest **współbieżnością**. Chociaż współbieżność jest kluczowa dla wydajności i responsywności systemu, rodzi ona fundamentalne problemy: jak zapewnić, aby równoczesne operacje odczytu i zapisu nie prowadziły do uszkodzenia danych lub niespójnych wyników? Mechanizmy kontroli współbieżności to zestaw technik stosowanych przez systemy zarządzania bazami danych (RDBMS) w celu zarządzania współbieżnym dostępem i zagwarantowania właściwości izolacji (litera 'I' w ACID), zapewniając, że transakcje nie zakłócają się nawzajem.

#### Problemy (anomalie) współbieżnego dostępu

Gdy wiele transakcji operuje na tych samych danych w sposób niekontrolowany, mogą wystąpić następujące anomalie:

1.  **Utracona modyfikacja (Lost Update):**
    *   **Scenariusz:** Dwie transakcje (T1 i T2) odczytują tę samą wartość (np. stan konta = 100). T1 dodaje 10 i zapisuje 110. Niemal w tym samym czasie T2 odejmuje 20 od *początkowej* wartości 100 i zapisuje 80. Ostateczny wynik to 80, a modyfikacja wykonana przez T1 (dodanie 10) została utracona.

2.  **Odczyt niezatwierdzonych danych (Dirty Read):**
    *   **Scenariusz:** Transakcja T1 modyfikuje dane (np. zmienia cenę produktu), ale jeszcze nie zatwierdziła zmian. Transakcja T2 odczytuje tę nową, "brudną" cenę. Następnie T1 z jakiegoś powodu jest wycofywana (rollback). W rezultacie T2 operuje na danych, które formalnie nigdy nie istniały w bazie.

3.  **Niespójny (niepowtarzalny) odczyt (Non-Repeatable Read):**
    *   **Scenariusz:** Transakcja T1 odczytuje wartość (np. cenę produktu). W międzyczasie transakcja T2 modyfikuje tę wartość i zatwierdza zmianę. Gdy T1 ponownie odczytuje tę samą wartość w ramach tej samej transakcji, otrzymuje inny wynik niż za pierwszym razem, co może prowadzić do niespójności obliczeń.

4.  **Odczyty fantomowe (Phantom Reads):**
    *   **Scenariusz:** Transakcja T1 wykonuje zapytanie, które zwraca zbiór wierszy (np. "ilu jest pracowników w dziale X?"). W międzyczasie transakcja T2 dodaje nowego pracownika do działu X i zatwierdza zmianę. Gdy T1 powtarza to samo zapytanie, otrzymuje inny wynik (o jeden wiersz więcej), ponieważ pojawił się "fantomowy" rekord, którego wcześniej nie było.

#### Mechanizmy kontroli współbieżności

Aby zapobiegać tym anomaliom, systemy RDBMS stosują różne strategie kontroli współbieżności. Dwie główne filozofie to pesymistyczna i optymistyczna kontrola.

**1. Pesymistyczna kontrola współbieżności: Blokowanie (Locking)**

Ta strategia zakłada, że konflikty są prawdopodobne, więc lepiej im zapobiegać, zanim wystąpią. Podstawowym mechanizmem jest **blokada (lock)**.

*   **Zasada działania:** Zanim transakcja uzyska dostęp do danych (do odczytu lub zapisu), musi najpierw założyć na nie odpowiednią blokadę. Jeśli inna transakcja już posiada blokadę na tych danych, która jest niekompatybilna, transakcja żądająca blokady musi poczekać.
*   **Rodzaje blokad:**
    *   **Blokada na odczyt (Shared Lock, S):** Wiele transakcji może jednocześnie posiadać blokadę typu S na tych samych danych. Pozwala to na jednoczesny odczyt przez wielu użytkowników.
    *   **Blokada na zapis (Exclusive Lock, X):** Tylko jedna transakcja może posiadać blokadę typu X na danych. Wyklucza ona wszystkie inne blokady (zarówno S, jak i X). Jest konieczna do modyfikacji lub usuwania danych.

*   **Protokół blokowania dwufazowego (Two-Phase Locking, 2PL):** To fundamentalny protokół zapewniający izolację. Każda transakcja przebiega w dwóch fazach:
    1.  **Faza narastania (Growing Phase):** Transakcja może uzyskiwać nowe blokady, ale nie może zwalniać żadnej z już posiadanych.
    2.  **Faza opadania (Shrinking Phase):** Transakcja może zwalniać blokady, ale nie może już prosić o żadne nowe.
    Protokół 2PL gwarantuje **szeregowalność** transakcji (wynik jest taki, jakby były wykonywane jedna po drugiej), ale nie zapobiega **zakleszczeniom (deadlocks)**.

*   **Zakleszczenie (Deadlock):** Sytuacja, w której transakcja T1 czeka na zasób zablokowany przez T2, a T2 czeka na zasób zablokowany przez T1. System musi posiadać mechanizm wykrywania zakleszczeń (np. przez analizę grafu oczekiwań) i ich rozwiązywania (zazwyczaj przez wycofanie jednej z transakcji).

**2. Optymistyczna kontrola współbieżności**

Ta strategia zakłada, że konflikty są rzadkie, więc pozwala transakcjom na pracę bez blokowania, a konflikty wykrywa dopiero na etapie zatwierdzania.

*   **Multiversion Concurrency Control (MVCC):** Najpopularniejsza implementacja optymistycznej kontroli (używana m.in. w PostgreSQL, Oracle, MySQL/InnoDB).
    *   **Zasada działania:** Zamiast nadpisywać dane, każda operacja zapisu tworzy **nową wersję** rekordu. Każda transakcja widzi spójny "obraz" (snapshot) bazy danych z momentu swojego rozpoczęcia. Transakcje odczytujące dane nie blokują transakcji zapisujących i na odwrót.
    *   **Zalety:** Znacznie wyższa współbieżność, ponieważ "czytelnicy nie blokują pisarzy, a pisarze nie blokują czytelników". Eliminuje problemy niespójnego odczytu i odczytów fantomowych dla transakcji odczytujących.
    *   **Wady:** Większe zużycie przestrzeni dyskowej (przechowywanie wielu wersji) i narzut związany z zarządzaniem wersjami i "sprzątaniem" starych, niepotrzebnych wersji (tzw. vacuuming).

#### Poziomy izolacji transakcji

Standard SQL definiuje cztery poziomy izolacji, które pozwalają programiście na wybór kompromisu między wydajnością a ścisłością gwarancji. Im wyższy poziom, tym mniejsza współbieżność, ale większe bezpieczeństwo.

1.  **Read Uncommitted:** Najniższy poziom. Pozwala na odczyt niezatwierdzonych danych (dirty reads).
2.  **Read Committed:** Domyślny poziom w wielu bazach. Zapobiega "dirty reads", ale wciąż możliwe są "non-repeatable reads" i "phantom reads".
3.  **Repeatable Read:** Zapobiega "dirty reads" i "non-repeatable reads", ale wciąż możliwe są "phantom reads".
4.  **Serializable:** Najwyższy poziom. Gwarantuje pełną izolację, eliminując wszystkie anomalie. System zapewnia, że wynik współbieżnego wykonania transakcji jest identyczny z pewnym ich szeregowym wykonaniem.

#### Podsumowanie

*   **Współbieżność** w bazach danych pozwala na jednoczesną pracę wielu użytkowników, ale stwarza ryzyko **anomalii** (utracona modyfikacja, brudny odczyt, niepowtarzalny odczyt, odczyt fantomowy).
*   Systemy RDBMS używają **mechanizmów kontroli współbieżności** do zarządzania tym ryzykiem i zapewnienia izolacji transakcji.
*   **Pesymistyczna kontrola (blokowanie)**, z protokołem **2PL** na czele, zapobiega konfliktom, zakładając blokady na dane, ale może prowadzić do **zakleszczeń**.
*   **Optymistyczna kontrola**, z mechanizmem **MVCC** jako głównym przedstawicielem, pozwala na większą współbieżność, tworząc wersje danych i unikając blokad przy odczycie.
*   **Poziomy izolacji** (od `Read Uncommitted` do `Serializable`) pozwalają na świadomy wybór kompromisu między wydajnością a spójnością danych.

**Typowe pytania egzaminacyjne:**
*   Dlaczego kontrola współbieżności jest potrzebna w systemach baz danych?
*   Proszę opisać anomalie, które mogą wystąpić przy współbieżnym dostępie do danych (np. utracona modyfikacja, brudny odczyt).
*   Na czym polega pesymistyczna kontrola współbieżności? Proszę opisać protokół blokowania dwufazowego (2PL).
*   Co to jest zakleszczenie (deadlock) i jak systemy bazodanowe sobie z nim radzą?
*   Na czym polega mechanizm MVCC (Multiversion Concurrency Control)?

---

# 14. Podstawowe obiekty, konstrukcje i znaczenie języka SQL

#### Wprowadzenie

SQL (Structured Query Language) to standardowy, uniwersalny język służący do komunikacji z relacyjnymi bazami danych. Jest to język **deklaratywny**, co oznacza, że użytkownik specyfikuje *co* chce osiągnąć (np. jakie dane pobrać), a nie *jak* system ma to zrobić. Ta cecha odróżnia go od języków imperatywnych (jak C++ czy Java) i pozwala na wysokopoziomową, intuicyjną pracę z danymi. Mimo że od jego powstania minęło kilkadziesiąt lat, SQL pozostaje jedną z najważniejszych i najbardziej pożądanych umiejętności w świecie IT, stanowiąc fundament dla analityków danych, programistów backendowych, administratorów baz danych i wielu innych profesji.

#### Podstawowe obiekty w bazie danych

SQL operuje na różnych obiektach, które tworzą strukturę bazy danych. Najważniejsze z nich to:

*   **Tabela (Table):** Podstawowy obiekt przechowujący dane, zorganizowany w wiersze i kolumny.
*   **Widok (View):** Wirtualna tabela, która jest wynikiem zapytania SQL. Nie przechowuje fizycznie danych, ale prezentuje je w określony sposób, pobierając je na bieżąco z tabel bazowych. Służy do upraszczania złożonych zapytań, ograniczania dostępu do danych i zapewniania spójnego interfejsu.
*   **Indeks (Index):** Specjalna struktura danych (najczęściej B-drzewo) powiązana z tabelą, która drastycznie przyspiesza operacje wyszukiwania danych. Działa podobnie do indeksu w książce – zamiast przeszukiwać całą tabelę, system może szybko zlokalizować odpowiednie wiersze za pomocą indeksu.
*   **Procedura składowana (Stored Procedure):** Zestaw prekompilowanych instrukcji SQL zapisany pod jedną nazwą w bazie danych. Może przyjmować parametry i zwracać wyniki. Używana do hermetyzacji logiki biznesowej i poprawy wydajności.
*   **Wyzwalacz (Trigger):** Procedura, która jest automatycznie uruchamiana w odpowiedzi na określone zdarzenie w tabeli (np. przed lub po operacji `INSERT`, `UPDATE` lub `DELETE`). Służy do wymuszania złożonych reguł biznesowych lub audytu zmian.

#### Podział i podstawowe konstrukcje języka SQL

Język SQL dzieli się na kilka podjęzyków, w zależności od przeznaczenia poleceń:

**1. DDL (Data Definition Language) – Język Definicji Danych**

Służy do tworzenia i zarządzania strukturą obiektów w bazie danych.

*   `CREATE`: Tworzy nowe obiekty.
    *   `CREATE TABLE NazwaTabeli (kolumna1 typ, kolumna2 typ, ...);`
    *   `CREATE VIEW NazwaWidoku AS SELECT ...;`
    *   `CREATE INDEX NazwaIndeksu ON NazwaTabeli (kolumna);`
*   `ALTER`: Modyfikuje istniejące obiekty.
    *   `ALTER TABLE NazwaTabeli ADD COLUMN nowa_kolumna typ;`
    *   `ALTER TABLE NazwaTabeli DROP COLUMN kolumna;`
*   `DROP`: Usuwa obiekty.
    *   `DROP TABLE NazwaTabeli;`
    *   `DROP INDEX NazwaIndeksu;`

**2. DML (Data Manipulation Language) – Język Manipulacji Danymi**

Służy do wstawiania, modyfikowania, usuwania i pobierania danych z tabel.

*   `SELECT`: Pobiera dane z bazy. Jest to najbardziej rozbudowane i najczęściej używane polecenie.
    *   `SELECT kolumna1, kolumna2 FROM NazwaTabeli WHERE warunek;`
*   `INSERT`: Wstawia nowe wiersze do tabeli.
    *   `INSERT INTO NazwaTabeli (kolumna1, kolumna2) VALUES (wartosc1, wartosc2);`
*   `UPDATE`: Modyfikuje istniejące wiersze.
    *   `UPDATE NazwaTabeli SET kolumna1 = nowa_wartosc WHERE warunek;`
*   `DELETE`: Usuwa wiersze z tabeli.
    *   `DELETE FROM NazwaTabeli WHERE warunek;`

**3. DQL (Data Query Language) – Język Zapytań do Danych**

Często wydzielany jako osobna kategoria, choć formalnie jest częścią DML. Obejmuje wyłącznie polecenie `SELECT` i jego liczne klauzule.

*   `FROM`: Określa tabelę (lub tabele), z których pobierane są dane.
*   `WHERE`: Filtruje wiersze na podstawie określonego warunku.
*   `GROUP BY`: Grupuje wiersze o tych samych wartościach w kolumnach w celu wykonania na nich funkcji agregujących.
*   `HAVING`: Filtruje grupy utworzone przez `GROUP BY`.
*   `ORDER BY`: Sortuje wyniki.
*   `JOIN`: Łączy wiersze z dwóch lub więcej tabel na podstawie powiązanej kolumny.
    *   `INNER JOIN`: Zwraca tylko pasujące wiersze z obu tabel.
    *   `LEFT JOIN`: Zwraca wszystkie wiersze z lewej tabeli i pasujące z prawej.
    *   `RIGHT JOIN`: Zwraca wszystkie wiersze z prawej tabeli i pasujące z lewej.
    *   `FULL OUTER JOIN`: Zwraca wszystkie wiersze, gdy istnieje dopasowanie w jednej z tabel.

**4. DCL (Data Control Language) – Język Kontroli Danych**

Służy do zarządzania uprawnieniami użytkowników.

*   `GRANT`: Nadaje uprawnienia (np. do odczytu, zapisu) użytkownikowi.
    *   `GRANT SELECT, UPDATE ON NazwaTabeli TO uzytkownik;`
*   `REVOKE`: Odbiera uprawnienia.
    *   `REVOKE UPDATE ON NazwaTabeli FROM uzytkownik;`

**5. TCL (Transaction Control Language) – Język Kontroli Transakcji**

Służy do zarządzania transakcjami.

*   `COMMIT`: Trwale zatwierdza zmiany wykonane w ramach transakcji.
*   `ROLLBACK`: Wycofuje wszystkie zmiany wykonane w bieżącej transakcji.
*   `SAVEPOINT`: Ustawia punkt kontrolny wewnątrz transakcji, do którego można się później cofnąć.

#### Znaczenie języka SQL

*   **Uniwersalność:** Jest standardem branżowym, obsługiwanym przez praktycznie wszystkie systemy RDBMS (np. PostgreSQL, MySQL, Oracle, SQL Server, SQLite). Znajomość SQL jest przenośna między różnymi technologiami.
*   **Efektywność:** Deklaratywna natura języka pozwala systemowi bazodanowemu na optymalizację wykonania zapytań (tzw. optymalizator zapytań), co jest często znacznie wydajniejsze niż ręczna implementacja dostępu do danych w języku imperatywnym.
*   **Potęga wyrazu:** Mimo pozornej prostoty, SQL pozwala na konstruowanie niezwykle złożonych zapytań, agregacji, łączenia danych z wielu tabel i wykonywania skomplikowanych analiz.
*   **Separacja logiki:** Umożliwia oddzielenie logiki biznesowej aplikacji od logiki dostępu do danych. Aplikacja wysyła zapytanie, a baza danych zajmuje się resztą.
*   **Podstawa analizy danych:** Jest to podstawowy język dla analityków danych, pozwalający na eksplorację, filtrowanie, agregowanie i przygotowywanie danych do dalszej analizy i wizualizacji.

#### Podsumowanie

*   **SQL** to standardowy, deklaratywny język do zarządzania i odpytywania relacyjnych baz danych.
*   Podstawowe **obiekty** w bazie to m.in. **tabele, widoki i indeksy**.
*   Język SQL dzieli się na podjęzyki: **DDL** (definicja danych), **DML** (manipulacja danymi), **DCL** (kontrola dostępu) i **TCL** (kontrola transakcji).
*   Najważniejsze polecenia to `CREATE`, `ALTER`, `DROP` (DDL) oraz `SELECT`, `INSERT`, `UPDATE`, `DELETE` (DML).
*   Kluczowe konstrukcje w zapytaniach `SELECT` to klauzule `WHERE`, `GROUP BY`, `ORDER BY` oraz operatory `JOIN` do łączenia tabel.
*   Znaczenie SQL wynika z jego **uniwersalności, wydajności i potęgi wyrazu**, co czyni go fundamentalnym narzędziem w świecie danych.

**Typowe pytania egzaminacyjne:**
*   Co to jest SQL i jaki jest jego charakter (deklaratywny/imperatywny)?
*   Proszę wymienić i opisać podjęzyki SQL (DDL, DML, DCL, TCL), podając po jednym przykładzie polecenia dla każdego z nich.
*   Do czego służy polecenie `SELECT`? Proszę wymienić i opisać jego najważniejsze klauzule.
*   Jaka jest różnica między `INNER JOIN` a `LEFT JOIN`?
*   Do czego służą widoki (VIEW) i indeksy (INDEX) w bazie danych?

---

# 15. Podstawowe zasady optymalizacji zapytań, w tym rodzaje i znaczenie indeksów w bazie danych

#### Wprowadzenie

Napisanie zapytania SQL, które zwraca poprawne dane, to tylko połowa sukcesu. W rzeczywistych systemach, operujących na milionach lub miliardach rekordów, kluczowe staje się to, *jak szybko* to zapytanie jest w stanie się wykonać. Optymalizacja zapytań to proces (i sztuka) modyfikowania zapytań i struktury bazy danych w celu zminimalizowania czasu ich wykonania i zużycia zasobów (CPU, I/O). Centralnym elementem tej optymalizacji są **indeksy** – specjalne struktury danych, które działają jak skorowidz w książce, pozwalając systemowi bazodanowemu na błyskawiczne odnajdywanie danych bez konieczności skanowania całej tabeli.

#### Proces optymalizacji zapytań

Kiedy wysyłamy zapytanie SQL do bazy danych, nie jest ono wykonywane dosłownie. Najpierw trafia do komponentu zwanego **optymalizatorem zapytań (query optimizer)**. Jego zadaniem jest przeanalizowanie zapytania i wygenerowanie najbardziej efektywnego **planu wykonania (execution plan)**.

1.  **Parsowanie zapytania:** Sprawdzenie poprawności składniowej.
2.  **Generowanie możliwych planów:** Optymalizator rozważa różne sposoby wykonania zapytania (np. różne kolejności łączenia tabel, różne metody dostępu do danych – skanowanie tabeli vs. użycie indeksu).
3.  **Wybór najlepszego planu:** Na podstawie wewnętrznych statystyk dotyczących danych (np. liczby wierszy, rozkładu wartości), optymalizator szacuje **koszt** każdego planu (wyrażony w abstrakcyjnych jednostkach) i wybiera ten o najniższym koszcie.

Zrozumienie tego procesu jest kluczowe. Naszym celem jako programistów jest pisanie zapytań i projektowanie schematu w taki sposób, aby pomóc optymalizatorowi w wyborze najlepszego planu.

#### Znaczenie i rodzaje indeksów

**Czym jest indeks?**

Indeks to zewnętrzna, posortowana struktura danych, która przechowuje wartości z jednej lub więcej kolumn tabeli oraz wskaźniki (fizyczne adresy) do odpowiadających im wierszy. Gdy szukamy wiersza po zaindeksowanej kolumnie, system zamiast skanować całą tabelę wiersz po wierszu (**Full Table Scan**), może bardzo szybko przeszukać znacznie mniejszą, posortowaną strukturę indeksu (np. za pomocą wyszukiwania binarnego), aby natychmiast zlokalizować potrzebne dane.

**Kiedy używać indeksów?**

Indeksy są najskuteczniejsze dla kolumn, które:

*   Często pojawiają się w klauzuli `WHERE`.
*   Są używane do łączenia tabel (klauzula `JOIN`).
*   Są używane do sortowania (klauzula `ORDER BY`).
*   Mają wysoką **kardynalność** (selektywność), czyli przyjmują wiele unikalnych wartości (np. kolumna `email` jest dobrym kandydatem na indeks, a kolumna `płeć` o dwóch wartościach – złym).

**Rodzaje indeksów:**

*   **Indeks jednokolumnowy (Single-column Index):** Najprostszy typ, oparty na wartościach z jednej kolumny.
*   **Indeks złożony (Composite/Compound Index):** Zbudowany na dwóch lub więcej kolumnach. Kolejność kolumn w definicji indeksu ma kluczowe znaczenie – powinien on odzwierciedlać kolejność kolumn w klauzuli `WHERE`.
*   **Indeks unikalny (Unique Index):** Gwarantuje, że wszystkie wartości w indeksowanej kolumnie (lub kombinacji kolumn) są unikalne. Klucze podstawowe (Primary Key) automatycznie otrzymują indeks unikalny.
*   **Indeks klastrowy (Clustered Index):** Specjalny typ indeksu, który fizycznie sortuje wiersze w tabeli na dysku zgodnie z porządkiem indeksu. Każda tabela może mieć co najwyżej jeden indeks klastrowy. W wielu systemach (np. SQL Server, MySQL/InnoDB) klucz podstawowy jest domyślnie indeksem klastrowym.
*   **Indeks nieklastrowy (Non-clustered Index):** Standardowy typ indeksu, który przechowuje wartości klucza i wskaźniki do fizycznych wierszy, ale nie zmienia ich kolejności na dysku. Tabela może mieć wiele indeksów nieklastrowych.

**Koszt indeksów:**

Indeksy nie są darmowe. Zajmują dodatkowe miejsce na dysku i, co ważniejsze, spowalniają operacje zapisu (`INSERT`, `UPDATE`, `DELETE`), ponieważ każda modyfikacja danych w tabeli wymaga również aktualizacji wszystkich powiązanych z nią indeksów. Dlatego kluczowe jest znalezienie złotego środka i indeksowanie tylko tych kolumn, które przyniosą realny zysk przy odczycie.

#### Podstawowe zasady optymalizacji zapytań

1.  **Indeksuj mądrze:** To najważniejsza zasada. Załóż indeksy na kolumnach używanych w `WHERE`, `JOIN` i `ORDER BY`. Używaj polecenia `EXPLAIN` (lub `EXPLAIN ANALYZE`), aby zobaczyć plan wykonania zapytania i sprawdzić, czy optymalizator korzysta z założonych indeksów.

2.  **Unikaj `SELECT *`:** Zawsze wymieniaj tylko te kolumny, których faktycznie potrzebujesz. `SELECT *` powoduje niepotrzebne obciążenie sieci i bazy danych, a także uniemożliwia zastosowanie niektórych optymalizacji, np. **covering index** (gdy wszystkie potrzebne dane znajdują się w samym indeksie, bez potrzeby sięgania do tabeli).

3.  **Pisz warunki `WHERE` przyjazne dla indeksów (SARGable - Search ARGument-able):** Unikaj stosowania funkcji na indeksowanych kolumnach. Zamiast `WHERE YEAR(data_zamowienia) = 2023` (co uniemożliwia użycie indeksu na `data_zamowienia`), napisz `WHERE data_zamowienia >= '2023-01-01' AND data_zamowienia < '2024-01-01'`.

4.  **Używaj `JOIN` zamiast podzapytań w `WHERE`:** W większości przypadków jawne złączenia (`JOIN`) są bardziej wydajne niż podzapytania skorelowane, ponieważ dają optymalizatorowi więcej możliwości wyboru strategii łączenia.

5.  **Ograniczaj liczbę wyników:** Używaj `LIMIT` (lub `TOP`, `FETCH FIRST`), gdy potrzebujesz tylko kilku pierwszych wierszy. Używaj `WHERE` do jak najwcześniejszego odfiltrowania jak największej liczby danych.

6.  **Zrozum działanie `GROUP BY`:** Agregowanie danych jest kosztowne. Upewnij się, że grupujesz po jak najmniejszej liczbie kolumn i filtrujesz dane w `WHERE` przed agregacją, a nie w `HAVING` po niej (jeśli to możliwe).

#### Przykład

**Problem:** Chcemy znaleźć nazwiska wszystkich pracowników z działu 'IT', którzy zostali zatrudnieni w 2022 roku.

**Zapytanie nieoptymalne:**
```sql
SELECT nazwisko FROM pracownicy WHERE dzial = 'IT' AND SUBSTRING(data_zatrudnienia, 1, 4) = '2022';
```
*Problem: Użycie funkcji `SUBSTRING` na kolumnie `data_zatrudnienia` uniemożliwia wykorzystanie indeksu na tej kolumnie.*

**Zapytanie zoptymalizowane:**
```sql
SELECT nazwisko FROM pracownicy WHERE dzial = 'IT' AND data_zatrudnienia >= '2022-01-01' AND data_zatrudnienia < '2023-01-01';
```
*Rozwiązanie: Warunek jest teraz "SARGable". Jeśli istnieje złożony indeks na `(dzial, data_zatrudnienia)`, to zapytanie będzie niezwykle szybkie.*

#### Podsumowanie

*   **Optymalizacja zapytań** to proces minimalizowania czasu ich wykonania, realizowany głównie przez **optymalizator zapytań** w RDBMS.
*   Najważniejszym narzędziem optymalizacji są **indeksy**, które przyspieszają odczyt danych kosztem spowolnienia operacji zapisu.
*   Kluczowe jest **zakładanie indeksów** na kolumnach używanych w klauzulach `WHERE`, `JOIN` i `ORDER BY`.
*   Podstawowe zasady pisania wydajnych zapytań to: **unikanie `SELECT *`**, pisanie warunków **przyjaznych dla indeksów (SARGable)**, preferowanie `JOIN` nad podzapytaniami i wczesne filtrowanie danych.
*   Narzędzie `EXPLAIN` jest niezbędne do analizy **planów wykonania** i weryfikacji, czy optymalizacje przynoszą zamierzony skutek.

**Typowe pytania egzaminacyjne:**
*   Jaki jest cel optymalizacji zapytań i kto jest za nią odpowiedzialny w systemie bazodanowym?
*   Co to jest indeks w bazie danych i jakie jest jego zadanie?
*   Kiedy warto zakładać indeksy, a kiedy mogą one być szkodliwe?
*   Proszę wymienić i opisać podstawowe zasady pisania zoptymalizowanych zapytań SQL.
*   Co to jest plan wykonania zapytania i do czego służy polecenie `EXPLAIN`?

---

# 16. Model architekturalny komputera wg. von Neumanna a model obliczeniowy komputera na podstawie maszyny Turinga i ich rola w informatyce

#### Wprowadzenie

U podstaw współczesnej informatyki leżą dwa fundamentalne, choć różne w swojej naturze, modele: maszyna Turinga jako teoretyczny model obliczalności oraz architektura von Neumanna jako praktyczny schemat budowy komputerów. Maszyna Turinga odpowiada na pytanie, *co* w ogóle da się obliczyć, definiując granice tego, co jest algorytmicznie możliwe. Architektura von Neumanna odpowiada na pytanie, *jak* zbudować uniwersalną maszynę, która te obliczenia może efektywnie realizować. Zrozumienie obu tych koncepcji i relacji między nimi jest kluczowe dla zrozumienia, czym jest i jak działa komputer – zarówno w sensie teoretycznym, jak i praktycznym.

#### Model obliczeniowy: Maszyna Turinga

Zaproponowana przez Alana Turinga w 1936 roku, maszyna Turinga nie jest fizycznym urządzeniem, lecz **abstrakcyjnym modelem matematycznym**, który miał na celu sformalizowanie pojęcia algorytmu.

**Elementy maszyny Turinga:**

1.  **Nieskończona taśma:** Podzielona na komórki, z których każda może przechowywać jeden symbol z określonego alfabetu.
2.  **Głowica:** Może odczytywać symbol z komórki, na której się znajduje, zapisywać w niej nowy symbol oraz przesuwać się o jedną komórkę w lewo lub w prawo.
3.  **Rejestr stanu:** Przechowuje aktualny stan maszyny, wybrany ze skończonego zbioru stanów.
4.  **Tablica przejść (program):** Zestaw reguł, które determinują działanie maszyny. Każda reguła ma postać: `(aktualny stan, odczytany symbol) -> (nowy stan, symbol do zapisu, ruch głowicy)`. Innymi słowy, na podstawie bieżącego stanu i symbolu pod głowicą, maszyna decyduje, co ma zapisać, do jakiego stanu przejść i w którą stronę się poruszyć.

**Rola i znaczenie w informatyce:**

*   **Definicja obliczalności:** Maszyna Turinga dostarczyła formalnej definicji tego, co to znaczy, że funkcja jest **obliczalna** (lub problem jest **rozstrzygalny**). Zgodnie z **hipotezą Churcha-Turinga**, każdy problem, który można rozwiązać za pomocą jakiegokolwiek intuicyjnie rozumianego algorytmu, można też rozwiązać za pomocą maszyny Turinga. Innymi słowy, maszyna Turinga jest tak potężna, jak każdy inny możliwy model obliczeniowy.
*   **Podstawa teorii złożoności:** Analiza liczby kroków lub komórek taśmy, jakich maszyna Turinga potrzebuje do rozwiązania problemu, jest podstawą teorii złożoności obliczeniowej i klasyfikacji problemów (np. klasy P i NP).
*   **Dowód istnienia problemów nierozstrzygalnych:** Turing użył swojego modelu, aby udowodnić, że istnieją problemy, których nie da się rozwiązać za pomocą żadnego algorytmu. Najsłynniejszym z nich jest **problem stopu** – nie istnieje uniwersalny algorytm, który byłby w stanie dla dowolnego programu i jego danych wejściowych rozstrzygnąć, czy ten program kiedykolwiek zakończy swoje działanie.

#### Model architekturalny: Architektura von Neumanna

Zaproponowana przez Johna von Neumanna w 1945 roku, architektura ta (znana też jako architektura Princeton) jest **praktycznym schematem budowy** uniwersalnego komputera cyfrowego. Niemal każdy współczesny komputer – od smartfona po superkomputer – jest zbudowany w oparciu o jej założenia.

**Główne komponenty architektury von Neumanna:**

1.  **Jednostka centralna (CPU - Central Processing Unit):** "Mózg" komputera, składający się z:
    *   **Jednostki arytmetyczno-logicznej (ALU - Arithmetic Logic Unit):** Wykonuje operacje arytmetyczne (dodawanie, odejmowanie) i logiczne (AND, OR, NOT).
    *   **Jednostki sterującej (CU - Control Unit):** Kieruje przepływem danych i instrukcji, interpretuje polecenia programu i steruje pracą pozostałych komponentów.
2.  **Pamięć operacyjna (Memory):** Przechowuje zarówno **dane**, na których operuje program, jak i **instrukcje** samego programu. Jest to kluczowa i definiująca cecha tej architektury – tzw. **koncepcja przechowywanego programu (stored-program concept)**.
3.  **System wejścia/wyjścia (I/O):** Umożliwia komunikację komputera ze światem zewnętrznym (np. klawiatura, mysz, monitor, dysk twardy).
4.  **Magistrala (Bus):** Zestaw połączeń, którymi przesyłane są dane, adresy i sygnały sterujące między CPU, pamięcią i systemem I/O.

**Rola i znaczenie w informatyce:**

*   **Uniwersalność:** Dzięki koncepcji przechowywanego programu, komputer von Neumanna nie jest maszyną do jednego, konkretnego zadania. Aby zmienić jego funkcję, wystarczy wczytać do pamięci inny program. To właśnie ta cecha uczyniła komputery tak uniwersalnym narzędziem.
*   **Cykl rozkazowy:** Praca komputera opiera się na powtarzalnym cyklu: **pobierz instrukcję** z pamięci, **zdekoduj** ją, **pobierz dane** (jeśli potrzebne), **wykonaj operację** i **zapisz wynik**.
*   **Wąskie gardło von Neumanna (von Neumann bottleneck):** Wspólna magistrala dla danych i instrukcji stanowi ograniczenie wydajności. CPU nie może jednocześnie pobierać instrukcji i danych z pamięci, co prowadzi do oczekiwania i spowalnia pracę. Jest to jedno z głównych wyzwań we współczesnej architekturze komputerów.

#### Porównanie i wzajemna relacja

| Cecha | Maszyna Turinga | Architektura von Neumanna |
|---|---|---|
| **Natura** | Abstrakcyjny model matematyczny | Praktyczny schemat budowy komputera |
| **Cel** | Zdefiniowanie granic obliczalności | Realizacja uniwersalnego komputera |
| **Pamięć** | Nieskończona, jednowymiarowa taśma | Skończona, adresowalna pamięć o dostępie swobodnym (RAM) |
| **Program** | Zakodowany w tablicy przejść (sprzętowy) | Przechowywany w pamięci razem z danymi (programowy) |
| **Znaczenie** | Podstawa teorii obliczeń i złożoności | Podstawa budowy niemal wszystkich współczesnych komputerów |

**Relacja:** Architektura von Neumanna jest fizyczną realizacją komputera, który jest **Turing-zupełny (Turing-complete)**. Oznacza to, że komputer o architekturze von Neumanna (z potencjalnie nieograniczoną pamięcią) jest w stanie zasymulować działanie dowolnej maszyny Turinga, a co za tym idzie – wykonać każdy możliwy do wykonania algorytm. Maszyna Turinga dostarcza teoretycznych ram mocy obliczeniowej, a architektura von Neumanna praktycznego sposobu na zbudowanie maszyny, która tę moc posiada.

#### Podsumowanie

*   **Maszyna Turinga** to **teoretyczny model obliczeń**, który zdefiniował, co jest algorytmicznie możliwe do obliczenia, i stał się fundamentem teorii obliczalności i złożoności. Jej kluczowym wkładem jest formalizacja pojęcia algorytmu i dowód na istnienie problemów nierozstrzygalnych.
*   **Architektura von Neumanna** to **praktyczny model budowy komputera**, którego najważniejszą cechą jest **koncepcja przechowywanego programu** – instrukcje i dane znajdują się w tej samej, wspólnej pamięci. To umożliwiło budowę uniwersalnych, programowalnych maszyn.
*   Komputer o architekturze von Neumanna jest **fizyczną implementacją** maszyny, która jest **Turing-zupełna**, czyli zdolna do wykonania każdego algorytmu.
*   Maszyna Turinga mówi nam o **granicach możliwości**, a architektura von Neumanna o **sposobie ich realizacji**.

**Typowe pytania egzaminacyjne:**
*   Proszę opisać podstawowe elementy maszyny Turinga i jej rolę w informatyce.
*   Proszę opisać podstawowe komponenty komputera o architekturze von Neumanna.
*   Na czym polega koncepcja przechowywanego programu (stored-program concept) i jakie jest jej znaczenie?
*   Proszę porównać maszynę Turinga i architekturę von Neumanna, wskazując na ich naturę, cel i rolę w informatyce.
*   Co to jest "wąskie gardło von Neumanna"?

---

# 17. Logika boolowska i jej zastosowania w warstwie sprzętowej komputerów

#### Wprowadzenie

Logika boolowska, nazwana na cześć George'a Boole'a, to dział matematyki i logiki zajmujący się operacjami na wartościach prawdy: **prawda (true)** i **fałsz (false)**. W świecie cyfrowych komputerów, gdzie informacja jest reprezentowana w systemie binarnym, te dwie wartości mają swoje bezpośrednie fizyczne odpowiedniki: wysoki i niski poziom napięcia elektrycznego, umownie oznaczane jako **1 (prawda)** i **0 (fałsz)**. Logika boolowska stanowi absolutny fundament, na którym zbudowana jest cała warstwa sprzętowa współczesnych komputerów. Każda operacja, od prostego dodawania dwóch liczb po skomplikowane instrukcje procesora, jest w swojej istocie realizowana przez fizyczne układy, które implementują podstawowe operacje tej logiki.

#### Podstawowe operacje i bramki logiczne

Algebra Boole'a definiuje trzy fundamentalne operacje, które w elektronice cyfrowej są realizowane przez tzw. **bramki logiczne**.

1.  **Koniunkcja (AND):**
    *   **Logika:** Operacja "i". Wynik jest prawdziwy (1) wtedy i tylko wtedy, gdy **oba** argumenty są prawdziwe (1).
    *   **Notacja:** $A \cdot B$ lub $A \land B$.
    *   **Bramka AND:** Układ elektroniczny z dwoma (lub więcej) wejściami i jednym wyjściem. Na wyjściu pojawi się stan wysoki (1) tylko wtedy, gdy na wszystkich wejściach będzie stan wysoki.

2.  **Alternatywa (OR):**
    *   **Logika:** Operacja "lub". Wynik jest prawdziwy (1), jeśli **co najmniej jeden** z argumentów jest prawdziwy (1).
    *   **Notacja:** $A + B$ lub $A \lor B$.
    *   **Bramka OR:** Układ, na którego wyjściu pojawi się stan wysoki (1), jeśli na którymkolwiek z wejść będzie stan wysoki.

3.  **Negacja (NOT):**
    *   **Logika:** Operacja "nie". Odwraca wartość logiczną argumentu. Prawda staje się fałszem, a fałsz prawdą.
    *   **Notacja:** $\neg A$ lub $\bar{A}$.
    *   **Bramka NOT (inwerter):** Układ z jednym wejściem i jednym wyjściem. Stan na wyjściu jest zawsze przeciwny do stanu na wejściu.

**Tablice prawdy dla podstawowych bramek:**

| A | B | A AND B | A OR B |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 |

| A | NOT A |
|---|---|
| 0 | 1 |
| 1 | 0 |

Oprócz tych trzech podstawowych, w praktyce używa się również innych bramek, które są ich kombinacjami, np. **NAND** (NOT AND), **NOR** (NOT OR) oraz **XOR** (exclusive OR - "albo", wynik jest prawdziwy, gdy wejścia są różne).

#### Zastosowania w warstwie sprzętowej

Bramki logiczne są elementarnymi klockami, z których buduje się bardziej złożone układy cyfrowe. Fizycznie, każda bramka jest zbudowana z kilku **tranzystorów**.

**1. Układy kombinacyjne (Combinational Circuits)**

Są to układy, w których stan wyjść zależy **wyłącznie od aktualnego stanu wejść**. Nie posiadają one pamięci. Z bramek logicznych buduje się m.in.:

*   **Sumatory (Adders):** Układy realizujące operację dodawania binarnego. Prosty **półsumator (half adder)** dodaje dwie pojedyncze cyfry binarne, dając w wyniku sumę i przeniesienie. **Pełny sumator (full adder)** dodaje trzy bity (dwa bity danych i bit przeniesienia z poprzedniej pozycji). Łącząc szeregowo wiele pełnych sumatorów, można zbudować układ dodający liczby wielobitowe.
*   **Multipleksery (Multiplexers, MUX):** Układy, które wybierają jeden z wielu sygnałów wejściowych i przekazują go na jedno wyjście. Wybór jest kontrolowany przez dodatkowe wejścia sterujące. Działają jak cyfrowy przełącznik.
*   **Demultipleksery (Demultiplexers, DEMUX):** Działają odwrotnie do multiplekserów – przekazują jeden sygnał wejściowy na jedno z wielu możliwych wyjść.
*   **Dekodery:** Konwertują kod binarny na określony sygnał wyjściowy. Np. dekoder "2 na 4" ma 2 wejścia i 4 wyjścia; w zależności od 2-bitowej liczby na wejściu, aktywuje jedno z czterech wyjść.

**2. Jednostka Arytmetyczno-Logiczna (ALU)**

ALU to serce procesora (CPU). Jest to złożony układ kombinacyjny, zbudowany z sumatorów, bramek logicznych i multiplekserów, odpowiedzialny za wykonywanie wszystkich operacji arytmetycznych (dodawanie, odejmowanie) i logicznych (AND, OR, XOR, NOT) na danych. Jednostka sterująca (CU) wysyła do ALU sygnały, które określają, jaką operację ma ona wykonać.

**3. Układy sekwencyjne (Sequential Circuits)**

Są to układy, w których stan wyjść zależy nie tylko od aktualnego stanu wejść, ale także od **stanów poprzednich**. Posiadają one element **pamięci**. Podstawowym budulcem układów sekwencyjnych są **przerzutniki (flip-flops)**.

*   **Przerzutnik (Flip-Flop):** Prosty układ, najczęściej zbudowany z dwóch sprzężonych ze sobą bramek NAND lub NOR, który potrafi przechowywać **jeden bit informacji**. Może znajdować się w jednym z dwóch stabilnych stanów (0 lub 1) i pozostaje w nim dopóki nie zostanie zmieniony przez sygnał wejściowy. Przerzutniki są podstawowym elementem budulcowym:
    *   **Rejestrów procesora:** Szybkich komórek pamięci wewnątrz CPU, przechowujących dane, na których aktualnie operuje ALU (np. akumulator, licznik programu).
    *   **Pamięci podręcznej (Cache):** Zbudowanej z milionów przerzutników (pamięć typu SRAM - Static RAM).

#### Przykład: Budowa półsumatora

Półsumator dodaje dwa bity, A i B, dając w wyniku bit sumy (S) i bit przeniesienia (C - Carry).

**Tablica prawdy:**
| A | B | S | C |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

Analizując tablicę, widzimy, że:
*   Kolumna Sumy (S) odpowiada operacji **XOR**: $S = A \oplus B$.
*   Kolumna Przeniesienia (C) odpowiada operacji **AND**: $C = A \cdot B$.

Oznacza to, że półsumator można zbudować z jednej bramki XOR i jednej bramki AND.

#### Podsumowanie

*   **Logika boolowska**, operująca na wartościach **prawda (1)** i **fałsz (0)**, jest matematycznym fundamentem działania cyfrowych komputerów.
*   Podstawowe operacje logiczne (AND, OR, NOT) są fizycznie realizowane przez **bramki logiczne**, zbudowane z tranzystorów.
*   Z bramek logicznych, jak z klocków, buduje się bardziej złożone **układy kombinacyjne** (np. sumatory, multipleksery), które nie mają pamięci.
*   Najważniejszym układem kombinacyjnym w procesorze jest **ALU**, wykonująca operacje arytmetyczne i logiczne.
*   Poprzez dodanie sprzężenia zwrotnego do bramek tworzy się **przerzutniki** – podstawowe komórki pamięci zdolne do przechowywania jednego bitu. Z nich buduje się **układy sekwencyjne**, takie jak **rejestry procesora** i **pamięć podręczna**.
*   W ten sposób cała złożona maszyneria komputera, od najprostszych obliczeń po przechowywanie danych, sprowadza się na najniższym poziomie do manipulacji sygnałami binarnymi zgodnie z zasadami logiki Boole'a.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać podstawowe operacje logiki Boole'a (AND, OR, NOT) i odpowiadające im bramki logiczne.
*   Jakie jest zastosowanie logiki boolowskiej w warstwie sprzętowej komputera?
*   Czym różnią się układy kombinacyjne od sekwencyjnych? Proszę podać po jednym przykładzie każdego z nich.
*   Do czego służy i z czego zbudowana jest jednostka ALU?
*   Co to jest przerzutnik i jaka jest jego rola w budowie komputera?

---

# 18. Zapis binarny liczb całkowitych, zapis zmiennoprzecinkowy liczb rzeczywistych, arytmetyka komputerowa

#### Wprowadzenie

Komputery, w swojej istocie, operują wyłącznie na bitach – zerach i jedynkach. Aby mogły one przetwarzać liczby, z których korzystamy na co dzień, konieczne jest zastosowanie odpowiednich systemów kodowania, które przełożą liczby dziesiętne na postać binarną. Sposób tej reprezentacji jest fundamentalnie różny dla liczb całkowitych i rzeczywistych. Zapis liczb całkowitych musi efektywnie obsługiwać liczby ujemne i umożliwiać prostą arytmetykę. Zapis liczb rzeczywistych (zmiennoprzecinkowych) to z kolei kompromis między zakresem a precyzją, pozwalający na reprezentowanie zarówno bardzo małych, jak i bardzo dużych wartości. Zrozumienie tych systemów jest kluczowe dla świadomości, jak komputer wykonuje obliczenia i jakie są tego ograniczenia.

#### Zapis binarny liczb całkowitych

Liczby całkowite można reprezentować na ustalonej liczbie bitów (np. 8, 16, 32, 64). Dla liczb naturalnych (nieujemnych) sprawa jest prosta – jest to standardowa konwersja z systemu dziesiętnego na binarny. Wyzwanie pojawia się przy liczbach ujemnych.

**Kod uzupełnień do dwóch (U2, Two's Complement)**

Jest to obecnie powszechnie stosowany standard zapisu liczb całkowitych ze znakiem. Jego popularność wynika z faktu, że operacje arytmetyczne (dodawanie, odejmowanie) wykonuje się na nim tak samo, jak na liczbach naturalnych, co znacznie upraszcza budowę jednostki arytmetyczno-logicznej (ALU).

**Zasady kodu U2 (na przykładzie 8 bitów):**

*   **Najstarszy bit (MSB - Most Significant Bit)** jest **bitem znaku**: 0 oznacza liczbę dodatnią lub zero, 1 oznacza liczbę ujemną.
*   **Liczby dodatnie:** Kodowane standardowo. Zakres od 0 do 127. Np. `01111111` to 127.
*   **Liczby ujemne:** Aby uzyskać kod liczby ujemnej (np. -X), należy:
    1.  Wziąć reprezentację binarną liczby dodatniej X.
    2.  Zanegować wszystkie bity (operacja NOT).
    3.  Dodać 1.

**Przykład: Zapis liczby -5 na 8 bitach w U2**
1.  Liczba dodatnia 5 to `00000101`.
2.  Negacja bitów: `11111010`.
3.  Dodanie 1: `11111011`. To jest zapis liczby -5 w U2.

**Zalety U2:**
*   Jedna reprezentacja zera (`00000000`).
*   Dodawanie i odejmowanie (realizowane jako dodawanie liczby przeciwnej) działają w ten sam sposób dla liczb dodatnich i ujemnych.

#### Zapis zmiennoprzecinkowy liczb rzeczywistych (Standard IEEE 754)

Liczby rzeczywiste (ułamki) wymagają innego podejścia. Standard IEEE 754 definiuje sposób ich zapisu, analogiczny do notacji naukowej (np. $1.23 \times 10^4$), ale w systemie binarnym.

Każda liczba zmiennoprzecinkowa składa się z trzech części:

1.  **Znak (S - Sign):** 1 bit. 0 dla liczby dodatniej, 1 dla ujemnej.
2.  **Cech (E - Exponent):** Określona liczba bitów (np. 8 dla pojedynczej precyzji). Przechowuje wykładnik potęgi, do której podnoszona jest podstawa systemu (czyli 2). Jest zapisana w **kodzie z nadmiarem**, aby umożliwić reprezentację zarówno dodatnich, jak i ujemnych wykładników.
3.  **Mantysa (M - Mantissa/Significand):** Pozostałe bity (np. 23 dla pojedynczej precyzji). Przechowuje ułamkową część liczby w postaci znormalizowanej. W normalizacji zakłada się, że przed przecinkiem jest zawsze "ukryta" jedynka (`1.mantysa`), co pozwala zaoszczędzić jeden bit i zwiększyć precyzję.

**Formaty IEEE 754:**

*   **Pojedyncza precyzja (single-precision, `float`):** 32 bity (1 bit znaku, 8 bitów cechy, 23 bity mantysy).
*   **Podwójna precyzja (double-precision, `double`):** 64 bity (1 bit znaku, 11 bitów cechy, 52 bity mantysy).

**Ograniczenia zapisu zmiennoprzecinkowego:**

*   **Ograniczona precyzja:** Nie wszystkie liczby dziesiętne (zwłaszcza ułamki) dają się dokładnie reprezentować w systemie binarnym. Np. liczba 0.1 nie ma skończonego rozwinięcia binarnego. Prowadzi to do **błędów zaokrągleń**.
*   **Specjalne wartości:** Standard definiuje kody dla nieskończoności (dodatniej i ujemnej), zera (dodatniego i ujemnego) oraz wartości **NaN (Not a Number)**, która jest wynikiem nieprawidłowych operacji (np. pierwiastek z liczby ujemnej).

#### Arytmetyka komputerowa

Arytmetyka komputerowa to sposób, w jaki ALU wykonuje operacje na liczbach binarnych.

*   **Dodawanie liczb całkowitych (U2):** Wykonywane jest tak samo jak standardowe dodawanie binarne. Ewentualne przeniesienie z najstarszego bitu jest ignorowane. System musi jednak wykrywać **nadmiar (overflow)**, czyli sytuację, gdy wynik operacji wykracza poza zakres możliwy do reprezentacji na danej liczbie bitów (np. suma dwóch dużych liczb dodatnich daje w wyniku liczbę ujemną).

*   **Odejmowanie liczb całkowitych (U2):** Realizowane jest jako dodawanie liczby przeciwnej. Aby obliczyć $A - B$, komputer oblicza $A + (-B)$, gdzie $-B$ jest reprezentacją liczby B w kodzie U2.

*   **Mnożenie i dzielenie:** Są to operacje bardziej złożone, realizowane za pomocą algorytmów opartych na wielokrotnym dodawaniu i przesunięciach bitowych.

*   **Arytmetyka zmiennoprzecinkowa:** Jest znacznie bardziej skomplikowana niż całkowitoliczbowa i często realizowana przez dedykowany koprocesor (FPU - Floating-Point Unit). Wymaga ona m.in.:
    1.  Porównania i wyrównania wykładników (cech).
    2.  Wykonania operacji (np. dodawania) na mantysach.
    3.  Normalizacji wyniku (przesunięcia mantysy i dostosowania wykładnika).
    4.  Zaokrąglenia wyniku do dostępnej precyzji.

#### Przykład

**Problem:** Dodaj $5 + (-3)$ na 8 bitach w kodzie U2.

1.  **Reprezentacje binarne:**
    *   $5 \rightarrow 00000101_2$
    *   $-3 \rightarrow$ (3 to `00000011` -> negacja `11111100` -> dodaj 1) $\rightarrow 11111101_2$

2.  **Dodawanie binarne:**
    ```
      00000101  (5)
    + 11111101  (-3)
    ----------
    1 00000010  (2)
    ```

3.  **Wynik:** Przeniesienie z ostatniej pozycji (dziewiąty bit) jest ignorowane. Wynik to `00000010`, czyli 2. Operacja się powiodła.

**Konsekwencja błędu zaokrąglenia:**

W wielu językach programowania wynik operacji `0.1 + 0.2` nie jest równy `0.3`. Dzieje się tak, ponieważ ani 0.1, ani 0.2 nie mają dokładnej, skończonej reprezentacji binarnej. Ich przybliżone wartości po zsumowaniu dają wynik bardzo bliski 0.3, ale nie identyczny (np. `0.30000000000000004`).

#### Podsumowanie

*   Liczby **całkowite ze znakiem** są najczęściej reprezentowane w **kodzie uzupełnień do dwóch (U2)**, który upraszcza operacje arytmetyczne.
*   Liczby **rzeczywiste** są reprezentowane w formacie **zmiennoprzecinkowym (standard IEEE 754)**, który składa się ze **znaku, cechy i mantysy**. Jest to kompromis między zakresem a precyzją.
*   **Arytmetyka komputerowa** definiuje, jak ALU wykonuje operacje na liczbach binarnych. Odejmowanie jest realizowane jako dodawanie liczby przeciwnej.
*   Arytmetyka zmiennoprzecinkowa jest złożona i podatna na **błędy zaokrągleń** z powodu niemożności dokładnego przedstawienia niektórych ułamków dziesiętnych.
*   Świadomość sposobu reprezentacji liczb i ograniczeń arytmetyki komputerowej jest niezbędna do pisania poprawnego i niezawodnego oprogramowania, zwłaszcza w zastosowaniach naukowych i finansowych.

**Typowe pytania egzaminacyjne:**
*   Na czym polega kodowanie liczb całkowitych w systemie U2? Proszę przedstawić w 8-bitowym kodzie U2 liczbę dodatnią i ujemną.
*   Jakie są trzy główne składniki liczby zmiennoprzecinkowej w standardzie IEEE 754?
*   Dlaczego zapis zmiennoprzecinkowy jest niedokładny? Proszę podać przykład.
*   Jak w komputerze realizowana jest operacja odejmowania liczb całkowitych?
*   Co to jest nadmiar (overflow) w arytmetyce komputerowej?

---

# 19. Miary wydajności procesorów, pamięci i systemów obliczeniowych

#### Wprowadzenie

Wydajność systemu komputerowego jest pojęciem złożonym i nie da się jej opisać jedną, uniwersalną liczbą. W zależności od zastosowania, interesować nas może szybkość wykonywania pojedynczego zadania, liczba zadań realizowanych w jednostce czasu, czy zdolność do obsługi ogromnych zbiorów danych. Dlatego w informatyce stosuje się szereg różnych miar, które pozwalają ocenić i porównać wydajność poszczególnych komponentów – procesorów i pamięci – oraz całych systemów obliczeniowych. Zrozumienie tych miar jest kluczowe do świadomego wyboru sprzętu, optymalizacji oprogramowania i projektowania skalowalnych systemów.

#### I. Miary Wydajności Procesorów (CPU)

Wydajność procesora zależy od wielu czynników, a najpopularniejsze miary często bywają mylące, jeśli są rozpatrywane w izolacji.

1.  **Taktowanie (Częstotliwość zegara):**
    *   **Definicja:** Liczba cykli roboczych, jakie procesor wykonuje w ciągu jednej sekundy. Mierzona w hercach (Hz), a praktycznie w gigahercach (GHz).
    *   **Znaczenie:** Wyższe taktowanie oznacza, że procesor wykonuje więcej cykli na sekundę, co *potencjalnie* prowadzi do wyższej wydajności. Jest to jednak miara myląca, ponieważ nie mówi nic o tym, ile pracy jest wykonywane w *jednym cyklu*.

2.  **IPC (Instructions Per Cycle) – Instrukcje na cykl:**
    *   **Definicja:** Średnia liczba instrukcji, jakie procesor jest w stanie wykonać w jednym cyklu zegara.
    *   **Znaczenie:** Jest to kluczowa miara **efektywności architektury** procesora. Nowoczesne procesory (tzw. superskalarne) potrafią wykonywać wiele instrukcji jednocześnie (IPC > 1) dzięki technikom takim jak pipelining i zwielokrotnienie jednostek wykonawczych. Procesor A o taktowaniu 3 GHz i IPC=1.5 będzie wydajniejszy niż procesor B o taktowaniu 4 GHz i IPC=1.0.

3.  **MIPS (Million Instructions Per Second) – Miliony instrukcji na sekundę:**
    *   **Definicja:** Miara określająca, ile milionów prostych instrukcji (zazwyczaj całkowitoliczbowych) procesor może wykonać w ciągu sekundy.
    *   **Znaczenie:** Historycznie popularna miara, dziś rzadziej stosowana, ponieważ "instrukcja" nie jest jednostką standardową – jej złożoność różni się między architekturami (CISC vs. RISC) i typami operacji.

4.  **FLOPS (Floating-Point Operations Per Second) – Operacje zmiennoprzecinkowe na sekundę:**
    *   **Definicja:** Kluczowa miara wydajności w obliczeniach naukowych, inżynierskich, grafice 3D i uczeniu maszynowym. Określa liczbę operacji na liczbach zmiennoprzecinkowych (dodawanie, mnożenie), jaką procesor może wykonać w sekundzie. Używa się wielokrotności: GFLOPS (miliardy), TFLOPS (biliony), PFLOPS (biliardy).
    *   **Znaczenie:** Jest to standardowa miara wydajności superkomputerów (ranking TOP500) i procesorów graficznych (GPU).

5.  **Liczba rdzeni i wątków:**
    *   **Definicja:** **Rdzeń (core)** to w pełni funkcjonalna jednostka przetwarzająca wewnątrz procesora. **Wątek (thread)** to sekwencja instrukcji, którą rdzeń może wykonywać. Technologie takie jak Hyper-Threading (Intel) pozwalają jednemu fizycznemu rdzeniowi obsługiwać dwa wątki jednocześnie.
    *   **Znaczenie:** Większa liczba rdzeni i wątków pozwala na prawdziwą **równoległość**, czyli jednoczesne wykonywanie wielu zadań. Jest to kluczowe dla wydajności w zastosowaniach wielozadaniowych i oprogramowaniu potrafiącym zrównoleglić obliczenia.

#### II. Miary Wydajności Pamięci

Wydajność podsystemu pamięci jest równie ważna jak wydajność CPU, ponieważ nawet najszybszy procesor będzie bezczynny, jeśli musi czekać na dane.

1.  **Pojemność (Capacity):**
    *   **Definicja:** Ilość danych, jaką pamięć może przechować. Mierzona w bajtach i ich wielokrotnościach (kilobajty - KB, megabajty - MB, gigabajty - GB, terabajty - TB).
    *   **Znaczenie:** Określa, jak duże programy i zbiory danych mogą być aktywnie przetwarzane.

2.  **Hierarchia Pamięci:** Wydajność pamięci należy rozpatrywać w kontekście jej hierarchii, gdzie każdy kolejny poziom jest większy, ale wolniejszy i tańszy:
    *   **Rejestry procesora:** Najszybsze, najmniejsze, wewnątrz CPU.
    *   **Pamięć podręczna (Cache) L1, L2, L3:** Bardzo szybka, mała, pośredniczy między CPU a RAM.
    *   **Pamięć operacyjna (RAM):** Wolniejsza, znacznie większa.
    *   **Pamięć masowa (SSD, HDD):** Najwolniejsza, największa.

3.  **Przepustowość (Bandwidth):**
    *   **Definicja:** Szybkość, z jaką dane mogą być odczytywane z pamięci lub zapisywane do niej. Mierzona w megabajtach na sekundę (MB/s) lub gigabajtach na sekundę (GB/s).
    *   **Znaczenie:** Wysoka przepustowość jest kluczowa w zastosowaniach przetwarzających duże strumienie danych (np. obróbka wideo, gry, symulacje).

4.  **Opóźnienie (Latency):**
    *   **Definicja:** Czas, jaki upływa od momentu zażądania danych z pamięci do momentu ich otrzymania. Mierzony w nanosekundach (ns).
    *   **Znaczenie:** Niskie opóźnienie jest krytyczne dla responsywności systemu i wydajności operacji na małych, losowo rozrzuconych danych.

#### III. Miary Wydajności Systemów Obliczeniowych

Oceniając cały system, używamy bardziej ogólnych miar, które opisują jego zdolność do przetwarzania zadań.

1.  **Przepustowość (Throughput):**
    *   **Definicja:** Liczba zadań, operacji lub transakcji, jakie system jest w stanie ukończyć w jednostce czasu. Przykłady: liczba zapytań do bazy danych na sekundę, liczba klatek na sekundę (FPS) w grze.
    *   **Znaczenie:** Kluczowa miara dla systemów serwerowych, które muszą obsługiwać wielu użytkowników jednocześnie.

2.  **Czas odpowiedzi (Response Time) / Opóźnienie (Latency):**
    *   **Definicja:** Całkowity czas, jaki upływa od zainicjowania zadania do jego ukończenia.
    *   **Znaczenie:** Kluczowa miara dla systemów interaktywnych, gdzie liczy się odczuwalna przez użytkownika szybkość reakcji.

3.  **Prawo Amdahla:**
    *   **Definicja:** Prawo opisujące teoretyczne przyspieszenie, jakie można uzyskać, zrównoleglając wykonanie zadania. Mówi ono, że przyspieszenie jest **ograniczone przez część zadania, która musi być wykonana sekwencyjnie** i nie da się jej zrównoleglić.
    *   **Znaczenie:** Pokazuje, że dodawanie kolejnych procesorów nie zawsze prowadzi do proporcjonalnego wzrostu wydajności. Jeśli 10% programu musi działać sekwencyjnie, to nawet przy nieskończonej liczbie procesorów maksymalne przyspieszenie wyniesie 10x.

4.  **Testy wzorcowe (Benchmarks):**
    *   **Definicja:** Standardowe programy i zestawy zadań, które służą do mierzenia i porównywania wydajności różnych systemów w kontrolowanych warunkach. Przykłady: SPEC (dla CPU), Linpack (dla superkomputerów), 3DMark (dla GPU).
    *   **Znaczenie:** Pozwalają na obiektywne porównanie różnych architektur i konfiguracji sprzętowych w konkretnych, typowych zastosowaniach.

#### Podsumowanie

*   Wydajność **procesora** zależy od kombinacji **taktowania (GHz)** i **efektywności architektury (IPC)**. W zastosowaniach naukowych kluczową miarą jest **FLOPS**.
*   Wydajność **pamięci** to kompromis między **pojemnością**, **przepustowością** a **opóźnieniem**, co jest odzwierciedlone w **hierarchii pamięci**.
*   Wydajność całego **systemu obliczeniowego** opisuje się przez **przepustowość** (ile zadań na sekundę) i **czas odpowiedzi** (jak szybko wykonuje się jedno zadanie).
*   **Prawo Amdahla** przypomina, że potencjał zrównoleglenia obliczeń jest zawsze ograniczony przez ich sekwencyjną część.
*   Żadna pojedyncza miara nie jest wystarczająca. Pełna ocena wydajności wymaga analizy wielu metryk w kontekście konkretnego zastosowania, często przy użyciu standardowych **testów wzorcowych**.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać podstawowe miary wydajności procesora. Dlaczego samo taktowanie nie jest wiarygodną miarą?
*   Co to jest IPC i jakie ma znaczenie?
*   Proszę opisać hierarchię pamięci w komputerze, uwzględniając jej pojemność i szybkość na poszczególnych poziomach.
*   Czym różni się przepustowość od opóźnienia w kontekście pamięci i systemów obliczeniowych?
*   Na czym polega prawo Amdahla i jakie ma praktyczne znaczenie w kontekście systemów wieloprocesorowych?

---

# 20. Podstawowe elementy i znaczenie systemów wbudowanych

#### Wprowadzenie

Systemy wbudowane (ang. *embedded systems*) to niewidzialne konie pociągowe rewolucji cyfrowej. Są to specjalizowane systemy komputerowe, które stanowią integralną część większego urządzenia, maszyny lub instalacji, realizując w nim ściśle określoną funkcję sterującą, monitorującą lub komunikacyjną. W przeciwieństwie do komputerów ogólnego przeznaczenia (jak PC czy laptop), użytkownik systemu wbudowanego często nie jest nawet świadomy jego istnienia. Systemy te są wszechobecne – od prostych mikrokontrolerów w pralce czy mikrofalówce, przez złożone jednostki sterujące silnikiem (ECU) w samochodzie, po zaawansowane systemy awioniki w samolotach. Ich znaczenie polega na dodawaniu "inteligencji" do otaczających nas przedmiotów, co umożliwia ich automatyzację, optymalizację i komunikację.

#### Podstawowe elementy systemu wbudowanego

Typowy system wbudowany składa się z warstwy sprzętowej i programowej, które są ze sobą ściśle powiązane.

**1. Sprzęt (Hardware):**

Sercem każdego systemu wbudowanego jest jednostka przetwarzająca, ale w odróżnieniu od komputerów PC, jest ona zintegrowana z wieloma peryferiami na jednej płytce drukowanej (PCB).

*   **Mikrokontroler (MCU - Microcontroller Unit):** Najczęstszy wybór dla systemów wbudowanych. Jest to "komputer w jednej kostce" – układ scalony, który integruje w sobie:
    *   **Procesor (CPU):** Uproszczony, zoptymalizowany pod kątem niskiego poboru mocy.
    *   **Pamięć:** Niewielka ilość pamięci RAM (dla danych tymczasowych) i pamięci Flash lub ROM (dla programu).
    *   **Peryferia:** Zintegrowane interfejsy wejścia/wyjścia (I/O), takie jak porty cyfrowe (GPIO), przetworniki analogowo-cyfrowe (ADC), interfejsy komunikacyjne (UART, I2C, SPI), timery i liczniki.
*   **Pamięć:** Oprócz tej wbudowanej w MCU, system może posiadać zewnętrzną pamięć RAM (dla bardziej złożonych zadań) i pamięć Flash (do przechowywania większych ilości danych).
*   **Urządzenia wejścia/wyjścia (I/O):**
    *   **Czujniki (Sensors):** "Zmysły" systemu, które zbierają dane z otoczenia (np. czujnik temperatury, akcelerometr, czujnik ciśnienia).
    *   **Elementy wykonawcze (Actuators):** "Mięśnie" systemu, które wpływają na otoczenie (np. silnik elektryczny, dioda LED, przekaźnik, zawór).
    *   **Interfejsy komunikacyjne:** Umożliwiają komunikację z innymi systemami (np. moduły Wi-Fi, Bluetooth, CAN, Ethernet).
*   **Zasilanie:** Układ zarządzający energią, kluczowy w urządzeniach bateryjnych.

**2. Oprogramowanie (Software/Firmware):**

Oprogramowanie dla systemu wbudowanego, często nazywane **firmwarem**, jest zapisane w pamięci nieulotnej (Flash/ROM) i jest ściśle dostosowane do konkretnego sprzętu i zadania.

*   **Specyficzne dla aplikacji:** Program wykonuje jedno, dedykowane zadanie w pętli (tzw. *super-loop*) lub w odpowiedzi na przerwania.
*   **System operacyjny czasu rzeczywistego (RTOS - Real-Time Operating System):** W bardziej złożonych systemach stosuje się specjalistyczne systemy operacyjne, które gwarantują wykonanie określonych zadań w ściśle zdefiniowanych ramach czasowych. Jest to kluczowe w systemach, gdzie opóźnienie może mieć katastrofalne skutki (np. system ABS w samochodzie, sterowanie robotem przemysłowym).
*   **Sterowniki urządzeń (Device Drivers):** Niskopoziomowe oprogramowanie pośredniczące między systemem operacyjnym a konkretnymi komponentami sprzętowymi.

#### Kluczowe cechy i ograniczenia systemów wbudowanych

Systemy wbudowane różnią się od komputerów ogólnego przeznaczenia kilkoma fundamentalnymi cechami:

*   **Dedykowane zadanie:** Są zaprojektowane do wykonywania jednej, konkretnej funkcji, co pozwala na wysoką optymalizację.
*   **Niezawodność i stabilność:** Muszą działać nieprzerwanie przez długi czas bez możliwości resetowania (np. rozrusznik serca, systemy w satelicie).
*   **Ograniczenia zasobów:** Działają na sprzęcie o ograniczonej mocy obliczeniowej, małej ilości pamięci i minimalnym poborze mocy.
*   **Wymagania czasu rzeczywistego:** Wiele systemów musi reagować na zdarzenia w ściśle określonym, przewidywalnym czasie (systemy *hard real-time* i *soft real-time*).
*   **Bezpośrednia interakcja ze sprzętem:** Oprogramowanie ma bezpośredni dostęp do portów I/O, czujników i elementów wykonawczych.
*   **Koszt:** Przy produkcji masowej, koszt pojedynczej jednostki jest kluczowym czynnikiem projektowym.

#### Znaczenie i przykłady zastosowań

Znaczenie systemów wbudowanych wynika z ich wszechobecności i roli w automatyzacji niemal każdego aspektu nowoczesnego życia i przemysłu.

| Kategoria | Przykłady zastosowań |
|---|---|
| **Elektronika konsumencka** | Pralki, lodówki, telewizory (Smart TV), routery Wi-Fi, smartwatche, aparaty cyfrowe. |
| **Motoryzacja** | Jednostka sterująca silnikiem (ECU), system ABS, poduszki powietrzne, system inforozrywki, nawigacja GPS. |
| **Przemysł (Automatyka)** | Sterowniki PLC, roboty przemysłowe, systemy monitorowania procesów produkcyjnych, inteligentne czujniki. |
| **Medycyna** | Rozruszniki serca, pompy insulinowe, monitory EKG, sprzęt diagnostyczny (np. tomografy). |
| **Lotnictwo i wojsko** | Systemy awioniki (fly-by-wire), systemy nawigacji i naprowadzania, drony. |
| **Internet Rzeczy (IoT)** | Inteligentne oświetlenie, termostaty, zamki do drzwi, czujniki środowiskowe. |

#### Podsumowanie

*   **System wbudowany** to specjalizowany system komputerowy, będący integralną częścią większego urządzenia i realizujący w nim dedykowaną funkcję.
*   Jego sercem jest zazwyczaj **mikrokontroler (MCU)**, integrujący CPU, pamięć i peryferia w jednym układzie.
*   Systemy te charakteryzują się **wysoką niezawodnością, ograniczeniami zasobów (moc, pamięć, energia)** oraz często **wymaganiami czasu rzeczywistego**.
*   Oprogramowanie (**firmware**) jest ściśle powiązane ze sprzętem; w bardziej złożonych systemach wykorzystuje się **systemy operacyjne czasu rzeczywistego (RTOS)**.
*   Systemy wbudowane są fundamentem **automatyzacji, Internetu Rzeczy (IoT)** i "inteligencji" w urządzeniach codziennego użytku, przemyśle, medycynie i wielu innych dziedzinach.

**Typowe pytania egzaminacyjne:**
*   Co to jest system wbudowany i czym różni się od komputera ogólnego przeznaczenia?
*   Proszę wymienić i opisać podstawowe elementy sprzętowe systemu wbudowanego.
*   Co to jest mikrokontroler i co zazwyczaj wchodzi w jego skład?
*   Jakie są kluczowe cechy i ograniczenia systemów wbudowanych?
*   Proszę podać przykłady zastosowań systemów wbudowanych w co najmniej trzech różnych dziedzinach.

---

# 21. Rola i zadania systemu operacyjnego, podstawowe elementy i rodzaje systemów operacyjnych

#### Wprowadzenie

System operacyjny (OS - Operating System) to fundamentalne oprogramowanie, które działa jako pośrednik między użytkownikiem komputera a jego sprzętem. Bez systemu operacyjnego, komputer byłby jedynie zbiorem bezużytecznych komponentów elektronicznych. OS zarządza wszystkimi zasobami komputera, tworzy środowisko do uruchamiania aplikacji i dostarcza interfejs, za pomocą którego użytkownik może komunikować się z maszyną. Jego nadrzędnym celem jest umożliwienie korzystania z komputera w sposób wygodny i wydajny, ukrywając przed użytkownikiem i programami złożoność operacji sprzętowych.

#### Rola i zadania systemu operacyjnego

System operacyjny pełni dwie główne role: **zarządcy zasobów** i **maszyny wirtualnej**.

**1. Rola zarządcy zasobów (Resource Manager):**

System operacyjny zarządza wszystkimi zasobami sprzętowymi i programowymi komputera, przydzielając je sprawiedliwie i wydajnie między konkurujące ze sobą procesy.

*   **Zarządzanie procesorem (CPU):** Decyduje, który z wielu gotowych do wykonania procesów otrzyma w danym momencie dostęp do procesora. Realizuje to za pomocą **algorytmów szeregowania (scheduling)**, które mają na celu maksymalizację wykorzystania CPU i minimalizację czasu oczekiwania.
*   **Zarządzanie pamięcią operacyjną (RAM):** Przydziela pamięć procesom, które jej potrzebują, i zwalnia ją po ich zakończeniu. Śledzi, które części pamięci są w użyciu i przez kogo. Implementuje mechanizmy **pamięci wirtualnej**, które pozwalają programom używać więcej pamięci, niż jest fizycznie dostępne.
*   **Zarządzanie urządzeniami wejścia/wyjścia (I/O):** Steruje pracą wszystkich urządzeń peryferyjnych (dysk twardy, klawiatura, mysz, drukarka) za pomocą **sterowników (drivers)**. Zarządza dostępem do tych urządzeń i obsługuje komunikację z nimi.
*   **Zarządzanie systemem plików:** Organizuje dane na nośnikach pamięci masowej (dyski twarde, SSD) w postaci hierarchicznej struktury plików i katalogów. Zapewnia mechanizmy do tworzenia, usuwania, odczytu i zapisu plików oraz kontroli dostępu do nich.

**2. Rola maszyny wirtualnej (Virtual Machine / Extended Machine):**

System operacyjny tworzy **abstrakcję** nad surowym sprzętem, prezentując użytkownikowi i programistom uproszczony, spójny i łatwiejszy w użyciu model komputera.

*   **Ukrywanie złożoności sprzętu:** Programista nie musi wiedzieć, jak fizycznie sterować głowicą dysku twardego, aby zapisać plik. Zamiast tego, korzysta z prostych wywołań systemowych, takich jak `open()`, `write()`, `close()`, a system operacyjny tłumaczy je na niskopoziomowe operacje sprzętowe.
*   **Udostępnianie interfejsu:** Dostarcza interfejsu, za pomocą którego użytkownicy i programy mogą wchodzić w interakcje z systemem. Może to być **interfejs wiersza poleceń (CLI - Command Line Interface)** lub **graficzny interfejs użytkownika (GUI - Graphical User Interface)**.

#### Podstawowe elementy systemu operacyjnego

Architektura większości nowoczesnych systemów operacyjnych składa się z kilku kluczowych komponentów:

1.  **Jądro (Kernel):**
    *   **Definicja:** Serce systemu operacyjnego. Jest to część oprogramowania, która działa w najbardziej uprzywilejowanym trybie procesora (tryb jądra) i ma bezpośredni dostęp do całego sprzętu. To właśnie jądro jest odpowiedzialne za realizację wszystkich kluczowych zadań OS, takich jak zarządzanie procesami, pamięcią i urządzeniami I/O.
    *   **Rodzaje jąder:**
        *   **Monolityczne:** Wszystkie podstawowe usługi (zarządzanie procesami, pamięcią, systemem plików, sterowniki) są zintegrowane w jednym, dużym programie. *Przykład: Linux, jądra systemów z rodziny Unix.*
        *   **Mikrojądro:** Jądro zawiera tylko absolutnie niezbędne minimum funkcji (komunikacja międzyprocesowa, podstawowe zarządzanie pamięcią). Pozostałe usługi działają jako osobne procesy w trybie użytkownika. *Przykład: QNX, Minix.*

2.  **Powłoka (Shell):**
    *   **Definicja:** Program, który stanowi podstawowy interfejs między użytkownikiem a jądrem systemu. Odczytuje polecenia od użytkownika i zleca ich wykonanie jądru.
    *   **Rodzaje powłok:**
        *   **Tekstowa (CLI):** Np. `bash` w Linuksie, `cmd.exe` lub `PowerShell` w Windows.
        *   **Graficzna (GUI):** Np. środowisko pulpitu w Windows, GNOME/KDE w Linuksie, Aqua w macOS.

3.  **System plików (File System):**
    *   **Definicja:** Komponent odpowiedzialny za organizację i zarządzanie danymi na nośnikach pamięci masowej. Definiuje, jak pliki są nazywane, przechowywane i strukturyzowane. *Przykłady: NTFS (Windows), ext4 (Linux), APFS (macOS).*

4.  **Wywołania systemowe (System Calls):**
    *   **Definicja:** Specjalny, ściśle zdefiniowany interfejs, za pomocą którego programy działające w trybie użytkownika mogą prosić jądro o wykonanie uprzywilejowanych operacji (np. utworzenie pliku, alokacja pamięci, utworzenie nowego procesu).

#### Rodzaje systemów operacyjnych

Systemy operacyjne można klasyfikować według różnych kryteriów:

*   **Ze względu na liczbę użytkowników i zadań:**
    *   **Jednoużytkownikowe, jednozadaniowe:** Proste systemy, które mogą wykonywać tylko jeden program w danym czasie. *Przykład: MS-DOS.*
    *   **Wielozadaniowe:** Pozwalają jednemu użytkownikowi na uruchomienie wielu programów jednocześnie (współbieżnie). *Przykład: Windows, macOS, Linux.*
    *   **Wieloużytkownikowe:** Pozwalają wielu użytkownikom na jednoczesną pracę na tym samym komputerze, zapewniając im izolację i ochronę zasobów. *Przykład: Systemy serwerowe, takie jak Linux Server, Windows Server.*

*   **Ze względu na zastosowanie:**
    *   **Systemy czasu rzeczywistego (RTOS - Real-Time Operating Systems):** Używane w systemach wbudowanych, gdzie kluczowa jest gwarancja wykonania zadania w ściśle określonym czasie. *Przykład: QNX, FreeRTOS.*
    *   **Systemy dla urządzeń mobilnych:** Zoptymalizowane pod kątem obsługi ekranów dotykowych i oszczędzania energii. *Przykład: Android, iOS.*
    *   **Systemy serwerowe:** Zaprojektowane pod kątem niezawodności, wydajności i obsługi wielu jednoczesnych połączeń sieciowych. *Przykład: Linux (w dystrybucjach serwerowych), Windows Server.*
    *   **Systemy desktopowe:** Przeznaczone dla komputerów osobistych, z naciskiem na wygodny interfejs graficzny. *Przykład: Windows 11, macOS, Ubuntu.*

#### Podsumowanie

*   **System operacyjny** to oprogramowanie zarządzające zasobami komputera i tworzące środowisko do uruchamiania programów.
*   Jego główne **zadania** to zarządzanie procesorem, pamięcią, urządzeniami I/O i systemem plików.
*   Podstawowe **elementy** OS to **jądro** (serce systemu), **powłoka** (interfejs użytkownika) i **system plików**.
*   **Rodzaje systemów operacyjnych** można klasyfikować m.in. ze względu na wielozadaniowość, liczbę użytkowników oraz specyficzne zastosowania (desktopowe, serwerowe, mobilne, czasu rzeczywistego).
*   System operacyjny jest niezbędny do funkcjonowania każdego nowoczesnego komputera, stanowiąc pomost między skomplikowanym sprzętem a potrzebami użytkowników i aplikacji.

**Typowe pytania egzaminacyjne:**
*   Jaka jest rola i jakie są podstawowe zadania systemu operacyjnego?
*   Proszę wymienić i opisać podstawowe elementy składowe systemu operacyjnego.
*   Czym jest jądro systemu operacyjnego i jakie są jego główne funkcje?
*   Proszę wymienić i scharakteryzować co najmniej trzy rodzaje systemów operacyjnych.
*   Na czym polega rola systemu operacyjnego jako zarządcy zasobów?

---

# 22. Pojęcie procesu i wątku, stany procesu/wątku, przełączanie kontekstu, algorytmy szeregowania procesów

#### Wprowadzenie

Wielozadaniowość, czyli zdolność systemu operacyjnego do pozornego, jednoczesnego wykonywania wielu programów, jest fundamentalną cechą nowoczesnych komputerów. U jej podstaw leżą pojęcia **procesu** i **wątku**, które stanowią podstawowe jednostki pracy zarządzane przez system operacyjny. Zrozumienie, czym są procesy i wątki, jak system zarządza ich cyklem życia, jak przełącza się między nimi i na jakiej podstawie decyduje, który z nich ma być w danej chwili wykonywany, jest kluczowe dla zrozumienia wewnętrznych mechanizmów działania każdego współczesnego systemu operacyjnego.

#### Pojęcie procesu i wątku

**Proces (Process):**

*   **Definicja:** Proces to **instancja wykonywanego programu**. Jest to byt dynamiczny, posiadający własne, wydzielone zasoby. Gdy uruchamiamy aplikację (np. przeglądarkę internetową), system operacyjny tworzy dla niej nowy proces.
*   **Zasoby procesu:** Każdy proces posiada swój własny, izolowany zestaw zasobów, w tym:
    *   **Prywatną przestrzeń adresową:** Każdy proces "myśli", że ma do dyspozycji całą pamięć komputera. System operacyjny (dzięki mechanizmom pamięci wirtualnej) zapewnia, że jeden proces nie może bezpośrednio uzyskać dostępu do pamięci innego.
    *   **Deskryptory plików:** Lista otwartych plików i połączeń sieciowych.
    *   **Kontekst wykonawczy:** Stan rejestrów procesora, w tym licznik rozkazów.

**Wątek (Thread):**

*   **Definicja:** Wątek to **podstawowa jednostka wykonania w ramach procesu**. Jest to pojedyncza, sekwencyjna ścieżka wykonywania instrukcji. Każdy proces ma co najmniej jeden wątek (wątek główny). Proces może jednak tworzyć dodatkowe wątki, aby wykonywać kilka zadań równolegle.
*   **Zasoby wątku:** Wątki działające w obrębie tego samego procesu **współdzielą** jego zasoby, w tym przestrzeň adresową i otwarte pliki. Każdy wątek posiada jednak swój własny, niezależny:
    *   **Licznik rozkazów (Program Counter):** Wskazuje, którą instrukcję ma wykonać.
    *   **Zestaw rejestrów:** Przechowuje stan obliczeń danego wątku.
    *   **Stos (Stack):** Przechowuje zmienne lokalne i adresy powrotów z funkcji.

**Kluczowa różnica:** Procesy są od siebie w pełni **izolowane** (ciężkie, "heavyweight"), podczas gdy wątki w ramach jednego procesu **współdzielą zasoby** (lekkie, "lightweight"). Tworzenie nowego wątku jest znacznie "tańsze" (szybsze i mniej zasobożerne) niż tworzenie nowego procesu. Współdzielenie pamięci przez wątki ułatwia komunikację między nimi, ale jednocześnie stwarza ryzyko konfliktów i wymaga stosowania mechanizmów synchronizacji (np. semaforów, mutexów).

#### Stany procesu/wątku

Z perspektywy systemu operacyjnego, każdy proces (lub wątek) znajduje się w jednym z kilku możliwych stanów. Model pięciu stanów jest najczęściej spotykany:

1.  **Nowy (New):** Proces został właśnie utworzony, ale system operacyjny nie przydzielił mu jeszcze żadnych zasobów i nie jest on gotowy do wykonania.
2.  **Gotowy (Ready):** Proces posiada wszystkie niezbędne zasoby do działania (oprócz procesora) i czeka w kolejce na swoją kolej do przydziału czasu CPU.
3.  **Wykonywany (Running):** Proces aktualnie wykonuje swoje instrukcje na procesorze.
4.  **Oczekujący / Zablokowany (Waiting / Blocked):** Proces nie może kontynuować pracy, ponieważ czeka na jakieś zdarzenie, np. na zakończenie operacji wejścia/wyjścia (I/O), na zwolnienie zasobu przez inny proces, lub na sygnał od użytkownika.
5.  **Zakończony (Terminated):** Proces zakończył swoje działanie (normalnie lub w wyniku błędu) i system operacyjny zwalnia jego zasoby.

**Przejścia między stanami:**
*   Nowy -> Gotowy: System dopuszcza proces do wykonania.
*   Gotowy -> Wykonywany: Planista (scheduler) przydziela procesor.
*   Wykonywany -> Gotowy: Procesowi skończył się kwant czasu lub został wywłaszczony przez proces o wyższym priorytecie.
*   Wykonywany -> Oczekujący: Proces zażądał operacji I/O lub czeka na zasób.
*   Oczekujący -> Gotowy: Zdarzenie, na które czekał proces, zaszło.
*   Wykonywany -> Zakończony: Proces zakończył działanie.

#### Przełączanie kontekstu (Context Switching)

Przełączanie kontekstu to mechanizm, który pozwala systemowi operacyjnemu na przerwanie wykonywania jednego procesu i wznowienie wykonywania innego. Jest to operacja kluczowa dla wielozadaniowości z wywłaszczaniem.

**Proces przełączania kontekstu:**
1.  System operacyjny decyduje o zmianie wykonywanego procesu (np. z powodu upłynięcia kwantu czasu).
2.  **Zapisuje kontekst** bieżącego procesu: stan wszystkich rejestrów procesora (w tym licznika rozkazów) jest zapisywany w specjalnej strukturze danych w pamięci jądra, zwanej blokiem kontrolnym procesu (PCB - Process Control Block).
3.  **Wczytuje kontekst** nowego procesu: stan rejestrów dla procesu, który ma teraz być wykonywany, jest ładowany z jego PCB do rejestrów procesora.
4.  Nowy proces wznawia swoje działanie dokładnie od miejsca, w którym został przerwany.

Przełączanie kontekstu jest operacją **kosztowną**, ponieważ jest to czysty narzut – w jej trakcie procesor nie wykonuje żadnej użytecznej pracy. Dlatego systemy operacyjne starają się minimalizować częstotliwość tej operacji.

#### Algorytmy szeregowania procesów (Scheduling Algorithms)

Planista (scheduler) to komponent jądra, który decyduje, który z procesów w stanie "Gotowy" powinien otrzymać procesor. Wybór ten jest dokonywany na podstawie algorytmu szeregowania. Celem tych algorytmów jest m.in. maksymalizacja wykorzystania CPU, maksymalizacja przepustowości (liczby ukończonych procesów) i minimalizacja czasu oczekiwania.

**Podstawowe algorytmy szeregowania:**

1.  **FCFS (First-Come, First-Served) – "Pierwszy w kolejce, pierwszy obsłużony"**
    *   **Zasada:** Procesy są obsługiwane w kolejności, w jakiej zgłosiły się do wykonania. Implementowane za pomocą prostej kolejki FIFO.
    *   **Wady:** Niewywłaszczający. Długi proces może zablokować na długo wszystkie inne, nawet te bardzo krótkie (tzw. efekt konwoju).

2.  **SJF (Shortest Job First) – "Najpierw najkrótsze zadanie"**
    *   **Zasada:** Wybierany jest proces, który ma najkrótszy przewidywany czas wykonania.
    *   **Zalety:** Optymalny pod względem minimalizacji średniego czasu oczekiwania.
    *   **Wady:** Trudno jest dokładnie przewidzieć czas wykonania procesu. Może prowadzić do **głodzenia (starvation)** długich procesów, jeśli ciągle napływają nowe, krótkie zadania.

3.  **Szeregowanie rotacyjne (Round Robin, RR)**
    *   **Zasada:** Każdy proces otrzymuje niewielki, stały **kwant czasu (time slice)** na wykonanie. Jeśli go nie ukończy, jest przerywany (wywłaszczany), przenoszony na koniec kolejki procesów gotowych, a procesor jest przydzielany następnemu procesowi z kolejki.
    *   **Zalety:** Prosty, sprawiedliwy, zapewnia dobrą responsywność w systemach interaktywnych.
    *   **Wady:** Wydajność jest bardzo wrażliwa na długość kwantu czasu – zbyt krótki powoduje duży narzut na przełączanie kontekstu, zbyt długi upodabnia algorytm do FCFS.

4.  **Szeregowanie priorytetowe (Priority Scheduling):**
    *   **Zasada:** Każdy proces ma przypisany priorytet, a procesor jest przydzielany procesowi o najwyższym priorytecie. Może być wywłaszczające lub niewywłaszczające.
    *   **Wady:** Może prowadzić do głodzenia procesów o niskim priorytecie. Rozwiązaniem jest **starzenie (aging)** – stopniowe zwiększanie priorytetu procesów, które długo czekają.

#### Podsumowanie

*   **Proces** to wykonywany program z własnymi, izolowanymi zasobami. **Wątek** to jednostka wykonania w ramach procesu, współdzieląca jego zasoby.
*   Każdy proces przechodzi przez cykl życia, zmieniając swój **stan** (np. gotowy, wykonywany, oczekujący).
*   **Przełączanie kontekstu** to mechanizm pozwalający na zmianę aktualnie wykonywanego procesu, co jest podstawą wielozadaniowości.
*   **Algorytmy szeregowania** (np. FCFS, SJF, Round Robin) są używane przez system operacyjny do decydowania, który proces powinien w danej chwili otrzymać dostęp do CPU.
*   Zarządzanie procesami i wątkami to jedno z najważniejszych i najbardziej złożonych zadań systemu operacyjnego, mające bezpośredni wpływ na wydajność i responsywność całego komputera.

**Typowe pytania egzaminacyjne:**
*   Jaka jest różnica między procesem a wątkiem?
*   Proszę opisać i narysować diagram stanów procesu.
*   Na czym polega i jaki jest koszt przełączania kontekstu?
*   Proszę wymienić i krótko scharakteryzować co najmniej dwa algorytmy szeregowania procesów.
*   Dlaczego algorytm SJF, mimo że jest optymalny, nie jest powszechnie stosowany w praktyce?

---

# 23. Problem wzajemnego wykluczania i jego rozwiązania, synchronizacja procesów i wątków, problem zakleszczenia

#### Wprowadzenie

We współbieżnym świecie systemów operacyjnych, gdzie wiele procesów i wątków działa jednocześnie, pojawia się fundamentalny problem koordynacji ich działań. Gdy dwa lub więcej wątków próbuje w tym samym czasie uzyskać dostęp do współdzielonego zasobu (np. zmiennej w pamięci, pliku, drukarki), może dojść do tzw. **wyścigu (race condition)**, prowadzącego do niespójności danych i nieprzewidywalnych błędów. Aby temu zapobiec, systemy operacyjne muszą dostarczać mechanizmów, które zapewnią uporządkowany dostęp do zasobów. Problemy te – **wzajemne wykluczanie**, **synchronizacja** i potencjalne **zakleszczenie** – stanowią rdzeń zagadnień związanych z programowaniem współbieżnym.

#### Problem wzajemnego wykluczania (Mutual Exclusion)

*   **Sekcja krytyczna (Critical Section):** Jest to fragment kodu programu, w którym proces lub wątek uzyskuje dostęp do współdzielonego zasobu. Może to być modyfikacja globalnej zmiennej, zapis do pliku itp.
*   **Problem wzajemnego wykluczania:** Polega na zapewnieniu, że w danej chwili co najwyżej **jeden** proces/wątek może wykonywać swoją sekcję krytyczną. Jeśli jeden proces znajduje się w swojej sekcji krytycznej, żaden inny proces nie może wejść do swojej (jeśli dotyczy ona tego samego zasobu).

**Rozwiązania problemu wzajemnego wykluczania:**

Rozwiązania muszą spełniać trzy warunki: 1) **Wzajemne wykluczanie** musi być zapewnione. 2) **Postęp** – jeśli żaden proces nie jest w sekcji krytycznej, a pewne procesy chcą do niej wejść, to wybór jednego z nich nie może być odkładany w nieskończoność. 3) **Ograniczone oczekiwanie** – musi istnieć granica liczby wejść innych procesów do sekcji krytycznej, podczas gdy dany proces czeka na swoją kolej.

Podstawowe mechanizmy implementujące wzajemne wykluczanie to:

1.  **Mutex (Mutual Exclusion Object):**
    *   **Definicja:** Najprostszy i najpopularniejszy mechanizm synchronizacyjny. Jest to rodzaj binarnego semafora lub "zamka" (lock), który może znajdować się w jednym z dwóch stanów: **zamknięty** lub **otwarty**.
    *   **Działanie:** Przed wejściem do sekcji krytycznej, wątek próbuje "zamknąć" mutex. Jeśli mu się to uda (mutex był otwarty), wchodzi do sekcji krytycznej. Po jej opuszczeniu, "otwiera" mutex. Jeśli inny wątek spróbuje zamknąć już zamknięty mutex, zostanie zablokowany i przejdzie w stan oczekiwania, aż mutex zostanie zwolniony.

2.  **Semafor (Semaphore):**
    *   **Definicja:** Bardziej ogólny mechanizm synchronizacyjny, wprowadzony przez Edsgera Dijkstrę. Semafor to licznik całkowity, na którym można wykonywać tylko dwie niepodzielne (atomowe) operacje: `wait()` (lub `P`) i `signal()` (lub `V`).
    *   **Działanie:**
        *   `wait(S)`: Jeśli wartość semafora `S` jest większa od zera, dekrementuje ją. Jeśli `S` jest równe zero, proces jest blokowany.
        *   `signal(S)`: Inkrementuje wartość semafora `S`. Jeśli jakieś procesy były zablokowane na tym semaforze, jeden z nich jest odblokowywany.
    *   **Rodzaje:**
        *   **Semafor binarny:** Przyjmuje tylko wartości 0 i 1. Może działać jak mutex.
        *   **Semafor zliczający:** Może przyjmować dowolne wartości nieujemne. Używany do zarządzania dostępem do puli zasobów (np. gdy mamy 5 drukarek, semafor jest inicjalizowany wartością 5).

#### Synchronizacja procesów i wątków

Synchronizacja to pojęcie szersze niż wzajemne wykluczanie. Obejmuje ono wszystkie mechanizmy koordynujące kolejność wykonywania operacji przez różne procesy/wątki. Oprócz zapewnienia wyłącznego dostępu, synchronizacja pozwala na rozwiązywanie bardziej złożonych problemów, takich jak **problem producenta-konsumenta** (jeden wątek produkuje dane, drugi je konsumuje, trzeba zapewnić, by producent nie zapisywał do pełnego bufora, a konsument nie czytał z pustego) czy **problem czytelników i pisarzy**.

Inne mechanizmy synchronizacji to m.in.:

*   **Monitory:** Wysokopoziomowa konstrukcja programistyczna (obecna np. w Javie jako słowo kluczowe `synchronized`), która hermetyzuje dane i procedury operujące na nich, automatycznie zapewniając wzajemne wykluczanie. Wewnątrz monitora mogą istnieć **zmienne warunkowe**, pozwalające wątkom na oczekiwanie na spełnienie określonych warunków.
*   **Bariery:** Mechanizm pozwalający grupie wątków na zatrzymanie się w pewnym punkcie i oczekiwanie, aż wszystkie wątki z tej grupy do niego dotrą, zanim będą mogły kontynuować.

#### Problem zakleszczenia (Deadlock)

Zakleszczenie to najpoważniejszy problem, jaki może wyniknąć z nieprawidłowej synchronizacji. Jest to sytuacja, w której **dwa lub więcej procesów czeka na siebie nawzajem**, blokując się w nieskończoność, ponieważ każdy z nich posiada zasób, którego potrzebuje inny, i jednocześnie czeka na zasób posiadany przez ten inny proces.

**Warunki konieczne do wystąpienia zakleszczenia (Warunki Coffmana):**

Aby doszło do zakleszczenia, muszą być spełnione **jednocześnie** cztery poniższe warunki:

1.  **Wzajemne wykluczanie:** Co najmniej jeden zasób musi być niepodzielny (w danej chwili może go używać tylko jeden proces).
2.  **Trzymanie i oczekiwanie (Hold and Wait):** Proces, który już posiada co najmniej jeden zasób, żąda przydziału kolejnych zasobów, które są aktualnie przydzielone innym procesom.
3.  **Brak wywłaszczania (No Preemption):** Zasób nie może być siłą odebrany procesowi, który go posiada. Może on być zwolniony tylko dobrowolnie przez ten proces.
4.  **Cykliczne oczekiwanie (Circular Wait):** Istnieje zamknięty łańcuch procesów $(P_0, P_1, ..., P_n)$, w którym $P_0$ czeka na zasób trzymany przez $P_1$, $P_1$ czeka na zasób trzymany przez $P_2$, ..., a $P_n$ czeka na zasób trzymany przez $P_0$.

**Metody radzenia sobie z zakleszczeniami:**

*   **Zapobieganie (Prevention):** Projektowanie systemu tak, aby co najmniej jeden z czterech warunków koniecznych nigdy nie mógł zaistnieć (np. przez wymuszenie z góry alokacji wszystkich potrzebnych zasobów lub wprowadzenie globalnego porządku ich pozyskiwania).
*   **Unikanie (Avoidance):** System dynamicznie analizuje stan alokacji zasobów i nie zezwala na przydział, który mógłby w przyszłości doprowadzić do zakleszczenia. Wymaga to posiadania apriorycznej wiedzy o maksymalnym zapotrzebowaniu procesów na zasoby. Klasycznym przykładem jest **algorytm bankiera**.
*   **Wykrywanie i usuwanie (Detection and Recovery):** System pozwala na wystąpienie zakleszczenia, ale okresowo uruchamia algorytm, który je wykrywa (np. przez analizę grafu alokacji zasobów), a następnie je likwiduje, najczęściej przez przymusowe wywłaszczenie zasobów lub zabicie jednego z zakleszczonych procesów.
*   **Ignorowanie:** Najczęstsza metoda stosowana w systemach ogólnego przeznaczenia (Windows, Linux). Zakłada się, że zakleszczenia zdarzają się na tyle rzadko, że koszt implementacji skomplikowanych mechanizmów zapobiegania lub wykrywania jest niewspółmiernie wysoki do korzyści. W razie wystąpienia zakleszczenia, problem jest rozwiązywany ręcznie przez użytkownika lub administratora (np. przez restart systemu lub ubicie procesów).

#### Podsumowanie

*   **Problem wzajemnego wykluczania** polega na zapewnieniu wyłącznego dostępu do współdzielonych zasobów w **sekcjach krytycznych**.
*   Podstawowymi mechanizmami rozwiązującymi ten problem są **mutexy** (zamki) i **semafory**.
*   **Synchronizacja** to szersze pojęcie koordynacji działań współbieżnych procesów, realizowane także przez monitory czy bariery.
*   **Zakleszczenie (deadlock)** to sytuacja, w której grupa procesów blokuje się wzajemnie, czekając na zasoby posiadane przez inne procesy z tej grupy.
*   Do wystąpienia zakleszczenia konieczne jest jednoczesne spełnienie **czterech warunków Coffmana** (wzajemne wykluczanie, trzymanie i oczekiwanie, brak wywłaszczania, cykliczne oczekiwanie).
*   Metody radzenia sobie z zakleszczeniami to **zapobieganie, unikanie, wykrywanie i usuwanie** lub – najczęściej – **ignorowanie** problemu.

**Typowe pytania egzaminacyjne:**
*   Na czym polega problem wzajemnego wykluczania i jakie warunki musi spełniać jego rozwiązanie?
*   Jaka jest różnica między mutexem a semaforem?
*   Proszę wymienić i opisać cztery warunki konieczne do wystąpienia zakleszczenia.
*   Jakie są strategie radzenia sobie z problemem zakleszczeń w systemach operacyjnych?
*   Co to jest sekcja krytyczna i dlaczego dostęp do niej musi być kontrolowany?

---

# 24. Zarządzanie pamięcią operacyjną, pojęcie pamięci wirtualnej, segmentacja i stronicowanie pamięci

#### Wprowadzenie

Zarządzanie pamięcią operacyjną (RAM) jest jednym z najbardziej fundamentalnych i złożonych zadań systemu operacyjnego. Polega ono na efektywnym przydzielaniu tego ograniczonego zasobu pomiędzy wiele konkurujących ze sobą procesów. Celem jest nie tylko zapewnienie każdemu procesowi niezbędnej przestrzeni do działania, ale także ochrona pamięci jednego procesu przed dostępem ze strony innego oraz umożliwienie współdzielenia danych. Aby sprostać tym wyzwaniom, nowoczesne systemy operacyjne wykorzystują zaawansowaną technikę zwaną **pamięcią wirtualną**, która jest najczęściej implementowana za pomocą **stronicowania** i (historycznie lub w połączeniu) **segmentacji**.

#### Zarządzanie pamięcią operacyjną

Podstawowe zadania modułu zarządzania pamięcią w systemie operacyjnym to:

*   **Śledzenie wykorzystania pamięci:** System musi wiedzieć, które fragmenty pamięci są wolne, a które zajęte i przez jaki proces.
*   **Alokacja i dealokacja:** Przydzielanie pamięci procesom, gdy o nią proszą, i zwalnianie jej (czynienie dostępną dla innych), gdy proces kończy działanie.
*   **Ochrona pamięci:** Zapewnienie, że proces może uzyskać dostęp tylko do własnej, przydzielonej mu przestrzeni adresowej, a próba odwołania się do pamięci innego procesu zostanie zablokowana.
*   **Translacja adresów:** Przekształcanie adresów logicznych, generowanych przez program, na adresy fizyczne w pamięci RAM.

#### Pamięć wirtualna (Virtual Memory)

**Pojęcie:** Pamięć wirtualna to potężna technika abstrakcji, która daje każdemu procesowi iluzję posiadania własnej, prywatnej i ciągłej przestrzeni adresowej (tzw. **wirtualnej przestrzeni adresowej**), zaczynającej się od zera. W rzeczywistości, pamięć ta jest fragmentarycznie i nieciągle rozmieszczona w fizycznej pamięci RAM, a jej część może być tymczasowo przechowywana na dysku twardym w tzw. **pliku wymiany (swap file)** lub partycji wymiany.

**Kluczowe korzyści z pamięci wirtualnej:**

1.  **Izolacja procesów:** Każdy proces działa we własnej, odseparowanej przestrzeni adresowej, co zapewnia ochronę i bezpieczeństwo. Proces A nie może "zobaczyć" ani zmodyfikować pamięci procesu B.
2.  **Większa przestrzeń adresowa niż fizyczna pamięć RAM:** Program może operować na znacznie większej ilości danych, niż mieści się w fizycznej pamięci RAM. Części programu i dane, które nie są aktualnie używane, mogą być przechowywane na dysku i ładowane do RAM tylko wtedy, gdy są potrzebne.
3.  **Efektywne współdzielenie pamięci:** Różne procesy mogą łatwo współdzielić te same biblioteki lub dane, mapując je do swoich wirtualnych przestrzeni adresowych. Fizycznie, dana biblioteka istnieje w pamięci RAM tylko w jednej kopii.

Mechanizm pamięci wirtualnej jest realizowany sprzętowo przez **jednostkę zarządzania pamięcią (MMU - Memory Management Unit)**, która jest częścią procesora. MMU w locie tłumaczy każdy adres wirtualny generowany przez CPU na odpowiadający mu adres fizyczny w RAM.

#### Segmentacja i stronicowanie pamięci

Segmentacja i stronicowanie to dwie główne techniki implementacji pamięci wirtualnej.

**1. Segmentacja (Segmentation):**

*   **Koncepcja:** Wirtualna przestrzeń adresowa procesu jest dzielona na logiczne, spójne bloki o **zmiennej długości**, zwane **segmentami**. Każdy segment odpowiada logicznej części programu, np. segment kodu, segment danych, segment stosu.
*   **Adresowanie:** Adres wirtualny składa się z dwóch części: **numeru segmentu** i **przesunięcia (offsetu)** wewnątrz tego segmentu.
*   **Translacja:** MMU używa **tablicy segmentów (segment table)**, aby znaleźć adres bazowy i rozmiar danego segmentu w pamięci fizycznej, a następnie dodaje do niego przesunięcie.
*   **Zalety:** Logiczny podział, łatwość implementacji ochrony (np. segment kodu można oznaczyć jako tylko do odczytu).
*   **Wady:** Prowadzi do **fragmentacji zewnętrznej**. Po pewnym czasie działania systemu, w pamięci fizycznej powstaje wiele małych, nieciągłych, wolnych bloków, które są zbyt małe, aby pomieścić nowy, duży segment, mimo że ich łączna suma mogłaby być wystarczająca.

**2. Stronicowanie (Paging):**

*   **Koncepcja:** Pamięć fizyczna jest dzielona na bloki o **stałym, niewielkim rozmiarze**, zwane **ramkami (frames)**. Wirtualna przestrzeń adresowa procesu jest również dzielona na bloki o tej samej wielkości, zwane **stronami (pages)**.
*   **Adresowanie:** Adres wirtualny składa się z dwóch części: **numeru strony** i **przesunięcia (offsetu)** wewnątrz tej strony.
*   **Translacja:** MMU używa **tablicy stron (page table)** dla każdego procesu. Tablica ta mapuje numer strony wirtualnej na numer ramki w pamięci fizycznej. Numer ramki jest następnie łączony z przesunięciem, tworząc adres fizyczny.
*   **Zalety:** Eliminuje problem fragmentacji zewnętrznej. Każda wolna ramka może być użyta do przechowania dowolnej strony. Ułatwia implementację mechanizmu wymiany stron z dyskiem.
*   **Wady:** Powoduje **fragmentację wewnętrzną** (jeśli ostatnia strona programu nie jest w pełni wykorzystana, pozostała część ramki jest marnowana). Tablice stron mogą być bardzo duże.

**Błąd strony (Page Fault):**

Jest to kluczowy mechanizm stronicowania na żądanie. Gdy proces próbuje odwołać się do strony, której nie ma aktualnie w pamięci RAM (jest na dysku), MMU generuje przerwanie zwane **błędem strony**. System operacyjny przejmuje kontrolę, odnajduje brakującą stronę na dysku, wczytuje ją do wolnej ramki w RAM, aktualizuje tablicę stron i wznawia przerwany proces.

**Segmentacja ze stronicowaniem:**

Nowoczesne systemy (jak te oparte na architekturze x86-64) łączą obie techniki. Przestrzeń adresowa jest najpierw dzielona na logiczne segmenty, a następnie każdy segment jest stronicowany. Daje to korzyści obu podejść: logiczną organizację segmentacji i elastyczność zarządzania pamięcią stronicowania.

#### Porównanie segmentacji i stronicowania

| Cecha | Segmentacja | Stronicowanie |
|---|---|---|
| **Podział pamięci** | Bloki o zmiennej długości (segmenty) | Bloki o stałej wielkości (strony/ramki) |
| **Logika podziału** | Zorientowana na użytkownika/programistę (kod, dane, stos) | Niewidoczna dla programisty, narzucona przez sprzęt |
| **Rozmiar** | Różne rozmiary segmentów | Jednolity rozmiar stron i ramek |
| **Fragmentacja** | Zewnętrzna (trudna do zarządzania) | Wewnętrzna (łatwiejsza do opanowania) |
| **Struktury danych** | Tablica segmentów | Tablica stron |

#### Podsumowanie

*   **Zarządzanie pamięcią** to kluczowe zadanie OS, obejmujące alokację, ochronę i translację adresów.
*   **Pamięć wirtualna** to abstrakcja, która daje każdemu procesowi iluzję posiadania własnej, dużej i ciągłej przestrzeni adresowej, zapewniając izolację i umożliwiając uruchamianie programów większych niż fizyczna pamięć RAM.
*   Mechanizm ten jest realizowany sprzętowo przez **MMU**.
*   **Segmentacja** dzieli pamięć na logiczne bloki o zmiennej długości, co prowadzi do fragmentacji zewnętrznej.
*   **Stronicowanie** dzieli pamięć na fizyczne bloki o stałej wielkości, eliminując fragmentację zewnętrzną kosztem niewielkiej fragmentacji wewnętrznej. Jest to dominująca technika w nowoczesnych systemach operacyjnych.
*   **Błąd strony (page fault)** to mechanizm umożliwiający ładowanie danych z dysku do pamięci RAM na żądanie.

**Typowe pytania egzaminacyjne:**
*   Na czym polega zarządzanie pamięcią i jakie są jego główne zadania?
*   Co to jest pamięć wirtualna i jakie są jej główne zalety?
*   Proszę porównać mechanizmy segmentacji i stronicowania, wskazując ich wady i zalety.
*   Co to jest błąd strony (page fault) i jak jest obsługiwany przez system operacyjny?
*   Czym jest fragmentacja zewnętrzna i wewnętrzna?

---

# 25. System plików, organizacja i implementacja, metody dostępu do plików

#### Wprowadzenie

System plików to jeden z najważniejszych i najbardziej widocznych dla użytkownika komponentów systemu operacyjnego. Odpowiada on za organizację, przechowywanie i zarządzanie danymi na nośnikach pamięci masowej (takich jak dyski twarde, dyski SSD, pendrive'y). System plików tworzy logiczną abstrakcję nad fizycznym, blokowym charakterem nośnika, prezentując dane w postaci hierarchicznej struktury plików i katalogów. Dzięki niemu użytkownicy i programy mogą w prosty i ustandaryzowany sposób tworzyć, odczytywać, modyfikować i usuwać dane, nie martwiąc się o niskopoziomowe szczegóły ich fizycznego rozmieszczenia na dysku.

#### Organizacja systemu plików

System plików ma dwojaką strukturę: logiczną (widoczną dla użytkownika) i fizyczną (sposób zapisu na nośniku).

**1. Logiczna organizacja:**

*   **Plik (File):** Podstawowa, nazwana jednostka przechowywania informacji. Z perspektywy systemu operacyjnego, plik to ciąg bajtów. To, jak te bajty są interpretowane (jako tekst, obraz, program), zależy od aplikacji.
*   **Atrybuty pliku:** Każdy plik posiada zbiór metadanych, które go opisują, np.: nazwa, typ, rozmiar, data utworzenia, data modyfikacji, właściciel, uprawnienia dostępu (odczyt, zapis, wykonanie).
*   **Katalog (Directory / Folder):** Specjalny rodzaj pliku, który służy do grupowania innych plików i katalogów. Katalogi tworzą **hierarchiczną, drzewiastą strukturę**, która pozwala na logiczne uporządkowanie danych. Główny katalog w tej strukturze to **katalog główny (root directory)**.
*   **Ścieżka (Path):** Unikalny adres pliku lub katalogu w hierarchii systemu plików. Może być **absolutna** (zaczynająca się od katalogu głównego, np. `/home/user/document.txt`) lub **względna** (względem bieżącego katalogu roboczego, np. `../images/photo.jpg`).

**2. Fizyczna organizacja:**

Nośnik danych (dysk) jest dzielony na **bloki** o stałym rozmiarze (np. 4 KB). System plików zarządza tymi blokami, decydując, które z nich przechowują dane konkretnych plików, a które są wolne.

#### Implementacja systemu plików

Implementacja systemu plików obejmuje struktury danych na dysku, które pozwalają zarządzać plikami, katalogami i wolną przestrzenią.

**1. Struktury na dysku:**

*   **Boot Block (Sektor rozruchowy):** Pierwszy blok partycji, zawierający informacje niezbędne do uruchomienia systemu operacyjnego z tej partycji.
*   **Superblok (Superblock):** Zawiera kluczowe metadane o całym systemie plików: jego typ, rozmiar, liczbę bloków, wskaźniki do innych kluczowych struktur.
*   **Mapa wolnych bloków (Free-space map):** Struktura danych (najczęściej mapa bitowa), która śledzi, które bloki na dysku są wolne, a które zajęte.
*   **Struktury opisujące pliki:** Sposób przechowywania metadanych plików i wskaźników do bloków z danymi. Najważniejsze podejścia to:
    *   **Tablica alokacji plików (FAT - File Allocation Table):** Używana w systemach FAT16/FAT32. Jest to tablica, w której każdy wpis odpowiada jednemu blokowi na dysku. Wpisy te tworzą **łańcuchy (listy powiązane)**, wskazując na kolejne bloki należące do danego pliku. Metadane pliku (nazwa, rozmiar) są przechowywane osobno, w strukturze katalogu.
    *   **I-węzeł (inode - index node):** Używana w systemach uniksowych (np. ext4, UFS). I-węzeł to struktura danych przechowująca **wszystkie metadane pliku** (rozmiar, uprawnienia, daty) oraz **wskaźniki do bloków z danymi**. W katalogu przechowywana jest tylko nazwa pliku i numer odpowiadającego mu i-węzła. To podejście oddziela nazwę pliku od jego metadanych.

**2. Metody alokacji plików na dysku:**

System plików musi decydować, jak przydzielać bloki dyskowe dla plików. Istnieją trzy główne strategie:

*   **Alokacja ciągła (Contiguous Allocation):** Plik zajmuje ciągły zestaw bloków na dysku. Dostęp jest bardzo szybki, ale metoda ta cierpi na **fragmentację zewnętrzną** i wymaga znajomości rozmiaru pliku z góry.
*   **Alokacja listowa / łańcuchowa (Linked Allocation):** Bloki pliku są rozproszone po dysku, a każdy blok zawiera wskaźnik do następnego bloku. Eliminuje fragmentację zewnętrzną, ale uniemożliwia szybki dostęp swobodny (aby dostać się do n-tego bloku, trzeba przejść przez n-1 poprzednich). Implementacją tej metody jest system FAT.
*   **Alokacja indeksowa (Indexed Allocation):** Dla każdego pliku tworzony jest specjalny **blok indeksowy** (lub i-węzeł), który zawiera listę wskaźników do wszystkich bloków danych tego pliku. Umożliwia szybki dostęp swobodny i eliminuje fragmentację zewnętrzną. Jest to najpopularniejsza metoda, stosowana w systemach opartych na i-węzłach.

#### Metody dostępu do plików

System operacyjny udostępnia programom różne sposoby odczytywania i zapisywania danych w plikach.

1.  **Dostęp sekwencyjny (Sequential Access):**
    *   **Opis:** Najprostsza i najczęstsza metoda. Dane są przetwarzane w porządku, jeden bajt (lub rekord) po drugim, od początku do końca. System utrzymuje wskaźnik na bieżącą pozycję w pliku, który przesuwa się po każdej operacji odczytu/zapisu.
    *   **Przykład:** Odczyt pliku tekstowego, odtwarzanie pliku muzycznego.

2.  **Dostęp swobodny / bezpośredni (Direct / Random Access):**
    *   **Opis:** Umożliwia odczyt lub zapis danych w dowolnym miejscu pliku, bez konieczności przetwarzania danych poprzedzających. Program może natychmiast "przeskoczyć" do dowolnego bloku lub bajtu pliku.
    *   **Przykład:** Operacje na plikach baz danych, gdzie konieczny jest szybki dostęp do konkretnego rekordu.

3.  **Dostęp indeksowany (Indexed Access):**
    *   **Opis:** Bardziej złożona metoda, oparta na dostępie swobodnym. Plik zawiera indeks (spis treści), który pozwala na szybkie wyszukanie rekordu na podstawie jego klucza, a następnie odczytanie go za pomocą dostępu swobodnego.
    *   **Przykład:** Systemy zarządzania bazami danych (DBMS) często implementują własne, zaawansowane metody dostępu indeksowanego na poziomie aplikacji.

#### Podsumowanie

*   **System plików** to mechanizm OS do organizacji danych na nośnikach masowych, tworzący abstrakcję w postaci **plików i katalogów**.
*   **Organizacja logiczna** opiera się na hierarchicznej strukturze katalogów, a **fizyczna** na zarządzaniu blokami dyskowymi.
*   **Implementacja** systemu plików obejmuje struktury takie jak **FAT** lub **i-węzły (inode)**, które mapują pliki na bloki dyskowe, oraz metody alokacji (ciągła, listowa, **indeksowa**).
*   System operacyjny udostępnia dwie podstawowe **metody dostępu** do danych w plikach: **sekwencyjny** (jeden po drugim) i **swobodny** (bezpośredni dostęp do dowolnej lokalizacji).
*   Wybór konkretnego systemu plików (np. NTFS, ext4, APFS) ma duży wpływ na wydajność, niezawodność i funkcjonalność (np. obsługę uprawnień, księgowanie) operacji plikowych.

**Typowe pytania egzaminacyjne:**
*   Jaka jest rola i jakie są zadania systemu plików?
*   Proszę opisać różnicę między logiczną a fizyczną organizacją systemu plików.
*   Na czym polega metoda alokacji indeksowej i jakie ma zalety w porównaniu do alokacji ciągłej i listowej?
*   Czym jest i-węzeł (inode) i jakie informacje przechowuje?
*   Proszę porównać metody dostępu sekwencyjnego i swobodnego do plików.

---

# 26. Model warstwowy ISO/OSI i TCP/IP, protokoły i ich rola w komunikacji sieciowej

#### Wprowadzenie

Komunikacja w sieciach komputerowych jest niezwykle złożonym procesem, obejmującym zagadnienia od fizycznego przesyłania bitów przez kabel po interpretację danych przez aplikację użytkownika. Aby uporać się z tą złożonością, stosuje się **modele warstwowe**, które dzielą cały proces komunikacji na mniejsze, zarządzalne i ustandaryzowane części, zwane **warstwami**. Każda warstwa odpowiada za realizację określonego zadania i świadczy usługi dla warstwy wyższej, korzystając jednocześnie z usług warstwy niższej. Dwa najważniejsze modele warstwowe w historii sieci komputerowych to teoretyczny **model odniesienia ISO/OSI** oraz praktyczny **model TCP/IP**, na którym opiera się dzisiejszy Internet.

#### Model warstwowy ISO/OSI

Model OSI (Open Systems Interconnection), opracowany przez Międzynarodową Organizację Normalizacyjną (ISO), jest **modelem referencyjnym (teoretycznym)**, który miał na celu standaryzację protokołów sieciowych. Składa się on z siedmiu warstw.

1.  **Warstwa 7: Aplikacji (Application Layer):** Najbliższa użytkownikowi. Zapewnia interfejs między aplikacjami a siecią. *Protokoły: HTTP, FTP, SMTP, DNS.*
2.  **Warstwa 6: Prezentacji (Presentation Layer):** Odpowiada za translację, kompresję i szyfrowanie danych, zapewniając, że dane wysłane z jednego systemu będą czytelne dla systemu docelowego. Dba o jednolitą reprezentację danych.
3.  **Warstwa 5: Sesji (Session Layer):** Zarządza sesjami komunikacyjnymi między aplikacjami. Odpowiada za otwieranie, zamykanie i synchronizację dialogu między hostami.
4.  **Warstwa 4: Transportu (Transport Layer):** Zapewnia niezawodną lub nieniezawodną komunikację między **procesami** na różnych hostach. Segmentuje dane i zarządza kontrolą przepływu i retransmisją. *Protokoły: TCP, UDP.*
5.  **Warstwa 3: Sieci (Network Layer):** Odpowiada za logiczne adresowanie (adresy IP) i **routing (wyznaczanie trasy)** pakietów przez sieć. Jej zadaniem jest dostarczenie pakietu od hosta źródłowego do docelowego. *Protokoły: IP, ICMP.*
6.  **Warstwa 2: Łącza danych (Data Link Layer):** Odpowiada za niezawodne przesyłanie danych w ramach jednego segmentu sieci lokalnej (LAN). Zarządza fizycznym adresowaniem (adresy MAC), wykrywaniem i korekcją błędów. *Protokoły: Ethernet, PPP.*
7.  **Warstwa 1: Fizyczna (Physical Layer):** Odpowiada za fizyczne przesyłanie strumienia bitów przez medium transmisyjne (np. kabel miedziany, światłowód, fale radiowe). Definiuje parametry elektryczne i mechaniczne.

#### Model TCP/IP

Model TCP/IP (Transmission Control Protocol/Internet Protocol) jest **modelem praktycznym**, który został faktycznie zaimplementowany i na którym działa cały Internet. Jest prostszy i składa się z czterech warstw.

1.  **Warstwa 4: Aplikacji (Application Layer):** Odpowiada warstwom Aplikacji, Prezentacji i Sesji z modelu OSI. Obsługuje konkretne protokoły sieciowe używane przez aplikacje. *Protokoły: HTTP, FTP, SMTP, DNS.*
2.  **Warstwa 3: Transportu (Transport Layer):** Odpowiednik warstwy Transportu z modelu OSI. Zapewnia komunikację między procesami. *Protokoły: TCP, UDP.*
3.  **Warstwa 2: Internetu (Internet Layer):** Odpowiednik warstwy Sieci z modelu OSI. Odpowiada za adresowanie i routing pakietów. *Protokół: IP.*
4.  **Warstwa 1: Dostępu do sieci (Network Access Layer):** Odpowiednik warstw Łącza danych i Fizycznej z modelu OSI. Odpowiada za przesyłanie danych w sieci lokalnej i interakcję z fizycznym medium.

| Model ISO/OSI | Model TCP/IP |
|---|---|
| 7. Aplikacji | 4. Aplikacji |
| 6. Prezentacji | |
| 5. Sesji | |
| 4. Transportu | 3. Transportu |
| 3. Sieci | 2. Internetu |
| 2. Łącza danych | 1. Dostępu do sieci |
| 1. Fizyczna | |

#### Rola protokołów i proces enkapsulacji

**Protokół sieciowy** to formalny zbiór reguł i konwencji, które określają, jak urządzenia w sieci mają się ze sobą komunikować. Definiuje on format, kolejność i znaczenie przesyłanych wiadomości. Każda warstwa w modelu komunikuje się ze swoim odpowiednikiem na drugim urządzeniu za pomocą właściwego dla niej protokołu.

**Enkapsulacja (hermetyzacja):**

Jest to kluczowy proces w komunikacji warstwowej. Gdy dane przemieszczają się w dół stosu protokołów (od warstwy aplikacji do fizycznej) na urządzeniu wysyłającym, każda warstwa dodaje do danych swój własny **nagłówek** (a czasem i stopkę), zawierający informacje sterujące potrzebne do realizacji jej zadań. Proces ten można porównać do wkładania listu do koperty, a następnie tej koperty do większej paczki.

1.  Dane z aplikacji trafiają do **warstwy transportu**, która dzieli je na **segmenty** i dodaje nagłówek TCP lub UDP (zawierający m.in. porty źródłowy i docelowy).
2.  Segment jest przekazywany do **warstwy sieci**, która dodaje nagłówek IP (zawierający m.in. adresy IP źródłowy i docelowy), tworząc **pakiet**.
3.  Pakiet trafia do **warstwy łącza danych**, która dodaje swój nagłówek i stopkę (zawierające m.in. adresy MAC), tworząc **ramkę**.
4.  Ramka jest konwertowana na strumień bitów i wysyłana przez **warstwę fizyczną**.

Na urządzeniu odbierającym zachodzi proces odwrotny – **dekapsulacja**. Każda warstwa odczytuje i usuwa swój nagłówek, interpretuje zawarte w nim informacje i przekazuje pozostałe dane do warstwy wyższej.

#### Przykład: Wyświetlanie strony WWW

1.  **Warstwa aplikacji:** Przeglądarka (klient HTTP) chce pobrać stronę. Tworzy żądanie HTTP GET i przekazuje je w dół.
2.  **Warstwa transportu:** System operacyjny tworzy segment TCP. Do żądania HTTP dodawany jest nagłówek TCP z portem docelowym 80 (standard dla HTTP) i losowym portem źródłowym.
3.  **Warstwa sieci:** Do segmentu TCP dodawany jest nagłówek IP z adresem IP twojego komputera (źródłowym) i adresem IP serwera WWW (docelowym), tworząc pakiet.
4.  **Warstwa łącza danych:** Do pakietu IP dodawany jest nagłówek Ethernet z adresem MAC twojej karty sieciowej (źródłowym) i adresem MAC routera (docelowym), tworząc ramkę.
5.  **Warstwa fizyczna:** Ramka jest wysyłana jako sygnał elektryczny przez kabel sieciowy.

Na serwerze WWW proces dekapsulacji przebiega w odwrotnej kolejności, aż serwer HTTP otrzyma czyste żądanie GET i będzie mógł na nie odpowiedzieć.

#### Podsumowanie

*   **Modele warstwowe (ISO/OSI, TCP/IP)** dzielą złożony proces komunikacji sieciowej na zarządzalne, ustandaryzowane warstwy.
*   **Model ISO/OSI** jest 7-warstwowym modelem teoretycznym, a **model TCP/IP** jest 4-warstwowym modelem praktycznym, na którym opiera się Internet.
*   **Protokół sieciowy** to zbiór reguł komunikacji dla danej warstwy.
*   **Enkapsulacja** to proces dodawania nagłówków przez kolejne warstwy stosu protokołów podczas wysyłania danych.
*   Dzięki podejściu warstwowemu, zmiana implementacji w jednej warstwie (np. wymiana kabla miedzianego na światłowód w warstwie fizycznej) nie wpływa na działanie pozostałych warstw, co zapewnia elastyczność i łatwość rozwoju technologii sieciowych.

**Typowe pytania egzaminacyjne:**
*   Jaki jest cel stosowania modeli warstwowych w sieciach komputerowych?
*   Proszę porównać model ISO/OSI i TCP/IP, wymieniając warstwy każdego z nich.
*   Na czym polega proces enkapsulacji danych? Proszę opisać go na przykładzie.
*   Jakie są zadania warstwy transportu i warstwy sieci w modelu OSI?
*   Co to jest protokół sieciowy i jaką pełni rolę?

---

# 27. Adresacja w sieciach komputerowych: adresy fizyczne, logiczne i porty, rola i zadania protokołów ARP, DNS, DHCP

#### Wprowadzenie

Aby komunikacja w sieci komputerowej była możliwa, każde urządzenie i każda usługa muszą posiadać unikalny identyfikator. System adresacji w sieciach jest wielopoziomowy i analogiczny do systemu pocztowego: potrzebujemy zarówno ogólnego adresu (jak adres zamieszkania), aby dostarczyć przesyłkę do właściwego budynku, jak i bardziej szczegółowego identyfikatora (jak numer mieszkania lub imię i nazwisko), aby trafiła ona do konkretnej osoby. W sieciach komputerowych tę rolę pełnią adresy fizyczne (MAC), adresy logiczne (IP) i numery portów, a ich prawidłowe działanie i wzajemne powiązanie jest zarządzane przez kluczowe protokoły pomocnicze: ARP, DNS i DHCP.

#### Poziomy adresacji

**1. Adresy fizyczne (MAC - Media Access Control)**

*   **Warstwa:** 2 (Łącza danych).
*   **Definicja:** Unikalny, 48-bitowy identyfikator, "wypalony" na stałe w karcie sieciowej (NIC) przez jej producenta. Jest to adres sprzętowy.
*   **Format:** Zazwyczaj zapisywany jako 12 cyfr szesnastkowych, podzielonych na 6 par (np. `00:1A:2B:3C:4D:5E`). Pierwsze 6 cyfr identyfikuje producenta karty.
*   **Rola:** Używany do adresowania i dostarczania **ramek** w obrębie **jednej sieci lokalnej (LAN)**. Przełączniki (switche) sieciowe używają adresów MAC do przesyłania danych między urządzeniami w tej samej sieci.
*   **Ograniczenie:** Adres MAC jest adresem lokalnym i nie jest używany do przesyłania danych między różnymi sieciami (nie jest "rutowalny").

**2. Adresy logiczne (IP - Internet Protocol)**

*   **Warstwa:** 3 (Sieci).
*   **Definicja:** 32-bitowy (w wersji IPv4) lub 128-bitowy (w wersji IPv6) adres, który jednoznacznie identyfikuje urządzenie w globalnej sieci Internet. Jest to adres logiczny, co oznacza, że jest konfigurowalny i może się zmieniać (np. po podłączeniu do innej sieci).
*   **Format (IPv4):** Zapisywany jako 4 liczby dziesiętne oddzielone kropkami, gdzie każda liczba reprezentuje 8 bitów (oktet) i przyjmuje wartość od 0 do 255 (np. `192.168.1.101`).
*   **Rola:** Używany do adresowania i dostarczania **pakietów** między hostami w **różnych sieciach**. Routery używają adresów IP do wyznaczania najlepszej trasy dla pakietów w Internecie.

**3. Porty (Ports)**

*   **Warstwa:** 4 (Transportu).
*   **Definicja:** 16-bitowy numer (od 0 do 65535), który identyfikuje konkretny **proces lub usługę** działającą na danym hoście. Nie jest to adres fizyczny, lecz logiczny punkt końcowy komunikacji.
*   **Rola:** Pozwala jednemu komputerowi (o jednym adresie IP) na jednoczesne prowadzenie wielu rozmów sieciowych. Gdy dane docierają do komputera, adres IP kieruje je do właściwej maszyny, a numer portu kieruje je do właściwej aplikacji (np. port 80 dla serwera WWW, port 25 dla serwera poczty SMTP).
*   **Analogia:** Adres IP to adres budynku, a numer portu to numer mieszkania w tym budynku.

#### Kluczowe protokoły pomocnicze

Te trzy poziomy adresacji muszą ze sobą współpracować. Służą do tego specjalne protokoły, które działają w tle, automatyzując procesy konfiguracyjne i translacji adresów.

**1. ARP (Address Resolution Protocol) – Protokół Rozpoznawania Adresów**

*   **Problem do rozwiązania:** Jak wysłać dane do komputera w tej samej sieci lokalnej, znając tylko jego adres IP? Do zbudowania ramki w warstwie 2 potrzebny jest docelowy adres MAC.
*   **Rola i działanie:** ARP tłumaczy **adresy IP na adresy MAC** w sieci lokalnej. Gdy host A chce wysłać pakiet do hosta B (w tej samej sieci LAN), a zna tylko jego adres IP, wysyła w sieć rozgłoszenie (broadcast) ARP z pytaniem: "Kto ma adres IP `192.168.1.101`? Proszę o podanie swojego adresu MAC". Host B, rozpoznając swój adres IP, odpowiada komunikatem ARP zawierającym jego adres MAC. Host A zapisuje to mapowanie (IP -> MAC) w swojej lokalnej **tablicy ARP (ARP cache)**, aby nie musieć powtarzać tego procesu przy kolejnych pakietach.

**2. DHCP (Dynamic Host Configuration Protocol) – Protokół Dynamicznej Konfiguracji Hosta**

*   **Problem do rozwiązania:** Ręczna konfiguracja adresów IP, masek podsieci i bram domyślnych na każdym urządzeniu w sieci jest niepraktyczna i podatna na błędy.
*   **Rola i działanie:** DHCP automatyzuje proces konfiguracji sieciowej. Gdy nowe urządzenie podłącza się do sieci, wysyła ono rozgłoszenie DHCP z prośbą o przydzielenie adresu IP. **Serwer DHCP** (zazwyczaj działający na routerze) odbiera to żądanie i przydziela urządzeniu na określony czas (dzierżawa) wolny adres IP ze swojej puli, a także przekazuje mu inne niezbędne informacje, takie jak adres maski podsieci, adres bramy domyślnej i adresy serwerów DNS.

**3. DNS (Domain Name System) – System Nazw Domenowych**

*   **Problem do rozwiązania:** Ludziom trudno jest zapamiętywać numeryczne adresy IP (np. `216.58.214.206`). Znacznie łatwiej jest posługiwać się zrozumiałymi nazwami (np. `www.google.com`).
*   **Rola i działanie:** DNS to rozproszona, hierarchiczna baza danych, która tłumaczy **czytelne dla człowieka nazwy domenowe na adresy IP**. Gdy wpisujesz w przeglądarce adres `www.google.com`, twój komputer wysyła zapytanie do serwera DNS. Serwer DNS odnajduje w swojej bazie (lub pyta o to inne serwery) odpowiedni adres IP i zwraca go do twojego komputera. Dopiero wtedy przeglądarka może nawiązać połączenie z serwerem Google, używając uzyskanego adresu IP.

#### Podsumowanie

*   Komunikacja sieciowa opiera się na trójpoziomowym systemie adresacji:
    *   **Adresy MAC** (warstwa 2) do komunikacji w sieci lokalnej.
    *   **Adresy IP** (warstwa 3) do komunikacji między sieciami.
    *   **Porty** (warstwa 4) do identyfikacji konkretnych aplikacji na hoście.
*   Trzy kluczowe protokoły pomocnicze automatyzują działanie sieci:
    *   **DHCP** automatycznie przydziela adresy IP i konfigurację sieciową.
    *   **DNS** tłumaczy nazwy domenowe (np. `google.com`) na adresy IP.
    *   **ARP** tłumaczy adresy IP na adresy MAC w sieci lokalnej.
*   Współdziałanie tych mechanizmów sprawia, że korzystanie z sieci jest dla użytkownika proste i intuicyjne, mimo ogromnej złożoności procesów zachodzących "pod spodem".

**Typowe pytania egzaminacyjne:**
*   Proszę opisać trzy poziomy adresacji w sieciach komputerowych (MAC, IP, port) i wskazać, w której warstwie modelu OSI każdy z nich operuje.
*   Jaka jest rola i zasada działania protokołu ARP?
*   Do czego służy protokół DHCP?
*   Na czym polega działanie systemu DNS?
*   Jaka jest różnica między adresem fizycznym a logicznym?

---

# 28. Podstawowe urządzenia sieciowe i ich rola w przesyle danych: koncentrator, przełącznik, router

#### Wprowadzenie

Sieci komputerowe, od małych sieci domowych po globalny Internet, są zbudowane z wielu połączonych ze sobą urządzeń. Oprócz komputerów i serwerów (tzw. hostów), kluczową rolę odgrywają specjalistyczne urządzenia pośredniczące, które zarządzają przepływem danych. Trzy najbardziej podstawowe z nich to **koncentrator (hub)**, **przełącznik (switch)** i **router**. Każde z tych urządzeń operuje na innej warstwie modelu komunikacyjnego i pełni inną, specyficzną rolę w procesie przesyłania danych, a ich ewolucja odzwierciedla rosnącą "inteligencję" sieci.

#### Koncentrator (Hub)

*   **Warstwa modelu OSI:** 1 (Fizyczna).
*   **Rola:** Najprostsze urządzenie służące do łączenia wielu komputerów w jedną sieć lokalną (LAN) o topologii gwiazdy.
*   **Zasada działania:** Koncentrator działa jak prosty "rozgałęziacz" elektryczny. Każdy sygnał (strumień bitów) otrzymany na jednym z jego portów jest natychmiast, bez żadnej analizy, **kopiowany i rozsyłany na wszystkie pozostałe porty**. Wszystkie podłączone do niego urządzenia znajdują się w jednej, wspólnej **domenie kolizji**, co oznacza, że jeśli dwa urządzenia zaczną nadawać w tym samym czasie, dojdzie do kolizji (zniekształcenia sygnału), a transmisja musi zostać powtórzona.
*   **Analiza:** Jest to urządzenie bardzo prymitywne i nieefektywne. Generuje niepotrzebny ruch w sieci (każdy słyszy transmisję każdego) i drastycznie obniża wydajność wraz ze wzrostem liczby podłączonych urządzeń. Z tego powodu koncentratory są dziś urządzeniami **historycznymi** i zostały całkowicie wyparte przez przełączniki.

#### Przełącznik (Switch)

*   **Warstwa modelu OSI:** 2 (Łącza danych).
*   **Rola:** Podobnie jak koncentrator, łączy urządzenia w sieć lokalną, ale robi to w sposób inteligentny.
*   **Zasada działania:** Przełącznik analizuje każdą przychodzącą **ramkę** danych. Odczytuje z jej nagłówka **źródłowy i docelowy adres MAC**. Na podstawie źródłowych adresów MAC buduje i utrzymuje **tablicę adresów MAC**, która kojarzy konkretny adres MAC z portem, do którego podłączone jest dane urządzenie. Gdy przełącznik otrzymuje ramkę, sprawdza docelowy adres MAC w swojej tablicy i przesyła ramkę **tylko do tego jednego, właściwego portu**, do którego podłączony jest odbiorca. Jeśli docelowego adresu MAC nie ma w tablicy, przełącznik zachowuje się jak koncentrator i rozsyła ramkę na wszystkie porty (oprócz źródłowego).
*   **Analiza:** Dzięki inteligentnemu przesyłaniu ramek, przełącznik znacząco redukuje niepotrzebny ruch w sieci i zwiększa jej wydajność. Co najważniejsze, każdy port przełącznika tworzy **osobną domenę kolizji**. Oznacza to, że wiele par urządzeń może prowadzić transmisję jednocześnie, bez wzajemnego zakłócania się. Przełączniki są podstawowym budulcem współczesnych sieci LAN.

#### Router

*   **Warstwa modelu OSI:** 3 (Sieci).
*   **Rola:** Najbardziej zaawansowane z tych trzech urządzeń. Jego głównym zadaniem jest **łączenie różnych sieci komputerowych** (np. połączenie naszej sieci domowej z Internetem) i **wyznaczanie najlepszej trasy (routing)** dla pakietów między tymi sieciami.
*   **Zasada działania:** Router operuje na **pakietach** i podejmuje decyzje na podstawie **adresów IP**. Każdy port routera jest podłączony do innej sieci. Gdy router otrzymuje pakiet, analizuje jego nagłówek IP, a konkretnie **docelowy adres IP**. Na podstawie swojej **tablicy routingu** (która jest budowana dynamicznie za pomocą protokołów routingu, np. OSPF, BGP), router decyduje, do której sieci i na który ze swoich portów powinien przesłać pakiet dalej, aby ten zbliżył się do celu. Routery tworzą barierę dla rozgłoszeń (broadcastów) i dzielą sieć na osobne **domeny rozgłoszeniowe**.
*   **Analiza:** Routery są kręgosłupem Internetu. Umożliwiają globalną komunikację, znajdując ścieżki dla danych w skomplikowanej siatce połączonych ze sobą sieci. Domowe routery często łączą w sobie funkcje routera, przełącznika i bezprzewodowego punktu dostępowego (Access Point).

#### Porównanie urządzeń

| Cecha | Koncentrator (Hub) | Przełącznik (Switch) | Router |
|---|---|---|---|
| **Warstwa OSI** | 1 (Fizyczna) | 2 (Łącza danych) | 3 (Sieci) |
| **Jednostka danych** | Bity | Ramki | Pakiety |
| **Adresowanie** | Brak (działa na sygnale elektrycznym) | Adresy MAC (fizyczne) | Adresy IP (logiczne) |
| **Podejmowanie decyzji** | Brak (rozsyła na wszystkie porty) | Przesyła do konkretnego portu na podstawie adresu MAC | Przesyła do innej sieci na podstawie adresu IP |
| **Domena kolizji** | Jedna duża | Osobna dla każdego portu | Osobna dla każdego portu |
| **Domena rozgłoszeniowa** | Jedna duża | Jedna duża | Osobna dla każdego portu |
| **Główne zadanie** | Łączenie urządzeń (przestarzałe) | Łączenie urządzeń w **jednej sieci** | Łączenie **różnych sieci** i routing |

#### Podsumowanie

*   **Koncentrator** to proste, historyczne urządzenie warstwy 1, które bezmyślnie rozsyła sygnał na wszystkie porty, tworząc jedną, dużą domenę kolizji.
*   **Przełącznik** to inteligentne urządzenie warstwy 2, które uczy się adresów MAC podłączonych urządzeń i przesyła ramki tylko do właściwego odbiorcy, znacząco zwiększając wydajność sieci lokalnej.
*   **Router** to urządzenie warstwy 3, które łączy różne sieci i podejmuje decyzje o dalszej drodze pakietów na podstawie ich docelowych adresów IP, umożliwiając globalną komunikację w Internecie.
*   Zrozumienie różnic między tymi urządzeniami jest fundamentalne dla projektowania, budowy i diagnozowania problemów w każdej sieci komputerowej.

**Typowe pytania egzaminacyjne:**
*   Proszę porównać działanie koncentratora, przełącznika i routera, wskazując, w której warstwie modelu OSI każde z nich operuje.
*   Na podstawie jakich adresów przełącznik i router podejmują decyzje o przesłaniu danych?
*   Czym jest domena kolizji i domena rozgłoszeniowa? Które z omawianych urządzeń je tworzą?
*   Jak przełącznik buduje swoją tablicę adresów MAC?
*   Jakie jest główne zadanie routera w sieci komputerowej?

---

# 29. Rola i zadania wybranych protokołów warstwy aplikacji: HTTP, FTP, SMTP, DNS

#### Wprowadzenie

Warstwa aplikacji jest najwyższą warstwą w modelach OSI i TCP/IP, najbliższą użytkownikowi. To właśnie na tym poziomie działają protokoły, które definiują reguły komunikacji dla konkretnych zastosowań sieciowych, takich jak przeglądanie stron internetowych, przesyłanie plików czy wysyłanie poczty elektronicznej. Protokoły te stanowią fundament usług, z których korzystamy na co dzień w Internecie. Zrozumienie roli i zadań kluczowych protokołów – HTTP, FTP, SMTP i DNS – jest niezbędne do zrozumienia, jak działają najpopularniejsze aplikacje sieciowe.

#### HTTP (Hypertext Transfer Protocol) – Protokół Transferu Hipertekstu

*   **Rola:** Fundamentalny protokół World Wide Web. Jego głównym zadaniem jest umożliwienie komunikacji między przeglądarką internetową (klientem) a serwerem WWW w celu pobierania zasobów, takich jak dokumenty HTML, obrazy, arkusze stylów (CSS) i skrypty.
*   **Zasada działania:** HTTP działa w modelu **żądanie-odpowiedź (request-response)**.
    1.  **Klient (przeglądarka)** wysyła na serwer **żądanie HTTP**. Żądanie to zawiera **metodę** (np. `GET` – pobierz zasób, `POST` – wyślij dane do przetworzenia), adres URL zasobu oraz dodatkowe nagłówki.
    2.  **Serwer** odbiera żądanie, przetwarza je, lokalizuje zasób i odsyła do klienta **odpowiedź HTTP**. Odpowiedź zawiera **kod stanu** (np. `200 OK` – wszystko w porządku, `404 Not Found` – nie znaleziono zasobu), nagłówki oraz treść właściwego zasobu (np. kod HTML strony).
*   **Cechy:**
    *   **Bezstanowy (Stateless):** Każde żądanie jest traktowane przez serwer jako niezależna transakcja. Serwer nie pamięta poprzednich żądań od tego samego klienta. (Stan jest zarządzany po stronie klienta za pomocą ciasteczek - cookies).
    *   **Tekstowy:** Komunikaty HTTP są w dużej mierze czytelne dla człowieka.
*   **HTTPS (HTTP Secure):** Jest to bezpieczna wersja protokołu HTTP, która szyfruje całą komunikację za pomocą protokołów SSL/TLS, zapewniając poufność i integralność przesyłanych danych.

#### FTP (File Transfer Protocol) – Protokół Transferu Plików

*   **Rola:** Specjalizowany protokół przeznaczony do przesyłania (pobierania i wysyłania) plików między komputerami w sieci.
*   **Zasada działania:** FTP jest protokołem **stanowym** i wykorzystuje **dwa oddzielne połączenia TCP**:
    1.  **Połączenie sterujące (Control Connection):** Ustanawiane na porcie 21 serwera. Służy do przesyłania poleceń (np. `USER`, `PASS`, `LIST`, `RETR` - pobierz, `STOR` - wyślij) i odpowiedzi między klientem a serwerem. To połączenie jest aktywne przez całą sesję.
    2.  **Połączenie danych (Data Connection):** Ustanawiane dynamicznie (na porcie 20 w trybie aktywnym lub na losowym porcie w trybie pasywnym) dla każdego transferu pliku lub listingu katalogu. Po zakończeniu transferu jest zamykane.
*   **Cechy:**
    *   **Wymaga uwierzytelnienia:** Zazwyczaj wymaga podania nazwy użytkownika i hasła (choć istnieje tryb anonimowy).
    *   **Nieszyfrowany:** W swojej podstawowej wersji przesyła dane (w tym hasła) otwartym tekstem, co jest niebezpieczne. Bezpiecznymi alternatywami są FTPS (FTP over SSL/TLS) i SFTP (SSH File Transfer Protocol).

#### SMTP (Simple Mail Transfer Protocol) – Protokół Prostej Poczty

*   **Rola:** Standardowy protokół używany do **wysyłania** poczty elektronicznej w Internecie. Jego zadaniem jest przekazanie wiadomości e-mail od klienta poczty do serwera pocztowego nadawcy, a następnie "przepchnięcie" jej między kolejnymi serwerami pocztowymi aż do serwera odbiorcy.
*   **Zasada działania:** SMTP działa na zasadzie "push" (pchania). Klient SMTP (np. Outlook, Thunderbird) łączy się z serwerem SMTP (zazwyczaj na porcie 25, 587 lub 465) i za pomocą serii poleceń (`HELO`, `MAIL FROM`, `RCPT TO`, `DATA`) przekazuje wiadomość do wysłania.
*   **Ograniczenie:** SMTP służy **tylko do wysyłania** poczty. Do odbierania i pobierania wiadomości z serwera na komputer użytkownika służą inne protokoły, takie jak **POP3 (Post Office Protocol 3)** lub **IMAP (Internet Message Access Protocol)**.

#### DNS (Domain Name System) – System Nazw Domenowych

*   **Rola:** Kluczowa usługa działająca w tle, często nazywana "książką telefoniczną Internetu". Jej zadaniem jest tłumaczenie **czytelnych dla człowieka nazw domenowych** (np. `www.wikipedia.org`) na **numeryczne adresy IP** (np. `208.80.154.224`), które są niezbędne do nawiązania połączenia w sieci.
*   **Zasada działania:** DNS to globalna, rozproszona i hierarchiczna baza danych. Gdy aplikacja (np. przeglądarka) chce poznać adres IP danej domeny, jej systemowy **resolver** wysyła zapytanie do skonfigurowanego serwera DNS.
    1.  Lokalny serwer DNS sprawdza swoją pamięć podręczną (cache).
    2.  Jeśli nie znajdzie odpowiedzi, pyta **serwery główne (root servers)** o adres serwera dla domeny najwyższego poziomu (np. `.org`).
    3.  Następnie pyta serwer `.org` o adres serwera autorytatywnego dla domeny `wikipedia.org`.
    4.  Na koniec pyta serwer `wikipedia.org` o adres IP dla `www.wikipedia.org` i zwraca go do klienta.
*   **Cechy:**
    *   **Hierarchiczny:** Struktura domen przypomina odwrócone drzewo (od serwerów głównych, przez domeny TLD, po domeny drugiego poziomu).
    *   **Rozproszony:** Baza danych jest rozproszona na tysiącach serwerów na całym świecie, co zapewnia niezawodność i skalowalność.

#### Podsumowanie

| Protokół | Port (standardowy) | Główne zadanie | Model działania |
|---|---|---|---|
| **HTTP** | 80 | Przesyłanie zawartości stron WWW | Żądanie-odpowiedź, bezstanowy |
| **FTP** | 21 (sterujące), 20 (dane) | Transfer plików | Dwa połączenia, stanowy |
| **SMTP** | 25, 587, 465 | Wysyłanie poczty e-mail | "Push", polecenia tekstowe |
| **DNS** | 53 | Tłumaczenie nazw domen na adresy IP | Zapytanie-odpowiedź, hierarchiczny |

*   **HTTP** jest fundamentem przeglądania stron internetowych.
*   **FTP** to wyspecjalizowane narzędzie do transferu plików.
*   **SMTP** odpowiada za wysyłanie e-maili, podczas gdy POP3/IMAP służą do ich odbierania.
*   **DNS** działa w tle, umożliwiając korzystanie z łatwych do zapamiętania nazw zamiast skomplikowanych adresów IP.

**Typowe pytania egzaminacyjne:**
*   Jaka jest rola protokołu HTTP i na czym polega jego model działania?
*   Czym różni się protokół FTP od HTTP pod względem sposobu nawiązywania połączeń?
*   Do czego służy protokół SMTP, a do czego POP3/IMAP?
*   Proszę opisać rolę i hierarchiczną naturę systemu DNS.
*   Dlaczego protokół HTTP nazywany jest protokołem bezstanowym?

---

# 30. Podstawowe zagadnienia bezpieczeństwa sieci komputerowych: zagrożenia, metody ochrony, kryptografia

#### Wprowadzenie

Bezpieczeństwo sieci komputerowych to zbiór technologii, procesów i praktyk mających na celu ochronę sieci, urządzeń i danych przed nieautoryzowanym dostępem, atakiem, uszkodzeniem lub wyciekiem. W dzisiejszym połączonym świecie, gdzie informacja jest jednym z najcenniejszych zasobów, zapewnienie bezpieczeństwa jest absolutnie kluczowe. Obejmuje ono trzy fundamentalne filary, znane jako **triada CIA**: **Poufność (Confidentiality)**, **Integralność (Integrity)** i **Dostępność (Availability)**.

*   **Poufność:** Zapewnienie, że informacje są dostępne tylko dla upoważnionych osób.
*   **Integralność:** Gwarancja, że dane nie zostały zmienione w nieautoryzowany sposób podczas przechowywania lub przesyłania.
*   **Dostępność:** Zapewnienie, że systemy i dane są dostępne dla upoważnionych użytkowników wtedy, gdy są potrzebne.

#### Podstawowe zagrożenia sieciowe

Zagrożenia dla bezpieczeństwa sieci można podzielić na kilka głównych kategorii:

1.  **Złośliwe oprogramowanie (Malware):** Szeroka kategoria oprogramowania zaprojektowanego, by uszkodzić lub zinfiltrować system komputerowy. Obejmuje:
    *   **Wirusy:** Kod, który dołącza się do istniejących programów i replikuje się, gdy są one uruchamiane.
    *   **Robaki (Worms):** Samoreplikujące się programy, które rozprzestrzeniają się przez sieć, wykorzystując luki w zabezpieczeniach.
    *   **Konie trojańskie (Trojans):** Oprogramowanie udające użyteczną aplikację, ale w rzeczywistości wykonujące szkodliwe działania w tle.
    *   **Ransomware:** Szyfruje pliki ofiary i żąda okupu za ich odblokowanie.
    *   **Spyware:** Potajemnie zbiera informacje o użytkowniku i jego aktywności.

2.  **Ataki socjotechniczne (Social Engineering):** Manipulowanie ludźmi w celu skłonienia ich do ujawnienia poufnych informacji (np. haseł, danych karty kredytowej).
    *   **Phishing:** Masowe wysyłanie fałszywych wiadomości e-mail, które wyglądają jak autentyczne (np. od banku) i nakłaniają do kliknięcia w złośliwy link lub podania danych na fałszywej stronie.

3.  **Ataki typu "odmowa usługi" (Denial of Service - DoS):**
    *   **DoS/DDoS (Distributed DoS):** Atak mający na celu uniemożliwienie działania usługi lub serwera poprzez zalanie go ogromną liczbą zapytań lub fałszywego ruchu sieciowego, co prowadzi do wyczerpania jego zasobów (mocy obliczeniowej, przepustowości) i niedostępności dla legalnych użytkowników.

4.  **Ataki na poziomie sieci:**
    *   **Podsłuchiwanie (Eavesdropping / Sniffing):** Przechwytywanie i analizowanie pakietów przesyłanych w sieci w celu wykradzenia nieszyfrowanych informacji (np. haseł).
    *   **Podszywanie się (Spoofing):** Fałszowanie adresu IP lub MAC w celu podszycia się pod inne, zaufane urządzenie w sieci.
    *   **Atak Man-in-the-Middle (MITM):** Atakujący potajemnie umieszcza się między dwiema komunikującymi się stronami, przechwytując, a potencjalnie i modyfikując ich komunikację.

#### Metody ochrony sieci

Ochrona sieci wymaga wielowarstwowego podejścia (tzw. **defense in depth**), które łączy różne technologie i dobre praktyki.

1.  **Zapora sieciowa (Firewall):**
    *   **Rola:** Podstawowy element obrony. Jest to bariera (sprzętowa lub programowa) umieszczona między siecią wewnętrzną (zaufaną) a siecią zewnętrzną (niezaufaną, np. Internetem). Filtruje przychodzący i wychodzący ruch sieciowy na podstawie zdefiniowanego zestawu reguł bezpieczeństwa, blokując nieautoryzowane połączenia.

2.  **Systemy wykrywania i zapobiegania włamaniom (IDS/IPS):**
    *   **IDS (Intrusion Detection System):** Monitoruje ruch sieciowy w poszukiwaniu oznak złośliwej aktywności lub naruszeń polityki bezpieczeństwa. W razie wykrycia podejrzanego wzorca, generuje alert dla administratora.
    *   **IPS (Intrusion Prevention System):** Ewolucja IDS. Oprócz wykrywania, potrafi również aktywnie **blokować** zidentyfikowane zagrożenia w czasie rzeczywistym.

3.  **Wirtualne Sieci Prywatne (VPN - Virtual Private Network):**
    *   **Rola:** Tworzy bezpieczny, szyfrowany "tunel" dla ruchu sieciowego przez sieć publiczną (Internet). Umożliwia zdalnym pracownikom bezpieczny dostęp do zasobów firmowych i zapewnia poufność podczas korzystania z niezaufanych sieci (np. publicznego Wi-Fi).

4.  **Segmentacja sieci:** Dzielenie dużej sieci na mniejsze, izolowane podsieci (VLANy). Jeśli jedna podsieć zostanie skompromitowana, atakujący ma utrudniony dostęp do pozostałych części sieci.

5.  **Oprogramowanie antywirusowe i antymalware:** Instalowane na punktach końcowych (komputerach, serwerach) w celu wykrywania i usuwania złośliwego oprogramowania.

#### Rola kryptografii

Kryptografia to nauka o technikach szyfrowania i deszyfrowania informacji w celu zapewnienia ich poufności i integralności. Jest ona fundamentem bezpiecznej komunikacji.

**1. Kryptografia symetryczna (z kluczem tajnym):**

*   **Zasada:** Ten sam klucz jest używany zarówno do **szyfrowania**, jak i **deszyfrowania** danych. Obie strony komunikacji muszą w bezpieczny sposób wejść w posiadanie tego samego tajnego klucza.
*   **Algorytmy:** AES (Advanced Encryption Standard), DES, 3DES.
*   **Zalety:** Bardzo szybka i wydajna.
*   **Wady:** Problem bezpiecznej dystrybucji klucza. Jak przekazać tajny klucz drugiej stronie przez niezaufany kanał?

**2. Kryptografia asymetryczna (z kluczem publicznym):**

*   **Zasada:** Wykorzystuje parę matematycznie powiązanych kluczy: **klucz publiczny** i **klucz prywatny**.
    *   **Klucz publiczny:** Może być swobodnie dystrybuowany. Służy do **szyfrowania** danych i **weryfikacji podpisu cyfrowego**.
    *   **Klucz prywatny:** Musi być utrzymywany w ścisłej tajemnicy przez właściciela. Służy do **deszyfrowania** danych (zaszyfrowanych kluczem publicznym) i **tworzenia podpisu cyfrowego**.
*   **Algorytmy:** RSA, ECC (Elliptic Curve Cryptography).
*   **Zalety:** Rozwiązuje problem dystrybucji klucza. Umożliwia stosowanie **podpisów cyfrowych**, które zapewniają autentyczność i niezaprzeczalność.
*   **Wady:** Znacznie wolniejsza od kryptografii symetrycznej.

**Zastosowanie w praktyce (model hybrydowy):** W praktyce (np. w protokole TLS/SSL używanym przez HTTPS) łączy się zalety obu podejść. Kryptografia asymetryczna jest używana na początku do bezpiecznego uzgodnienia i wymiany jednorazowego klucza symetrycznego, a następnie cała dalsza komunikacja jest szyfrowana za pomocą znacznie szybszej kryptografii symetrycznej.

#### Podsumowanie

*   **Bezpieczeństwo sieci** ma na celu ochronę **poufności, integralności i dostępności** danych i systemów.
*   Główne **zagrożenia** to m.in. **malware, phishing, ataki DoS** i ataki sieciowe, takie jak **podsłuchiwanie i MITM**.
*   Podstawowe **metody ochrony** to **firewalle, systemy IDS/IPS, VPN-y**, segmentacja sieci i oprogramowanie antywirusowe.
*   **Kryptografia** jest kluczowym narzędziem zapewniającym poufność i integralność. Wyróżniamy kryptografię **symetryczną** (szybką, jeden klucz) i **asymetryczną** (wolniejszą, para kluczy publiczny/prywatny), które w praktyce są łączone w model hybrydowy.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać trzy filary bezpieczeństwa informacji (triada CIA).
*   Jakie są najczęstsze zagrożenia dla bezpieczeństwa sieci? Proszę opisać co najmniej dwa z nich.
*   Jaka jest rola zapory sieciowej (firewall) i czym różni się system IDS od IPS?
*   Proszę porównać kryptografię symetryczną i asymetryczną, wskazując ich wady i zalety.
*   Do czego służy i jak działa VPN?

---

# 31. Cykl życia oprogramowania i jego modele (modele wytwarzania oprogramowania)

#### Wprowadzenie

Inżynieria oprogramowania to dyscyplina zajmująca się stosowaniem usystematyzowanego, zdyscyplinowanego i mierzalnego podejścia do projektowania, tworzenia, wdrażania i utrzymania oprogramowania. Kluczowym pojęciem w tej dziedzinie jest **cykl życia oprogramowania (SDLC - Software Development Life Cycle)**, który definiuje ramy procesowe dla wszystkich działań związanych z oprogramowaniem, od jego koncepcji aż po wycofanie z użytku. Aby uporządkować ten proces, stworzono różne **modele wytwarzania oprogramowania**, które opisują sekwencję i współzależności poszczególnych etapów pracy.

#### Cykl życia oprogramowania (SDLC)

SDLC to ustrukturyzowany proces, który dzieli tworzenie oprogramowania na serię następujących po sobie faz. Celem jest zapewnienie wysokiej jakości produktu końcowego, który spełnia oczekiwania klienta i jest dostarczony na czas i w ramach budżetu. Typowe fazy cyklu życia to:

1.  **Analiza i specyfikacja wymagań:** Najważniejszy etap, polegający na zebraniu, zrozumieniu i udokumentowaniu potrzeb i oczekiwań klienta oraz użytkowników końcowych. Określa się tu, **co** system ma robić (wymagania funkcjonalne) i **jak** ma to robić (wymagania niefunkcjonalne, np. dotyczące wydajności, bezpieczeństwa).
2.  **Projektowanie (Design):** Na podstawie zebranych wymagań tworzony jest szczegółowy projekt systemu. Obejmuje on:
    *   **Projekt architektury (High-Level Design):** Definiuje ogólną strukturę systemu, jego główne komponenty i interakcje między nimi.
    *   **Projekt szczegółowy (Low-Level Design):** Opisuje wewnętrzną logikę każdego komponentu, struktury danych, algorytmy.
3.  **Implementacja (Kodowanie):** Faza, w której projekt jest przekształcany w działający kod programu przy użyciu wybranego języka programowania i narzędzi.
4.  **Testowanie:** Kluczowy etap weryfikacji i walidacji oprogramowania. Ma na celu wykrycie błędów i upewnienie się, że system spełnia zdefiniowane wymagania. Obejmuje różne poziomy testów: jednostkowe, integracyjne, systemowe i akceptacyjne.
5.  **Wdrożenie (Deployment):** Instalacja gotowego, przetestowanego oprogramowania w środowisku produkcyjnym, czyli u klienta. Może to być prosty proces lub złożona operacja wymagająca migracji danych i szkolenia użytkowników.
6.  **Utrzymanie (Maintenance):** Najdłuższa i często najkosztowniejsza faza cyklu życia. Obejmuje wszelkie działania po wdrożeniu produktu, takie jak naprawa błędów zgłaszanych przez użytkowników, dostosowywanie oprogramowania do zmieniającego się środowiska oraz dodawanie nowych funkcjonalności.

#### Modele wytwarzania oprogramowania

Model wytwarzania oprogramowania opisuje, w jaki sposób poszczególne fazy SDLC są zorganizowane w czasie. Wybór odpowiedniego modelu zależy od charakteru projektu, jego złożoności, stabilności wymagań i kultury organizacyjnej zespołu.

**1. Model kaskadowy (Waterfall Model):**

*   **Opis:** Najstarszy i najbardziej tradycyjny model. Jest to podejście **sekwencyjne i liniowe**, w którym każda faza musi zostać w pełni zakończona, zanim rozpocznie się następna. Proces przypomina spływającą wodę w wodospadzie – nie ma powrotu do wcześniejszych etapów.
*   **Zalety:** Prosty do zrozumienia i zarządzania, silny nacisk na dokumentację, idealny dla projektów o bardzo stabilnych i dobrze zdefiniowanych na początku wymaganiach.
*   **Wady:** Bardzo niska elastyczność. Jakikolwiek błąd popełniony na wczesnym etapie jest bardzo kosztowny do naprawienia. Klient widzi działający produkt dopiero na samym końcu. Nie nadaje się do złożonych projektów, gdzie wymagania mogą się zmieniać.

**2. Modele ewolucyjne i przyrostowe (Evolutionary & Incremental Models):**

*   **Opis:** Grupa modeli, które zakładają tworzenie oprogramowania w kolejnych **przyrostach (inkrementach)** lub **iteracjach**. Zamiast budować cały system za jednym razem, dostarcza się kolejne, coraz bardziej kompletne i funkcjonalne wersje produktu.
    *   **Model przyrostowy:** W każdej iteracji dodawana jest nowa, w pełni ukończona (zaprojektowana, zakodowana, przetestowana) część funkcjonalności.
    *   **Model ewolucyjny (w tym prototypowy i spiralny):** W każdej iteracji tworzony jest działający prototyp, który jest prezentowany klientowi. Na podstawie jego opinii, prototyp jest udoskonalany i rozwijany w kolejnych iteracjach, ewoluując w kierunku finalnego produktu.
*   **Zalety:** Elastyczność i łatwość adaptacji do zmieniających się wymagań. Klient wcześnie i regularnie widzi działające części systemu, co pozwala na bieżąco zbierać jego feedback. Ryzyko jest rozłożone na wiele iteracji.
*   **Wady:** Wymaga dobrego planowania i projektowania architektury, aby kolejne przyrosty dobrze ze sobą współgrały. Może prowadzić do "puchnięcia" projektu, jeśli nie ma kontroli nad zakresem.

**3. Metodyki zwinne (Agile Methods):**

*   **Opis:** To nie jest jeden model, ale raczej **filozofia i zbiór zasad** wytwarzania oprogramowania, które kładą nacisk na **adaptacyjność, współpracę z klientem, szybkie dostarczanie działającego oprogramowania i reagowanie na zmiany**. Agile jest podejściem iteracyjnym i przyrostowym.
*   **Manifest Agile:**
    *   **Ludzie i interakcje** ponad procesy i narzędzia.
    *   **Działające oprogramowanie** ponad obszerną dokumentację.
    *   **Współpraca z klientem** ponad formalne negocjacje.
    *   **Reagowanie na zmiany** ponad podążanie za planem.
*   **Przykłady metodyk zwinnych:**
    *   **Scrum:** Najpopularniejsza metodyka zwinna. Praca jest zorganizowana w krótkie, stałej długości iteracje zwane **sprintami** (zwykle 2-4 tygodnie). Zespół jest samoorganizujący się i interdyscyplinarny.
    *   **Kanban:** Koncentruje się na wizualizacji przepływu pracy (na tablicy Kanban) i ograniczaniu pracy w toku (WIP - Work In Progress) w celu maksymalizacji wydajności.
*   **Zalety:** Najwyższy stopień elastyczności, idealne dla złożonych projektów z niepewnymi lub szybko zmieniającymi się wymaganiami. Wysokie zaangażowanie klienta i duża motywacja zespołu.
*   **Wady:** Wymaga dużej dyscypliny i doświadczenia od zespołu. Może być trudny do wdrożenia w dużych, biurokratycznych organizacjach.

#### Porównanie modeli

| Cecha | Model kaskadowy | Modele przyrostowe/ewolucyjne | Metodyki zwinne (Agile) |
|---|---|---|---|
| **Podejście** | Liniowe, sekwencyjne | Iteracyjne, przyrostowe | Iteracyjne, przyrostowe, adaptacyjne |
| **Elastyczność** | Bardzo niska | Średnia do wysokiej | Bardzo wysoka |
| **Dokumentacja** | Obszerna, kluczowa | Umiarkowana | Minimalna, "w sam raz" |
| **Zaangażowanie klienta** | Niskie (na początku i na końcu) | Regularne (po każdej iteracji) | Ciągłe, codzienne |
| **Dostarczanie produktu** | Jednorazowo, na końcu projektu | W częściach (przyrostach) | Często, małe, działające fragmenty |
| **Najlepszy dla** | Prostych projektów o stałych wymaganiach | Średnio złożonych projektów | Złożonych projektów o zmiennych wymaganiach |

#### Podsumowanie

*   **Cykl życia oprogramowania (SDLC)** to ustrukturyzowany proces obejmujący fazy od analizy wymagań po utrzymanie.
*   **Modele wytwarzania oprogramowania** definiują, jak te fazy są zorganizowane.
*   **Model kaskadowy** to sztywne, sekwencyjne podejście, odpowiednie tylko dla najprostszych projektów.
*   **Modele przyrostowe i ewolucyjne** wprowadzają iteracyjność, dostarczając oprogramowanie w częściach i zbierając feedback od klienta.
*   **Metodyki zwinne (Agile)**, takie jak Scrum, to nowoczesne, elastyczne podejście, które stawia na adaptacyjność, współpracę i szybkie dostarczanie wartości biznesowej w złożonych i dynamicznych projektach.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać fazy cyklu życia oprogramowania.
*   Na czym polega model kaskadowy? Jakie są jego główne wady i zalety?
*   Proszę porównać model kaskadowy z modelem iteracyjnym.
*   Jakie są cztery główne wartości Manifestu Agile?
*   Do jakiego typu projektów najlepiej nadają się metodyki zwinne, a do jakich model kaskadowy?

---

# 32. Analiza i projektowanie algorytmów, złożoność obliczeniowa, notacja asymptotyczna

#### Wprowadzenie

Algorytm to precyzyjny przepis na rozwiązanie określonego problemu, składający się ze skończonej sekwencji jednoznacznych kroków. Analiza i projektowanie algorytmów to centralna dziedzina informatyki, która zajmuje się nie tylko tworzeniem poprawnych algorytmów, ale przede wszystkim tworzeniem algorytmów **efektywnych**. Efektywność algorytmu mierzy się ilością zasobów, jakie on zużywa – głównie **czasu (liczby operacji)** i **pamięci**. Aby móc obiektywnie porównywać algorytmy i przewidywać ich zachowanie dla dużych zbiorów danych, wprowadzono pojęcie **złożoności obliczeniowej** i formalny zapis w postaci **notacji asympotycznej**.

#### Analiza algorytmów i złożoność obliczeniowa

Analiza algorytmu polega na określeniu jego zapotrzebowania na zasoby w zależności od **rozmiaru danych wejściowych (n)**. Na przykład dla algorytmu sortującego, `n` to liczba elementów do posortowania.

*   **Złożoność czasowa (Time Complexity):** Określa, jak liczba podstawowych operacji wykonywanych przez algorytm rośnie wraz ze wzrostem rozmiaru danych `n`. Nie mierzymy rzeczywistego czasu w sekundach (bo zależy on od szybkości komputera), ale właśnie liczbę operacji (np. porównań, przypisań).
*   **Złożoność pamięciowa (Space Complexity):** Określa, ile dodatkowej pamięci (oprócz danych wejściowych) algorytm potrzebuje do swojego działania, w zależności od `n`.

Analizując złożoność, często rozważamy trzy przypadki:

*   **Przypadek optymistyczny (Best Case):** Najkorzystniejszy układ danych wejściowych (np. sortowanie już posortowanej tablicy).
*   **Przypadek pesymistyczny (Worst Case):** Najmniej korzystny układ danych (np. sortowanie tablicy posortowanej w odwrotnej kolejności). **To najważniejsza i najczęściej analizowana miara**, ponieważ daje gwarancję, że algorytm nigdy nie zachowa się gorzej.
*   **Przypadek średni (Average Case):** Oczekiwana wydajność dla losowych danych. Często trudna do precyzyjnego obliczenia.

#### Notacja asympotyczna (O, Ω, Θ)

Notacja asympotyczna to matematyczny sposób opisywania zachowania funkcji dla dużych wartości argumentów. W informatyce służy do klasyfikowania algorytmów według ich złożoności, ignorując stałe czynniki i składniki niższego rzędu, ponieważ dla dużych `n` liczy się tylko **tempo wzrostu** funkcji złożoności.

**1. Notacja O (Duże O – Big O):**

*   **Znaczenie:** Określa **górne ograniczenie** (asymptotyczny sufit) złożoności. Mówi nam, że w najgorszym przypadku algorytm nie będzie działał wolniej niż pewna funkcja.
*   **Formalnie:** `f(n) = O(g(n))` oznacza, że istnieją takie stałe `c > 0` i `n₀`, że dla każdego `n > n₀` zachodzi `0 ≤ f(n) ≤ c * g(n)`.
*   **Przykład:** Jeśli algorytm ma złożoność `O(n²)`, oznacza to, że jego czas wykonania rośnie co najwyżej kwadratowo w stosunku do rozmiaru danych. Jest to najczęściej używana notacja, ponieważ opisuje pesymistyczny scenariusz.

**2. Notacja Ω (Duża Omega – Big Omega):**

*   **Znaczenie:** Określa **dolne ograniczenie** (asymptotyczna podłoga) złożoności. Mówi nam, że w najlepszym przypadku algorytm nie będzie działał szybciej niż pewna funkcja.
*   **Formalnie:** `f(n) = Ω(g(n))` oznacza, że istnieją takie stałe `c > 0` i `n₀`, że dla każdego `n > n₀` zachodzi `0 ≤ c * g(n) ≤ f(n)`.
*   **Przykład:** Każdy algorytm sortujący oparty na porównaniach musi w najgorszym przypadku wykonać co najmniej `Ω(n log n)` porównań.

**3. Notacja Θ (Duża Theta – Big Theta):**

*   **Znaczenie:** Określa **ścisłe ograniczenie** (asymptotycznie dokładne). Mówi nam, że tempo wzrostu złożoności algorytmu jest takie samo jak tempo wzrostu danej funkcji.
*   **Formalnie:** `f(n) = Θ(g(n))` wtedy i tylko wtedy, gdy `f(n) = O(g(n))` i `f(n) = Ω(g(n))`.
*   **Przykład:** Wyszukiwanie elementu w nieposortowanej tablicy ma złożoność `Θ(n)`, ponieważ w średnim i pesymistycznym przypadku musimy przejrzeć prawie wszystkie elementy.

**Typowe klasy złożoności (od najlepszej do najgorszej):**

| Notacja | Nazwa | Przykład |
|---|---|---|
| **Θ(1)** | Stała | Dostęp do elementu tablicy przez indeks. |
| **Θ(log n)** | Logarytmiczna | Wyszukiwanie binarne w posortowanej tablicy. |
| **Θ(n)** | Liniowa | Wyszukiwanie elementu w nieposortowanej tablicy. |
| **Θ(n log n)** | Liniowo-logarytmiczna | Wydajne algorytmy sortowania (np. przez scalanie, szybkie). |
| **Θ(n²)** | Kwadratowa | Proste algorytmy sortowania (np. bąbelkowe, przez wstawianie). |
| **Θ(n³)** | Sześcienna | Mnożenie macierzy (naiwny algorytm). |
| **Θ(2ⁿ)** | Wykładnicza | Problem komiwojażera (rozwiązanie siłowe). |
| **Θ(n!)** | Silnia | Generowanie wszystkich permutacji zbioru. |

#### Projektowanie algorytmów

Projektowanie algorytmów to sztuka tworzenia efektywnych rozwiązań problemów. Istnieje kilka fundamentalnych technik (paradygmatów) projektowania:

*   **Dziel i zwyciężaj (Divide and Conquer):** Problem jest dzielony na mniejsze, niezależne podproblemy tego samego typu. Podproblemy są rozwiązywane rekurencyjnie, a ich wyniki są następnie łączone w celu uzyskania rozwiązania oryginalnego problemu. *Przykłady: sortowanie przez scalanie (Merge Sort), sortowanie szybkie (Quick Sort), wyszukiwanie binarne.*
*   **Programowanie dynamiczne (Dynamic Programming):** Stosowane, gdy podproblemy nie są niezależne i wielokrotnie rozwiązujemy te same podproblemy. Rozwiązania mniejszych podproblemów są zapamiętywane (w tablicy) i ponownie wykorzystywane do rozwiązywania większych. *Przykłady: obliczanie liczb Fibonacciego, problem najdłuższego wspólnego podciągu, problem plecakowy.*
*   **Metoda zachłanna (Greedy Method):** Na każdym kroku algorytm dokonuje lokalnie optymalnego wyboru w nadziei, że doprowadzi to do globalnie optymalnego rozwiązania. Nie zawsze działa, ale jeśli działa, jest zazwyczaj bardzo prosta i szybka. *Przykłady: algorytm Dijkstry (znajdowanie najkrótszej ścieżki w grafie), algorytm Kruskala (znajdowanie minimalnego drzewa rozpinającego), wydawanie reszty.*

#### Podsumowanie

*   **Analiza algorytmów** pozwala ocenić ich **efektywność** pod względem czasu i pamięci w zależności od rozmiaru danych `n`.
*   **Złożoność obliczeniowa** jest formalnym opisem tej efektywności, najczęściej rozpatrywanym w **przypadku pesymistycznym**.
*   **Notacja asympotyczna (O, Ω, Θ)** służy do klasyfikowania algorytmów, opisując tempo wzrostu ich złożoności dla dużych `n`. Notacja **O** jest najczęściej stosowana, gdyż określa górną granicę złożoności.
*   Algorytmy o złożoności **wielomianowej** (np. `O(n²)`, `O(n³)`), a zwłaszcza **liniowej** (`O(n)`) czy **logarytmicznej** (`O(log n)`), uważa się za **efektywne**. Algorytmy o złożoności **wykładniczej** (`O(2ⁿ)`) są uważane za **nieefektywne** i praktycznie bezużyteczne dla większych `n`.
*   Główne **techniki projektowania algorytmów** to m.in. **dziel i zwyciężaj, programowanie dynamiczne i metoda zachłanna**.

**Typowe pytania egzaminacyjne:**
*   Co to jest złożoność czasowa i pamięciowa algorytmu?
*   Proszę wyjaśnić znaczenie notacji O, Ω i Θ na przykładach.
*   Proszę uszeregować następujące złożoności od najlepszej do najgorszej: O(n!), O(n log n), O(n²), O(log n), O(2ⁿ).
*   Na czym polega metoda projektowania algorytmów "dziel i zwyciężaj"?
*   Czym różni się programowanie dynamiczne od metody zachłannej?

---

# 33. Paradygmaty programowania: imperatywny, obiektowy, funkcyjny, deklaratywny

#### Wprowadzenie

Paradygmat programowania to fundamentalny styl lub sposób myślenia o programowaniu i konstrukcji programów komputerowych. Nie jest to konkretny język czy narzędzie, ale raczej zbiór idei, koncepcji i zasad, które kształtują sposób, w jaki programista podchodzi do rozwiązania problemu. Różne paradygmaty oferują różne sposoby strukturyzacji kodu, zarządzania złożonością i modelowania rzeczywistości. Zrozumienie głównych paradygmatów – imperatywnego, obiektowego, funkcyjnego i deklaratywnego – jest kluczowe dla każdego programisty, ponieważ pozwala na wybór odpowiedniego narzędzia do zadania i pisanie bardziej czytelnego, elastycznego i łatwiejszego w utrzymaniu kodu.

#### Paradygmat imperatywny (Imperative Programming)

*   **Idea:** Najstarszy i najbardziej podstawowy paradygmat. Program jest postrzegany jako **sekwencja poleceń (instrukcji)**, które krok po kroku **zmieniają stan programu** (wartości zmiennych w pamięci). Programista dokładnie opisuje, **jak** komputer ma wykonać zadanie.
*   **Kluczowe koncepcje:** Zmienne, instrukcje przypisania, pętle (`for`, `while`), instrukcje warunkowe (`if-else`).
*   **Podparadygmaty:**
    *   **Programowanie proceduralne:** Rozwinięcie programowania imperatywnego, w którym kod jest grupowany w **procedury (funkcje)**. Pozwala to na lepszą organizację i ponowne wykorzystanie kodu. *Przykłady języków: C, Pascal, Fortran.*
*   **Analogia:** Przepis kulinarny, który krok po kroku opisuje, co należy zrobić, aby przygotować potrawę.
*   **Przykład (JavaScript):**
    ```javascript
    function sumArray(arr) {
      let sum = 0; // Inicjalizacja stanu
      for (let i = 0; i < arr.length; i++) {
        sum += arr[i]; // Modyfikacja stanu w każdej iteracji
      }
      return sum;
    }
    ```

#### Paradygmat obiektowy (Object-Oriented Programming - OOP)

*   **Idea:** Ewolucja paradygmatu imperatywnego, która ma na celu zarządzanie złożonością dużych systemów. Program jest modelowany jako **zbiór współpracujących ze sobą obiektów**. Obiekt to byt, który łączy w sobie **dane (atrybuty)** i **zachowanie (metody)** operujące na tych danych.
*   **Kluczowe koncepcje:**
    *   **Hermetyzacja (Encapsulation):** Ukrywanie wewnętrznego stanu obiektu i udostępnianie go na zewnątrz tylko poprzez publiczny interfejs (metody). Chroni to dane przed nieautoryzowanym dostępem i modyfikacją.
    *   **Dziedziczenie (Inheritance):** Mechanizm, który pozwala tworzyć nowe klasy (klasy potomne) na podstawie istniejących (klasy bazowe), dziedzicząc ich atrybuty i metody. Umożliwia ponowne wykorzystanie kodu i tworzenie hierarchii klas.
    *   **Polimorfizm (Polymorphism):** Zdolność obiektów różnych klas do odpowiadania na to samo wywołanie metody w sposób specyficzny dla swojej klasy. Pozwala to na pisanie bardziej ogólnego i elastycznego kodu.
    *   **Abstrakcja (Abstraction):** Koncentrowanie się na istotnych cechach obiektu i ignorowanie nieistotnych szczegółów. Interfejs obiektu jest abstrakcją jego implementacji.
*   **Przykłady języków:** Java, C++, C#, Python, Ruby.

#### Paradygmat funkcyjny (Functional Programming - FP)

*   **Idea:** Podejście, w którym obliczenia są traktowane jako **ewaluacja funkcji matematycznych**. Kładzie nacisk na unikanie **stanu i danych mutowalnych (zmiennych)**. Zamiast opisywać, *jak* coś zrobić, programista opisuje, *co* chce osiągnąć, komponując ze sobą funkcje.
*   **Kluczowe koncepcje:**
    *   **Czyste funkcje (Pure Functions):** Funkcje, które dla tych samych danych wejściowych zawsze zwracają ten sam wynik i nie mają **efektów ubocznych** (nie modyfikują stanu poza swoim zasięgiem, nie wykonują operacji I/O).
    *   **Niezmienność (Immutability):** Dane raz utworzone nie mogą być modyfikowane. Zamiast zmieniać istniejącą strukturę danych, tworzy się nową z wprowadzonymi zmianami.
    *   **Funkcje wyższego rzędu (Higher-Order Functions):** Funkcje, które mogą przyjmować inne funkcje jako argumenty lub zwracać funkcje jako wynik.
*   **Zalety:** Kod jest łatwiejszy do rozumowania, testowania i zrównoleglania (brak współdzielonego stanu eliminuje wyścigi).
*   **Przykłady języków:** Haskell, Lisp, F#, a także elementy funkcyjne w JavaScript, Python, Java.
*   **Przykład (JavaScript):**
    ```javascript
    function sumArray(arr) {
      return arr.reduce((sum, current) => sum + current, 0);
    }
    ```

#### Paradygmat deklaratywny (Declarative Programming)

*   **Idea:** Nadrzędny paradygmat w stosunku do programowania funkcyjnego. Programista opisuje **logikę obliczeń i pożądany wynik**, a nie szczegółowy **przepływ sterowania**. Mówimy **"co"** chcemy osiągnąć, a nie **"jak"** to zrobić. System sam znajduje sposób na realizację celu.
*   **Podparadygmaty:**
    *   **Programowanie funkcyjne** (opisane wyżej).
    *   **Programowanie logiczne:** Program jest zbiorem faktów i reguł logicznych. Wykonanie polega na zadaniu pytania (query), a system próbuje znaleźć odpowiedź, dedukując na podstawie znanych faktów i reguł. *Przykład: Prolog.*
    *   **Języki zapytań do baz danych:** *Przykład: SQL.* Zapytanie `SELECT * FROM Users WHERE Country = 'Poland';` opisuje, *co* chcemy uzyskać, a nie *jak* silnik bazy danych ma krok po kroku przeszukać tabele i odfiltrować wyniki.

#### Porównanie: Imperatywny vs Deklaratywny

| Cecha | Imperatywny | Deklaratywny |
|---|---|---|
| **Fokus** | **Jak** osiągnąć cel (krok po kroku) | **Co** ma być osiągnięte (jaki ma być wynik) |
| **Stan** | Jawne zarządzanie i modyfikacja stanu | Unikanie lub ukrywanie zarządzania stanem |
| **Przepływ sterowania** | Jawnie zdefiniowany przez programistę (pętle, warunki) | Ukryty, domyślny dla systemu |
| **Poziom abstrakcji** | Niższy | Wyższy |

#### Podsumowanie

*   **Paradygmat imperatywny** koncentruje się na opisywaniu krok po kroku, jak zmieniać stan programu w celu osiągnięcia wyniku.
*   **Paradygmat obiektowy** organizuje kod wokół obiektów, które łączą dane i zachowanie, zarządzając złożonością za pomocą hermetyzacji, dziedziczenia i polimorfizmu.
*   **Paradygmat funkcyjny** traktuje programowanie jako kompozycję czystych, bezstanowych funkcji, promując niezmienność danych.
*   **Paradygmat deklaratywny** jest podejściem wysokopoziomowym, w którym programista opisuje pożądany rezultat, a nie sposób jego osiągnięcia.
*   Wiele nowoczesnych języków programowania (np. Python, JavaScript, C#) jest **wieloparadygmatowa**, co pozwala programistom na elastyczne łączenie różnych stylów w zależności od potrzeb.

**Typowe pytania egzaminacyjne:**
*   Co to jest paradygmat programowania?
*   Proszę porównać paradygmat imperatywny i deklaratywny.
*   Jakie są cztery filary programowania obiektowego? Proszę krótko opisać każdy z nich.
*   Czym jest czysta funkcja i jakie ma to znaczenie w programowaniu funkcyjnym?
*   Podaj przykład języka dla każdego z głównych paradygmatów.

---

# 34. Programowanie obiektowe: klasy, obiekty, dziedziczenie, polimorfizm

#### Wprowadzenie

Programowanie obiektowe (OOP - Object-Oriented Programming) to dominujący paradygmat programowania, który zrewolucjonizował sposób tworzenia oprogramowania, zwłaszcza dużych i złożonych systemów. Jego fundamentalna idea polega na modelowaniu problemu jako zbioru **obiektów**, które oddziałują na siebie nawzajem. Obiekt łączy w sobie dane (stan) i operacje na tych danych (zachowanie), co odzwierciedla sposób, w jaki postrzegamy byty w realnym świecie. Zrozumienie kluczowych koncepcji OOP – klas, obiektów, dziedziczenia i polimorfizmu – jest absolutnie niezbędne dla każdego nowoczesnego programisty.

#### Klasy i Obiekty

**Klasa (Class):**

*   **Definicja:** Klasa to **szablon, wzorzec lub "foremka"** do tworzenia obiektów. Definiuje ona strukturę i zachowanie dla pewnego typu obiektów. Klasa określa, jakie **atrybuty (pola, zmienne)** będą przechowywać stan obiektu oraz jakie **metody (funkcje)** będą mogły na tym stanie operować.
*   **Analogia:** Jeśli chcemy zbudować dom, najpierw potrzebujemy **projektu (planu architektonicznego)**. Ten projekt to właśnie klasa. Definiuje on, że dom będzie miał okna, drzwi, dach (atrybuty) oraz że będzie można otworzyć drzwi czy zamknąć okna (metody).

**Obiekt (Object):**

*   **Definicja:** Obiekt to **konkretna instancja (egzemplarz)** klasy. Jest to byt istniejący w pamięci komputera, stworzony na podstawie szablonu zdefiniowanego przez klasę. Każdy obiekt ma swój własny, niezależny stan (wartości atrybutów).
*   **Analogia:** Na podstawie jednego projektu (klasy `Dom`) możemy zbudować **wiele konkretnych domów** (obiektów). Każdy z tych domów jest osobnym bytem, może mieć inny kolor elewacji, a jego drzwi mogą być otwarte lub zamknięte niezależnie od innych domów.

**Przykład (Python):**
```python
# Definicja klasy (szablonu)
class Dog:
    # Konstruktor - metoda wywoływana podczas tworzenia nowego obiektu
    def __init__(self, name, age):
        self.name = name  # Atrybut
        self.age = age    # Atrybut

    # Metoda (zachowanie)
    def bark(self):
        print(f"{self.name} says: Woof!")

# Tworzenie obiektów (konkretnych instancji klasy Dog)
my_dog = Dog("Rex", 5)
another_dog = Dog("Buddy", 2)

# Wywoływanie metod na obiektach
my_dog.bark()       # Output: Rex says: Woof!
another_dog.bark()  # Output: Buddy says: Woof!
```

#### Cztery filary programowania obiektowego

Siła programowania obiektowego opiera się na czterech fundamentalnych mechanizmach:

**1. Hermetyzacja (Encapsulation):**

*   **Idea:** Zwijanie danych (atrybutów) i metod operujących na tych danych w jedną całość (obiekt) oraz **ukrywanie szczegółów implementacyjnych** przed światem zewnętrznym. Dostęp do wewnętrznego stanu obiektu jest kontrolowany i możliwy tylko poprzez jego publiczny interfejs (metody publiczne).
*   **Cel:** Ochrona danych przed przypadkową lub nieautoryzowaną modyfikacją, co zwiększa spójność i bezpieczeństwo. Pozwala na zmianę wewnętrznej implementacji obiektu bez wpływu na kod, który z niego korzysta.

**2. Abstrakcja (Abstraction):**

*   **Idea:** Prezentowanie użytkownikowi obiektu tylko istotnych informacji i ukrywanie nieistotnej złożoności. Skupiamy się na tym, **co** obiekt robi, a nie **jak** to robi.
*   **Cel:** Upraszcza interakcję z obiektem. Użytkownik nie musi znać skomplikowanych wewnętrznych mechanizmów, aby móc z niego korzystać. Interfejs obiektu jest abstrakcją jego działania.
*   **Przykład:** Prowadząc samochód, używamy prostego interfejsu (kierownica, pedały), nie musząc znać szczegółów działania silnika spalinowego.

**3. Dziedziczenie (Inheritance):**

*   **Idea:** Mechanizm, który pozwala tworzyć nowe klasy (**klasy potomne/pochodne**) na podstawie istniejących klas (**klasy bazowe/nadrzędne**). Klasa potomna **dziedziczy** (przejmuje) wszystkie atrybuty i metody klasy bazowej, a dodatkowo może dodawać własne lub modyfikować (przesłaniać) odziedziczone.
*   **Cel:** Ponowne wykorzystanie kodu (zasada DRY - Don't Repeat Yourself) i tworzenie hierarchii klas opartych na relacji "jest rodzajem" (ang. *is-a*). Na przykład `Pies` jest rodzajem `Zwierzęcia`.
*   **Przykład (Python):**
    ```python
    class Animal:
        def speak(self):
            print("Animal makes a sound")

    class Cat(Animal):  # Cat dziedziczy po Animal
        def speak(self):  # Przesłonięcie metody z klasy bazowej
            print("Cat says: Meow")
    ```

**4. Polimorfizm (Polymorphism):**

*   **Idea:** Z greckiego "wielopostaciowość". Jest to zdolność obiektów różnych, ale powiązanych ze sobą (np. przez dziedziczenie) klas do reagowania na to samo wywołanie metody w sposób specyficzny dla swojej klasy. Oznacza to, że możemy traktować obiekty różnych typów w jednolity sposób.
*   **Cel:** Pisanie bardziej ogólnego, elastycznego i rozszerzalnego kodu. Możemy napisać funkcję, która operuje na obiektach klasy bazowej, a ona będzie poprawnie działać z wszystkimi obiektami klas potomnych.
*   **Przykład (Python):**
    ```python
    def make_animal_speak(animal_object):
        animal_object.speak() # Nie musimy wiedzieć, czy to pies, czy kot

    cat = Cat()
    dog = Dog("Rex", 5) # Zakładając, że Dog też dziedziczy po Animal

    make_animal_speak(cat) # Output: Cat says: Meow
    make_animal_speak(dog) # Output: Rex says: Woof!
    ```

#### Podsumowanie

*   **Klasa** to szablon, a **obiekt** to konkretna instancja klasy.
*   **Hermetyzacja** łączy dane i metody, ukrywając implementację.
*   **Abstrakcja** upraszcza interakcję z obiektem, pokazując tylko to, co istotne.
*   **Dziedziczenie** pozwala na ponowne wykorzystanie kodu i tworzenie hierarchii klas.
*   **Polimorfizm** umożliwia traktowanie obiektów różnych typów w jednolity sposób, co prowadzi do elastycznego i rozszerzalnego kodu.
*   Te cztery filary współdziałają ze sobą, tworząc potężny paradygmat do budowy solidnego, skalowalnego i łatwego w utrzymaniu oprogramowania.

**Typowe pytania egzaminacyjne:**
*   Jaka jest różnica między klasą a obiektem? Proszę podać analogię.
*   Proszę opisać cztery podstawowe filary programowania obiektowego.
*   Na czym polega mechanizm dziedziczenia i jakie przynosi korzyści?
*   Co to jest polimorfizm i jakie ma praktyczne zastosowanie? Proszę podać przykład.
*   Jaki jest cel stosowania hermetyzacji?

---

# 35. Podstawowe struktury danych: tablica, lista, stos, kolejka, drzewo, graf

#### Wprowadzenie

Struktura danych to fundamentalne pojęcie w informatyce, oznaczające konkretny sposób organizacji, przechowywania i zarządzania danymi w pamięci komputera. Wybór odpowiedniej struktury danych jest kluczowy dla efektywności algorytmów, które na tych danych operują. Różne struktury oferują różne kompromisy pod względem szybkości wykonywania operacji (takich jak dodawanie, usuwanie, wyszukiwanie) oraz zapotrzebowania na pamięć. Zrozumienie właściwości podstawowych struktur danych – tablicy, listy, stosu, kolejki, drzewa i grafu – jest niezbędne do pisania wydajnego i dobrze zorganizowanego kodu.

#### Liniowe struktury danych

Charakteryzują się tym, że elementy są ułożone w sekwencji, jeden po drugim.

**1. Tablica (Array):**

*   **Opis:** Najprostsza struktura danych. Jest to zbiór elementów tego samego typu, przechowywanych w **ciągłym bloku pamięci**. Każdy element ma swój unikalny **indeks** (numer porządkowy, zazwyczaj od 0), który pozwala na natychmiastowy dostęp do niego.
*   **Zalety:** Bardzo szybki dostęp do dowolnego elementu (`O(1)`), jeśli znamy jego indeks.
*   **Wady:** Zazwyczaj ma stały, niezmienny rozmiar, określony w momencie tworzenia. Wstawianie lub usuwanie elementu w środku tablicy jest bardzo kosztowne (`O(n)`), ponieważ wymaga przesunięcia wszystkich kolejnych elementów.

**2. Lista (Linked List):**

*   **Opis:** Zbiór elementów (węzłów), które nie muszą być przechowywane w ciągłej pamięci. Każdy węzeł zawiera dane oraz **wskaźnik (referencję)** do następnego węzła w sekwencji. Wyróżniamy listy jednokierunkowe i dwukierunkowe (gdzie każdy węzeł ma też wskaźnik do poprzednika).
*   **Zalety:** Dynamiczny rozmiar. Łatwe i szybkie wstawianie oraz usuwanie elementów w dowolnym miejscu (`O(1)`), jeśli mamy wskaźnik na sąsiedni element.
*   **Wady:** Brak bezpośredniego dostępu do elementów. Aby znaleźć n-ty element, trzeba przejść przez `n-1` poprzednich (złożoność `O(n)`). Wymaga dodatkowej pamięci na przechowywanie wskaźników.

**3. Stos (Stack):**

*   **Opis:** Abstrakcyjna struktura danych działająca zgodnie z zasadą **LIFO (Last-In, First-Out) – ostatni na wejściu, pierwszy na wyjściu**. Operacje można wykonywać tylko na jednym końcu, zwanym **wierzchołkiem stosu**.
*   **Operacje:**
    *   `push(element)`: Dodaje element na wierzch stosu.
    *   `pop()`: Usuwa i zwraca element z wierzchołka stosu.
*   **Analogia:** Stos talerzy – możemy położyć nowy talerz tylko na wierzchu i zdjąć tylko ten, który jest na samej górze.
*   **Implementacja:** Może być łatwo zaimplementowany za pomocą tablicy lub listy.
*   **Zastosowanie:** Historia operacji (Cofnij/Undo), analiza wyrażeń matematycznych, zarządzanie wywołaniami funkcji w programie (stos wywołań).

**4. Kolejka (Queue):**

*   **Opis:** Abstrakcyjna struktura danych działająca zgodnie z zasadą **FIFO (First-In, First-Out) – pierwszy na wejściu, pierwszy na wyjściu**.
*   **Operacje:**
    *   `enqueue(element)`: Dodaje element na koniec kolejki.
    *   `dequeue()`: Usuwa i zwraca element z początku kolejki.
*   **Analogia:** Kolejka ludzi w sklepie – pierwsza osoba, która weszła, jest pierwszą obsłużoną.
*   **Implementacja:** Może być zaimplementowana za pomocą listy powiązanej lub specjalnej tablicy cyklicznej.
*   **Zastosowanie:** Buforowanie danych, szeregowanie zadań w systemach operacyjnych, algorytmy przeszukiwania grafów (BFS).

#### Nieliniowe struktury danych

Charakteryzują się bardziej złożonymi, hierarchicznymi lub sieciowymi powiązaniami między elementami.

**5. Drzewo (Tree):**

*   **Opis:** Hierarchiczna struktura danych składająca się z węzłów połączonych krawędziami. Posiada jeden wyróżniony węzeł – **korzeń (root)**. Każdy węzeł (oprócz korzenia) ma dokładnie jednego rodzica i może mieć wiele dzieci. Węzły bez dzieci to **liście (leaves)**.
*   **Drzewo binarne:** Specjalny typ drzewa, w którym każdy węzeł ma co najwyżej dwoje dzieci (lewe i prawe).
*   **Binarne drzewo poszukiwań (BST - Binary Search Tree):** Uporządkowane drzewo binarne, w którym dla każdego węzła wszystkie wartości w jego lewym poddrzewie są mniejsze, a w prawym poddrzewie – większe. Pozwala to na bardzo szybkie wyszukiwanie, wstawianie i usuwanie elementów (średnio `O(log n)`).
*   **Zastosowanie:** Reprezentacja hierarchii (np. system plików, struktura dokumentu HTML - DOM), binarne drzewa poszukiwań, implementacja tablic symboli.

**6. Graf (Graph):**

*   **Opis:** Najbardziej ogólna struktura danych. Składa się ze zbioru **wierzchołków (vertices)** i zbioru **krawędzi (edges)**, które łączą pary wierzchołków. W przeciwieństwie do drzew, grafy nie mają hierarchicznej struktury ani wyróżnionego korzenia.
*   **Rodzaje:**
    *   **Nieskierowany:** Krawędzie są dwukierunkowe (połączenie z A do B jest tym samym co z B do A).
    *   **Skierowany:** Krawędzie mają określony kierunek.
    *   **Ważony:** Każda krawędź ma przypisaną wagę (koszt).
*   **Reprezentacja w pamięci:**
    *   **Macierz sąsiedztwa:** Dwuwymiarowa tablica, gdzie `M[i][j] = 1` jeśli istnieje krawędź między wierzchołkiem `i` a `j`.
    *   **Lista sąsiedztwa:** Dla każdego wierzchołka przechowujemy listę jego sąsiadów.
*   **Zastosowanie:** Modelowanie sieci (komputerowych, społecznościowych, drogowych), analiza zależności, znajdowanie najkrótszych ścieżek.

#### Podsumowanie

| Struktura | Dostęp | Wstawianie/Usuwanie | Główne cechy |
|---|---|---|---|
| **Tablica** | `O(1)` (przez indeks) | `O(n)` (w środku) | Ciągła pamięć, stały rozmiar. |
| **Lista** | `O(n)` | `O(1)` (jeśli znamy sąsiada) | Dynamiczny rozmiar, nieciągła pamięć. |
| **Stos** | `O(1)` (na wierzchołku) | `O(1)` (na wierzchołku) | LIFO (Last-In, First-Out). |
| **Kolejka** | `O(1)` (na końcach) | `O(1)` (na końcach) | FIFO (First-In, First-Out). |
| **Drzewo (BST)** | `O(log n)` | `O(log n)` | Struktura hierarchiczna, szybkie wyszukiwanie. |
| **Graf** | - | - | Modelowanie dowolnych relacji i sieci. |

*   Wybór struktury danych to kluczowa decyzja projektowa, która ma bezpośredni wpływ na wydajność programu.
*   **Tablice** są idealne, gdy potrzebujemy szybkiego dostępu do elementów, a ich liczba jest znana. **Listy** sprawdzają się, gdy często dodajemy i usuwamy elementy.
*   **Stosy i kolejki** to abstrakcyjne typy danych o specyficznych regułach dostępu (LIFO/FIFO), używane w wielu algorytmach.
*   **Drzewa i grafy** pozwalają modelować złożone, nieliniowe relacje między danymi.

**Typowe pytania egzaminacyjne:**
*   Proszę porównać tablicę i listę, wskazując ich wady i zalety.
*   Na czym polega zasada LIFO i FIFO? Które struktury danych je implementują?
*   Do czego służy binarne drzewo poszukiwań (BST)?
*   Jakie są dwa główne sposoby reprezentacji grafu w pamięci komputera?
*   Podaj przykład zastosowania dla stosu i dla kolejki.

---

# 36. Algorytmy sortowania: bąbelkowe, przez wstawianie, przez wybór, szybkie, przez scalanie

#### Wprowadzenie

Sortowanie, czyli porządkowanie zbioru danych według określonego klucza (np. rosnąco lub malejąco), jest jednym z najbardziej fundamentalnych i wszechobecnych problemów w informatyce. Istnieje wiele różnych algorytmów sortowania, które różnią się od siebie podejściem, wydajnością (złożonością obliczeniową) i zapotrzebowaniem na pamięć. Zrozumienie, jak działają najważniejsze z nich oraz jakie są ich wady i zalety, jest kluczowe dla wyboru odpowiedniej metody w zależności od specyfiki problemu. Algorytmy sortowania dzieli się zazwyczaj na dwie grupy: proste (ale nieefektywne) oraz zaawansowane (znacznie wydajniejsze).

#### Proste algorytmy sortowania – złożoność O(n²)

Te algorytmy są łatwe do zrozumienia i zaimplementowania, ale ich kwadratowa złożoność czasowa sprawia, że są niepraktyczne dla dużych zbiorów danych.

**1. Sortowanie bąbelkowe (Bubble Sort):**

*   **Idea:** Wielokrotne przechodzenie przez zbiór i porównywanie par sąsiednich elementów. Jeśli są one w złej kolejności, zamieniane są miejscami. Proces jest powtarzany do momentu, aż podczas jednego pełnego przejścia nie dokona się żadna zamiana. Nazwa pochodzi od efektu "wypływania" największych (lub najmniejszych) elementów na koniec zbioru, niczym bąbelki powietrza.
*   **Złożoność czasowa:** O(n²) w przypadku średnim i pesymistycznym. O(n) w optymistycznym (gdy dane są już posortowane, a algorytm ma flagę sprawdzającą, czy dokonano zamiany).
*   **Zalety:** Bardzo prosta implementacja.
*   **Wady:** Ekstremalnie niewydajny, nawet dla niewielkich zbiorów danych. Ma głównie wartość edukacyjną.

**2. Sortowanie przez wstawianie (Insertion Sort):**

*   **Idea:** Dzieli zbiór na dwie części: posortowaną i nieposortowaną. Algorytm pobiera kolejne elementy z części nieposortowanej i wstawia je w odpowiednie miejsce w części posortowanej, przesuwając w prawo większe elementy, aby zrobić miejsce.
*   **Analogia:** Przypomina sortowanie kart w ręku – bierzemy nową kartę i wsuwamy ją w odpowiednie miejsce wśród już posiadanych, posortowanych kart.
*   **Złożoność czasowa:** O(n²) w przypadku średnim i pesymistycznym. O(n) w optymistycznym (gdy dane są posortowane).
*   **Zalety:** Prosta implementacja. Jest to algorytm **adaptacyjny** – bardzo wydajny dla danych, które są już częściowo posortowane.
*   **Wady:** Niewydajny dla dużych, losowych zbiorów danych.

**3. Sortowanie przez wybór (Selection Sort):**

*   **Idea:** Również dzieli zbiór na część posortowaną i nieposortowaną. W każdym przejściu algorytm znajduje najmniejszy (lub największy) element w części nieposortowanej i zamienia go miejscami z pierwszym elementem tej części, tym samym rozszerzając część posortowaną o jeden element.
*   **Złożoność czasowa:** Zawsze O(n²), niezależnie od początkowego uporządkowania danych.
*   **Zalety:** Prosta koncepcja. Wykonuje minimalną możliwą liczbę zamian elementów (co najwyżej n-1), co może być zaletą, gdy operacja zamiany jest bardzo kosztowna.
*   **Wady:** Niewydajny i nieadaptacyjny (zawsze wykonuje tyle samo porównań).

#### Zaawansowane algorytmy sortowania – złożoność O(n log n)

Te algorytmy wykorzystują bardziej zaawansowane techniki (głównie rekurencję i metodę "dziel i zwyciężaj"), aby osiągnąć znacznie lepszą wydajność, która pozwala na sortowanie milionów elementów w rozsądnym czasie.

**4. Sortowanie szybkie (Quicksort):**

*   **Idea:** Jeden z najpopularniejszych i najszybszych algorytmów sortowania. Działa na zasadzie **"dziel i zwyciężaj"**.
    1.  **Podział (Partition):** Wybierz jeden element ze zbioru, zwany **pivotem** (lub elementem osiowym). Przemebluj zbiór tak, aby wszystkie elementy mniejsze od pivota znalazły się przed nim, a wszystkie większe – za nim. Pivot trafia na swoją ostateczną, posortowaną pozycję.
    2.  **Zwyciężaj (Conquer):** Rekurencyjnie zastosuj sortowanie szybkie dla dwóch podzbiorów (elementów mniejszych od pivota i elementów większych od pivota).
*   **Złożoność czasowa:** O(n log n) w przypadku średnim i optymistycznym. **O(n²) w przypadku pesymistycznym**, który występuje, gdy jako pivot systematycznie wybierany jest element najmniejszy lub największy (np. w już posortowanej tablicy przy naiwnym wyborze pivota). W praktyce stosuje się techniki losowego wyboru pivota, aby tego uniknąć.
*   **Zalety:** Bardzo szybki w praktyce (małe stałe w złożoności). Jest algorytmem działającym **w miejscu (in-place)**, co oznacza, że nie wymaga dodatkowej pamięci (lub wymaga jej bardzo mało, O(log n) na stosie rekurencji).
*   **Wady:** Niestabilny. Wrażliwy na pesymistyczny przypadek.

**5. Sortowanie przez scalanie (Merge Sort):**

*   **Idea:** Klasyczny przykład algorytmu **"dziel i zwyciężaj"**.
    1.  **Dziel (Divide):** Dziel zbiór na dwie równe połowy.
    2.  **Zwyciężaj (Conquer):** Rekurencyjnie sortuj obie połowy.
    3.  **Łącz (Combine/Merge):** Scal dwie posortowane już połowy w jeden posortowany zbiór. Krok scalania polega na jednoczesnym przeglądaniu obu podzbiorów i wybieraniu mniejszego elementu do wynikowej tablicy.
*   **Złożoność czasowa:** Zawsze O(n log n), niezależnie od początkowego ułożenia danych. Jest to jego największa zaleta.
*   **Zalety:** Gwarantowana wydajność O(n log n). Jest to algorytm **stabilny** (nie zmienia względnej kolejności równych elementów).
*   **Wady:** W typowej implementacji **nie działa w miejscu** – wymaga dodatkowej pamięci o rozmiarze O(n) na potrzeby operacji scalania.

#### Porównanie złożoności algorytmów sortowania

| Algorytm | Złożoność średnia | Złożoność pesymistyczna | Złożoność pamięciowa | Stabilność |
|---|---|---|---|---|
| Bąbelkowe | O(n²) | O(n²) | O(1) | Tak |
| Przez wstawianie | O(n²) | O(n²) | O(1) | Tak |
| Przez wybór | O(n²) | O(n²) | O(1) | Nie |
| **Szybkie (Quicksort)** | **O(n log n)** | O(n²) | O(log n) | Nie |
| **Przez scalanie (Merge Sort)** | **O(n log n)** | **O(n log n)** | O(n) | Tak |

#### Podsumowanie

*   Algorytmy sortowania można podzielić na proste, o złożoności **O(n²)** (bąbelkowe, przez wstawianie, przez wybór), oraz zaawansowane, o złożoności **O(n log n)** (szybkie, przez scalanie).
*   **Sortowanie bąbelkowe i przez wybór** mają głównie wartość historyczną i edukacyjną ze względu na bardzo niską wydajność.
*   **Sortowanie przez wstawianie** jest przydatne dla małych lub częściowo posortowanych zbiorów.
*   **Sortowanie szybkie (Quicksort)** jest w praktyce jednym z najszybszych algorytmów ogólnego przeznaczenia, ale jego wydajność w pesymistycznym przypadku jest słaba.
*   **Sortowanie przez scalanie (Merge Sort)** gwarantuje wydajność O(n log n) w każdym przypadku, ale wymaga dodatkowej pamięci.
*   Wybór algorytmu sortowania jest kompromisem między gwarantowaną wydajnością, zapotrzebowaniem na pamięć i stabilnością.

**Typowe pytania egzaminacyjne:**
*   Proszę opisać zasadę działania sortowania bąbelkowego.
*   Na czym polega metoda "dziel i zwyciężaj" na przykładzie sortowania szybkiego lub przez scalanie?
*   Proszę porównać złożoność obliczeniową sortowania szybkiego i przez scalanie w przypadku średnim i pesymistycznym.
*   Który z prostych algorytmów sortowania jest najwydajniejszy dla danych częściowo posortowanych?
*   Co to znaczy, że algorytm sortowania jest stabilny?

---

# 37. Algorytmy wyszukiwania: liniowe, binarne

#### Wprowadzenie

Wyszukiwanie, czyli proces odnajdywania określonego elementu (lub jego pozycji) w zbiorze danych, jest jedną z najczęściej wykonywanych operacji w programowaniu. Podobnie jak w przypadku sortowania, istnieje wiele algorytmów realizujących to zadanie, a ich efektywność zależy w dużej mierze od tego, czy zbiór danych jest uporządkowany. Dwa najbardziej fundamentalne algorytmy wyszukiwania to **wyszukiwanie liniowe**, które działa na każdym zbiorze, oraz znacznie wydajniejsze **wyszukiwanie binarne**, które wymaga, aby zbiór był posortowany.

#### Wyszukiwanie liniowe (Linear Search)

*   **Idea:** Najprostszy możliwy algorytm wyszukiwania, znany również jako wyszukiwanie sekwencyjne. Polega na przeglądaniu zbioru danych **element po elemencie**, od początku do końca, i porównywaniu każdego elementu z wartością szukaną. Proces kończy się, gdy element zostanie znaleziony (sukces) lub gdy dojdziemy do końca zbioru bez jego odnalezienia (porażka).
*   **Warunek wstępny:** Brak. Algorytm działa zarówno na zbiorach posortowanych, jak i nieposortowanych.
*   **Zasada działania:**
    1.  Zacznij od pierwszego elementu w zbiorze (indeks 0).
    2.  Porównaj bieżący element z wartością szukaną.
    3.  Jeśli są równe, zwróć pozycję (indeks) bieżącego elementu i zakończ.
    4.  Jeśli nie są równe, przejdź do następnego elementu.
    5.  Jeśli przejrzano cały zbiór i nie znaleziono elementu, zwróć informację o niepowodzeniu (np. wartość -1).
*   **Złożoność czasowa:**
    *   **Pesymistyczna:** O(n). Występuje, gdy szukany element znajduje się na samym końcu zbioru lub nie ma go wcale. Musimy wtedy przejrzeć wszystkie `n` elementów.
    *   **Średnia:** O(n). Średnio musimy przejrzeć połowę zbioru.
    *   **Optymistyczna:** O(1). Występuje, gdy szukany element jest pierwszym elementem zbioru.
*   **Zalety:** Prostota implementacji. Działa na każdym rodzaju zbioru liniowego, bez względu na uporządkowanie.
*   **Wady:** Bardzo niska wydajność dla dużych zbiorów danych.

**Przykład (Python):**
```python
def linear_search(data, target):
    for i in range(len(data)):
        if data[i] == target:
            return i  # Znaleziono, zwróć indeks
    return -1         # Nie znaleziono
```

#### Wyszukiwanie binarne (Binary Search)

*   **Idea:** Znacznie wydajniejszy algorytm, który działa na zasadzie **"dziel i zwyciężaj"**. Jego działanie można porównać do szukania słowa w słowniku lub książce telefonicznej. Zamiast przeglądać strona po stronie, otwieramy książkę mniej więcej w połowie i sprawdzamy, czy szukane słowo jest przed czy po otwartej stronie. Następnie powtarzamy ten proces dla odpowiedniej połowy, za każdym razem redukując przeszukiwany obszar o połowę.
*   **Warunek wstępny:** Zbiór danych **musi być posortowany**.
*   **Zasada działania:**
    1.  Ustaw wskaźniki na początek (`left`) i koniec (`right`) przeszukiwanego zbioru.
    2.  Dopóki `left <= right`:
        a. Znajdź środkowy element: `mid = (left + right) // 2`.
        b. Porównaj środkowy element z wartością szukaną:
           *   Jeśli są równe – element został znaleziony. Zwróć jego pozycję (`mid`) i zakończ.
           *   Jeśli szukany element jest **mniejszy** od środkowego – odrzuć prawą połowę zbioru, ustawiając `right = mid - 1`.
           *   Jeśli szukany element jest **większy** od środkowego – odrzuć lewą połowę zbioru, ustawiając `left = mid + 1`.
    3.  Jeśli pętla się zakończy (czyli `left > right`), oznacza to, że elementu nie ma w zbiorze. Zwróć informację o niepowodzeniu.
*   **Złożoność czasowa:**
    *   **Pesymistyczna:** O(log n). W każdym kroku redukujemy problem o połowę. Liczba kroków potrzebnych do przeszukania zbioru o wielkości `n` jest logarytmiczna.
    *   **Średnia:** O(log n).
    *   **Optymistyczna:** O(1). Występuje, gdy szukany element jest pierwszym sprawdzonym elementem środkowym.
*   **Zalety:** Ekstremalnie wydajne, nawet dla bardzo dużych zbiorów danych. Dla miliona elementów wyszukiwanie binarne potrzebuje co najwyżej około 20 porównań, podczas gdy liniowe – miliona.
*   **Wady:** Wymaga, aby zbiór był posortowany. Jeśli dane nie są posortowane, koszt ich wcześniejszego posortowania (zazwyczaj O(n log n)) może przewyższyć korzyści z szybkiego wyszukiwania, zwłaszcza jeśli wyszukiwanie wykonujemy tylko raz.

**Przykład (Python):**
```python
def binary_search(sorted_data, target):
    left, right = 0, len(sorted_data) - 1
    while left <= right:
        mid = (left + right) // 2
        if sorted_data[mid] == target:
            return mid
        elif target < sorted_data[mid]:
            right = mid - 1
        else:
            left = mid + 1
    return -1
```

#### Porównanie wyszukiwania liniowego i binarnego

| Cecha | Wyszukiwanie liniowe | Wyszukiwanie binarne |
|---|---|---|
| **Warunek wstępny** | Brak | Zbiór musi być posortowany |
| **Złożoność czasowa** | O(n) | O(log n) |
| **Podejście** | Sekwencyjne | Dziel i zwyciężaj |
| **Wydajność dla dużych `n`** | Bardzo niska | Bardzo wysoka |
| **Zastosowanie** | Małe lub nieposortowane zbiory | Duże, posortowane zbiory |

#### Podsumowanie

*   **Wyszukiwanie liniowe** to prosty, sekwencyjny algorytm o złożoności **O(n)**, który działa na każdym zbiorze, ale jest nieefektywny dla dużych danych.
*   **Wyszukiwanie binarne** to bardzo wydajny algorytm o złożoności **O(log n)**, który działa na zasadzie "dziel i zwyciężaj", ale **wymaga, aby dane były wcześniej posortowane**.
*   Wybór między tymi dwoma algorytmami jest fundamentalnym kompromisem w programowaniu: jeśli dane są nieposortowane i wyszukujemy w nich rzadko, wyszukiwanie liniowe może wystarczyć. Jeśli jednak wyszukiwanie jest częstą operacją na dużym zbiorze, koszt jednorazowego posortowania danych (złożoność O(n log n)) i późniejszego wielokrotnego stosowania wyszukiwania binarnego (złożoność O(log n)) jest niemal zawsze opłacalny.

**Typowe pytania egzaminacyjne:**
*   Proszę opisać zasadę działania wyszukiwania liniowego i binarnego.
*   Jaki jest podstawowy warunek, który musi spełniać zbiór danych, aby można było zastosować wyszukiwanie binarne?
*   Proszę porównać złożoność obliczeniową wyszukiwania liniowego i binarnego.
*   W jakiej sytuacji zastosowanie wyszukiwania binarnego może nie być opłacalne, mimo że jest ono znacznie szybsze?
*   Ile w przybliżeniu porównań wykona wyszukiwanie binarne dla zbioru liczącego 1024 elementy?

---

# 38. Algorytmy grafowe: przeszukiwanie wszerz i w głąb, algorytm Dijkstry, algorytmy Kruskala i Prima

#### Wprowadzenie

Grafy są jedną z najbardziej uniwersalnych struktur danych, pozwalającą modelować złożone relacje i sieci w wielu dziedzinach – od sieci komputerowych i drogowych, przez sieci społecznościowe, po analizę zależności w projektach. Algorytmy grafowe to potężne narzędzia, które pozwalają na analizę tych struktur i rozwiązywanie praktycznych problemów, takich jak znajdowanie połączeń, wyznaczanie najkrótszych ścieżek czy tworzenie optymalnych sieci. Do najważniejszych i najbardziej fundamentalnych algorytmów grafowych należą algorytmy przeszukiwania (BFS i DFS), algorytm Dijkstry oraz algorytmy poszukiwania minimalnego drzewa rozpinającego (Kruskala i Prima).

#### Przeszukiwanie grafu

Przeszukiwanie grafu (lub przechodzenie grafu) polega na systematycznym odwiedzaniu wszystkich jego wierzchołków w określonej kolejności. Dwa podstawowe algorytmy realizujące to zadanie to BFS i DFS.

**1. Przeszukiwanie wszerz (BFS - Breadth-First Search):**

*   **Idea:** Algorytm eksploruje graf "warstwa po warstwie". Zaczynając od wierzchołka startowego, najpierw odwiedza wszystkich jego bezpośrednich sąsiadów, następnie sąsiadów tych sąsiadów, i tak dalej.
*   **Struktura danych:** Wykorzystuje **kolejkę (FIFO)** do przechowywania wierzchołków do odwiedzenia.
*   **Zasada działania:**
    1.  Dodaj wierzchołek startowy do kolejki i oznacz go jako odwiedzony.
    2.  Dopóki kolejka nie jest pusta:
        a. Pobierz wierzchołek `u` z początku kolejki.
        b. Dla każdego nieodwiedzonego sąsiada `v` wierzchołka `u`:
           i. Oznacz `v` jako odwiedzony.
           ii. Dodaj `v` na koniec kolejki.
*   **Zastosowanie:** Znajdowanie **najkrótszej ścieżki** w grafach nieważonych (pod względem liczby krawędzi), testowanie spójności grafu, wykrywanie cykli.

**2. Przeszukiwanie w głąb (DFS - Depth-First Search):**

*   **Idea:** Algorytm eksploruje graf, podążając jedną ścieżką tak głęboko, jak to możliwe. Gdy dotrze do "ślepego zaułka" (wierzchołka bez nieodwiedzonych sąsiadów), cofa się i próbuje eksplorować inną, alternatywną ścieżkę.
*   **Struktura danych:** Wykorzystuje **stos (LIFO)** (jawnie lub niejawnie poprzez rekurencję) do przechowywania wierzchołków.
*   **Zasada działania (rekurencyjna):**
    1.  Oznacz wierzchołek startowy `u` jako odwiedzony.
    2.  Dla każdego nieodwiedzonego sąsiada `v` wierzchołka `u`:
        a. Wywołaj rekurencyjnie DFS dla `v`.
*   **Zastosowanie:** Wykrywanie cykli w grafie, sortowanie topologiczne (porządkowanie zadań z zależnościami), znajdowanie spójnych składowych.

| Cecha | BFS (wszerz) | DFS (w głąb) |
|---|---|---|
| **Struktura danych** | Kolejka (FIFO) | Stos (LIFO) / Rekurencja |
| **Kolejność odwiedzania** | Warstwa po warstwie | Jak najgłębiej jedną ścieżką |
| **Znajdowanie ścieżki** | Znajduje najkrótszą ścieżkę (w grafie nieważonym) | Znajduje dowolną ścieżkę |

#### Algorytm Dijkstry – najkrótsza ścieżka z jednego źródła

*   **Problem:** Znalezienie najkrótszych ścieżek z jednego, wybranego wierzchołka startowego do wszystkich pozostałych wierzchołków w **grafie ważonym, w którym wagi krawędzi są nieujemne**.
*   **Idea:** Jest to algorytm **zachłanny**. Utrzymuje zbiór wierzchołków, do których najkrótsza ścieżka jest już znana. W każdym kroku, spośród wierzchołków spoza tego zbioru, wybiera ten, do którego prowadzi aktualnie najkrótsza znana ścieżka, i dodaje go do zbioru. Następnie aktualizuje (relaksuje) odległości do jego sąsiadów.
*   **Zasada działania:**
    1.  Ustaw odległość do wierzchołka startowego na 0, a do wszystkich innych na nieskończoność.
    2.  Stwórz kolejkę priorytetową zawierającą wszystkie wierzchołki (priorytetem jest odległość).
    3.  Dopóki kolejka nie jest pusta:
        a. Wybierz i usuń z kolejki wierzchołek `u` o najmniejszej odległości.
        b. Dla każdego sąsiada `v` wierzchołka `u`:
           i. Jeśli nowa ścieżka do `v` (przez `u`) jest krótsza niż dotychczas znana (`odległość(u) + waga(u,v) < odległość(v)`), zaktualizuj odległość do `v`.
*   **Zastosowanie:** Routing w sieciach komputerowych (np. protokół OSPF), nawigacja GPS.

#### Minimalne drzewo rozpinające (MST - Minimum Spanning Tree)

*   **Problem:** Dla danego spójnego, nieskierowanego i ważonego grafu, znaleźć podgraf, który jest drzewem, łączy wszystkie wierzchołki i ma **minimalną możliwą sumę wag krawędzi**. Innymi słowy, jak połączyć wszystkie miasta siecią dróg o minimalnym łącznym koszcie budowy?

**1. Algorytm Kruskala:**

*   **Idea:** Algorytm **zachłanny**, który buduje MST, dodając kolejne krawędzie w porządku rosnących wag, pod warunkiem, że dodanie krawędzi nie tworzy cyklu.
*   **Zasada działania:**
    1.  Stwórz listę wszystkich krawędzi i posortuj je rosnąco według wag.
    2.  Stwórz las, w którym każdy wierzchołek jest osobnym drzewem.
    3.  Przechodź przez posortowaną listę krawędzi. Dla każdej krawędzi `(u, v)`:
        a. Jeśli wierzchołki `u` i `v` należą do różnych drzew (sprawdzenie za pomocą struktury zbiorów rozłącznych), dodaj tę krawędź do MST i połącz drzewa zawierające `u` i `v`.
*   **Zastosowanie:** Projektowanie sieci (telekomunikacyjnych, energetycznych) o minimalnym koszcie.

**2. Algorytm Prima:**

*   **Idea:** Również algorytm **zachłanny**, ale działający inaczej. Zaczyna od jednego wierzchołka i "rozrasta" drzewo, w każdym kroku dodając do niego najtańszą krawędź, która łączy wierzchołek już będący w drzewie z wierzchołkiem spoza drzewa.
*   **Zasada działania:** Przypomina algorytm Dijkstry.
    1.  Zacznij od dowolnego wierzchołka i dodaj go do MST.
    2.  Użyj kolejki priorytetowej do przechowywania krawędzi łączących wierzchołki w MST z tymi spoza niego.
    3.  Dopóki MST nie obejmuje wszystkich wierzchołków:
        a. Wybierz z kolejki krawędź o najmniejszej wadze, która łączy wierzchołek `u` (w MST) z wierzchołkiem `v` (poza MST).
        b. Dodaj `v` i krawędź `(u,v)` do MST.
        c. Zaktualizuj kolejkę, dodając do niej krawędzie wychodzące z `v`.

#### Podsumowanie

*   **BFS i DFS** to fundamentalne algorytmy do przechodzenia grafu, różniące się strategią eksploracji (wszerz vs w głąb) i wykorzystywaną strukturą danych (kolejka vs stos).
*   **Algorytm Dijkstry** rozwiązuje problem najkrótszej ścieżki z jednego źródła w grafach z nieujemnymi wagami, działając na zasadzie zachłannej relaksacji krawędzi.
*   **Minimalne Drzewo Rozpinające (MST)** to podgraf o minimalnej sumie wag, łączący wszystkie wierzchołki. Dwa klasyczne algorytmy do jego znajdowania to:
    *   **Algorytm Kruskala**, który sortuje wszystkie krawędzie i dodaje najtańsze, które nie tworzą cyklu.
    *   **Algorytm Prima**, który "rozrasta" drzewo od jednego wierzchołka, dodając najtańsze krawędzie wychodzące.

**Typowe pytania egzaminacyjne:**
*   Proszę porównać algorytmy przeszukiwania wszerz (BFS) i w głąb (DFS).
*   Do czego służy algorytm Dijkstry i jakie jest jego główne ograniczenie?
*   Co to jest minimalne drzewo rozpinające (MST)?
*   Na czym polega różnica w podejściu między algorytmem Kruskala a algorytmem Prima?
*   Który algorytm przeszukiwania grafu należy użyć, aby znaleźć najkrótszą ścieżkę w grafie nieważonym?

---

# 39. Klasy złożoności P i NP, problemy NP-zupełne

#### Wprowadzenie

Teoria złożoności obliczeniowej to dziedzina informatyki teoretycznej, która klasyfikuje problemy obliczeniowe według ich wewnętrznej "trudności", czyli ilości zasobów (głównie czasu) potrzebnych do ich rozwiązania. W sercu tej teorii leżą klasy złożoności **P** i **NP** oraz pojęcie **problemów NP-zupełnych**. Kwestia relacji między klasami P i NP jest jednym z najważniejszych nierozwiązanych problemów w informatyce i matematyce, znanym jako **problem P vs NP**.

#### Klasa P (Polynomial Time)

*   **Definicja:** Klasa **P** zawiera wszystkie **problemy decyzyjne**, które mogą być rozwiązane przez deterministyczną maszynę Turinga (czyli standardowy komputer) w **czasie wielomianowym**. Oznacza to, że istnieje algorytm, którego złożoność czasowa jest ograniczona przez wielomian od rozmiaru danych wejściowych `n` (np. O(n), O(n²), O(n³)).
*   **Znaczenie:** Problemy należące do klasy P są uważane za **"łatwe"** lub **"obliczalnie trafnialne" (tractable)**. Oznacza to, że możemy dla nich napisać efektywne algorytmy, które znajdują rozwiązanie w rozsądnym czasie, nawet dla dużych danych wejściowych.
*   **Przykłady problemów w klasie P:**
    *   Sortowanie tablicy.
    *   Wyszukiwanie binarne.
    *   Mnożenie dwóch liczb.
    *   Znajdowanie najkrótszej ścieżki w grafie (algorytm Dijkstry).
    *   Znajdowanie minimalnego drzewa rozpinającego (algorytmy Kruskala i Prima).

#### Klasa NP (Nondeterministic Polynomial Time)

*   **Definicja (intuicyjna i najważniejsza):** Klasa **NP** zawiera wszystkie **problemy decyzyjne**, dla których, jeśli ktoś poda nam potencjalne rozwiązanie ("certyfikat"), jesteśmy w stanie **zweryfikować jego poprawność** w czasie wielomianowym.
*   **Analogia:** Rozwiązywanie Sudoku może być bardzo trudne i czasochłonne (znalezienie rozwiązania), ale jeśli ktoś poda nam wypełnioną planszę, bardzo szybko możemy sprawdzić, czy jest ona poprawnym rozwiązaniem (weryfikacja). Dlatego problem Sudoku należą do klasy NP.
*   **Ważna uwaga:** NP **nie** oznacza "nie-wielomianowy" (non-polynomial). Oznacza "niedeterministyczny wielomianowy". Nazwa pochodzi od formalnej definicji, mówiącej, że problemy te mogą być rozwiązane w czasie wielomianowym na hipotetycznej **niedeterministycznej maszynie Turinga** (maszynie, która potrafi "odgadnąć" właściwą ścieżkę obliczeń).
*   **Relacja do P:** Każdy problem z klasy P należą też do NP. Jeśli potrafimy coś szybko rozwiązać, to tym bardziej potrafimy szybko zweryfikować podane rozwiązanie (po prostu je ignorując i rozwiązując problem od zera). Zatem **P ⊆ NP**.

#### Problem P vs NP

Największe pytanie w teorii złożoności brzmi: **Czy P = NP?**

*   **Co by oznaczało, gdyby P = NP?** Oznaczałoby to, że każdy problem, dla którego można szybko zweryfikować rozwiązanie, można również szybko rozwiązać. Kreatywność zrównałaby się z umiejętnością weryfikacji. Miałoby to niewyobrażalne konsekwencje, np. łamanie większości współczesnych systemów kryptograficznych, automatyczne dowodzenie twierdzeń matematycznych, rewolucję w projektowaniu lekow i logistyce.
*   **Co by oznaczało, gdyby P ≠ NP?** Oznaczałoby to, że istnieją problemy, które są fundamentalnie **"trudne"** – łatwo sprawdzić ich rozwiązanie, ale znalezienie go jest obliczeniowo niewykonalne dla dużych instancji. Byłoby to potwierdzenie, że pewne problemy są po prostu poza zasięgiem efektywnych algorytmów.

**Stan obecny:** Powszechnie uważana się, że **P ≠ NP**, ale nikt do tej pory nie był w stanie tego udowodnić. Jest to jeden z siedmiu Problemów Milenijnych, za którego rozwiązanie Instytut Matematyczny Claya oferuje nagrodę miliona dolarów.

#### Problemy NP-zupełne (NP-Complete, NPC)

*   **Idea:** W obrębie klasy NP znajdują się problemy, które są uważane za **"najtrudniejsze" problemy w NP**. Tworzą one podklasę NP-zupełną.
*   **Definicja:** Problem decyzyjny jest NP-zupełny, jeśli spełnia dwa warunki:
    1.  **Należą do klasy NP** (można szybko zweryfikować jego rozwiązanie).
    2.  **Jest NP-trudny (NP-hard)**, co oznacza, że każdy inny problem z klasy NP można do niego **zredukować w czasie wielomianowym**.
*   **Redukcja wielomianowa:** To technika, która pozwala przekształcić dowolną instancję problemu A w instancję problemu B w czasie wielomianowym, tak że rozwiązanie dla B daje nam rozwiązanie dla A. Mówiąc prościej, jeśli problem A redukuje się do B, to B jest co najmniej tak trudny jak A.
*   **Znaczenie:** Jeśli ktokolwiek znalazłby efektywny (wielomianowy) algorytm dla **choćby jednego** problemu NP-zupełnego, oznaczałoby to, że można efektywnie rozwiązać **wszystkie** problemy w NP, co dowiodłoby, że P = NP.
*   **Przykłady problemów NP-zupełnych:**
    *   **Problem spełnialności formuł boole'owskich (SAT):** Czy dla danej formuły logicznej istnieje takie przypisanie wartości (prawda/fałsz) zmiennym, aby cała formuła była prawdziwa? (Historycznie pierwszy problem, dla którego udowodniono NP-zupełność – twierdzenie Cooka-Levina).
    *   **Problem komiwojażera (wersja decyzyjna):** Czy istnieje trasa o długości nie większej niż `k`, która odwiedza każde miasto dokładnie raz?
    *   **Problem kolorowania grafu:** Czy można pokolorować wierzchołki grafu używając co najwyżej `k` kolorów, tak aby żadne dwa sąsiednie wierzchołki nie miały tego samego koloru?
    *   **Problem plecakowy (wersja decyzyjna).**
    *   **Problem cyklu Hamiltona.**

#### Podsumowanie

*   **Klasa P:** Problemy rozwiązywalne w czasie wielomianowym ("łatwe").
*   **Klasa NP:** Problemy, których rozwiązania można zweryfikować w czasie wielomianowym ("łatwe do sprawdzenia").
*   **P vs NP:** Nierozwiązane pytanie, czy P = NP. Powszechnie uważana się, że nie.
*   **Problemy NP-zupełne (NPC):** "Najtrudniejsze" problemy w klasie NP. Znalezienie efektywnego rozwiązania dla jednego z nich oznacza znalezienie rozwiązania dla wszystkich problemów w NP.
*   W praktyce, gdy okazuje się, że problem jest NP-zupełny, zazwyczaj porzuca się poszukiwania dokładnego, efektywnego algorytmu na rzecz **algorytmów aproksymacyjnych** (dających rozwiązanie bliskie optymalnemu) lub **heurystyk** (które dobrze działają w typowych przypadkach, ale nie dają gwarancji).

**Typowe pytania egzaminacyjne:**
*   Co to jest klasa złożoności P, a co to jest klasa NP? Proszę podać intuicyjną definicję NP.
*   Jaka jest relacja między klasami P i NP?
*   Na czym polega problem P vs NP?
*   Co to jest problem NP-zupełny? Jakie dwa warunki musi spełniać?
*   Jakie jest znaczenie faktu, że problem jest NP-zupełny?

---

# 40. Grafika rastrowa i wektorowa, modele barw

#### Wprowadzenie

Grafika komputerowa to dziedzina informatyki zajmująca się tworzeniem i manipulowaniem obrazami za pomocą komputerów. Wszystkie obrazy cyfrowe, od prostych ikon po fotorealistyczne zdjęcia, muszą być w jakiś sposób reprezentowane w pamięci komputera. Istnieją dwa fundamentalnie różne podejścia do tej reprezentacji: **grafika rastrowa** i **grafika wektorowa**. Różnią się one sposobem opisu obrazu, co ma kluczowe konsekwencje dla ich właściwości, zastosowań i możliwości edycji. Niezależnie od sposobu reprezentacji, kluczowym elementem obrazu jest kolor, który jest opisywany za pomocą **modeli barw**.

#### Grafika rastrowa (Bitmapowa)

*   **Sposób reprezentacji:** Obraz jest reprezentowany jako **prostokątna siatka (mapa) małych, pojedynczych punktów zwanych pikselami**. Każdy piksel ma przypisany określony kolor. Jakość i szczegółowość obrazu zależą od jego **rozdzielczości** (liczby pikseli w poziomie i pionie, np. 1920x1080) oraz **głębi kolorów** (liczby bitów użytych do opisania koloru jednego piksela).
*   **Analogia:** Obraz rastrowy przypomina mozaikę lub obraz namalowany na kartce w kratkę, gdzie każda kratka jest zamalowana jednym, jednolitym kolorem.
*   **Skalowanie:** Największą wadą grafiki rastrowej jest **utrata jakości podczas skalowania (powiększania)**. Ponieważ obraz składa się ze stałej liczby pikseli, powiększenie go polega na powiększeniu poszczególnych pikseli, co prowadzi do efektu "pikselozy" – widocznych kwadratów i postrzępionych krawędzi.
*   **Zalety:**
    *   Idealna do reprezentacji obrazów o dużej złożoności tonalnej i kolorystycznej, takich jak **fotografie** i skomplikowane obrazy cyfrowe.
    *   Łatwość edycji na poziomie pojedynczych pikseli (np. retusz w programie Adobe Photoshop).
*   **Wady:**
    *   Utrata jakości przy skalowaniu.
    *   Duże rozmiary plików, zwłaszcza przy wysokiej rozdzielczości i głębi kolorów.
*   **Typowe formaty plików:** JPG/JPEG, PNG, GIF, BMP, TIFF.
*   **Oprogramowanie:** Adobe Photoshop, GIMP, Paint.

#### Grafika wektorowa

*   **Sposób reprezentacji:** Obraz jest opisywany nie za pomocą siatki pikseli, ale jako **zbiór obiektów geometrycznych (prymitywów)**, takich jak linie, krzywe (np. krzywe Béziera), okręgi i wielokąty. Te obiekty są zdefiniowane za pomocą **wzorów matematycznych**, które określają ich kształt, położenie, kolor wypełnienia i obrysu.
*   **Analogia:** Obraz wektorowy przypomina instrukcję rysowania: "narysuj czerwoną linię z punktu A do punktu B, a następnie narysuj niebieskie koło o środku w punkcie C i promieniu R".
*   **Skalowanie:** Największą zaletą grafiki wektorowej jest **bezstratna skalowalność**. Ponieważ obraz jest opisany matematycznie, można go dowolnie powiększać lub pomniejszać bez jakiejkolwiek utraty jakości. Program po prostu przelicza wzory dla nowego rozmiaru i rysuje obiekty od nowa, zachowując idealnie gładkie krawędzie.
*   **Zalety:**
    *   Nieskończona skalowalność bez utraty jakości.
    *   Zazwyczaj małe rozmiary plików (przechowujemy wzory, a nie informacje o każdym pikselu).
    *   Łatwość edycji poszczególnych obiektów (zmiana kształtu, koloru, położenia).
*   **Wady:**
    *   Nie nadaje się do reprezentowania obrazów fotorealistycznych o złożonych przejściach tonalnych.
*   **Typowe formaty plików:** SVG, AI, EPS, CDR, PDF (może zawierać zarówno grafikę wektorową, jak i rastrową).
*   **Oprogramowanie:** Adobe Illustrator, Inkscape, CorelDRAW.

| Cecha | Grafika rastrowa | Grafika wektorowa |
|---|---|---|
| **Reprezentacja** | Siatka pikseli | Obiekty matematyczne |
| **Skalowanie** | Utrata jakości | Bezstratne |
| **Rozmiar pliku** | Duży | Mały |
| **Główne zastosowanie** | Fotografie, złożone obrazy | Logotypy, ikony, ilustracje, diagramy, czcionki |

#### Modele barw

Model barw to abstrakcyjny model matematyczny opisujący sposób, w jaki kolory mogą być reprezentowane jako zestawy liczb (współrzędnych). Dwa najczęściej używane modele w grafice komputerowej to RGB i CMYK.

**1. Model RGB (Red, Green, Blue):**

*   **Idea:** Model **addytywny**, używany w urządzeniach emitujących światło, takich jak **monitory, ekrany smartfonów, skanery**. Każdy kolor jest tworzony przez **mieszanie (dodawanie) światła** w trzech podstawowych barwach: czerwonej, zielonej i niebieskiej.
*   **Reprezentacja:** Kolor jest opisywany przez trzy wartości, zazwyczaj z zakresu 0-255, które określają intensywność każdej ze składowych.
    *   `RGB(0, 0, 0)` to kolor czarny (brak światła).
    *   `RGB(255, 255, 255)` to kolor biały (pełne natężenie wszystkich składowych).
    *   `RGB(255, 0, 0)` to czysta czerwień.

**2. Model CMYK (Cyan, Magenta, Yellow, Key):**

*   **Idea:** Model **subtraktywny**, używany w **druku**. Kolor powstaje przez **odejmowanie (pochłanianie) światła** od białej powierzchni (papieru) za pomocą nakładanych farb drukarskich: cyjanu, magenty i żółtego.
*   **Reprezentacja:** Kolor jest opisywany przez cztery wartości procentowe (0-100), które określają stopień pokrycia każdą z farb.
    *   `CMYK(0, 0, 0, 0)` to kolor biały (brak farby).
    *   Teoretycznie zmieszanie C, M i Y w 100% powinno dać czerń, ale w praktyce daje brudny brąz. Dlatego dodaje się czwartą, kluczową składową **K (Key)**, czyli czarną farbę, aby uzyskać głęboką czerń i oszczędzić tusz.

**Inne modele:**

*   **HSL/HSB (Hue, Saturation, Lightness/Brightness):** Bardziej intuicyjny dla człowieka model, który opisuje kolor przez jego **odcień** (Hue – pozycja na kole barw, 0-360°), **nasycenie** (Saturation – intensywność koloru, 0-100%) i **jasność** (Lightness/Brightness – 0-100%).

#### Podsumowanie

*   **Grafika rastrowa** opisuje obraz za pomocą siatki pikseli i jest idealna do zdjęć, ale traci jakość przy powiększaniu.
*   **Grafika wektorowa** opisuje obraz za pomocą wzorów matematycznych, co pozwala na bezstratne skalowanie i jest idealna do logotypów, ikon i ilustracji.
*   **Model RGB** to addytywny model barw (mieszanie światła) używany w wyświetlaczach.
*   **Model CMYK** to subtraktywny model barw (mieszanie farb) używany w druku.
*   Przygotowując projekt do wyświetlania na ekranie, należy pracować w przestrzeni barw RGB. Przygotowując projekt do druku, należy go skonwertować do CMYK.

**Typowe pytania egzaminacyjne:**
*   Proszę porównać grafikę rastrową i wektorową, wskazując ich główne wady i zalety.
*   Dlaczego grafika wektorowa skaluje się bezstratnie, a rastrowa nie?
*   Podaj przykład zastosowania dla grafiki rastrowej i wektorowej.
*   Na czym polega różnica między addytywnym modelem barw (RGB) a subtraktywnym (CMYK)?
*   Dlaczego w modelu CMYK stosuje się dodatkową, czarną farbę (K)?

---

# 41. Interfejsy użytkownika, interakcja człowiek-komputer, podstawowe zasady projektowania interfejsów

#### Wprowadzenie

**Interfejs użytkownika (UI - User Interface)** to przestrzeń, w której dochodzi do interakcji między człowiekiem a maszyną (komputerem, aplikacją, stroną internetową). Jest to wszystko, co użytkownik widzi, słyszy i z czym może wejść w interakcję, aby osiągnąć swój cel. Z kolei **interakcja człowiek-komputer (HCI - Human-Computer Interaction)** to szersza, interdyscyplinarna dziedzina nauki, która bada, projektuje i ocenia systemy interaktywne, koncentrując się na tym, aby były one użyteczne, łatwe w obsłudze i przyjemne dla użytkowników. Celem dobrego projektowania interfejsów jest stworzenie pomostu między możliwościami technologii a potrzebami i ograniczeniami człowieka.

#### Rodzaje interfejsów użytkownika

1.  **Graficzny interfejs użytkownika (GUI - Graphical User Interface):** Najpopularniejszy typ interfejsu. Użytkownik wchodzi w interakcję z systemem za pomocą wizualnych reprezentacji (okna, ikony, menu, przyciski) i urządzeń wskazujących (mysz, touchpad). *Przykład: systemy operacyjne Windows, macOS.*
2.  **Interfejs wiersza poleceń (CLI - Command-Line Interface):** Użytkownik komunikuje się z systemem, wpisując tekstowe polecenia. Wymaga znajomości składni, ale jest bardzo potężny i efektywny dla zaawansowanych użytkowników. *Przykład: terminal w Linuksie, wiersz poleceń w Windows.*
3.  **Interfejs głosowy (VUI - Voice User Interface):** Interakcja odbywa się za pomocą mowy. *Przykład: asystenci głosowi tacy jak Siri, Google Assistant, Alexa.*
4.  **Interfejs dotykowy:** Interakcja odbywa się poprzez dotyk ekranu. *Przykład: smartfony, tablety.*
5.  **Interfejs oparty na gestach:** System reaguje na ruchy ciała użytkownika. *Przykład: kontroler Kinect.*

#### Interakcja człowiek-komputer (HCI)

HCI to dziedzina, która czerpie z informatyki, psychologii, socjologii i projektowania. Jej głównym celem jest zrozumienie, jak ludzie używają technologii, i na tej podstawie tworzenie systemów, które są:

*   **Użyteczne (Useful):** Pozwalają osiągnąć zamierzony cel.
*   **Używalne (Usable):** Są łatwe do nauczenia się i efektywne w obsłudze.
*   **Pożądane (Desirable):** Ich wygląd i odczucia z użytkowania są przyjemne.
*   **Dostępne (Accessible):** Mogą z nich korzystać również osoby z niepełnosprawnościami.

Kluczowym pojęciem w HCI jest **użyteczność (usability)**, która opisuje, jak łatwo użytkownicy mogą korzystać z interfejsu w celu osiągnięcia konkretnych celów. Dobrze zaprojektowany interfejs powinien być intuicyjny, czyli jego obsługa powinna być naturalna i nie wymagać od użytkownika dużego wysiłku poznawczego.

#### Podstawowe zasady projektowania interfejsów

Istnieje wiele zbiorów zasad i heurystyk, które pomagają projektantom tworzyć dobre interfejsy. Do najbardziej znanych i uniwersalnych należą **10 heurystyk użyteczności Jakoba Nielsena** oraz **8 złotych zasad Bena Shneidermana**. Poniżej przedstawiono ich syntezę w postaci kluczowych zasad.

**1. Zapewnij spójność i trzymaj się standardów (Consistency and Standards):**
*   Użytkownicy nie powinni musieć się zastanawiać, czy różne słowa, sytuacje lub akcje oznaczają to samo. Elementy interfejsu o tej samej funkcji powinny wyglądać i zachowywać się tak samo w całej aplikacji. Należy również stosować powszechnie przyjęte konwencje (np. ikona kosza do usuwania, podkreślony tekst jako link).

**2. Pokazuj status systemu (Visibility of System Status):**
*   System powinien zawsze informować użytkownika o tym, co się dzieje, poprzez odpowiednie komunikaty zwrotne w rozsądnym czasie. Użytkownik musi wiedzieć, czy jego akcja została przyjęta, czy system pracuje, czy wystąpił błąd. *Przykład: paski postępu, animacje ładowania, komunikaty potwierdzające.*

**3. Projektuj dla użytkownika, nie dla systemu (Match Between System and the Real World):**
*   System powinien mówić językiem użytkownika, używając słów, zwrotów i pojęć mu znanych, a nie terminologii technicznej. Informacje powinny być prezentowane w naturalnej i logicznej kolejności.

**4. Daj użytkownikowi kontrolę i swobodę (User Control and Freedom):**
*   Użytkownicy często popełniają błędy. Należy zapewnić im wyraźnie oznaczone "wyjście awaryjne", aby mogli bez problemu cofnąć niechcianą akcję. Niezbędne są funkcje **Cofnij (Undo)** i **Powtórz (Redo)**.

**5. Zapobiegaj błędom (Error Prevention):**
*   Jeszcze lepsze niż dobre komunikaty o błędach jest staranne projektowanie, które zapobiega ich występowaniu. Należy eliminować warunki sprzyjające błędom lub sprawdzać je i prezentować użytkownikom opcję potwierdzenia, zanim podejmą ostateczną decyzję. *Przykład: pytanie "Czy na pewno chcesz usunąć ten plik?" lub wyszarzanie niedostępnych opcji.*

**6. Pozwalaj rozpoznawać, zamiast zmuszać do pamiętania (Recognition Rather Than Recall):**
*   Minimalizuj obciążenie pamięci użytkownika, czyniąc obiekty, akcje i opcje widocznymi. Użytkownik nie powinien musieć pamiętać informacji z jednej części interfejsu, aby użyć jej w innej. Instrukcje użytkowania systemu powinny być widoczne lub łatwo dostępne, gdy są potrzebne.

**7. Zapewnij elastyczność i efektywność (Flexibility and Efficiency of Use):**
*   Interfejs powinien być wygodny zarówno dla początkujących, jak i zaawansowanych użytkowników. Należy umożliwić personalizację i stosowanie **skrótów (akceleratorów)**, takich jak skróty klawiaturowe czy gesty, które przyspieszają pracę ekspertom, ale nie są widoczne dla nowicjuszy.

**8. Dbaj o estetykę i minimalistyczny design (Aesthetic and Minimalist Design):**
*   Interfejsy nie powinny zawierać informacji, które są nieistotne lub rzadko potrzebne. Każdy dodatkowy element w interfejsie konkuruje z istotnymi elementami i zmniejsza ich względną widoczność. Należy dążyć do prostoty i przejrzystości.

**9. Pomagaj rozpoznawać, diagnozować i naprawiać błędy (Help Users Recognize, Diagnose, and Recover from Errors):**
*   Komunikaty o błędach powinny być wyrażone prostym językiem (bez kodów błędów), precyzyjnie wskazywać problem i konstruktywnie sugerować rozwiązanie.

**10. Zapewnij pomoc i dokumentację (Help and Documentation):**
*   Chociaż najlepiej jest, gdy system można obsługiwać bez dokumentacji, może być konieczne zapewnienie pomocy. Wszelkie takie informacje powinny być łatwe do wyszukania, skoncentrowane na zadaniu użytkownika, zawierać konkretne kroki do wykonania i nie być zbyt obszerne.

#### Podsumowanie

*   **Interfejs użytkownika (UI)** to medium interakcji między człowiekiem a maszyną.
*   **Interakcja człowiek-komputer (HCI)** to nauka o projektowaniu użytecznych i przyjaznych systemów interaktywnych.
*   Dobrze zaprojektowany interfejs jest **spójny, przewidywalny, daje poczucie kontroli i minimalizuje obciążenie poznawcze użytkownika**.
*   Stosowanie się do fundamentalnych zasad projektowania, takich jak **heurystyki Nielsena**, pozwala tworzyć produkty cyfrowe, które są nie tylko funkcjonalne, ale także efektywne i satysfakcjonujące w użyciu.

**Typowe pytania egzaminacyjne:**
*   Co to jest interfejs użytkownika i jakie są jego rodzaje?
*   Czym zajmuje się dziedzina interakcji człowiek-komputer (HCI)?
*   Proszę wymienić i opisać co najmniej trzy podstawowe zasady projektowania interfejsów użytkownika.
*   Na czym polega zasada "rozpoznawaj, zamiast zmuszać do pamiętania"?
*   Dlaczego zapobieganie błędom jest ważniejsze niż dobre komunikaty o błędach?

---

# 42. Inżynieria wymagań: proces, wymagania funkcjonalne i niefunkcjonalne

#### Wprowadzenie

**Inżynieria wymagań (Requirements Engineering)** to zdyscyplinowany i systematyczny proces definiowania, dokumentowania i zarządzania wymaganiami w cyklu życia oprogramowania. Jest to absolutnie kluczowy etap każdego projektu informatycznego, ponieważ to właśnie na nim określa się, **co** system ma robić i jakie ma mieć właściwości. Błędy popełnione na etapie zbierania i analizy wymagań są najdroższe do naprawienia – im później w projekcie zostaną odkryte, tym większy mają wpływ na architekturę, kod i harmonogram. Celem inżynierii wymagań jest zapewnienie, że tworzony produkt będzie dokładnie tym, czego potrzebują interesariusze (klienci, użytkownicy, sponsorzy).

#### Proces inżynierii wymagań

Proces ten jest iteracyjny i składa się z kilku powiązanych ze sobą działań:

1.  **Pozyskiwanie wymagań (Elicitation):**
    *   **Cel:** Odkrycie, zrozumienie i zebranie wymagań od wszystkich interesariuszy. Jest to proces komunikacji i współpracy.
    *   **Techniki:** Wywiady z klientami i użytkownikami, warsztaty, ankiety, obserwacja użytkowników w ich naturalnym środowisku pracy, analiza istniejących dokumentów i systemów, burze mózgów.

2.  **Analiza wymagań (Analysis):**
    *   **Cel:** Przetworzenie zebranych, często niekompletnych i sprzecznych informacji w spójny i zrozumiały model. Na tym etapie wymagania są klasyfikowane, negocjowane i priorytetyzowane.
    *   **Działania:** Rozwiązywanie konfliktów między wymaganiami różnych interesariuszy, identyfikacja zależności, budowanie prototypów w celu weryfikacji zrozumienia potrzeb, modelowanie (np. za pomocą diagramów przypadków użycia UML).

3.  **Specyfikacja wymagań (Specification):**
    *   **Cel:** Formalne i jednoznaczne udokumentowanie przeanalizowanych wymagań. Wynikiem tego etapu jest **Dokument Specyfikacji Wymagań Oprogramowania (SRS - Software Requirements Specification)**.
    *   **Charakterystyka dobrej specyfikacji:** Powinna być kompletna, spójna, jednoznaczna, weryfikowalna i modyfikowalna. Musi stanowić solidną podstawę dla projektantów, programistów i testerów.

4.  **Walidacja wymagań (Validation):**
    *   **Cel:** Sprawdzenie, czy udokumentowane wymagania rzeczywiście odzwierciedlają potrzeby interesariuszy i czy zdefiniowany system będzie dla nich użyteczny. Innymi słowy, czy "budujemy właściwy produkt?".
    *   **Techniki:** Przeglądy i inspekcje dokumentu SRS z udziałem klienta, testowanie prototypów, pisanie scenariuszy testowych na podstawie wymagań.

5.  **Zarządzanie wymaganiami (Management):**
    *   **Cel:** Kontrolowanie zmian w wymaganiach w trakcie trwania projektu. Wymagania nie są statyczne – zmieniają się w miarę lepszego zrozumienia problemu i ewolucji potrzeb biznesowych.
    *   **Działania:** Ustanowienie procesu zgłaszania i akceptacji zmian (change management), utrzymywanie powiązań (traceability) między wymaganiami a innymi artefaktami projektu (projektem, kodem, testami), aby móc ocenić wpływ każdej zmiany.

#### Klasyfikacja wymagań

Wymagania dzieli się na dwie główne kategorie: funkcjonalne i niefunkcjonalne.

**1. Wymagania funkcjonalne (Functional Requirements):**

*   **Definicja:** Opisują **co system ma robić** – jakie funkcje, zadania lub usługi ma udostępniać użytkownikowi. Definiują zachowanie systemu w odpowiedzi na określone dane wejściowe lub sytuacje.
*   **Charakterystyka:** Są zazwyczaj konkretne, mierzalne i łatwe do zweryfikowania. Odpowiadają na pytanie "Co system robi?".
*   **Przykłady:**
    *   "System musi umożliwiać użytkownikowi zalogowanie się za pomocą adresu e-mail i hasła."
    *   "Użytkownik musi mieć możliwość dodania produktu do koszyka."
    *   "System powinien generować miesięczny raport sprzedaży w formacie PDF."
    *   "Po dokonaniu zakupu, system ma wysłać e-mail z potwierdzeniem do klienta."

**2. Wymagania niefunkcjonalne (Non-functional Requirements - NFRs):**

*   **Definicja:** Opisują **jak system ma działać** – określają **jakość, właściwości i ograniczenia** systemu, a nie jego konkretne funkcje. Są to kryteria, według których oceniana jest operacja systemu, a nie jego zachowanie.
*   **Charakterystyka:** Często są trudniejsze do precyzyjnego zdefiniowania i zmierzenia. Odpowiadają na pytanie "Jak dobrze system coś robi?".
*   **Kategorie i przykłady:**
    *   **Wydajność (Performance):** "Strona główna musi załadować się w czasie poniżej 2 sekund.", "System musi być w stanie obsłużyć 1000 jednoczesnych użytkowników."
    *   **Użyteczność (Usability):** "Nowy użytkownik powinien być w stanie dokonać zakupu w czasie poniżej 5 minut bez potrzeby czytania instrukcji."
    *   **Niezawodność (Reliability):** "System musi być dostępny przez 99.9% czasu."
    *   **Bezpieczeństwo (Security):** "Hasła użytkowników muszą być przechowywane w postaci zaszyfrowanej.", "System musi być odporny na ataki typu SQL Injection."
    *   **Przenośność (Portability):** "Aplikacja musi działać na systemach operacyjnych Windows 10 i macOS."
    *   **Ograniczenia projektowe:** "System musi być zaimplementowany w języku Java.", "System musi korzystać z bazy danych PostgreSQL."

| Cecha | Wymagania funkcjonalne | Wymagania niefunkcjonalne |
|---|---|---|
| **Odpowiada na pytanie** | Co system robi? | Jak dobrze system to robi? |
| **Fokus** | Zachowanie, funkcje | Jakość, właściwości, ograniczenia |
| **Weryfikacja** | Można sprawdzić, czy funkcja działa, czy nie | Często wymaga pomiarów i subiektywnej oceny |
| **Przykład** | "Dodaj do koszyka" | "Strona musi być szybka" |

#### Podsumowanie

*   **Inżynieria wymagań** to kluczowy proces zapewniający, że tworzony system spełni oczekiwania interesariuszy.
*   Proces ten obejmuje **pozyskiwanie, analizę, specyfikację, walidację i zarządzanie** wymaganiami.
*   **Wymagania funkcjonalne** definiują, **co** system robi (jego funkcje).
*   **Wymagania niefunkcjonalne** definiują, **jak** system działa (jego jakość i ograniczenia).
*   Zarówno wymagania funkcjonalne, jak i niefunkcjonalne są równie ważne dla sukcesu projektu. System, który ma wszystkie funkcje, ale jest powolny, trudny w obsłudze i niestabilny, jest w praktyce bezużyteczny.

**Typowe pytania egzaminacyjne:**
*   Jakie są główne etapy procesu inżynierii wymagań?
*   Czym różnią się wymagania funkcjonalne od niefunkcjonalnych? Proszę podać po dwa przykłady każdego z nich.
*   Jaki jest cel walidacji wymagań?
*   Dlaczego zarządzanie zmianami w wymaganiach jest ważne w trakcie projektu?
*   Proszę podać przykład wymagania dotyczącego wydajności i bezpieczeństwa.

---

# 43. Wzorce projektowe: kreacyjne, strukturalne i behawioralne (pojęcia i przykłady)

#### Wprowadzenie

**Wzorzec projektowy (Design Pattern)** to uniwersalne, sprawdzone i wielokrotnego użytku rozwiązanie często powtarzającego się problemu projektowego w inżynierii oprogramowania. Nie jest to gotowy fragment kodu, który można skopiować, ale raczej **opis lub szablon** tego, jak rozwiązać dany problem w określonym kontekście. Wzorce projektowe dostarczają wspólnego słownictwa dla programistów i pozwalają tworzyć bardziej elastyczne, eleganckie i łatwe w utrzymaniu systemy obiektowe. Najbardziej znany katalog wzorców został opisany w 1994 roku w książce "Design Patterns: Elements of Reusable Object-Oriented Software" przez czterech autorów, znanych jako **"Banda Czterech" (Gang of Four, GoF)**. Podzielili oni 23 wzorce na trzy główne kategorie: kreacyjne, strukturalne i behawioralne.

#### Wzorce kreacyjne (Creational Patterns)

Zajmują się **procesem tworzenia obiektów**. Pozwalają uniezależnić system od tego, jak jego obiekty są tworzone, komponowane i reprezentowane. Zwiększają elastyczność systemu w decydowaniu, które obiekty należy utworzyć w danej sytuacji.

*   **Singleton (Singleton):**
    *   **Problem:** Jak zapewnić, że dana klasa będzie miała **tylko jedną instancję (jeden obiekt)** w całej aplikacji i zapewnić globalny punkt dostępu do tej instancji?
    *   **Rozwiązanie:** Klasa sama kontroluje proces tworzenia swojego obiektu. Ukrywa swój konstruktor i udostępnia statyczną metodę, która zwraca jedyną istniejącą instancję (tworząc ją przy pierwszym wywołaniu).
    *   **Przykład:** Zarządzanie połączeniem z bazą danych, obsługa logowania do pliku, zarządzanie konfiguracją aplikacji.

*   **Fabryka (Factory Method):**
    *   **Problem:** Jak pozwolić klasie na tworzenie obiektów, ale dać jej podklasom możliwość decydowania, jakiego dokładnie typu obiekty będą tworzone?
    *   **Rozwiązanie:** W klasie bazowej definiuje się interfejs (metodę abstrakcyjną) do tworzenia obiektów, ale implementację tej metody pozostawia się podklasom. Każda podklasa może zwrócić inny typ obiektu.
    *   **Przykład:** Aplikacja do obsługi dokumentów. Klasa bazowa `Application` ma metodę `createDocument()`. Podklasy `WordApplication` i `PdfApplication` implementują tę metodę, tworząc odpowiednio obiekty `WordDocument` i `PdfDocument`.

#### Wzorce strukturalne (Structural Patterns)

Zajmują się **kompozycją klas i obiektów** w celu tworzenia większych struktur. Ułatwiają projektowanie, identyfikując proste sposoby realizacji relacji między bytami.

*   **Dekorator (Decorator):**
    *   **Problem:** Jak dynamicznie (w trakcie działania programu) dodawać nowe funkcjonalności do obiektu bez modyfikowania jego klasy?
    *   **Rozwiązanie:** Tworzy się obiekty "dekoratorów", które "opakowują" oryginalny obiekt. Dekorator ma ten sam interfejs co obiekt, który opakowuje, deleguje do niego wywołania, ale może dodać własne zachowanie przed lub po wywołaniu oryginalnej metody.
    *   **Przykład:** Mamy obiekt `TextView` wyświetlający tekst. Możemy go opakować w dekorator `BorderDecorator`, który doda ramkę, a następnie w `ScrollbarDecorator`, który doda paski przewijania. Funkcjonalność jest dodawana warstwowo.

*   **Adapter (Adapter):**
    *   **Problem:** Jak sprawić, by dwie klasy o niekompatybilnych interfejsach mogły ze sobą współpracować?
    *   **Rozwiązanie:** Tworzy się klasę "adaptera", która działa jak tłumacz. Implementuje ona interfejs oczekiwany przez klienta, ale wewnętrznie deleguje wywołania do obiektu o niekompatybilnym interfejsie, dokonując niezbędnej konwersji.
    *   **Przykład:** Mamy nową bibliotekę, która oczekuje obiektów z metodą `get_data()`, ale nasz stary system dostarcza obiekty z metodą `fetchData()`. Adapter implementuje `get_data()`, a w środku wywołuje `fetchData()` na starym obiekcie.

#### Wzorce behawioralne (behawioralne) (Behavioral Patterns)

Zajmują się **algorytmami i przypisywaniem odpowiedzialności między obiektami**. Opisują złożone schematy komunikacji i współpracy między obiektami.

*   **Strategia (Strategy):**
    *   **Problem:** Jak zdefiniować rodzinę algorytmów, zamknąć każdy z nich w osobnym obiekcie i uczynić je wymiennymi, tak aby algorytm mógł być zmieniany w trakcie działania programu?
    *   **Rozwiązanie:** Definiuje się wspólny interfejs dla wszystkich algorytmów (strategii). Główny obiekt (kontekst) przechowuje referencję do obiektu strategii i deleguje do niego wykonanie algorytmu, zamiast implementować go samemu. W dowolnym momencie można podmienić obiekt strategii na inny.
    *   **Przykład:** Obiekt `ImageCompressor` może używać różnych strategii kompresji (`JpegStrategy`, `PngStrategy`). Użytkownik może wybrać, która strategia ma być użyta.

*   **Obserwator (Observer):**
    *   **Problem:** Jak zdefiniować zależność jeden-do-wielu między obiektami, tak aby zmiana stanu jednego obiektu (obserwowanego) powodowała automatyczne powiadomienie i aktualizację wszystkich zależnych od niego obiektów (obserwatorów)?
    *   **Rozwiązanie:** Obiekt obserwowany (zwany też podmiotem) utrzymuje listę swoich obserwatorów. Gdy jego stan się zmienia, przechodzi przez listę i wywołuje na każdym obserwatorze metodę `update()`.
    *   **Przykład:** Arkusz kalkulacyjny. Komórki (obserwatorzy) obserwują inne komórki (podmioty). Gdy wartość w jednej komórce się zmienia, wszystkie komórki, które na niej bazują, są automatycznie przeliczane. Inny przykład to system powiadomień w mediach społecznościowych.

#### Podsumowanie

| Kategoria | Cel | Przykładowe wzorce |
|---|---|---|
| **Kreacyjne** | Kontrola nad procesem tworzenia obiektów | Singleton, Fabryka, Budowniczy |
| **Strukturalne** | Tworzenie większych struktur z klas i obiektów | Dekorator, Adapter, Fasada, Kompozyt |
| **Behawioralne** | Zarządzanie komunikacją i współpracą między obiektami | Strategia, Obserwator, Polecenie, Iterator |

*   Wzorce projektowe to **sprawdzone rozwiązania typowych problemów**, a nie sztywne reguły.
*   Dostarczają **wspólnego języka** dla programistów, ułatwiając komunikację.
*   Stosowanie wzorców prowadzi do tworzenia kodu, który jest bardziej **elastyczny, reużywalny i łatwiejszy w utrzymaniu**.
*   Kluczem jest nie tylko znajomość samych wzorców, ale przede wszystkim umiejętność **rozpoznania problemu**, który dany wzorzec rozwiązuje.

**Typowe pytania egzaminacyjne:**
*   Co to jest wzorzec projektowy i dlaczego warto je stosować?
*   Proszę wymienić trzy główne kategorie wzorców projektowych i opisać, czym się one zajmują.
*   Na czym polega wzorzec Singleton i jaki problem rozwiązuje?
*   Proszę porównać wzorce Strategia i Dekorator. Jaki jest ich główny cel?
*   Podaj przykład z życia wzięty dla wzorca Obserwator.

---

# 44. Testowanie oprogramowania: poziomy testów, techniki czarno- i białoskrzynkowe

#### Wprowadzenie

**Testowanie oprogramowania** to kluczowy proces w inżynierii oprogramowania, którego celem jest weryfikacja i walidacja produktu, znajdowanie defektów (błędów) oraz ocena jego jakości. Testowanie nie jest jednorazową czynnością, ale procesem trwającym przez cały cykl życia oprogramowania. Jego głównym celem nie jest udowodnienie, że program działa, ale aktywne poszukiwanie sytuacji, w których program **nie działa** poprawnie. Dobre testowanie zwiększa pewność, że oprogramowanie spełnia zdefiniowane wymagania i będzie działać niezawodnie w środowisku produkcyjnym.

#### Poziomy testów

Testowanie jest zorganizowane w hierarchiczną strukturę poziomów, które odpowiadają kolejnym etapom integracji systemu. Koncepcję tę często wizualizuje się jako **piramidę testów**.

**1. Testy jednostkowe (Unit Tests):**

*   **Poziom:** Najniższy i najbardziej fundamentalny. Stanowią podstawę piramidy.
*   **Przedmiot testów:** Testowanie **najmniejszych, izolowanych fragmentów kodu** – pojedynczych funkcji, metod lub klas. Celem jest sprawdzenie, czy dana "jednostka" działa poprawnie w izolacji od reszty systemu.
*   **Kto wykonuje:** Zazwyczaj programiści, równolegle z pisaniem kodu.
*   **Charakterystyka:** Są bardzo szybkie, tanie w tworzeniu i utrzymaniu. Powinno ich być najwięcej w projekcie. Często wykorzystuje się do nich obiekty-zaślepki (mocki, stuby), aby odizolować testowaną jednostkę od jej zewnętrznych zależności (np. bazy danych, API).

**2. Testy integracyjne (Integration Tests):**

*   **Poziom:** Środkowy. Skupiają się na interakcjach między komponentami.
*   **Przedmiot testów:** Weryfikacja, czy **kilka połączonych ze sobą modułów lub komponentów systemu poprawnie współpracuje**. Celem jest wykrycie błędów w interfejsach i komunikacji między częściami systemu.
*   **Kto wykonuje:** Programiści lub dedykowani testerzy.
*   **Charakterystyka:** Są wolniejsze i bardziej złożone niż testy jednostkowe. Sprawdzają np. czy aplikacja poprawnie komunikuje się z bazą danych, czy wywołania API między dwoma serwisami działają zgodnie z oczekiwaniami.

**3. Testy systemowe (System Tests):**

*   **Poziom:** Wysoki. Testowanie całego, zintegrowanego systemu.
*   **Przedmiot testów:** Weryfikacja, czy **kompletny, zintegrowany system jako całość spełnia zdefiniowane wymagania funkcjonalne i niefunkcjonalne**. System jest testowany w środowisku jak najbardziej zbliżonym do produkcyjnego.
*   **Kto wykonuje:** Głównie dedykowani testerzy.
*   **Charakterystyka:** Są to testy kompleksowe, ale też czasochłonne i kosztowne. Sprawdzają działanie systemu z perspektywy "end-to-end" (od początku do końca).

**4. Testy akceptacyjne (Acceptance Tests):**

*   **Poziom:** Najwyższy. Szczyt piramidy.
*   **Przedmiot testów:** Walidacja, czy system spełnia **potrzeby biznesowe klienta i jest gotowy do wdrożenia**. Celem jest uzyskanie akceptacji od klienta lub użytkowników końcowych.
*   **Kto wykonuje:** Klient, użytkownicy końcowi lub testerzy w ich imieniu.
*   **Charakterystyka:** Koncentrują się na scenariuszach biznesowych, a nie na szczegółach technicznych. Odpowiadają na pytanie: "Czy ten system rozwiązuje nasz problem?".

#### Techniki projektowania testów

Techniki te opisują, w jaki sposób projektuje się przypadki testowe. Dwie główne kategorie to techniki czarnoskrzynkowe i białoskrzynkowe.

**1. Techniki czarnoskrzynkowe (Black-Box Testing):**

*   **Idea:** Tester traktuje system jak **"czarną skrzynkę"**. Nie ma wiedzy o jego wewnętrznej strukturze, implementacji ani kodzie źródłowym. Testy są projektowane wyłącznie na podstawie **specyfikacji wymagań** – sprawdzane jest, czy dla określonych danych wejściowych system generuje oczekiwane dane wyjściowe.
*   **Fokus:** Testowanie **funkcjonalności** z perspektywy użytkownika.
*   **Przykładowe techniki:**
    *   **Partycjonowanie równoważności (Equivalence Partitioning):** Dzielenie danych wejściowych na klasy (partycje), dla których system powinien zachowywać się tak samo. Testuje się po jednym reprezentancie z każdej klasy.
    *   **Analiza wartości brzegowych (Boundary Value Analysis):** Koncentracja na testowaniu wartości na granicach partycji równoważności, ponieważ to tam najczęściej występują błędy.
    *   **Tablice decyzyjne (Decision Tables):** Stosowane do testowania złożonych reguł biznesowych.

**2. Techniki białoskrzynkowe (White-Box Testing):**

*   **Idea:** Tester ma pełną wiedzę o **wewnętrznej strukturze, logice i kodzie źródłowym** systemu. Testy są projektowane tak, aby "przejść" przez określone ścieżki w kodzie i sprawdzić jego wewnętrzne działanie.
*   **Fokus:** Testowanie **struktury** kodu i jego pokrycia.
*   **Przykładowe techniki (miary pokrycia kodu):**
    *   **Pokrycie instrukcji (Statement Coverage):** Czy każda linijka kodu została wykonana co najmniej raz?
    *   **Pokrycie decyzji/gałęzi (Decision/Branch Coverage):** Czy każdy możliwy wynik każdej instrukcji warunkowej (np. `if`, `while`) został przetestowany (zarówno gałąź `true`, jak i `false`)?
    *   **Pokrycie ścieżek (Path Coverage):** Czy każda możliwa ścieżka wykonania przez funkcję została przetestowana? (Zazwyczaj niemożliwe do osiągnięcia w praktyce).

| Cecha | Techniki czarnoskrzynkowe | Techniki białoskrzynkowe |
|---|---|---|
| **Wiedza o systemie** | Brak (testowanie "z zewnątrz") | Pełna (testowanie "od wewnątrz") |
| **Podstawa projektowania testów** | Specyfikacja wymagań | Struktura kodu |
| **Cel** | Weryfikacja funkcjonalności | Weryfikacja logiki i pokrycia kodu |
| **Kto wykonuje** | Głównie testerzy | Głównie programiści |
| **Stosowane na poziomie** | Głównie systemowym i akceptacyjnym | Głównie jednostkowym i integracyjnym |

#### Podsumowanie

*   **Testowanie** to proces poszukiwania błędów, zorganizowany w **poziomy**: jednostkowe, integracyjne, systemowe i akceptacyjne.
*   **Piramida testów** sugeruje, że najwięcej powinno być szybkich testów jednostkowych, a najmniej – wolnych testów kompleksowych.
*   **Techniki czarnoskrzynkowe** koncentrują się na tym, **co** system robi (funkcjonalność), bez znajomości jego wewnętrznej budowy.
*   **Techniki białoskrzynkowe** koncentrują się na tym, **jak** system to robi, wykorzystując wiedzę o kodzie do zapewnienia jego pokrycia.
*   Kompleksowa strategia testowania powinna łączyć różne poziomy i techniki, aby zapewnić najwyższą jakość oprogramowania.

**Typowe pytania egzaminacyjne:**
*   Proszę wymienić i opisać cztery poziomy testowania oprogramowania.
*   Na czym polega różnica między testowaniem czarnoskrzynkowym a białoskrzynkowym?
*   Jaki jest cel testów jednostkowych i kto je zazwyczaj pisze?
*   Co to jest analiza wartości brzegowych i dlaczego jest ważna?
*   Co to jest pokrycie kodu i jaki jest jego związek z testowaniem białoskrzynkowym?

---

# 45. Systemy kontroli wersji, Git, GitHub

#### Wprowadzenie

**System kontroli wersji (VCS - Version Control System)** to oprogramowanie, które śledzi i zarządza zmianami w plikach na przestrzeni czasu. Chociaż może być używany do dowolnego typu plików, jest absolutnie niezbędnym narzędziem w nowoczesnym tworzeniu oprogramowania, gdzie pozwala zespołom programistów efektywnie współpracować nad tym samym kodem źródłowym. VCS umożliwia programistom pracę równoległą, śledzenie historii każdej zmiany, powrót do dowolnej poprzedniej wersji oraz łatwe łączenie zmian wprowadzonych przez różne osoby. Najpopularniejszym na świecie systemem kontroli wersji jest **Git**, a najpopularniejszą platformą do hostowania repozytoriów Gita jest **GitHub**.

#### Co to jest system kontroli wersji?

Wyobraź sobie pisanie dużej pracy zaliczeniowej. Bez VCS, prawdopodobnie kończysz z plikami o nazwach `praca_v1.doc`, `praca_v2_poprawki.doc`, `praca_finalna.doc`, `praca_finalna_ostateczna.doc`. Jeśli pracujesz z kimś, wysyłacie sobie te pliki e-mailem, co prowadzi do chaosu i trudności w połączeniu waszych zmian. System kontroli wersji rozwiązuje te problemy, działając jak "inteligentna maszyna czasu" dla twojego projektu:

*   **Rejestruje historię:** Zapisuje każdą zmianę jako "migawkę" (commit) stanu projektu w danym momencie.
*   **Umożliwia powrót:** Pozwala w każdej chwili wrócić do dowolnej zapisanej wersji.
*   **Wspiera pracę zespołową:** Umożliwia wielu osobom pracę nad tym samym projektem i inteligentne łączenie ich zmian.
*   **Tworzy gałęzie:** Pozwala na tworzenie oddzielnych "gałęzi" (branches) rozwoju, aby bezpiecznie pracować nad nowymi funkcjami bez wpływu na główną, stabilną wersję kodu.

#### Git – rozproszony system kontroli wersji

Git to darmowy, otwarty i niezwykle popularny **rozproszony system kontroli wersji (DVCS)**, stworzony przez Linusa Torvaldsa (twórcę Linuksa). "Rozproszony" oznacza, że każdy programista ma na swoim komputerze **pełną kopię całego repozytorium**, włącznie z całą jego historią. To różni go od starszych, scentralizowanych systemów (jak SVN), gdzie centralny serwer był jedynym miejscem przechowującym pełną historię.

**Podstawowe pojęcia w Gicie:**

*   **Repozytorium (Repository):** Folder projektu, w którym Git śledzi zmiany. Zawiera wszystkie pliki projektu oraz ukryty podfolder `.git` z całą historią i metadanymi.
*   **Commit:** "Migawka" lub "punkt zapisu" stanu projektu w danym momencie. Każdy commit ma unikalny identyfikator (hash) i zawiera informację o autorze, dacie oraz opis wprowadzonych zmian.
*   **Gałąź (Branch):** Niezależna linia rozwoju w projekcie. Główna gałąź to zazwyczaj `main` (dawniej `master`). Programiści tworzą nowe gałęzie, aby pracować nad nowymi funkcjami (np. `feature/add-login-button`), a po ich ukończeniu łączą je z gałęzią główną.
*   **Scalanie (Merge):** Proces łączenia zmian z jednej gałęzi do drugiej.

**Podstawowe polecenia Gita:**

1.  `git init`: Inicjalizuje nowe, puste repozytorium Gita w bieżącym folderze.
2.  `git clone [adres_repozytorium]`: Klonuje (pobiera) istniejące repozytorium ze zdalnego serwera na lokalny komputer.
3.  `git status`: Wyświetla stan plików w repozytorium (które pliki są zmodyfikowane, które nowe, itp.).
4.  `git add [nazwa_pliku]`: Dodaje zmiany z pliku do "poczekalni" (staging area), przygotowując je do commita.
5.  `git commit -m "Opis zmian"`: Zapisuje zmiany z poczekalni jako nowy commit w historii repozytorium.
6.  `git log`: Wyświetla historię commitów.
7.  `git branch [nazwa_gałęzi]`: Tworzy nową gałąź.
8.  `git checkout [nazwa_gałęzi]`: Przełącza się na inną gałąź.
9.  `git merge [nazwa_gałęzi]`: Scala zmiany z podanej gałęzi do gałęzi, na której aktualnie jesteśmy.
10. `git pull`: Pobiera zmiany ze zdalnego repozytorium i scala je z lokalną gałęzią.
11. `git push`: Wysyła lokalne commity na zdalny serwer.

#### GitHub – platforma do hostowania repozytoriów

*   **Co to jest?** GitHub to **serwis internetowy**, który oferuje hosting (przechowywanie) repozytoriów Gita w chmurze. Jest to platforma społecznościowa dla programistów, która rozbudowuje możliwości samego Gita o wiele dodatkowych narzędzi ułatwiających współpracę.
*   **Git vs GitHub:**
    *   **Git** to narzędzie (program działający w wierszu poleceń), które instalujesz na swoim komputerze do zarządzania historią zmian.
    *   **GitHub** to usługa (strona internetowa), która przechowuje twoje repozytoria Gita i umożliwia ci współpracę z innymi.
*   **Kluczowe funkcje GitHuba:**
    *   **Hosting repozytoriów:** Przechowywanie kodu i jego historii.
    *   **Pull Requests (PRs):** Mechanizm proponowania zmian w projekcie. Programista tworzy zmiany na swojej gałęzi, a następnie otwiera Pull Request, prosząc właściciela projektu o ich przejrzenie (code review) i włączenie do głównej gałęzi.
    *   **Issues (Zgłoszenia):** System do śledzenia zadań, błędów i propozycji nowych funkcji.
    *   **Actions:** Narzędzie do automatyzacji procesów, takich jak testowanie i wdrażanie kodu (CI/CD).
    *   **Wiki i dokumentacja:** Miejsce na tworzenie dokumentacji projektu.

#### Podsumowanie

*   **System kontroli wersji (VCS)** to narzędzie do śledzenia zmian w plikach, kluczowe dla pracy zespołowej nad oprogramowaniem.
*   **Git** to najpopularniejszy, **rozproszony** system kontroli wersji, który pozwala na pracę offline i daje każdemu programiście pełną historię projektu.
*   **GitHub** to **platforma hostingowa** dla repozytoriów Gita, która dodaje warstwę społecznościową i narzędzia do współpracy, takie jak Pull Requests i Issues.
*   Nie można mylić Gita z GitHubem. **Git to narzędzie, GitHub to usługa, która z tego narzędzia korzysta.** Praca z Gitem i GitHubem to dziś absolutny standard i jedna z najbardziej podstawowych umiejętności każdego programisty.

**Typowe pytania egzaminacyjne:**
*   Co to jest system kontroli wersji i jakie problemy rozwiązuje?
*   Czym różni się rozproszony system kontroli wersji (jak Git) od scentralizowanego?
*   Jaka jest różnica między Gitem a GitHubem?
*   Do czego służy polecenie `git commit`?
*   Na czym polega praca z gałęziami (branches) w Gicie?
*   Co to jest Pull Request w kontekście GitHuba?

---

# 46. Konteneryzacja, Docker

#### Wprowadzenie

**Konteneryzacja** to nowoczesna metoda wirtualizacji na poziomie systemu operacyjnego, która pozwala na spakowanie aplikacji wraz ze wszystkimi jej zależnościami (bibliotekami, plikami konfiguracyjnymi, środowiskiem uruchomieniowym) w jedną, przenośną jednostkę zwaną **kontenerem**. Kontener ten można następnie uruchomić w spójny i przewidywalny sposób na dowolnym komputerze, niezależnie od jego systemu operacyjnego czy konfiguracji. **Docker** to najpopularniejsza na świecie platforma open-source, która zautomatyzowała i spopularyzowała proces tworzenia, uruchamiania i zarządzania kontenerami.

#### Wirtualizacja vs Konteneryzacja

Aby zrozumieć konteneryzację, warto porównać ją z tradycyjną wirtualizacją za pomocą maszyn wirtualnych (VM).

*   **Maszyna wirtualna (VM):**
    *   **Jak działa:** Wirtualizuje **cały sprzęt fizyczny**. Na fizycznym serwerze (hoście) działa oprogramowanie zwane **hiperwizorem (hypervisor)**, które tworzy i zarządza maszynami wirtualnymi. Każda maszyna wirtualna zawiera **pełną kopię systemu operacyjnego gościa (Guest OS)**, a na nim dopiero instalowane są biblioteki i aplikacja.
    *   **Zalety:** Pełna izolacja na poziomie jądra systemu operacyjnego, co zapewnia wysokie bezpieczeństwo.
    *   **Wady:** Duży narzut zasobów (każda VM to osobny system operacyjny, który zużywa CPU, RAM i miejsce na dysku), wolny czas uruchamiania (minuty), duże rozmiary.

*   **Kontener:**
    *   **Jak działa:** Wirtualizuje **system operacyjny**, a nie sprzęt. Wszystkie kontenery działające na jednym hoście **dzielą to samo jądro systemu operacyjnego gospodarza**. Każdy kontener zawiera tylko aplikację i jej zależności. Z perspektywy aplikacji, kontener wygląda jak osobny system, ale w rzeczywistości jest to odizolowany proces działający na wspólnym jądrze.
    *   **Zalety:** Bardzo mały narzut zasobów, błyskawiczny czas uruchamiania (sekundy lub milisekundy), małe rozmiary, wysoka przenośność.
    *   **Wady:** Słabsza izolacja niż w przypadku VM (wspólne jądro systemu operacyjnego może być potencjalnym punktem ataku).

| Cecha | Maszyna wirtualna (VM) | Kontener |
|---|---|---|
| **Wirtualizacja** | Sprzętu | Systemu operacyjnego |
| **Izolacja** | Pełna (na poziomie jądra OS) | Na poziomie procesów |
| **Rozmiar** | Duży (gigabajty) | Mały (megabajty) |
| **Czas uruchamiania** | Wolny (minuty) | Szybki (sekundy) |
| **Zasoby** | Duży narzut | Mały narzut |

#### Docker – ekosystem konteneryzacji

Docker to nie tylko narzędzie do uruchamiania kontenerów, ale cały ekosystem, który ułatwia pracę z nimi. Kluczowe pojęcia w Dockerze to:

**1. Obraz (Image):**

*   **Definicja:** Szablon **tylko do odczytu**, który zawiera instrukcje do stworzenia kontenera. Obraz składa się z warstw, które reprezentują kolejne zmiany w systemie plików. Zawiera wszystko, co jest potrzebne do uruchomienia aplikacji: kod, środowisko uruchomieniowe, biblioteki, zmienne środowiskowe i pliki konfiguracyjne.
*   **Analogia:** W programowaniu obiektowym obraz jest jak **klasa**.

**2. Kontener (Container):**

*   **Definicja:** Uruchomiona **instancja** obrazu. Jest to lekki, przenośny i wykonywalny pakiet oprogramowania.
*   **Analogia:** W programowaniu obiektowym kontener jest jak **obiekt (instancja klasy)**. Można stworzyć wiele kontenerów z jednego obrazu.

**3. Dockerfile:**

*   **Definicja:** Prosty plik tekstowy, który zawiera **instrukcje krok po kroku**, jak zbudować obraz Dockera. Jest to przepis na obraz.
*   **Przykładowe instrukcje:**
    *   `FROM ubuntu:22.04`: Użyj oficjalnego obrazu Ubuntu jako podstawy.
    *   `WORKDIR /app`: Ustaw katalog roboczy wewnątrz kontenera.
    *   `COPY . .`: Skopiuj pliki z bieżącego folderu na hoście do kontenera.
    *   `RUN apt-get update && apt-get install -y python3`: Wykonaj polecenie wewnątrz kontenera (np. zainstaluj oprogramowanie).
    *   `CMD ["python3", "app.py"]`: Zdefiniuj domyślne polecenie do uruchomienia, gdy kontener startuje.

**4. Docker Hub / Registry:**

*   **Definicja:** Repozytorium do przechowywania i udostępniania obrazów Dockera. Docker Hub to publiczne, oficjalne repozytorium (jak GitHub dla kodu), ale można też tworzyć prywatne rejestry.

#### Dlaczego konteneryzacja jest tak popularna?

Konteneryzacja, a w szczególności Docker, zrewolucjonizowała sposób tworzenia, testowania i wdrażania oprogramowania, rozwiązując wiele powszechnych problemów:

*   **Rozwiązuje problem "u mnie działa"**: Gwarantuje, że oprogramowanie będzie działać tak samo w każdym środowisku (deweloperskim, testowym, produkcyjnym), ponieważ całe środowisko jest spakowane razem z aplikacją.
*   **Upraszcza zarządzanie zależnościami**: Wszystkie zależności są zamknięte w kontenerze, co eliminuje konflikty między bibliotekami na maszynie hosta.
*   **Wspiera architekturę mikroserwisów**: Umożliwia łatwe budowanie i wdrażanie aplikacji jako zbioru małych, niezależnych i odizolowanych usług, z których każda działa we własnym kontenerze.
*   **Przyspiesza cykl deweloperski**: Lekkość i szybkość kontenerów ułatwiają szybkie budowanie, testowanie i wdrażanie zmian (CI/CD).
*   **Efektywne wykorzystanie zasobów**: Pozwala na uruchomienie znacznie większej liczby aplikacji na jednym serwerze w porównaniu do maszyn wirtualnych.

#### Podsumowanie

*   **Konteneryzacja** to technologia pakowania aplikacji i jej zależności w przenośne kontenery, które działają w izolacji, dzieląc jądro systemu operacyjnego hosta.
*   Jest to podejście znacznie **lżejsze i szybsze** od tradycyjnej wirtualizacji opartej na maszynach wirtualnych (VM).
*   **Docker** to wiodąca platforma do konteneryzacji, która dostarcza narzędzi do budowania (**Dockerfile**), uruchamiania (**kontenery**) i udostępniania (**obrazy**) aplikacji.
*   Konteneryzacja stała się fundamentem nowoczesnego wytwarzania oprogramowania, zwłaszcza w kontekście chmury, DevOps i architektury mikroserwisów.

**Typowe pytania egzaminacyjne:**
*   Na czym polega różnica między wirtualizacją a konteneryzacją?
*   Co to jest obraz (image) i kontener (container) w Dockerze? Jaka jest między nimi relacja?
*   Do czego służy plik Dockerfile?
*   Jakie są główne zalety stosowania konteneryzacji w procesie tworzenia oprogramowania?
*   Dlaczego kontenery uruchamiają się znacznie szybciej niż maszyny wirtualne?

---

# 47. Metodyki zwinne (Agile), Scrum, Kanban

#### Wprowadzenie

**Metodyki zwinne (Agile)** to rodzina iteracyjnych i przyrostowych podejść do tworzenia oprogramowania i zarządzania projektami, które powstały jako odpowiedź na ograniczenia tradycyjnych, sztywnych modeli, takich jak model kaskadowy (waterfall). Zamiast szczegółowego planowania całego projektu na początku, Agile kładzie nacisk na **elastyczność, współpracę z klientem, szybkie dostarczanie działających fragmentów produktu i adaptację do zmian**. Agile to nie jest jedna, konkretna metodyka, ale raczej **filozofia (mindset)** oparta na wartościach i zasadach sformułowanych w 2001 roku w **Manifeście Agile**. Dwie najpopularniejsze implementacje tej filozofii to **Scrum** i **Kanban**.

#### Manifest Agile

Manifest Agile to fundament myślenia zwinnego. Składa się z czterech kluczowych wartości:

1.  **Ludzie i interakcje** ponad procesy i narzędzia.
2.  **Działające oprogramowanie** ponad obszerną dokumentację.
3.  **Współpraca z klientem** ponad formalne negocjacje.
4.  **Reagowanie na zmiany** ponad podążanie za planem.

Nie oznacza to, że elementy po prawej stronie są nieważne, ale te po lewej są **cenione wyżej**.

#### Scrum

Scrum to nie jest metodyka, ale **ramy postępowania (framework)** do zarządzania złożonymi projektami. Jest to najbardziej popularne i ustrukturyzowane podejście zwinne. Praca w Scrumie jest zorganizowana w krótkie, stałej długości cykle zwane **Sprintami**.

**Elementy Scruma:**

**1. Role (Zespół Scrumowy):**
*   **Product Owner (Właściciel Produktu):** Osoba odpowiedzialna za **maksymalizację wartości produktu**. Zarządza Backlogiem Produktu, priorytetyzuje zadania i jest jedynym źródłem wymagań dla zespołu. Reprezentuje interesariuszy i klienta.
*   **Scrum Master:** "Służący lider" (servant-leader), który pomaga zespołowi zrozumieć i stosować zasady Scruma. Usuwa przeszkody, facylituje spotkania i dba o efektywność procesu.
*   **Developers (Deweloperzy):** Interdyscyplinarny i samoorganizujący się zespół specjalistów (programistów, testerów, analityków), którzy są odpowiedzialni za dostarczenie działającego przyrostu produktu w każdym Sprincie.

**2. Wydarzenia (Events):**
*   **Sprint:** "Serce" Scruma. Jest to iteracja o stałej długości (zazwyczaj 2-4 tygodnie), w trakcie której zespół tworzy gotowy do użycia, potencjalnie wdrażalny **Przyrost (Increment)** produktu.
*   **Planowanie Sprintu (Sprint Planning):** Spotkanie na początku Sprintu, podczas którego zespół wybiera zadania z Backlogu Produktu, które zobowiązuje się zrealizować, i tworzy plan ich wykonania (Backlog Sprintu).
*   **Codzienny Scrum (Daily Scrum):** Krótkie, 15-minutowe spotkanie dla Deweloperów, służące do synchronizacji pracy i planowania na najbliższe 24 godziny. Uczestnicy odpowiadają na trzy pytania: Co zrobiłem wczoraj? Co zrobię dzisiaj? Jakie mam przeszkody?
*   **Przegląd Sprintu (Sprint Review):** Nieformalne spotkanie na końcu Sprintu, podczas którego zespół prezentuje interesariuszom działający przyrost produktu i zbiera od nich informację zwrotną.
*   **Retrospektywa Sprintu (Sprint Retrospective):** Wewnętrzne spotkanie zespołu po Przeglądzie Sprintu, którego celem jest inspekcja i adaptacja procesu pracy. Zespół zastanawia się, co poszło dobrze, co można poprawić i jakie usprawnienia wprowadzić w następnym Sprincie.

**3. Artefakty (Artifacts):**
*   **Backlog Produktu (Product Backlog):** Uporządkowana według priorytetów, dynamiczna lista wszystkiego, co może być potrzebne w produkcie (funkcjonalności, poprawki, zmiany). Jest to jedyne źródło pracy dla Zespołu Scrumowego.
*   **Backlog Sprintu (Sprint Backlog):** Zestaw elementów z Backlogu Produktu wybranych na dany Sprint plus plan ich dostarczenia.
*   **Przyrost (Increment):** Suma wszystkich elementów z Backlogu Produktu ukończonych podczas Sprintu i wszystkich poprzednich Sprintów. Każdy Przyrost musi być użyteczny i potencjalnie wdrażalny.

#### Kanban

Kanban to metoda zarządzania przepływem pracy, która wywodzi się z systemu produkcyjnego Toyoty. W przeciwieństwie do Scruma, nie narzuca stałych iteracji ani ról. Koncentruje się na **wizualizacji pracy, ograniczaniu pracy w toku i maksymalizacji przepływu**.

**Podstawowe praktyki Kanbana:**

1.  **Wizualizuj przepływ pracy (Visualize the Workflow):** Praca jest wizualizowana na **tablicy Kanban**, która jest podzielona na kolumny reprezentujące kolejne etapy procesu (np. "Do zrobienia", "W trakcie", "Testowanie", "Zrobione"). Zadania są reprezentowane przez karty, które przesuwają się po tablicy od lewej do prawej.
2.  **Ograniczaj pracę w toku (Limit Work In Progress - WIP):** Dla każdej kolumny (lub dla całego systemu) ustala się **limit WIP**, czyli maksymalną liczbę zadań, które mogą się w niej znajdować w danym momencie. To zapobiega powstawaniu "wąskich gardeł" i zmusza zespół do kończenia zadań, zanim zacznie nowe.
3.  **Zarządzaj przepływem (Manage Flow):** Zespół monitoruje przepływ pracy, identyfikuje i eliminuje blokery oraz dąży do tego, aby zadania przechodziły przez system jak najpłynniej i najszybciej.
4.  **Stosuj jawne zasady procesu (Make Process Policies Explicit):** Wszyscy w zespole muszą rozumieć, jak działa proces (np. co oznacza, że zadanie jest "Zrobione").
5.  **Implementuj pętle informacji zwrotnej (Implement Feedback Loops):** Regularne spotkania (np. codzienne stand-upy, przeglądy) służą do synchronizacji i adaptacji.
6.  **Ulepszaj współpracę, ewoluuj eksperymentalnie (Improve Collaboratively, Evolve Experimentally):** Kanban promuje kulturę ciągłego doskonalenia (Kaizen).

#### Scrum vs Kanban

| Cecha | Scrum | Kanban |
|---|---|---|
| **Rytm pracy** | Regularne, stałej długości Sprinty | Ciągły przepływ (continuous flow) |
| **Dostarczanie** | Na koniec każdego Sprintu | W dowolnym momencie, gdy zadanie jest gotowe |
| **Role** | Zdefiniowane (Product Owner, Scrum Master, Deweloperzy) | Brak narzuconych ról |
| **Metryki** | Prędkość (Velocity) zespołu | Czas cyklu (Cycle Time), przepustowość (Throughput) |
| **Zmiany w trakcie** | Backlog Sprintu jest stały w trakcie Sprintu | Zmiany mogą być wprowadzane w dowolnym momencie |
| **Najlepszy dla** | Złożonych projektów z możliwością planowania na 2-4 tygodnie | Pracy operacyjnej, utrzymaniowej, gdzie priorytety często się zmieniają |

#### Podsumowanie

*   **Agile** to filozofia elastycznego tworzenia oprogramowania, oparta na wartościach z **Manifestu Agile**.
*   **Scrum** to ustrukturyzowany framework oparty na stałych iteracjach (Sprintach), zdefiniowanych rolach i wydarzeniach, idealny do rozwoju złożonych produktów.
*   **Kanban** to metoda optymalizacji przepływu pracy, oparta na wizualizacji i ograniczaniu pracy w toku, idealna dla procesów, gdzie zadania pojawiają się w sposób ciągły i nieprzewidywalny.
*   Wiele zespołów stosuje podejścia hybrydowe, np. **Scrumban**, łącząc elementy obu tych metod.

**Typowe pytania egzaminacyjne:**
*   Jakie są cztery wartości Manifestu Agile?
*   Proszę opisać role w Zespole Scrumowym.
*   Jaki jest cel Przeglądu Sprintu, a jaki Retrospektywy Sprintu?
*   Na czym polega zasada ograniczania pracy w toku (WIP) w Kanbanie?
*   Proszę porównać Scrum i Kanban pod względem rytmu pracy i sposobu dostarczania wartości.

---

# 48. Ciągła integracja i ciągłe dostarczanie (CI/CD), Jenkins, GitHub Actions

#### Wprowadzenie

**CI/CD** to skrót od **Ciągłej Integracji (Continuous Integration)** i **Ciągłego Dostarczania/Wdrażania (Continuous Delivery/Deployment)**. Jest to zbiór praktyk, filozofia i kultura pracy w nowoczesnym wytwarzaniu oprogramowania, które mają na celu automatyzację i przyspieszenie procesu dostarczania zmian w kodzie od programisty do użytkownika końcowego. Celem CI/CD jest tworzenie oprogramowania w krótkich cyklach, zapewniając, że można je niezawodnie wydać w dowolnym momencie. Automatyzacja tego procesu jest realizowana za pomocą narzędzi takich jak **Jenkins** czy **GitHub Actions**, które orkiestrują tzw. **potok (pipeline) CI/CD**.

#### Ciągła Integracja (Continuous Integration - CI)

*   **Idea:** Praktyka, w której programiści **często (co najmniej raz dziennie) integrują swoje zmiany w kodzie do wspólnego, centralnego repozytorium** (np. do głównej gałęzi w Gicie).
*   **Proces:** Każda taka integracja jest automatycznie weryfikowana przez **automatyczny build (kompilację) i uruchomienie zestawu testów** (głównie jednostkowych i integracyjnych). Proces ten odbywa się na dedykowanym serwerze CI.
*   **Cel:** Wczesne i szybkie wykrywanie błędów integracyjnych. Zamiast czekać tygodniami na "wielką integrację" i rozwiązywać setki konfliktów, problemy są identyfikowane i naprawiane na bieżąco, gdy są jeszcze małe i tanie do usunięcia. CI daje zespołowi pewność, że główna gałąź kodu jest zawsze w stabilnym, działającym stanie.

#### Ciągłe Dostarczanie (Continuous Delivery - CD)

*   **Idea:** Rozszerzenie Ciągłej Integracji. Praktyka polegająca na tym, że każda zmiana, która pomyślnie przejdzie przez wszystkie etapy automatycznych testów w potoku CI, jest automatycznie **przygotowywana do wdrożenia na środowisko produkcyjne**.
*   **Proces:** Po etapie CI, kod jest automatycznie wdrażany na środowisko testowe lub stagingowe, gdzie przechodzi bardziej kompleksowe testy (np. systemowe, akceptacyjne). Jeśli te testy również zakończą się sukcesem, artefakt (np. paczka instalacyjna, obraz Dockera) jest gotowy do wdrożenia na produkcję.
*   **Kluczowa cecha:** Ostatni krok – **faktyczne wdrożenie na produkcję – jest manualny**. Wymaga kliknięcia przycisku przez człowieka (np. Product Managera, lidera zespołu). Daje to biznesowi kontrolę nad tym, kiedy dana zmiana trafi do użytkowników.

#### Ciągłe Wdrażanie (Continuous Deployment - CD)

*   **Idea:** Najbardziej zaawansowana forma CI/CD. Jest to kolejny krok po Ciągłym Dostarczaniu.
*   **Proces:** Każda zmiana, która pomyślnie przejdzie przez cały zautomatyzowany potok testów, jest **automatycznie i natychmiastowo wdrażana na środowisko produkcyjne** bez żadnej interwencji człowieka.
*   **Cel:** Maksymalne skrócenie cyklu od pomysłu do dostarczenia wartości użytkownikowi. Wymaga bardzo wysokiego poziomu zaufania do zautomatyzowanego procesu testowania.

**CI → Continuous Delivery → Continuous Deployment** (każdy kolejny jest nadzbiorem poprzedniego)

#### Potok (Pipeline) CI/CD

Potok CI/CD to zautomatyzowana sekwencja kroków, przez które musi przejść kod od momentu commita do wdrożenia. Typowy potok wygląda następująco:

1.  **Commit:** Programista wysyła zmiany do repozytorium kodu (np. `git push`).
2.  **Build (Budowanie):** Serwer CI pobiera kod, kompiluje go i tworzy artefakt.
3.  **Test (Testowanie):** Uruchamiany jest zautomatyzowany zestaw testów (jednostkowych, integracyjnych).
4.  **Deploy (Wdrażanie):** Jeśli wszystkie poprzednie kroki się powiodły, aplikacja jest wdrażana na kolejne środowiska (testowe, stagingowe, a na końcu produkcyjne).

#### Narzędzia CI/CD

**1. Jenkins:**

*   **Co to jest:** Jeden z najstarszych, najbardziej znanych i potężnych serwerów automatyzacji typu open-source. Jest niezwykle elastyczny i rozszerzalny dzięki ogromnej liczbie dostępnych wtyczek (pluginów).
*   **Charakterystyka:**
    *   **Samodzielny serwer:** Wymaga własnej infrastruktury i konfiguracji.
    *   **Potoki jako kod (Pipeline as Code):** Potoki CI/CD definiuje się w specjalnym pliku tekstowym zwanym `Jenkinsfile`, który jest przechowywany razem z kodem w repozytorium. Pozwala to na wersjonowanie i przeglądanie definicji potoku.
    *   **Elastyczność:** Może być używany do automatyzacji praktycznie każdego zadania, nie tylko związanego z CI/CD.

**2. GitHub Actions:**

*   **Co to jest:** Narzędzie do automatyzacji przepływów pracy wbudowane bezpośrednio w platformę GitHub. Pozwala na tworzenie potoków CI/CD, które są uruchamiane w odpowiedzi na zdarzenia w repozytorium (np. push, utworzenie Pull Requesta).
*   **Charakterystyka:**
    *   **Zintegrowany z GitHubem:** Bardzo łatwa konfiguracja dla projektów hostowanych na GitHubie.
    *   **Potoki jako kod:** Przepływy pracy (workflows) definiuje się w plikach YAML przechowywanych w folderze `.github/workflows` w repozytorium.
    *   **Udostępniane akcje:** Ogromny marketplace gotowych "akcji" (małych, reużywalnych skryptów), które można łatwo włączyć do swojego potoku (np. akcja do logowania w chmurze AWS, akcja do budowania obrazu Dockera).
    *   **Infrastruktura:** Działa na zarządzanych przez GitHub "runnerach" (maszynach wirtualnych), ale można też skonfigurować własne.

| Cecha | Jenkins | GitHub Actions |
|---|---|---|
| **Typ** | Samodzielny serwer automatyzacji | Zintegrowana platforma CI/CD |
| **Konfiguracja** | Wymaga własnej instalacji i zarządzania | Wbudowane w GitHub, prosta konfiguracja |
| **Definicja potoku** | `Jenkinsfile` (język Groovy) | Pliki YAML |
| **Ekosystem** | Ogromna baza wtyczek (pluginów) | Marketplace gotowych akcji |
| **Integracja** | Integruje się ze wszystkim | Najlepsza integracja z ekosystemem GitHuba |

#### Podsumowanie

*   **CI/CD** to kluczowe praktyki DevOps, które automatyzują proces budowania, testowania i wdrażania oprogramowania.
*   **Ciągła Integracja (CI)** polega na częstym łączeniu zmian i ich automatycznym testowaniu.
*   **Ciągłe Dostarczanie (Continuous Delivery)** zapewnia, że każda zmiana jest gotowa do wdrożenia na produkcję za jednym kliknięciem.
*   **Ciągłe Wdrażanie (Continuous Deployment)** automatycznie wdraża każdą pomyślnie przetestowaną zmianę na produkcję.
*   **Jenkins** i **GitHub Actions** to popularne narzędzia, które pozwalają na implementację potoków CI/CD, automatyzując cały cykl życia aplikacji.

**Typowe pytania egzaminacyjne:**
*   Co oznaczają skróty CI i CD? Jaka jest między nimi różnica?
*   Jakie są główne korzyści z wdrożenia Ciągłej Integracji w projekcie?
*   Proszę opisać typowe etapy potoku CI/CD.
*   Czym jest Jenkins, a czym GitHub Actions?
*   Na czym polega idea "Pipeline as Code"?

---

# 49. Architektura i usługi sieci Internet

#### Wprowadzenie

Internet to globalna, zdecentralizowana sieć połączonych ze sobą sieci komputerowych, która zrewolucjonizowała komunikację, dostęp do informacji i sposób prowadzenia biznesu. Jego architektura i zasady działania opierają się na zestawie otwartych protokołów komunikacyjnych, z których najważniejszy to **pakiet protokołów TCP/IP**. Architektura ta umożliwia świadczenie ogromnej liczby różnorodnych **usług**, takich jak strony WWW, poczta elektroniczna czy przesyłanie plików, które stały się nieodłączną częścią naszego życia.

#### Architektura sieci Internet

Architektura Internetu jest z natury **zdecentralizowana i hierarchiczna**. Nie ma jednego centralnego punktu zarządzania. Składa się z tysięcy połączonych ze sobą, niezależnie zarządzanych sieci (tzw. systemów autonomicznych - AS), które należą do dostawców usług internetowych (ISP), firm, uniwersytetów i rządów.

**1. Model warstwowy TCP/IP:**

Podstawą komunikacji w Internecie jest model TCP/IP, który dzieli złożony proces komunikacji na cztery abstrakcyjne warstwy. Każda warstwa odpowiada za inne zadanie i korzysta z usług warstwy niższej.

*   **Warstwa aplikacji (Application Layer):** Najwyższa warstwa, z którą bezpośrednio interaguje użytkownik. Definiuje protokoły dla konkretnych usług internetowych (np. HTTP dla stron WWW, SMTP dla poczty e-mail).
*   **Warstwa transportowa (Transport Layer):** Odpowiada za komunikację między procesami na komputerach końcowych. Zapewnia niezawodne (protokół **TCP**) lub nieniezawodne (protokół **UDP**) dostarczanie danych.
*   **Warstwa internetowa (Internet Layer):** Odpowiada za adresowanie i routing pakietów danych w sieci. Jej głównym protokołem jest **IP (Internet Protocol)**, który definiuje adresy IP i zajmuje się przesyłaniem pakietów od źródła do celu przez potencjalnie wiele sieci pośrednich.
*   **Warstwa dostępu do sieci (Network Access Layer):** Najniższa warstwa, odpowiedzialna za fizyczne przesyłanie danych w ramach jednej sieci lokalnej (np. przez Ethernet, Wi-Fi).

**2. Modele architektury aplikacji sieciowych:**

*   **Model Klient-Serwer (Client-Server):** Dominujący model w Internecie. W tym modelu wyróżniamy dwa typy uczestników:
    *   **Serwer:** Potężny, zawsze włączony komputer, który posiada zasoby lub świadczy usługi (np. serwer WWW przechowujący pliki strony, serwer pocztowy). Czeka pasywnie na żądania od klientów.
    *   **Klient:** Komputer lub aplikacja (np. przeglądarka internetowa, klient poczty), która inicjuje komunikację, wysyłając żądanie do serwera i oczekując na odpowiedź.
    *   **Charakterystyka:** Centralizacja usług, łatwość zarządzania i bezpieczeństwa. Większość usług internetowych (WWW, e-mail) działa w tym modelu.
*   **Model Peer-to-Peer (P2P):**
    *   **Idea:** W tym modelu nie ma stałego podziału na klientów i serwery. Każdy uczestnik sieci (peer - równy) może jednocześnie pełnić rolę zarówno klienta (pobierając dane od innych), jak i serwera (udostępniając dane innym).
    *   **Charakterystyka:** Decentralizacja, skalowalność (im więcej uczestników, tym większa wydajność sieci), odporność na awarie pojedynczych węzłów.
    *   **Zastosowanie:** Systemy wymiany plików (np. BitTorrent), niektóre komunikatory internetowe, kryptowaluty (np. Bitcoin).

#### Podstawowe usługi sieci Internet

Usługi internetowe to aplikacje działające w warstwie aplikacji modelu TCP/IP, które dostarczają użytkownikom konkretnych funkcjonalności.

**1. World Wide Web (WWW):**

*   **Opis:** Najpopularniejsza usługa internetowa. Jest to globalny system połączonych ze sobą dokumentów hipertekstowych (stron internetowych), które można przeglądać za pomocą przeglądarki internetowej.
*   **Kluczowe technologie:**
    *   **HTTP (Hypertext Transfer Protocol):** Protokół do przesyłania żądań i odpowiedzi między przeglądarką a serwerem WWW.
    *   **HTML (Hypertext Markup Language):** Język do strukturyzacji i opisywania zawartości stron internetowych.
    *   **URL (Uniform Resource Locator):** Standardowy format adresowania zasobów w Internecie (np. `https://www.example.com`).

**2. Poczta elektroniczna (E-mail):**

*   **Opis:** Usługa umożliwiająca przesyłanie wiadomości tekstowych i załączników między użytkownikami.
*   **Kluczowe protokoły:**
    *   **SMTP (Simple Mail Transfer Protocol):** Używany do **wysyłania** wiadomości od klienta do serwera i między serwerami.
    *   **POP3 (Post Office Protocol 3) / IMAP (Internet Message Access Protocol):** Używane do **odbierania** wiadomości z serwera przez klienta poczty.

**3. Usługa nazw domenowych (DNS - Domain Name System):**

*   **Opis:** Kluczowa usługa działająca w tle, często nazywana "książką telefoniczną Internetu". Jej zadaniem jest tłumaczenie **czytelnych dla człowieka nazw domenowych** (np. `www.wikipedia.org`) na **numeryczne adresy IP** (np. `208.80.154.224`), które są niezbędne do nawiązania połączenia.
*   **Działanie:** Działa jako rozproszona, hierarchiczna baza danych. Gdy wpisujesz adres w przeglądarce, twój komputer wysyła zapytanie do serwera DNS, aby uzyskać odpowiadający mu adres IP.

**4. Usługa przesyłania plików (FTP - File Transfer Protocol):**

*   **Opis:** Protokół przeznaczony do transferu (pobierania i wysyłania) plików między komputerami w sieci. Działa w modelu klient-serwer.
*   **Charakterystyka:** Wykorzystuje dwa oddzielne połączenia: jedno do sterowania sesją, a drugie do przesyłania danych. W swojej podstawowej formie jest nieszyfrowany.

#### Podsumowanie

*   Architektura Internetu jest **zdecentralizowana** i opiera się na **warstwowym modelu TCP/IP**.
*   Dominującym modelem komunikacji aplikacji jest **klient-serwer**, w którym klient żąda usług od centralnego serwera. Alternatywą jest model **P2P**, gdzie każdy uczestnik jest równy.
*   Na fundamencie tej architektury działają kluczowe **usługi internetowe**:
    *   **WWW** do przeglądania stron (protokół HTTP).
    *   **E-mail** do komunikacji (protokoły SMTP, POP3/IMAP).
    *   **DNS** do tłumaczenia nazw domen na adresy IP.
    *   **FTP** do przesyłania plików.
*   Zrozumienie tych podstawowych koncepcji jest niezbędne do pojmowania, jak działa współczesny, połączony cyfrowy świat.

**Typowe pytania egzaminacyjne:**
*   Proszę opisać warstwy modelu TCP/IP.
*   Na czym polega różnica między modelem klient-serwer a modelem P2P? Proszę podać przykłady zastosowań obu modeli.
*   Jaka jest rola usługi DNS w działaniu Internetu?
*   Jakie protokoły są używane do wysyłania, a jakie do odbierania poczty elektronicznej?
*   Co oznaczają skróty HTTP, HTML i URL w kontekście usługi WWW?

---

# 50. Podstawowe pojęcia z zakresu bezpieczeństwa IT: zagrożenie, podatność, ryzyko, polityka bezpieczeństwa

#### Wprowadzenie

Bezpieczeństwo IT (informatyczne) to dziedzina zajmująca się ochroną systemów komputerowych, sieci i danych przed kradzieżą, uszkodzeniem, nieautoryzowanym dostępem lub innymi zagrożeniami. Celem jest zapewnienie trzech fundamentalnych atrybutów informacji, znanych jako **triada CIA**: **Poufności (Confidentiality)**, **Integralności (Integrity)** i **Dostępności (Availability)**. Zrozumienie podstawowych pojęć, takich jak zagrożenie, podatność i ryzyko, jest kluczowe do budowania skutecznej strategii obronnej, której ramy formalizuje **polityka bezpieczeństwa**.

#### Triada bezpieczeństwa CIA

*   **Poufność (Confidentiality):** Zapewnienie, że informacja jest dostępna tylko dla autoryzowanych osób. Ochrona przed nieuprawnionym ujawnieniem. *Mechanizmy: szyfrowanie, kontrola dostępu.*
*   **Integralność (Integrity):** Zapewnienie, że informacja jest kompletna, dokładna i nie została w nieautoryzowany sposób zmodyfikowana. Ochrona przed nieuprawnioną zmianą. *Mechanizmy: funkcje skrótu (hash), podpisy cyfrowe.*
*   **Dostępność (Availability):** Zapewnienie, że autoryzowani użytkownicy mają dostęp do informacji i zasobów wtedy, gdy tego potrzebują. Ochrona przed przerwami w działaniu usług. *Mechanizmy: redundancja, backupy, ochrona przed atakami DoS.*

#### Kluczowe pojęcia

**1. Zasób / Aktywo (Asset):**

*   **Definicja:** Dowolny element, który ma wartość dla organizacji i wymaga ochrony. Mogą to być dane (dane klientów, własność intelektualna), sprzęt (serwery, laptopy), oprogramowanie, a nawet reputacja firmy.

**2. Zagrożenie (Threat):**

*   **Definicja:** Potencjalne zdarzenie lub okoliczność (celowe lub przypadkowe), które może spowodować szkodę w systemie lub organizacji poprzez naruszenie poufności, integralności lub dostępności zasobów.
*   **Analogia:** Złodziej, który może okraść dom.
*   **Przykłady:**
    *   **Złośliwe oprogramowanie (malware):** Wirusy, trojany, ransomware.
    *   **Ataki sieciowe:** Phishing, ataki DoS (Denial of Service), Man-in-the-Middle.
    *   **Błędy ludzkie:** Przypadkowe usunięcie danych, kliknięcie w złośliwy link.
    *   **Awarie sprzętu, klęski żywiołowe.**

**3. Podatność (Vulnerability):**

*   **Definicja:** **Słabość lub luka** w zasobie, systemie, procesie lub mechanizmie kontrolnym, która może zostać wykorzystana przez zagrożenie.
*   **Analogia:** Otwarte okno lub niezamknięte drzwi w domu, które może wykorzystać złodziej.
*   **Przykłady:**
    *   **Błąd w oprogramowaniu:** Luka w kodzie aplikacji webowej umożliwiająca atak SQL Injection.
    *   **Brak aktualizacji:** Niezałatany system operacyjny lub oprogramowanie.
    *   **Słabe hasła:** Łatwe do odgadnięcia hasła użytkowników.
    *   **Brak procedur:** Brak polityki tworzenia kopii zapasowych.

**4. Ryzyko (Risk):**

*   **Definicja:** Prawdopodobieństwo, że dane zagrożenie wykorzysta daną podatność, oraz wielkość potencjalnych strat (wpływ) z tym związanych. Ryzyko to połączenie zagrożenia, podatności i wartości zasobu.
*   **Wzór (uproszczony):** `Ryzyko = Prawdopodobieństwo (Zagrożenie x Podatność) x Wpływ`
*   **Analogia:** Ryzyko, że złodziej wejdzie przez otwarte okno i ukradnie cenny obraz. Jeśli obraz jest bezwartościowy, ryzyko finansowe jest niskie. Jeśli prawdopodobieństwo pojawienia się złodzieja jest zerowe, ryzyko również jest niskie.
*   **Zarządzanie ryzykiem:** Proces identyfikacji, oceny i reagowania na ryzyko. Możliwe reakcje to:
    *   **Akceptacja:** Świadome zaakceptowanie ryzyka (gdy koszt zabezpieczeń przewyższa potencjalne straty).
    *   **Unikanie:** Eliminacja ryzyka poprzez rezygnację z działania, które je generuje.
    *   **Transfer:** Przeniesienie ryzyka na inny podmiot (np. poprzez wykupienie ubezpieczenia).
    *   **Mitygacja:** Zmniejszenie ryzyka poprzez wdrożenie zabezpieczeń (mechanizmów kontrolnych), które redukują prawdopodobieństwo lub wpływ.

#### Polityka bezpieczeństwa informacji (PBI)

*   **Definicja:** Formalny dokument najwyższego szczebla, który określa **cele, zasady, zakres i odpowiedzialność** za bezpieczeństwo informacji w organizacji. Jest to fundament systemu zarządzania bezpieczeństwem informacji (SZBI).
*   **Cel:** Ustanowienie jasnych wytycznych i zobowiązania kierownictwa do ochrony zasobów informacyjnych. Polityka odpowiada na pytanie **"co" i "dlaczego"** ma być chronione, a nie na pytanie "jak" (to jest zadanie dla bardziej szczegółowych procedur i standardów).
*   **Typowe elementy polityki bezpieczeństwa:**
    *   **Cel i zakres:** Co obejmuje polityka i dlaczego jest ważna.
    *   **Zobowiązanie kierownictwa:** Oświadczenie o wsparciu dla inicjatyw bezpieczeństwa.
    *   **Klasyfikacja informacji:** Zasady podziału danych ze względu na ich wrażliwość (np. publiczne, wewnętrzne, poufne, tajne).
    *   **Zasady kontroli dostępu:** Kto i na jakich zasadach ma mieć dostęp do informacji.
    *   **Zasady dotyczące haseł:** Wymagania co do złożoności, długości i cyklu życia haseł.
    *   **Bezpieczeństwo fizyczne:** Zasady ochrony sprzętu i pomieszczeń.
    *   **Zarządzanie incydentami:** Procedury reagowania na incydenty bezpieczeństwa.
    *   **Szkolenie i świadomość:** Wymagania dotyczące edukacji pracowników w zakresie bezpieczeństwa.
    *   **Odpowiedzialność:** Kto jest odpowiedzialny za poszczególne aspekty bezpieczeństwa.

#### Podsumowanie

*   Bezpieczeństwo IT opiera się na zapewnieniu **poufności, integralności i dostępności** informacji (triada CIA).
*   **Zagrożenie** to potencjalne niebezpieczeństwo, **podatność** to słabość, która pozwala zagrożeniu zadziałać, a **ryzyko** to prawdopodobieństwo i skutki tego zdarzenia.
*   Nie da się wyeliminować wszystkich zagrożeń, ale można zarządzać ryzykiem, głównie poprzez **łatanie podatności** (wdrażanie zabezpieczeń).
*   **Polityka bezpieczeństwa informacji** to formalny dokument, który stanowi podstawę dla wszystkich działań związanych z bezpieczeństwem w organizacji, definiując cele i zasady, które mają prowadzić do skutecznej ochrony jej zasobów.

**Typowe pytania egzaminacyjne:**
*   Proszę wyjaśnić, czym jest triada bezpieczeństwa CIA.
*   Jaka jest relacja między zagrożeniem, podatnością a ryzykiem? Proszę podać przykład ilustrujący te trzy pojęcia.
*   Co to jest polityka bezpieczeństwa informacji i jaki jest jej główny cel?
*   Proszę podać przykład podatności i zagrożenia, które może ją wykorzystać.
*   Na czym polega mitygacja ryzyka?

---

# 51. Kryptografia symetryczna i asymetryczna, klucz publiczny i prywatny, podpis cyfrowy

#### Wprowadzenie

**Kryptografia** to nauka o technikach umożliwiających bezpieczną komunikację w obecności stron trzecich. Jej głównym celem jest zapewnienie poufności i integralności danych poprzez ich **szyfrowanie**, czyli przekształcanie informacji (tekstu jawnego) w postać niezrozumiałą (szyfrogram) dla osób nieupoważnionych. Kluczem do tego procesu są **algorytmy szyfrujące** i **klucze kryptograficzne**. Istnieją dwa fundamentalnie różne podejścia do szyfrowania: **kryptografia symetryczna** i **kryptografia asymetryczna**.

#### Kryptografia symetryczna (z kluczem tajnym)

*   **Idea:** Najstarsza i najprostsza forma kryptografii. W tym podejściu **ten sam klucz** (zwany kluczem tajnym lub współdzielonym) jest używany zarówno do **szyfrowania**, jak i do **deszyfrowania** danych.
*   **Analogia:** Dwoje ludzi zamyka wiadomość w skrzynce na kłódkę i oboje mają identyczny klucz do tej kłódki. Nadawca zamyka skrzynkę, a odbiorca otwiera ją tym samym kluczem.
*   **Zalety:**
    *   **Szybkość:** Algorytmy symetryczne są bardzo wydajne obliczeniowo i potrafią szyfrować duże ilości danych w krótkim czasie.
*   **Wady:**
    *   **Problem dystrybucji klucza:** Największym wyzwaniem jest bezpieczne przekazanie tajnego klucza między nadawcą a odbiorcą. Jeśli klucz zostanie przechwycony przez osobę trzecią podczas przesyłania, cała komunikacja jest skompromitowana.
*   **Przykłady algorytmów:**
    *   **AES (Advanced Encryption Standard):** Obecny standard szyfrowania, używany powszechnie m.in. do zabezpieczania transmisji Wi-Fi (WPA2/WPA3) i szyfrowania plików.
    *   **DES/3DES (Data Encryption Standard):** Starszy standard, obecnie uważany za niezbyt bezpieczny.

#### Kryptografia asymetryczna (z kluczem publicznym)

*   **Idea:** Rewolucyjne podejście wprowadzone w latach 70. XX wieku. W tym systemie używana jest **para matematycznie powiązanych ze sobą kluczy** dla każdego użytkownika:
    *   **Klucz publiczny (Public Key):** Może i powinien być swobodnie dystrybuowany. Każdy może go mieć. Służy do **szyfrowania** danych przeznaczonych dla właściciela pary kluczy.
    *   **Klucz prywatny (Private Key):** Musi być utrzymywany w absolutnej tajemnicy przez jego właściciela. Służy do **deszyfrowania** danych, które zostały zaszyfrowane odpowiadającym mu kluczem publicznym.
*   **Analogia:** Klucz publiczny to **otwarta kłódka**, którą możesz dać każdemu. Każdy może wziąć twoją kłódkę, zamknąć nią wiadomość w skrzynce i ci ją wysłać. Ale tylko ty, posiadając **jedyny pasujący klucz prywatny**, jesteś w stanie tę kłódkę otworzyć i odczytać wiadomość.
*   **Zalety:**
    *   **Rozwiązuje problem dystrybucji klucza:** Nie ma potrzeby bezpiecznego przesyłania tajnego klucza. Wystarczy udostępnić swój klucz publiczny.
    *   **Umożliwia realizację podpisu cyfrowego.**
*   **Wady:**
    *   **Powolność:** Algorytmy asymetryczne są znacznie bardziej złożone obliczeniowo i tysiące razy wolniejsze od algorytmów symetrycznych. Nie nadają się do szyfrowania dużych ilości danych.
*   **Przykłady algorytmów:**
    *   **RSA (Rivest-Shamir-Adleman):** Najpopularniejszy algorytm, oparty na trudności faktoryzacji (rozkładu na czynniki pierwsze) dużych liczb.
    *   **Kryptografia krzywych eliptycznych (ECC):** Nowocześniejsze podejście, które oferuje ten sam poziom bezpieczeństwa przy znacznie krótszych kluczach.

| Cecha | Kryptografia symetryczna | Kryptografia asymetryczna |
|---|---|---|
| **Liczba kluczy** | Jeden (współdzielony, tajny) | Dwa (publiczny i prywatny) |
| **Szybkość** | Bardzo szybka | Bardzo wolna |
| **Główne zastosowanie** | Szyfrowanie dużych ilości danych | Bezpieczna wymiana kluczy, podpisy cyfrowe |
| **Problem** | Bezpieczna dystrybucja klucza | Powolność działania |

#### Zastosowanie hybrydowe

W praktyce, aby połączyć zalety obu podejść, stosuje się **szyfrowanie hybrydowe**. Tak działa m.in. protokół **TLS/SSL**, który zabezpiecza komunikację w Internecie (HTTPS):

1.  **Wymiana klucza:** Przeglądarka (klient) używa **kryptografii asymetrycznej** (klucza publicznego serwera), aby bezpiecznie uzgodnić z serwerem jednorazowy, losowo wygenerowany **klucz symetryczny** (tzw. klucz sesji).
2.  **Szyfrowanie danych:** Cała dalsza komunikacja (przesyłanie danych strony WWW) jest szyfrowana za pomocą tego szybkiego, **symetrycznego klucza sesji**.

#### Podpis cyfrowy

Kryptografia asymetryczna umożliwia stworzenie mechanizmu **podpisu cyfrowego**, który zapewnia trzy kluczowe usługi bezpieczeństwa:

*   **Uwierzytelnienie (Authentication):** Potwierdzenie tożsamości nadawcy.
*   **Integralność (Integrity):** Gwarancja, że wiadomość nie została zmieniona po podpisaniu.
*   **Niezaprzeczalność (Non-repudiation):** Nadawca nie może wyprzeć się faktu podpisania wiadomości.

**Jak działa podpis cyfrowy?**

Proces jest "odwróceniem" szyfrowania asymetrycznego:

1.  **Tworzenie skrótu:** Nadawca tworzy skrót (hash) z treści wiadomości za pomocą funkcji skrótu (np. SHA-256).
2.  **Szyfrowanie skrótu:** Nadawca **szyfruje ten skrót za pomocą swojego klucza PRYWATNEGO**. Wynik tego szyfrowania to właśnie podpis cyfrowy, który jest dołączany do wiadomości.
3.  **Weryfikacja podpisu:** Odbiorca otrzymuje wiadomość i podpis. Następnie:
    a.  Samodzielnie oblicza skrót z otrzymanej wiadomości.
    b.  **Deszyfruje otrzymany podpis za pomocą klucza PUBLICZNEGO nadawcy**, uzyskując oryginalny skrót obliczony przez nadawcę.
    c.  Porównuje oba skróty. Jeśli są identyczne, oznacza to, że podpis jest prawidłowy – wiadomość pochodzi od właściciela klucza prywatnego i nie została zmieniona w trakcie przesyłania.

#### Podsumowanie

*   **Kryptografia symetryczna** używa **jednego klucza** do szyfrowania i deszyfrowania; jest **szybka**, ale ma problem z bezpieczną wymianą klucza.
*   **Kryptografia asymetryczna** używa **pary kluczy (publicznego i prywatnego)**; jest **wolna**, ale rozwiązuje problem wymiany klucza i umożliwia tworzenie **podpisów cyfrowych**.
*   **Podpis cyfrowy** jest tworzony przez zaszyfrowanie skrótu wiadomości **kluczem prywatnym** i służy do uwierzytelnienia nadawcy oraz zapewnienia integralności danych.
*   W praktyce najczęściej stosuje się **podejście hybrydowe**, używając kryptografii asymetrycznej do bezpiecznej wymiany klucza symetrycznego, którym następnie szyfrowane są dane.

**Typowe pytania egzaminacyjne:**
*   Proszę porównać kryptografię symetryczną i asymetryczną, wskazując ich wady i zalety.
*   Jaka jest rola klucza publicznego, a jaka prywatnego?
*   Jak działa podpis cyfrowy i jakie gwarancje bezpieczeństwa zapewnia?
*   Dlaczego w praktyce często stosuje się szyfrowanie hybrydowe?
*   Jaki problem rozwiązuje kryptografia asymetryczna, który jest największą wadą kryptografii symetrycznej?

---

# 52. Złośliwe oprogramowanie i ataki sieciowe

#### Wprowadzenie

Bezpieczeństwo w cyfrowym świecie jest nieustannie zagrożone przez szeroką gamę **złośliwego oprogramowania (malware)** oraz **ataków sieciowych**. Zrozumienie ich natury, metod działania i celów jest pierwszym krokiem do skutecznej obrony. Malware to ogólne określenie na wszelkie oprogramowanie stworzone w celu uszkodzenia, zakłócenia działania lub uzyskania nieautoryzowanego dostępu do systemów komputerowych. Ataki sieciowe to z kolei działania podejmowane w celu wykorzystania podatności w sieciach i systemach w celu kradzieży danych, zakłócenia usług lub innych szkodliwych działań.

#### Rodzaje złośliwego oprogramowania (Malware)

**1. Wirus (Virus):**

*   **Sposób działania:** Fragment kodu, który **dołącza się do istniejącego, legalnego programu** (tzw. nosiciela). Wirus wymaga interakcji użytkownika (np. uruchomienia zainfekowanego programu), aby się aktywować i rozprzestrzeniać. Gdy zainfekowany program jest uruchamiany, wirus replikuje się, infekując kolejne pliki.
*   **Analogia:** Biologiczny wirus, który potrzebuje komórki gospodarza do replikacji.

**2. Robak (Worm):**

*   **Sposób działania:** Samodzielny program, który w przeciwieństwie do wirusa, **nie potrzebuje nosiciela ani interakcji użytkownika do rozprzestrzeniania się**. Robaki aktywnie wykorzystują podatności w sieci (np. w systemach operacyjnych, usługach sieciowych), aby samodzielnie replikować się i infekować kolejne komputery.
*   **Cel:** Szybkie rozprzestrzenianie się i tworzenie botnetów (sieci zainfekowanych komputerów).

**3. Koń trojański (Trojan Horse):**

*   **Sposób działania:** Złośliwe oprogramowanie, które **podszywa się pod użyteczną lub legalną aplikację**, aby skłonić użytkownika do jego instalacji i uruchomienia. Trojan sam w sobie się nie replikuje, ale jego głównym celem jest otwarcie "tylnej furtki" (backdoor) w systemie, która umożliwia atakującemu zdalny dostęp i kontrolę nad komputerem.
*   **Analogia:** Mitologiczny koń trojański, który ukrywał greckich żołnierzy.

**4. Ransomware:**

*   **Sposób działania:** Rodzaj malware, który **szyfruje pliki na dysku ofiary**, uniemożliwiając do nich dostęp. Następnie wyświetla żądanie okupu (ransom), zazwyczaj w kryptowalucie, w zamian za klucz deszyfrujący.
*   **Cel:** Bezpośredni zysk finansowy.

**5. Spyware (Oprogramowanie szpiegujące):**

*   **Sposób działania:** Oprogramowanie, które potajemnie zbiera informacje o użytkowniku i jego aktywności bez jego wiedzy i zgody. Może rejestrować wciskane klawisze (**keylogger**), historię przeglądania, dane logowania, a nawet nagrywać obraz z kamery.
*   **Cel:** Kradzież poufnych informacji (dane osobowe, hasła, numery kart kredytowych).

**6. Adware (Oprogramowanie reklamowe):**

*   **Sposób działania:** Oprogramowanie, które automatycznie wyświetla niechciane reklamy (np. w postaci wyskakujących okienek) w celu generowania przychodu dla jego autora. Choć często jest tylko irytujące, może również zbierać dane o użytkowniku i stanowić zagrożenie dla prywatności.

#### Najczęstsze ataki sieciowe

**1. Phishing:**

*   **Sposób działania:** Atak z kategorii **inżynierii społecznej**. Atakujący podszywa się pod zaufaną osobę lub instytucję (np. bank, firmę kurierską, portal społecznościowy) i za pomocą fałszywych wiadomości e-mail, SMS lub na komunikatorach próbuje **wyłudzić od ofiary poufne informacje**, takie jak dane logowania, hasła czy numery kart kredytowych. Wiadomości te często zawierają link do fałszywej strony internetowej, która do złudzenia przypomina prawdziwą.

**2. Atak DoS (Denial of Service) i DDoS (Distributed Denial of Service):**

*   **Sposób działania:** Celem ataku jest **uniemożliwienie działania usługi sieciowej** (np. strony internetowej) poprzez jej przeciążenie. W ataku **DoS** ruch generowany jest z jednego źródła. W znacznie potężniejszym ataku **DDoS**, ruch jest generowany jednocześnie z wielu (tysięcy, a nawet milionów) zainfekowanych komputerów (botnetu) z całego świata, co sprawia, że obrona jest niezwykle trudna.

**3. Atak Man-in-the-Middle (MitM):**

*   **Sposób działania:** Atakujący potajemnie **przechwytuje i ewentualnie modyfikuje komunikację** między dwiema stronami, które są przekonane, że komunikują się bezpośrednio ze sobą. Atakujący staje się "człowiekiem pośrodku", mogąc podsłuchiwać i manipulować całym ruchem sieciowym.
*   **Przykład:** Atakujący w publicznej sieci Wi-Fi może przekierować ruch ofiary przez swój komputer, aby przechwycić np. dane logowania do banku (jeśli strona nie używa szyfrowania HTTPS).

**4. Wstrzyknięcie SQL (SQL Injection - SQLi):**

*   **Sposób działania:** Atak na aplikacje internetowe, które korzystają z bazy danych SQL. Polega na wstrzyknięciu złośliwego kodu SQL do pól formularza na stronie internetowej (np. w polu loginu lub hasła). Jeśli aplikacja jest podatna, wykonuje ten złośliwy kod na swojej bazie danych, co może prowadzić do ominięcia logowania, kradzieży, modyfikacji lub usunięcia danych.

**5. Cross-Site Scripting (XSS):**

*   **Sposób działania:** Atak na aplikacje internetowe, polegający na umieszczeniu (wstrzyknięciu) złośliwego skryptu (zazwyczaj JavaScript) na stronie internetowej, który następnie jest wykonywany w przeglądarce innych użytkowników odwiedzających tę stronę. Może to prowadzić do kradzieży sesji użytkownika, ciasteczek lub przekierowania na złośliwe strony.

#### Podsumowanie

*   **Malware** to szeroka kategoria złośliwego oprogramowania, obejmująca m.in. **wirusy** (potrzebują nosiciela), **robaki** (samodzielnie się replikują), **trojany** (udają legalne programy), **ransomware** (szyfrują dane dla okupu) i **spyware** (szpiegują użytkownika).
*   **Ataki sieciowe** wykorzystują podatności w systemach i sieciach. Do najczęstszych należą **phishing** (inżynieria społeczna), **DDoS** (przeciążanie usług), **Man-in-the-Middle** (podsłuchiwanie komunikacji) oraz ataki na aplikacje webowe jak **SQL Injection** i **XSS**.
*   Skuteczna obrona wymaga wielowarstwowego podejścia, obejmującego zarówno zabezpieczenia techniczne (antywirus, firewall, szyfrowanie), jak i, co najważniejsze, **świadomość i edukację użytkowników**, którzy często są najsłabszym ogniwem w łańcuchu bezpieczeństwa.

**Typowe pytania egzaminacyjne:**
*   Czym różni się wirus od robaka komputerowego?
*   Na czym polega działanie konia trojańskiego?
*   Proszę opisać atak typu phishing.
*   Jaki jest cel ataku DDoS?
*   Na czym polega atak SQL Injection i jakie mogą być jego konsekwencje?

---

# 53. Etyka w informatyce, kodeksy etyczne

#### Wprowadzenie

**Etyka w informatyce** to dziedzina filozofii, która zajmuje się analizą i rozwiązywaniem problemów moralnych pojawiających się w związku z tworzeniem i użytkowaniem technologii informatycznych. W miarę jak komputery i oprogramowanie stają się wszechobecne i mają coraz większy wpływ na każdy aspekt ludzkiego życia – od komunikacji, przez finanse, po opiekę zdrowotną – rośnie odpowiedzialność etyczna informatyków, programistów, analityków i administratorów. Aby pomóc profesjonalistom w podejmowaniu właściwych decyzji, największe organizacje branżowe, takie jak **ACM** i **IEEE**, opracowały **kodeksy etyczne**, które służą jako zbiór zasad i wytycznych postępowania.

#### Kluczowe dylematy etyczne w informatyce

*   **Prywatność:** Jak pogodzić gromadzenie i analizę ogromnych ilości danych (Big Data) z prawem jednostki do prywatności? Kto ma prawo do naszych danych i jak powinny być one chronione?
*   **Bezpieczeństwo:** Jaka jest odpowiedzialność twórców oprogramowania za luki w bezpieczeństwie, które mogą prowadzić do kradzieży danych lub innych szkód?
*   **Własność intelektualna:** Jakie są granice ochrony praw autorskich w cyfrowym świecie, gdzie kopiowanie jest trywialnie proste? Kiedy oprogramowanie open-source jest etycznym wyborem?
*   **Sztuczna inteligencja i algorytmy:** Jak zapewnić, że algorytmy (np. w systemach rekrutacyjnych, policyjnych, kredytowych) są sprawiedliwe i nie dyskryminują określonych grup społecznych? Kto jest odpowiedzialny za decyzje podejmowane przez autonomiczne systemy (np. autonomiczne pojazdy)?
*   **Wpływ na społeczeństwo:** Jaka jest rola informatyków w cyfrowej przepaści (digital divide), automatyzacji pracy i wpływie mediów społecznościowych na zdrowie psychiczne i dyskurs publiczny?
*   **Odpowiedzialność zawodowa:** Do jakiego stopnia informatyk jest odpowiedzialny za sposób, w jaki jego praca jest wykorzystywana przez pracodawcę lub klienta (np. tworzenie oprogramowania do inwigilacji lub celów wojskowych)?

#### Kodeksy etyczne

Kodeksy etyczne nie są zbiorem praw, ale raczej przewodnikiem moralnym, który ma inspirować i kierować profesjonalistów IT. Pomagają one w rozwiązywaniu dylematów i promują kulturę odpowiedzialności. Dwa najważniejsze kodeksy w świecie informatyki to:

**1. Kodeks Etyki i Postępowania Zawodowego ACM (Association for Computing Machinery):**

Jest to najbardziej wpływowy i szeroko rozpoznawany kodeks w branży. Jego najnowsza wersja z 2018 roku jest podzielona na cztery sekcje:

**Sekcja 1: Ogólne zasady etyczne.** To są fundamentalne wartości, które powinny przyświecać każdemu informatykowi. Obejmują one imperatywy takie jak:
*   **1.1 Przyczyniaj się do dobra społeczeństwa i ludzkości.** (Nadrzędna zasada).
*   **1.2 Unikaj wyrządzania krzywdy.** (Podstawowa zasada etyki – "po pierwsze nie szkodzić").
*   **1.3 Bądź uczciwy i godny zaufania.**
*   **1.4 Bądź sprawiedliwy i podejmuj działania, aby nie dyskryminować.**
*   **1.5 Szanuj pracę wymaganą do tworzenia nowych pomysłów, wynalazków i dzieł (własność intelektualna).**
*   **1.6 Szanuj prywatność.**
*   **1.7 Szanuj poufność.**

**Sekcja 2: Odpowiedzialność zawodowa.** Te zasady odnoszą się do zachowania w kontekście pracy zawodowej.
*   **2.1 Dąż do wysokiej jakości zarówno w procesach, jak i produktach pracy zawodowej.**
*   **2.2 Utrzymuj wysokie standardy kompetencji zawodowych, postępowania i praktyki etycznej.**
*   **2.5 Zapewnij kompleksową i dogłębną ocenę systemów komputerowych i ich wpływu, włączając analizę możliwego ryzyka.**
*   **2.8 Projektuj i implementuj systemy, które są solidne i bezpieczne.**

**Sekcja 3: Zasady dotyczące przywództwa.** Skierowane do liderów i osób na stanowiskach kierowniczych.
*   **3.1 Zapewnij, że dobro publiczne jest centralnym zagadnieniem podczas całej pracy.**
*   **3.7 Twórz możliwości nauki, rozwoju i awansu dla członków organizacji.**

**Sekcja 4: Zgodność z kodeksem.** Podkreśla obowiązek przestrzegania kodeksu przez wszystkich członków profesji.

**2. Kodeks Etyki IEEE (Institute of Electrical and Electronics Engineers):**

Jest to kodeks dla szerszej grupy inżynierów, w tym inżynierów oprogramowania. Jest bardziej zwięzły, ale jego duch jest bardzo podobny do kodeksu ACM. Zobowiązuje on członków m.in. do:

*   **Przyjmowania odpowiedzialności** za podejmowane decyzje inżynierskie i dbania o bezpieczeństwo, zdrowie i dobro publiczne.
*   **Unikania konfliktów interesów.**
*   **Bycia uczciwym i realistycznym** w swoich oświadczeniach i szacunkach.
*   **Odrzucania łapówkarstwa** we wszystkich jego formach.
*   **Doskonalenia swojej wiedzy technicznej** i podejmowania się zadań tylko w obszarze swoich kompetencji.
*   **Uczciwego krytykowania pracy innych**, bycia otwartym na krytykę i doceniania wkładu innych.
*   **Traktowania wszystkich ludzi sprawiedliwie.**
*   **Unikania wyrządzania krzywdy innym**, ich własności, reputacji lub zatrudnieniu poprzez fałszywe lub złośliwe działania.
*   **Pomagania kolegom** w ich rozwoju zawodowym i wspierania ich w przestrzeganiu kodeksu.

#### Podsumowanie

*   **Etyka w informatyce** to krytyczna refleksja nad moralnymi konsekwencjami technologii, która staje się coraz ważniejsza w miarę wzrostu jej wpływu na społeczeństwo.
*   Informatycy stają przed wieloma **dylematami etycznymi** dotyczącymi prywatności, bezpieczeństwa, sprawiedliwości algorytmicznej i własności intelektualnej.
*   **Kodeksy etyczne**, takie jak te stworzone przez **ACM** i **IEEE**, dostarczają ram i wytycznych, które pomagają profesjonalistom w podejmowaniu odpowiedzialnych decyzji.
*   Nadrzędną zasadą, która przewija się przez wszystkie kodeksy, jest **działanie na rzecz dobra publicznego i unikanie wyrządzania krzywdy**.
*   Przestrzeganie zasad etycznych to nie tylko obowiązek, ale także fundament budowania zaufania publicznego do zawodu informatyka i technologii, którą tworzy.

**Typowe pytania egzaminacyjne:**
*   Proszę podać i opisać co najmniej trzy dylematy etyczne, z którymi spotykają się współcześni informatycy.
*   Jaki jest cel istnienia kodeksów etycznych w zawodach technicznych?
*   Proszę wymienić i omówić co najmniej trzy ogólne zasady etyczne z kodeksu ACM.
*   Na czym polega zasada "unikaj wyrządzania krzywdy" w kontekście tworzenia oprogramowania?
*   Dlaczego kwestia sprawiedliwości algorytmów (algorithmic fairness) jest ważnym problemem etycznym?

---

# 54. Prawne aspekty oprogramowania: prawa autorskie, patenty, licencje

#### Wprowadzenie

Oprogramowanie, jako produkt intelektualnej pracy człowieka, podlega ochronie prawnej. Zrozumienie podstawowych mechanizmów tej ochrony – **praw autorskich**, **patentów** i **licencji** – jest kluczowe zarówno dla twórców, jak i użytkowników oprogramowania. Te trzy koncepcje regulują, kto jest właścicielem kodu, jak można go używać, modyfikować i dystrybuować. Błędne zrozumienie tych zasad może prowadzić do poważnych konsekwencji prawnych i finansowych.

#### Prawa autorskie (Copyright)

*   **Co chronią?** Prawo autorskie jest podstawową i automatyczną formą ochrony programów komputerowych. Chroni ono **sposób wyrażenia idei (ekspresję), a nie samą ideę, algorytm czy funkcjonalność**. W kontekście oprogramowania ochronie podlega przede wszystkim **kod źródłowy i kod maszynowy**, które są traktowane jak utwory literackie. Ochroną może być objęty również wygląd interfejsu użytkownika (jako utwór plastyczny) czy dokumentacja.
*   **Jak powstaje ochrona?** Ochrona prawnoautorska powstaje **automatycznie z chwilą ustalenia (stworzenia) utworu**, bez potrzeby jakiejkolwiek rejestracji. Twórca od razu nabywa dwa rodzaje praw:
    *   **Prawa autorskie osobiste:** Są niezbywalne i chronią więź twórcy z utworem (np. prawo do autorstwa, prawo do nienaruszalności treści).
    *   **Prawa autorskie majątkowe:** Są zbywalne i dają twórcy wyłączne prawo do korzystania z utworu, rozporządzania nim i pobierania wynagrodzenia za jego używanie (np. prawo do zwielokrotniania, modyfikowania, rozpowszechniania).
*   **Przejście praw:** W przypadku, gdy programista tworzy oprogramowanie w ramach stosunku pracy, prawa majątkowe do tego programu co do zasady przechodzą na pracodawcę.

#### Patenty (Patents)

*   **Co chronią?** W przeciwieństwie do praw autorskich, patent **chroni konkretny wynalazek – czyli nowatorskie, nieoczywiste i użyteczne rozwiązanie techniczne**. W kontekście oprogramowania, opatentować można nie kod, ale **innowacyjny algorytm, metodę przetwarzania danych lub proces realizowany przez oprogramowanie**.
*   **Jak powstaje ochrona?** Ochrona patentowa **nie powstaje automatycznie**. Wymaga złożenia wniosku i przejścia skomplikowanej i kosztownej procedury w urzędzie patentowym, który bada, czy wynalazek spełnia kryteria nowości, poziomu wynalazczego i przemysłowej stosowalności.
*   **Kontrowersje:** Patentowalność oprogramowania jest tematem kontrowersyjnym. Krytycy argumentują, że hamuje ona innowacyjność, pozwalając dużym firmom patentować ogólne idee i pozywać mniejszych konkurentów. W Europie prawo jest bardziej restrykcyjne niż w USA i wymaga, aby wynalazek wspomagany komputerowo miał "charakter techniczny".

| Cecha | Prawa autorskie | Patenty |
|---|---|---|
| **Przedmiot ochrony** | Ekspresja idei (kod) | Idea, wynalazek (algorytm, proces) |
| **Powstanie ochrony** | Automatyczne, w momencie stworzenia | Wymaga rejestracji w urzędzie patentowym |
| **Czas trwania** | Zazwyczaj całe życie twórcy + 70 lat | Zazwyczaj 20 lat od daty zgłoszenia |
| **Wymagania** | Oryginalność, indywidualny charakter | Nowość, poziom wynalazczy, stosowalność przemysłowa |

#### Licencje oprogramowania (Software Licenses)

*   **Co to jest?** Licencja to **umowa prawna** między właścicielem praw autorskich (licencjodawcą) a użytkownikiem (licencjobiorcą), która określa **warunki, na jakich użytkownik może korzystać z oprogramowania**. Ponieważ użytkownik co do zasady nie kupuje oprogramowania (nie staje się jego właścicielem), a jedynie prawo do korzystania z niego, licencja jest kluczowym dokumentem definiującym jego uprawnienia i obowiązki.

**Rodzaje licencji:**

**1. Oprogramowanie własnościowe (Proprietary Software):**
*   **Charakterystyka:** Oprogramowanie, którego kod źródłowy jest zamknięty i stanowi tajemnicę przedsiębiorstwa. Użytkownik otrzymuje jedynie wersję wykonywalną. Licencje te są zazwyczaj bardzo restrykcyjne.
*   **Przykłady:**
    *   **Licencja komercyjna:** Użytkownik płaci za prawo do korzystania z programu (np. Microsoft Windows, Adobe Photoshop).
    *   **Shareware:** Użytkownik może bezpłatnie testować program przez określony czas (trial) lub w ograniczonej funkcjonalności, po czym musi zapłacić za pełną wersję.
    *   **Freeware:** Oprogramowanie jest darmowe, ale jego kod źródłowy pozostaje zamknięty, a licencja może ograniczać np. użycie komercyjne.

**2. Oprogramowanie otwarte (Open Source):**
*   **Charakterystyka:** Oprogramowanie, którego kod źródłowy jest publicznie dostępny. Każdy może go przeglądać, modyfikować i rozpowszechniać. Licencje open-source gwarantują te wolności, ale mogą nakładać pewne warunki.
*   **Dwa główne typy licencji open-source:**
    *   **Licencje permisywne (Permissive):** Bardzo liberalne. Pozwalają na niemal dowolne wykorzystanie kodu, w tym włączenie go do oprogramowania własnościowego (zamkniętego), bez konieczności udostępniania własnych modyfikacji. Wymagają zazwyczaj jedynie zachowania informacji o oryginalnym autorze.
        *   *Przykłady: Licencja MIT, Apache 2.0, licencje BSD.*
    *   **Licencje typu copyleft (lub "wirusowe"):** Gwarantują, że oprogramowanie i wszystkie jego **pochodne wersje** pozostaną otwarte. Jeśli użyjesz kodu na licencji copyleft w swoim programie, to cały ten program również musisz udostępnić na tej samej licencji (udostępnić jego kod źródłowy).
        *   *Przykłady: GNU GPL (General Public License), AGPL.*

#### Podsumowanie

*   **Prawa autorskie** automatycznie chronią kod oprogramowania jako utwór literacki.
*   **Patenty** mogą chronić innowacyjne algorytmy i procesy, ale wymagają skomplikowanej rejestracji.
*   **Licencja** to umowa, która określa, jak użytkownik może korzystać z oprogramowania. Jest to kluczowy instrument prawny regulujący relacje między twórcą a użytkownikiem.
*   Licencje na **oprogramowanie własnościowe** są restrykcyjne i chronią interes komercyjny producenta.
*   Licencje **open-source** promują wolność i współpracę, ale dzielą się na **permisywne** (pozwalające na włączenie do kodu zamkniętego) i **copyleft** (wymagające, aby pochodne również były otwarte).
*   Wybór odpowiedniej licencji ma fundamentalne znaczenie dla modelu biznesowego i przyszłości projektu oprogramowania.

**Typowe pytania egzaminacyjne:**
*   Czym różni się ochrona prawnoautorska od ochrony patentowej w kontekście oprogramowania?
*   Co to jest licencja oprogramowania i jaki jest jej cel?
*   Proszę porównać licencje typu copyleft (np. GPL) z licencjami permisywnymi (np. MIT).
*   Czy można używać kodu na licencji open-source w projekcie komercyjnym?
*   Kiedy prawa autorskie do programu stworzonego przez pracownika należą do pracodawcy?

---

# 55. Chmura obliczeniowa: modele usług (IaaS, PaaS, SaaS) i wdrożenia (prywatna, publiczna, hybrydowa)

#### Wprowadzenie

**Chmura obliczeniowa (Cloud Computing)** to model dostarczania usług obliczeniowych – takich jak serwery, pamięć masowa, bazy danych, sieci, oprogramowanie i analityka – przez Internet ("chmurę"). Zamiast kupować, posiadać i utrzymywać własne centra danych i serwery, organizacje mogą wynajmować dostęp do tych usług od dostawcy chmury (np. Amazon Web Services - AWS, Microsoft Azure, Google Cloud Platform - GCP). Płaci się tylko za te zasoby, z których się korzysta, co pozwala na obniżenie kosztów, elastyczne skalowanie i szybsze wdrażanie innowacji. Usługi chmurowe są klasyfikowane według **modeli usług** (co dostajemy) i **modeli wdrożenia** (gdzie to działa).

#### Modele usług chmurowych

Modele te można przedstawić jako piramidę abstrakcji. Im wyżej w piramidzie, tym więcej zarządzania przejmuje na siebie dostawca chmury, a mniej odpowiedzialności spoczywa na użytkowniku.

**1. IaaS (Infrastructure as a Service - Infrastruktura jako usługa):**

*   **Co to jest?** Najbardziej podstawowy model. Dostawca chmury udostępnia **fundamentalne zasoby infrastruktury IT**: wirtualne maszyny (serwery), pamięć masową i sieci. Użytkownik wynajmuje wirtualny sprzęt.
*   **Użytkownik zarządza:** Systemem operacyjnym, oprogramowaniem pośredniczącym (middleware), środowiskiem uruchomieniowym i aplikacjami.
*   **Dostawca zarządza:** Fizycznymi serwerami, siecią i centrami danych.
*   **Analogia:** Wynajem działki budowlanej. Dostajesz ziemię i przyłącza, ale sam musisz zbudować dom, położyć instalacje i go urządzić.
*   **Dla kogo:** Administratorzy systemów, zespoły DevOps, firmy, które chcą mieć pełną kontrolę nad swoją infrastrukturą, ale nie chcą zarządzać fizycznym sprzętem.
*   **Przykłady:** Amazon EC2 (wirtualne serwery), Google Compute Engine, Microsoft Azure VMs.

**2. PaaS (Platform as a Service - Platforma jako usługa):**

*   **Co to jest?** Model, który dostarcza użytkownikom **kompletną platformę do tworzenia, testowania, wdrażania i zarządzania aplikacjami**, bez martwienia się o bazową infrastrukturę.
*   **Użytkownik zarządza:** Tylko swoją aplikacją i danymi.
*   **Dostawca zarządza:** Całą infrastrukturą (serwerami, siecią), systemem operacyjnym, oprogramowaniem pośredniczącym i środowiskiem uruchomieniowym (np. Java, Python, .NET).
*   **Analogia:** Wynajem umeblowanego mieszkania. Masz gotowe miejsce do życia z wszystkimi instalacjami, musisz tylko wnieść swoje rzeczy osobiste.
*   **Dla kogo:** Deweloperzy, którzy chcą skupić się wyłącznie na pisaniu kodu, a nie na zarządzaniu serwerami, systemami operacyjnymi i aktualizacjami.
*   **Przykłady:** Heroku, AWS Elastic Beanstalk, Google App Engine, Azure App Service.

**3. SaaS (Software as a Service - Oprogramowanie jako usługa):**

*   **Co to jest?** Najwyższy poziom abstrakcji. Dostawca udostępnia **gotową do użycia aplikację**, dostępną przez Internet, zazwyczaj w modelu subskrypcyjnym. Użytkownik po prostu loguje się i korzysta z oprogramowania przez przeglądarkę internetową.
*   **Użytkownik zarządza:** Niczym (poza ewentualną konfiguracją swojego konta).
*   **Dostawca zarządza:** Absolutnie wszystkim: infrastrukturą, platformą i samą aplikacją.
*   **Analogia:** Wynajem pokoju w hotelu. Wszystko jest gotowe i obsługiwane, ty tylko korzystasz z usługi.
*   **Dla kogo:** Użytkownicy końcowi, firmy, które potrzebują gotowych rozwiązań biznesowych bez żadnych inwestycji w IT.
*   **Przykłady:** Gmail, Microsoft 365, Salesforce, Dropbox, Netflix.

| | IaaS (Ty zarządzasz) | PaaS (Ty zarządzasz) | SaaS (Ty zarządzasz) |
|---|---|---|---|
| **Aplikacje** | ✅ | ✅ | ❌ |
| **Dane** | ✅ | ✅ | ❌ |
| **Środowisko uruchomieniowe** | ✅ | ❌ | ❌ |
| **Oprogramowanie pośredniczące** | ✅ | ❌ | ❌ |
| **System operacyjny** | ✅ | ❌ | ❌ |
| **Wirtualizacja** | ❌ | ❌ | ❌ |
| **Serwery** | ❌ | ❌ | ❌ |
| **Pamięć masowa** | ❌ | ❌ | ❌ |
| **Sieć** | ❌ | ❌ | ❌ |

#### Modele wdrożenia chmury

Modele te określają, gdzie fizycznie znajduje się infrastruktura chmurowa i kto jest jej właścicielem.

**1. Chmura publiczna (Public Cloud):**

*   **Opis:** Infrastruktura należy do zewnętrznego dostawcy (np. AWS, Google, Microsoft) i jest udostępniana wielu klientom przez publiczny Internet. Klienci dzielą te same zasoby sprzętowe (w modelu multi-tenant).
*   **Zalety:** Ogromna skalowalność, model pay-as-you-go (płacisz za to, co zużyjesz), brak kosztów początkowych, wysoka niezawodność.
*   **Wady:** Mniejsza kontrola nad infrastrukturą, potencjalne obawy dotyczące bezpieczeństwa i rezydencji danych.

**2. Chmura prywatna (Private Cloud):**

*   **Opis:** Infrastruktura jest dedykowana i używana wyłącznie przez jedną organizację. Może być zlokalizowana w centrum danych tej organizacji (on-premise) lub hostowana przez zewnętrznego dostawcę, ale na wyłączność.
*   **Zalety:** Maksymalna kontrola, wysokie bezpieczeństwo, łatwiejsze spełnienie rygorystycznych wymogów regulacyjnych.
*   **Wady:** Wysokie koszty początkowe i utrzymania, mniejsza elastyczność i skalowalność, organizacja jest w pełni odpowiedzialna za zarządzanie.

**3. Chmura hybrydowa (Hybrid Cloud):**

*   **Opis:** Połączenie chmury publicznej i prywatnej, które są ze sobą zintegrowane i umożliwiają przenoszenie danych i aplikacji między nimi. Organizacja może trzymać wrażliwe dane w chmurze prywatnej, a jednocześnie korzystać z ogromnej mocy obliczeniowej chmury publicznej do mniej krytycznych zadań lub obsługi skoków ruchu (cloud bursting).
*   **Zalety:** Elastyczność, optymalizacja kosztów, możliwość wykorzystania najlepszych cech obu światów.
*   **Wady:** Złożoność zarządzania i integracji.

#### Podsumowanie

*   **Chmura obliczeniowa** to model dostarczania zasobów IT na żądanie przez Internet.
*   **Modele usług** określają poziom abstrakcji: **IaaS** (infrastruktura), **PaaS** (platforma dla deweloperów) i **SaaS** (gotowe aplikacje).
*   **Modele wdrożenia** określają własność i lokalizację infrastruktury: **publiczna** (dzielona, u dostawcy), **prywatna** (dedykowana, własna lub u dostawcy) i **hybrydowa** (połączenie obu).
*   Wybór odpowiedniego modelu zależy od potrzeb biznesowych, wymagań bezpieczeństwa, budżetu i posiadanych kompetencji technicznych.

**Typowe pytania egzaminacyjne:**
*   Co to jest chmura obliczeniowa i jakie są jej główne zalety w porównaniu z tradycyjnym modelem IT?
*   Proszę porównać modele usług IaaS, PaaS i SaaS, podając przykłady dla każdego z nich.
*   Jaka jest różnica między chmurą publiczną a prywatną?
*   W jakiej sytuacji firma mogłaby zdecydować się na wdrożenie chmury hybrydowej?
*   Który model usługi chmurowej (IaaS, PaaS, SaaS) daje użytkownikowi największą kontrolę, a który najmniejszą?

---

# 56. Uczenie maszynowe: uczenie nadzorowane, nienadzorowane i ze wzmocnieniem

#### Wprowadzenie

**Uczenie maszynowe (Machine Learning - ML)** to dziedzina sztucznej inteligencji (AI), która koncentruje się na tworzeniu algorytmów i modeli, które potrafią **uczyć się na podstawie danych** i wyciągać z nich wnioski lub dokonywać przewidywań, bez bycia jawnie zaprogramowanymi do wykonania konkretnego zadania. Zamiast pisać sztywne reguły, programista "trenuje" model, dostarczając mu dużą ilość danych, a algorytm sam odkrywa w nich wzorce. Uczenie maszynowe można podzielić na trzy główne paradygmaty, różniące się rodzajem danych wejściowych i sposobem "uczenia" się modelu: **uczenie nadzorowane, nienadzorowane i ze wzmocnieniem**.

#### Uczenie nadzorowane (Supervised Learning)

*   **Idea:** Najpopularniejszy i najbardziej intuicyjny rodzaj uczenia maszynowego. Model uczy się na podstawie **oznakowanych (etykietowanych) danych treningowych**. Oznacza to, że dla każdej próbki danych wejściowych mamy przypisaną poprawną odpowiedź (etykietę).
*   **Analogia:** Uczeń (model) uczy się pod okiem nauczyciela (dane treningowe). Nauczyciel pokazuje uczniowi przykłady (np. zdjęcia zwierząt) i podaje poprawne odpowiedzi ("to jest kot", "to jest pies"). Po przejrzeniu wielu przykładów uczeń uczy się samodzielnie rozpoznawać nowe, nieznane mu wcześniej zdjęcia.
*   **Cel:** Nauczenie modelu funkcji, która potrafi mapować nowe, nieoznakowane dane wejściowe na poprawne dane wyjściowe.
*   **Dwa główne typy problemów:**
    *   **Klasyfikacja (Classification):** Przewidywanie **kategorii (etykiety dyskretnej)**. Odpowiedź na pytanie "Do jakiej grupy to należy?".
        *   *Przykłady:* Klasyfikacja e-maili jako "spam" lub "nie spam", rozpoznawanie cyfr na obrazach, diagnoza medyczna (pacjent "chory" lub "zdrowy"), analiza sentymentu (opinia "pozytywna" lub "negatywna").
        *   *Algorytmy:* Drzewa decyzyjne, regresja logistyczna, maszyny wektorów nośnych (SVM), sieci neuronowe.
    *   **Regresja (Regression):** Przewidywanie **wartości ciągłej (liczby)**. Odpowiedź na pytanie "Ile to będzie wynosić?".
        *   *Przykłady:* Prognozowanie ceny domu na podstawie jego cech (powierzchnia, lokalizacja), przewidywanie temperatury, prognozowanie sprzedaży.
        *   *Algorytmy:* Regresja liniowa, regresja wielomianowa, drzewa decyzyjne.

#### Uczenie nienadzorowane (Unsupervised Learning)

*   **Idea:** Model uczy się na podstawie **nieoznakowanych danych**. Nie ma "nauczyciela" ani poprawnych odpowiedzi. Zadaniem algorytmu jest samodzielne odkrycie ukrytej struktury, wzorców lub relacji w danych.
*   **Analogia:** Analityk, który dostaje ogromny zbiór danych o klientach i ma za zadanie samodzielnie znaleźć w nich interesujące grupy lub segmenty, nie wiedząc z góry, jakie one będą.
*   **Cel:** Zrozumienie danych i odkrycie w nich wewnętrznej struktury.
*   **Dwa główne typy problemów:**
    *   **Klastrowanie / Grupowanie (Clustering):** Automatyczne grupowanie podobnych do siebie próbek danych w klastry. Odpowiedź na pytanie "Jakie naturalne grupy istnieją w tych danych?".
        *   *Przykłady:* Segmentacja klientów na podstawie ich zachowań zakupowych, grupowanie artykułów informacyjnych według tematyki, grupowanie genów o podobnej ekspresji.
        *   *Algorytmy:* k-średnich (k-means), grupowanie hierarchiczne.
    *   **Redukcja wymiarowości (Dimensionality Reduction):** Zmniejszanie liczby zmiennych (cech) w danych przy jednoczesnym zachowaniu jak największej ilości informacji. Używane do wizualizacji danych wielowymiarowych i upraszczania modeli.
        *   *Przykłady:* Kompresja obrazu, analiza głównych składowych (PCA).

#### Uczenie ze wzmocnieniem (Reinforcement Learning)

*   **Idea:** Paradygmat inspirowany psychologią behawioralną. Model (zwany **agentem**) uczy się poprzez **interakcję ze środowiskiem**. Agent podejmuje akcje, a w odpowiedzi otrzymuje od środowiska informację o nowym stanie oraz **sygnał nagrody lub kary**. Celem agenta jest nauczenie się takiej strategii (polityki) podejmowania akcji, która maksymalizuje sumę otrzymanych nagród w długim okresie.
*   **Analogia:** Uczenie psa nowej sztuczki. Gdy pies wykonuje pożądaną akcję (np. siada na komendę), dostaje nagrodę (smakołyk). Gdy robi coś niepożądanego, nie dostaje nic. Metodą prób i błędów pies uczy się, jakie zachowanie prowadzi do nagrody.
*   **Cel:** Znalezienie optymalnej strategii działania w danym środowisku.
*   **Przykłady:**
    *   Uczenie maszyn gry w gry (np. szachy, Go - AlphaGo, gry komputerowe).
    *   Robotyka (uczenie robotów chodzenia, chwytania obiektów).
    *   Systemy rekomendacyjne, zarządzanie portfelem inwestycyjnym, optymalizacja ruchu ulicznego.

| Cecha | Uczenie nadzorowane | Uczenie nienadzorowane | Uczenie ze wzmocnieniem |
|---|---|---|---|
| **Dane wejściowe** | Oznakowane (z poprawnymi odpowiedziami) | Nieoznakowane | Brak danych, interakcja ze środowiskiem |
| **Cel** | Przewidywanie (klasyfikacja, regresja) | Odkrywanie struktury (klastrowanie) | Znalezienie optymalnej strategii działania |
| **Informacja zwrotna** | Bezpośrednia (poprawna odpowiedź) | Brak | Nagroda/kara (sygnał zwrotny) |
| **Przykład** | Rozpoznawanie spamu | Segmentacja klientów | Gra w szachy |

#### Podsumowanie

*   **Uczenie maszynowe** to potężne narzędzie do automatycznego odkrywania wzorców w danych.
*   **Uczenie nadzorowane** jest idealne do problemów predykcyjnych, gdy dysponujemy historycznymi danymi z poprawnymi odpowiedziami (np. klasyfikacja i regresja).
*   **Uczenie nienadzorowane** służy do eksploracji danych i odkrywania w nich ukrytych struktur, gdy nie mamy etykiet (np. klastrowanie).
*   **Uczenie ze wzmocnieniem** jest stosowane w problemach decyzyjnych, gdzie agent musi nauczyć się optymalnego zachowania poprzez metodę prób i błędów w interaktywnym środowisku.
*   Wybór odpowiedniego paradygmatu uczenia zależy od natury problemu i rodzaju dostępnych danych.

**Typowe pytania egzaminacyjne:**
*   Co to jest uczenie maszynowe i czym różni się od tradycyjnego programowania?
*   Proszę porównać uczenie nadzorowane i nienadzorowane. Jaka jest główna różnica w danych, na których operują?
*   Podaj przykład problemu klasyfikacji i problemu regresji.
*   Na czym polega uczenie ze wzmocnieniem? Proszę opisać ten proces na przykładzie.
*   Do jakiego typu uczenia maszynowego należy problem segmentacji klientów sklepu internetowego?

---

# 57. Sztuczne sieci neuronowe, głębokie uczenie (deep learning)

#### Wprowadzenie

**Sztuczne sieci neuronowe (Artificial Neural Networks - ANN)** to modele obliczeniowe inspirowane biologicznymi sieciami neuronowymi, które stanowią mózg człowieka. Są one fundamentem wielu nowoczesnych systemów sztucznej inteligencji. **Głębokie uczenie (Deep Learning)** to poddziedzina uczenia maszynowego, która wykorzystuje **głębokie sieci neuronowe** – czyli sieci o wielu warstwach – do automatycznego uczenia się złożonych wzorców i hierarchicznych reprezentacji bezpośrednio z danych. To właśnie rewolucja w głębokim uczeniu doprowadziła do przełomów w takich dziedzinach jak rozpoznawanie obrazów, przetwarzanie języka naturalnego i autonomiczne pojazdy.

#### Sztuczna sieć neuronowa

**1. Perceptron – podstawowy budulec:**

*   **Inspiracja:** Pojedynczy neuron biologiczny.
*   **Działanie:** Sztuczny neuron (perceptron) otrzymuje jeden lub więcej sygnałów wejściowych. Każde wejście ma przypisaną **wagę**, która symbolizuje jego ważność. Neuron sumuje wszystkie ważone wejścia, dodaje do nich stałą wartość zwaną **obciążeniem (bias)**, a następnie przepuszcza wynik przez **funkcję aktywacji**. Funkcja aktywacji decyduje, czy i z jaką siłą neuron ma "odpalić" (przekazać sygnał dalej).

**2. Architektura sieci:**

*   Neurony są zorganizowane w **warstwy**:
    *   **Warstwa wejściowa (Input Layer):** Otrzymuje surowe dane (np. piksele obrazu, słowa w zdaniu).
    *   **Warstwy ukryte (Hidden Layers):** Warstwy pośrednie między wejściem a wyjściem. To w nich zachodzi większość obliczeń i ekstrakcja cech. Sieć może mieć jedną lub więcej warstw ukrytych.
    *   **Warstwa wyjściowa (Output Layer):** Produkuje ostateczny wynik (np. prawdopodobieństwo, że na obrazie jest kot; przewidywaną cenę domu).
*   W najprostszej sieci (typu feedforward) sygnał przepływa w jednym kierunku: od warstwy wejściowej, przez warstwy ukryte, do warstwy wyjściowej.

**3. Proces uczenia (trenowania):**

*   Proces uczenia sieci neuronowej polega na **dostrajaniu jej wag i obciążeń** tak, aby dla danych wejściowych produkowała jak najbliższe prawdy wyniki. Odbywa się to w iteracyjnym procesie:
    1.  **Propagacja w przód (Forward Propagation):** Dane wejściowe są przepuszczane przez sieć, aby uzyskać wynik.
    2.  **Obliczenie błędu:** Wynik sieci jest porównywany z oczekiwanym wynikiem (etykietą), a różnica między nimi jest obliczana za pomocą **funkcji straty (loss function)**.
    3.  **Propagacja wsteczna (Backpropagation):** Błąd jest propagowany "wstecz" przez sieć, od warstwy wyjściowej do wejściowej.
    4.  **Aktualizacja wag:** Na podstawie obliczonego błędu, wagi i obciążenia w sieci są nieznacznie modyfikowane za pomocą algorytmu optymalizacji (np. **algorytmu spadku gradientowego - Gradient Descent**), aby zmniejszyć błąd w następnej iteracji.
*   Ten cykl powtarza się tysiące lub miliony razy na całym zbiorze treningowym, aż sieć nauczy się poprawnie generalizować i dokonywać trafnych predykcji na nowych danych.

#### Głębokie uczenie (Deep Learning)

*   **Deep Learning vs Machine Learning:** Głębokie uczenie **jest** uczeniem maszynowym. Jest to jego wyspecjalizowana poddziedzina. Główna różnica polega na tym, że tradycyjne uczenie maszynowe często wymaga od eksperta ręcznego przygotowania i selekcji cech z surowych danych (tzw. inżynieria cech). W głębokim uczeniu, **głęboka sieć neuronowa uczy się tych cech automatycznie** w sposób hierarchiczny. Pierwsze warstwy uczą się prostych cech (np. krawędzie, kolory), a kolejne warstwy składają je w coraz bardziej złożone koncepty (np. oczy, nos, całe twarze).
*   **Co oznacza "głęboka" sieć?** Termin "głęboka" odnosi się do dużej liczby warstw ukrytych w sieci (od kilku do setek). To właśnie ta głębia pozwala na naukę bardzo złożonych i abstrakcyjnych reprezentacji danych.

#### Główne architektury sieci głębokich

**1. Konwolucyjne Sieci Neuronowe (Convolutional Neural Networks - CNN):**

*   **Specjalizacja:** Przetwarzanie danych o strukturze siatki, przede wszystkim **obrazów**.
*   **Kluczowa idea:** Zamiast przetwarzać cały obraz na raz, CNN używają **filtrów (kernels)**, które przesuwają się po obrazie (operacja **konwolucji**), aby wykrywać lokalne wzorce, takie jak krawędzie, tekstury czy kształty. Dzięki współdzieleniu wag w filtrach, są one niezwykle wydajne w analizie danych wizualnych.
*   **Zastosowania:** Rozpoznawanie i klasyfikacja obrazów, detekcja obiektów, segmentacja obrazu, analiza obrazów medycznych.

**2. Rekurencyjne Sieci Neuronowe (Recurrent Neural Networks - RNN):**

*   **Specjalizacja:** Przetwarzanie **danych sekwencyjnych**, gdzie kolejność ma znaczenie.
*   **Kluczowa idea:** RNN posiadają wewnętrzną "pamięć" (stan ukryty), która pozwala im przetwarzać sekwencje krok po kroku, uwzględniając informacje z poprzednich kroków. Posiadają pętlę, która pozwala na przekazywanie informacji z jednego kroku sekwencji do następnego.
*   **Zastosowania:** Przetwarzanie języka naturalnego (tłumaczenie maszynowe, analiza sentymentu, generowanie tekstu), rozpoznawanie mowy, prognozowanie szeregów czasowych.
*   **Warianty:** Popularne i bardziej zaawansowane warianty RNN, które lepiej radzą sobie z długimi sekwencjami, to **LSTM (Long Short-Term Memory)** i **GRU (Gated Recurrent Unit)**.

#### Podsumowanie

*   **Sztuczne sieci neuronowe** to modele inspirowane działaniem mózgu, składające się z połączonych neuronów zorganizowanych w warstwy.
*   Uczą się one poprzez iteracyjne dostrajanie **wag** za pomocą algorytmu **propagacji wstecznej**.
*   **Głębokie uczenie** wykorzystuje **głębokie sieci neuronowe** (z wieloma warstwami ukrytymi) do automatycznego uczenia się hierarchicznych cech bezpośrednio z danych.
*   **Konwolucyjne Sieci Neuronowe (CNN)** są wyspecjalizowane w przetwarzaniu **obrazów**.
*   **Rekurencyjne Sieci Neuronowe (RNN)** są wyspecjalizowane w przetwarzaniu **danych sekwencyjnych** (np. tekstu, szeregów czasowych).
*   Głębokie uczenie jest siłą napędową obecnej rewolucji w sztucznej inteligencji, umożliwiając rozwiązywanie problemów, które jeszcze dekadę temu wydawały się poza zasięgiem.

**Typowe pytania egzaminacyjne:**
*   Jak w uproszczeniu działa pojedynczy sztuczny neuron?
*   Na czym polega proces uczenia sieci neuronowej? Proszę opisać rolę propagacji w przód i propagacji wstecznej.
*   Jaka jest główna różnica między tradycyjnym uczeniem maszynowym a głębokim uczeniem?
*   Do jakiego typu problemów najlepiej nadają się Konwolucyjne Sieci Neuronowe (CNN), a do jakich Rekurencyjne Sieci Neuronowe (RNN)?
*   Proszę podać dwa przykłady zastosowań głębokiego uczenia.

---

# 58. Przetwarzanie języka naturalnego (NLP)

#### Wprowadzenie

**Przetwarzanie języka naturalnego (Natural Language Processing - NLP)** to interdyscyplinarna dziedzina z pogranicza informatyki, sztucznej inteligencji i lingwistyki, której celem jest umożliwienie komputerom **rozumienia, interpretowania, manipulowania i generowania ludzkiego języka** (zarówno w formie tekstu, jak i mowy). Język ludzki jest z natury niejednoznaczny, pełen niuansów, metafor i kontekstu, co sprawia, że jego automatyczne przetwarzanie jest niezwykle trudnym zadaniem. NLP jest siłą napędową wielu aplikacji, z których korzystamy na co dzień, takich jak tłumacze online, chatboty, asystenci głosowi czy systemy analizy opinii.

#### Główne zadania i zastosowania NLP

*   **Tłumaczenie maszynowe (Machine Translation):** Automatyczne tłumaczenie tekstu z jednego języka na drugi (np. Tłumacz Google).
*   **Analiza sentymentu (Sentiment Analysis):** Określanie emocjonalnego zabarwienia (wydźwięku) tekstu – czy jest on pozytywny, negatywny czy neutralny. Używane do analizy opinii o produktach, recenzji filmów, komentarzy w mediach społecznościowych.
*   **Rozpoznawanie mowy (Speech Recognition):** Konwersja języka mówionego na tekst (np. dyktowanie w smartfonie, transkrypcja nagrań).
*   **Generowanie języka naturalnego (Natural Language Generation - NLG):** Tworzenie tekstu w języku naturalnym na podstawie ustrukturyzowanych danych (np. generowanie raportów pogodowych, opisów produktów).
*   **Systemy Pytanie-Odpowiedź (Question Answering - QA):** Systemy, które potrafią odpowiedzieć na pytania zadane w języku naturalnym (np. wyszukiwarki internetowe, chatboty).
*   **Rozpoznawanie nazwanych encji (Named Entity Recognition - NER):** Identyfikowanie i kategoryzowanie w tekście kluczowych informacji, takich jak imiona i nazwiska, nazwy organizacji, lokalizacje, daty.
*   **Modelowanie tematyczne (Topic Modeling):** Automatyczne odkrywanie głównych tematów w dużym zbiorze dokumentów.

#### Typowy potok (pipeline) przetwarzania tekstu

Zanim tekst zostanie poddany analizie przez zaawansowane modele, musi przejść przez serię kroków przygotowawczych (preprocessing), które sprowadzają go do ustrukturyzowanej, numerycznej formy, zrozumiałej dla komputera.

**1. Segmentacja (Segmentation):**

*   Dzielenie dłuższego tekstu na mniejsze jednostki, zazwyczaj na **zdania**.

**2. Tokenizacja (Tokenization):**

*   Dzielenie zdań na jeszcze mniejsze jednostki zwane **tokenami**, którymi najczęściej są **pojedyncze słowa** lub znaki interpunkcyjne. Na przykład zdanie "NLP jest fascynujące!" zostanie podzielone na tokeny: `["NLP", "jest", "fascynujące", "!"]`.

**3. Usunięcie stop-słów (Stop Words Removal):**

*   Usuwanie z tekstu najczęściej występujących, ale nieniosących wiele znaczenia słów, takich jak spójniki, przyimki, zaimki (np. "i", "w", "się", "jest", "ale"). Pozwala to skupić się na słowach kluczowych.

**4. Normalizacja:**

*   Sprowadzenie słów do ich podstawowej, kanonicznej formy. Ma to na celu traktowanie różnych form gramatycznych tego samego słowa jako jednego pojęcia (np. "idę", "poszedł", "szli" powinny być traktowane jako "iść"). Dwa główne podejścia to:
    *   **Stemming:** Upraszczająca heurystyka, która polega na **obcinaniu końcówek fleksyjnych** słów, aby sprowadzić je do rdzenia (stem). Jest to proces szybki, ale często niedokładny i może prowadzić do tworzenia nieistniejących słów (np. "uniwersytet" -> "uniwersyt").
    *   **Lematyzacja (Lemmatization):** Bardziej zaawansowane podejście, które wykorzystuje analizę morfologiczną i słownik, aby sprowadzić słowo do jego **formy podstawowej (lematu)**. Jest to proces wolniejszy, ale znacznie dokładniejszy (np. "idę" -> "iść", "byłem" -> "być").

**5. Wektoryzacja (Vectorization):**

*   Ostatni i kluczowy krok, polegający na **przekształceniu tekstu w postać numeryczną (wektory liczb)**, która może być przetworzona przez algorytmy uczenia maszynowego. Popularne techniki to:
    *   **Bag-of-Words (BoW):** Reprezentowanie dokumentu jako wektora, w którym każda pozycja odpowiada liczbie wystąpień danego słowa ze słownika w dokumencie. Ignoruje kolejność słów.
    *   **TF-IDF (Term Frequency-Inverse Document Frequency):** Ulepszenie BoW, które przypisuje wagę każdemu słowu w dokumencie. Waga jest tym wyższa, im częściej słowo występuje w danym dokumencie, ale jednocześnie im rzadziej występuje we wszystkich pozostałych dokumentach (co oznacza, że jest bardziej unikalne i charakterystyczne dla tego dokumentu).
    *   **Zanurzenia słów (Word Embeddings):** Nowoczesne podejście (np. **Word2Vec, GloVe, BERT**), w którym każde słowo jest reprezentowane jako gęsty wektor w wielowymiarowej przestrzeni. Słowa o podobnym znaczeniu mają podobne wektory (leżą blisko siebie w tej przestrzeni), co pozwala modelom na uchwycenie relacji semantycznych między słowami.

#### Podsumowanie

*   **Przetwarzanie języka naturalnego (NLP)** to dziedzina AI, która uczy komputery rozumieć i przetwarzać ludzki język.
*   NLP ma szerokie zastosowania, od **tłumaczenia maszynowego** i **analizy sentymentu** po **chatboty** i **rozpoznawanie mowy**.
*   Przetwarzanie tekstu zazwyczaj wymaga wieloetapowego **potoku (pipeline)**, który obejmuje m.in. **tokenizację**, **normalizację (stemming/lematyzację)** i **wektoryzację**.
*   Nowoczesne NLP w dużej mierze opiera się na **głębokim uczeniu** i modelach takich jak **sieci rekurencyjne (RNN)** i **transformery (np. BERT, GPT)**, które potrafią uczyć się złożonych reprezentacji języka (word embeddings) i rozumieć kontekst.

**Typowe pytania egzaminacyjne:**
*   Co to jest przetwarzanie języka naturalnego (NLP) i jakie są jego główne cele?
*   Proszę wymienić i opisać co najmniej trzy zastosowania NLP.
*   Na czym polega różnica między stemmingiem a lematyzacją?
*   Jaki jest cel wektoryzacji tekstu w NLP?
*   Co to jest analiza sentymentu?

---

# 59. Systemy rozproszone, Big Data

#### Wprowadzenie

**System rozproszony** to zbiór niezależnych komputerów (węzłów), które komunikują się ze sobą przez sieć i współpracują w celu osiągnięcia wspólnego celu, sprawiając wrażenie jednego, spójnego systemu dla użytkownika końcowego. Współczesny internet, usługi chmurowe i praktycznie każda duża aplikacja internetowa są z natury systemami rozproszonymi. Jednym z głównych motorów napędowych rozwoju systemów rozproszonych jest zjawisko **Big Data**, czyli potrzeba przetwarzania i analizowania ogromnych zbiorów danych, które przekraczają możliwości pojedynczego komputera.

#### Systemy rozproszone

**Kluczowe cechy i cele:**

*   **Współdzielenie zasobów (Resource Sharing):** Umożliwiają wielu użytkownikom i aplikacjom współdzielenie zasobów, takich jak drukarki, pliki, bazy danych czy moc obliczeniowa.
*   **Przezroczystość (Transparency):** Idealny system rozproszony ukrywa przed użytkownikiem swoją wewnętrzną złożoność. Użytkownik nie musi wiedzieć, na którym fizycznie komputerze wykonywane jest jego zadanie lub gdzie przechowywane są jego dane.
*   **Otwartość (Openness):** Są zbudowane w oparciu o standardowe, dobrze zdefiniowane interfejsy (np. protokoły sieciowe), co ułatwia ich rozbudowę i interoperacyjność.
*   **Skalowalność (Scalability):** System powinien być w stanie obsłużyć rosnącą liczbę użytkowników i zadań bez degradacji wydajności. W systemach rozproszonych skalowalność osiąga się głównie poprzez **skalowanie horyzontalne** – dodawanie kolejnych, standardowych maszyn (węzłów) do systemu.

**Wyzwania w systemach rozproszonych:**

*   **Współbieżność (Concurrency):** Wiele procesów może jednocześnie próbować uzyskać dostęp do tych samych zasobów, co wymaga skomplikowanych mechanizmów synchronizacji.
*   **Brak globalnego zegara:** Każdy komputer ma własny zegar, co utrudnia ustalenie dokładnej kolejności zdarzeń w systemie.
*   **Częściowe awarie (Partial Failures):** W przeciwieństwie do systemu scentralizowanego, który albo działa, albo nie, w systemie rozproszonym niektóre węzły mogą ulec awarii, podczas gdy inne wciąż działają. System musi być **odporny na awarie (fault-tolerant)** i potrafić kontynuować pracę mimo awarii jego części.
*   **Niezawodność komunikacji:** Komunikacja sieciowa jest z natury zawodna – wiadomości mogą być gubione, opóźniane lub dostarczane w innej kolejności.

#### Big Data

Big Data to termin opisujący ogromne, złożone zbiory danych, których przetwarzanie i analiza za pomocą tradycyjnych narzędzi jest niemożliwe lub niepraktyczne. Charakterystykę Big Data często opisuje się za pomocą modelu "V".

**Model 3V (później rozszerzany do 5V i więcej):**

1.  **Volume (Objętość/Wielkość):** Odnosi się do **ogromnej ilości** generowanych i przechowywanych danych. Mówimy tu o terabajtach, petabajtach, a nawet eksabajtach danych pochodzących z mediów społecznościowych, czujników IoT, transakcji finansowych itp.
2.  **Velocity (Szybkość/Prędkość):** Odnosi się do **wysokiej prędkości**, z jaką dane są generowane i muszą być przetwarzane, często w czasie rzeczywistym lub prawie rzeczywistym. Przykładem są dane giełdowe, strumienie kliknięć na stronach internetowych czy dane z czujników w autonomicznych pojazdach.
3.  **Variety (Różnorodność):** Odnosi się do **szerokiej gamy formatów i typów danych**. Dane te mogą być:
    *   **Ustrukturyzowane (Structured):** Dane o stałym formacie, łatwe do umieszczenia w tabelach relacyjnej bazy danych (np. dane z formularzy, transakcje).
    *   **Nieustrukturyzowane (Unstructured):** Dane bez z góry zdefiniowanego modelu, takie jak tekst, obrazy, wideo, pliki audio.
    *   **Półustrukturyzowane (Semi-structured):** Dane, które nie pasują do sztywnego schematu bazy relacyjnej, ale zawierają pewne znaczniki organizacyjne (np. pliki JSON, XML).

**Dodatkowe "V" często dodawane do modelu:**

*   **Veracity (Wiarygodność/Prawdziwość):** Odnosi się do jakości i zaufania do danych. Dane w zbiorach Big Data mogą być niekompletne, niespójne i niedokładne.
*   **Value (Wartość):** Odnosi się do zdolności do przekształcenia danych w wartość biznesową. Samo posiadanie danych nie ma znaczenia, jeśli nie potrafimy z nich wyciągnąć użytecznych wniosków.

#### Technologie Big Data

Do przetwarzania Big Data wykorzystuje się wyspecjalizowane systemy rozproszone, które potrafią rozdzielić obliczenia na setki lub tysiące maszyn (klaster). Najważniejszym ekosystemem w tym obszarze jest **Apache Hadoop**.

*   **Hadoop:** Platforma open-source do rozproszonego przechowywania i przetwarzania wielkich zbiorów danych. Jej dwa kluczowe komponenty to:
    *   **HDFS (Hadoop Distributed File System):** Rozproszony system plików, który dzieli duże pliki na bloki i przechowuje je w sposób redundantny na wielu maszynach w klastrze, zapewniając odporność na awarie.
    *   **MapReduce:** Paradygmat programowania i framework do przetwarzania danych w sposób równoległy. Proces składa się z dwóch faz: **Map** (gdzie dane są filtrowane i transformowane na poszczególnych węzłach) i **Reduce** (gdzie wyniki z fazy Map są agregowane w celu uzyskania ostatecznego rezultatu).
*   **Apache Spark:** Nowocześniejszy i znacznie szybszy następca MapReduce. Spark wykonuje obliczenia **w pamięci RAM** (in-memory), co drastycznie przyspiesza przetwarzanie w porównaniu do dyskowego modelu MapReduce. Stał się de facto standardem w przetwarzaniu Big Data. Oferuje bogate API do przetwarzania wsadowego, strumieniowego, uczenia maszynowego (MLlib) i przetwarzania grafów.

#### Podsumowanie

*   **Systemy rozproszone** to fundament nowoczesnej informatyki, umożliwiający budowanie skalowalnych i odpornych na awarie aplikacji poprzez koordynację pracy wielu połączonych siecią komputerów.
*   **Big Data** to zjawisko charakteryzujące się ogromną **objętością**, **szybkością** i **różnorodnością** danych, które wymagają specjalistycznych narzędzi do ich przetwarzania.
*   Wyzwania związane z Big Data są rozwiązywane za pomocą **systemów rozproszonych**, takich jak **Hadoop** i **Spark**, które pozwalają na równoległe przetwarzanie danych na dużą skalę.
*   Zrozumienie zasad działania systemów rozproszonych i technologii Big Data jest kluczowe w erze, gdzie dane stały się jednym z najcenniejszych zasobów.

**Typowe pytania egzaminacyjne:**
*   Co to jest system rozproszony i jakie są jego kluczowe cechy?
*   Proszę opisać model 3V charakteryzujący Big Data.
*   Jakie są główne wyzwania w projektowaniu systemów rozproszonych?
*   Jaka jest rola HDFS i MapReduce w ekosystemie Hadoop?
*   Dlaczego Apache Spark jest generalnie szybszy niż tradycyjny Hadoop MapReduce?

---

# 60. Internet Rzeczy (Internet of Things - IoT)

#### Wprowadzenie

**Internet Rzeczy (Internet of Things - IoT)** to koncepcja, w której przedmioty codziennego użytku – od zegarków i lodówek, przez samochody, aż po maszyny przemysłowe – są wyposażone w **czujniki, oprogramowanie i inne technologie**, które pozwalają im **łączyć się z internetem oraz wymieniać dane** między sobą i z innymi systemami. Celem IoT jest stworzenie inteligentniejszego, bardziej responsywnego świata poprzez połączenie świata fizycznego ze światem cyfrowym. Urządzenia te, zwane "inteligentnymi" (smart), mogą autonomicznie zbierać informacje o swoim otoczeniu, komunikować się i podejmować działania bez bezpośredniej interwencji człowieka.

#### Typowa architektura IoT

Architekturę systemu IoT można zazwyczaj podzielić na cztery kluczowe warstwy:

**1. Warstwa percepcji / urządzeń (Perception / Device Layer):**

*   **Komponenty:** To fizyczne "rzeczy" w IoT. Składa się z **czujników (sensorów)**, które zbierają dane ze świata fizycznego (np. temperatura, wilgotność, ruch, lokalizacja GPS, ciśnienie) oraz **aktuatorów (elementów wykonawczych)**, które mogą wpływać na ten świat (np. włączyć światło, zamknąć zamek, zmienić ustawienie termostatu).
*   **Zadanie:** Zbieranie danych i/lub wykonywanie akcji.

**2. Warstwa sieci / łączności (Network / Connectivity Layer):**

*   **Komponenty:** Ta warstwa jest odpowiedzialna za **przesyłanie danych** zebranych przez czujniki do systemów przetwarzania. Wykorzystuje do tego różne technologie komunikacyjne, zarówno krótko-, jak i długozasięgowe.
*   **Technologie:** Wi-Fi, Bluetooth, Zigbee, LoRaWAN, a także sieci komórkowe (4G/5G).
*   **Zadanie:** Zapewnienie niezawodnej komunikacji między urządzeniami a chmurą.

**3. Warstwa przetwarzania / platformy (Processing / Platform Layer):**

*   **Komponenty:** Zazwyczaj jest to **platforma chmurowa (cloud platform)**, która odbiera, przechowuje i przetwarza ogromne ilości danych napływających z urządzeń IoT. To tutaj odbywa się analiza danych, uczenie maszynowe i podejmowanie decyzji.
*   **Zadanie:** Analiza danych, wyciąganie wniosków, zarządzanie urządzeniami i wysyłanie poleceń do aktuatorów.

**4. Warstwa aplikacji / interfejsu (Application / Interface Layer):**

*   **Komponenty:** To warstwa, z którą **bezpośrednio interaguje użytkownik**. Może to być aplikacja mobilna, panel sterowania (dashboard) w przeglądarce internetowej lub interfejs API, który pozwala innym systemom na korzystanie z danych i funkcjonalności systemu IoT.
*   **Zadanie:** Prezentacja danych użytkownikowi i umożliwienie mu zarządzania systemem (np. zdalne włączenie ogrzewania w domu za pomocą smartfona).

#### Zastosowania IoT

Internet Rzeczy rewolucjonizuje wiele dziedzin życia i gospodarki:

*   **Inteligentny dom (Smart Home):** Urządzenia takie jak inteligentne termostaty (np. Nest), oświetlenie (np. Philips Hue), zamki, głośniki (np. Amazon Echo) i sprzęt AGD, które można zdalnie kontrolować i które mogą automatyzować swoje działanie (np. automatyczne wyłączanie świateł po wyjściu z domu).
*   **Urządzenia noszone (Wearables):** Inteligentne zegarki (smartwatche), opaski fitness i monitory zdrowia, które śledzą aktywność fizyczną, tętno, sen i inne parametry życiowe.
*   **Inteligentne miasto (Smart City):** Zastosowania mające na celu poprawę jakości życia mieszkańców i efektywności zarządzania miastem, np. inteligentne systemy zarządzania ruchem, inteligentne oświetlenie uliczne, które dostosowuje się do natężenia ruchu, systemy monitorowania jakości powietrza czy inteligentne zarządzanie odpadami.
*   **Przemysłowy Internet Rzeczy (Industrial IoT - IIoT):** Wykorzystanie czujników w fabrykach i maszynach do monitorowania ich stanu, przewidywania awarii (konserwacja predykcyjna), optymalizacji procesów produkcyjnych i zarządzania łańcuchem dostaw.
*   **Inteligentne rolnictwo (Smart Agriculture):** Czujniki wilgotności gleby, drony monitorujące stan upraw i automatyczne systemy nawadniania, które pomagają optymalizować zużycie wody i nawozów oraz zwiększać plony.
*   **Połączone samochody (Connected Cars):** Pojazdy wyposażone w dostęp do internetu, które mogą komunikować się z innymi pojazdami i infrastrukturą drogową, dostarczać informacji o ruchu w czasie rzeczywistym i oferować zaawansowane usługi dla kierowcy.

#### Wyzwania i zagrożenia

Rozwój IoT wiąże się również z poważnymi wyzwaniami, przede wszystkim w obszarze bezpieczeństwa i prywatności:

*   **Bezpieczeństwo:** Wiele tanich urządzeń IoT ma bardzo słabe lub nieistniejące zabezpieczenia, co czyni je łatwym celem dla hakerów. Przejęte urządzenia mogą być wykorzystane do tworzenia ogromnych **botnetów** (np. botnet Mirai, który sparaliżował część internetu w 2016 roku) lub do ataków na prywatność użytkowników (np. przejęcie kontroli nad kamerą w domu).
*   **Prywatność:** Urządzenia IoT zbierają ogromne ilości danych o naszych nawykach, zachowaniach, a nawet stanie zdrowia. Istnieje ryzyko, że dane te mogą być wykorzystywane w niepożądany sposób, sprzedawane stronom trzecim lub skradzione.
*   **Interoperacyjność:** Brak jednolitych standardów komunikacji między urządzeniami różnych producentów utrudnia tworzenie zintegrowanych systemów.

#### Podsumowanie

*   **Internet Rzeczy (IoT)** to sieć połączonych z internetem fizycznych obiektów, które zbierają i wymieniają dane.
*   Architektura IoT składa się z czterech warstw: **urządzeń, sieci, przetwarzania i aplikacji**.
*   IoT znajduje zastosowanie w wielu obszarach, od **inteligentnych domów** i **miast**, przez **przemysł**, po **rolnictwo**.
*   Największymi wyzwaniami dla dalszego rozwoju IoT są **bezpieczeństwo** (ochrona urządzeń przed atakami) i **prywatność** (ochrona danych zbieranych o użytkownikach).

**Typowe pytania egzaminacyjne:**
*   Co to jest Internet Rzeczy (IoT)?
*   Proszę opisać cztery główne warstwy typowej architektury IoT.
*   Podaj i opisz co najmniej trzy przykłady zastosowania IoT.
*   Jakie są największe zagrożenia związane z bezpieczeństwem urządzeń IoT?
*   Na czym polega koncepcja inteligentnego miasta (Smart City)?

# Odpowiedzi na pytania do obrony pracy inżynierskiej - Sieci Komputerowe

## 41. Usługi i protokoły warstwy aplikacji na przykładzie protokołu HTTP.

### Szczegółowe wyjaśnienie

**Warstwa aplikacji w modelu OSI/ISO**

Warstwa aplikacji to **najwyższa, siódma warstwa** w modelu odniesienia OSI (oraz w uproszczonym modelu TCP/IP). Jest to warstwa, która znajduje się "najbliżej" użytkownika i z którą bezpośrednio interagują aplikacje, takie jak przeglądarki internetowe, klienty poczty e-mail czy komunikatory. Jej głównym zadaniem jest dostarczenie **interfejsu** między oprogramowaniem a siecią oraz zdefiniowanie **reguł (protokołów)** komunikacji dla konkretnych usług sieciowych.

Innymi słowy, warstwa aplikacji nie zajmuje się tym, *jak* dane są przesyłane przez kable (warstwa fizyczna) czy jak odnaleźć drogę w sieci (warstwa sieci), ale **co** te dane oznaczają i w jakim formacie mają być wymieniane, aby aplikacje po obu stronach mogły się wzajemnie zrozumieć.

**Usługi i protokoły warstwy aplikacji**

Każda usługa sieciowa ma swój dedykowany protokół w warstwie aplikacji. Do najważniejszych należą:

*   **WWW (World Wide Web):** Protokół **HTTP** (Hypertext Transfer Protocol) i jego szyfrowana wersja **HTTPS**.
*   **Poczta elektroniczna:** Protokoły **SMTP** (Simple Mail Transfer Protocol) do wysyłania poczty, oraz **POP3** (Post Office Protocol) i **IMAP** (Internet Message Access Protocol) do jej odbierania.
*   **System nazw domenowych:** Protokół **DNS** (Domain Name System), który tłumaczy zrozumiałe dla ludzi nazwy domen (np. `www.google.com`) na adresy IP zrozumiałe dla komputerów.
*   **Transfer plików:** Protokół **FTP** (File Transfer Protocol).
*   **Zdalny dostęp:** Protokoły **Telnet** i **SSH** (Secure Shell).

**Przykład: Protokół HTTP (Hypertext Transfer Protocol)**

HTTP jest fundamentem komunikacji w ramach usługi WWW. Jest to protokół tekstowy, działający w architekturze **klient-serwer**, oparty na modelu **żądanie-odpowiedź (request-response)**.

**Charakterystyka HTTP:**

1.  **Klient-Serwer:** Komunikacja jest zawsze inicjowana przez klienta (np. przeglądarkę internetową), który wysyła **żądanie (request)** do serwera (np. serwera WWW, na którym znajduje się strona). Serwer przetwarza żądanie i odsyła **odpowiedź (response)**.
2.  **Bezstanowość (Stateless):** Każde żądanie HTTP jest traktowane przez serwer jako niezależna transakcja. Serwer **nie przechowuje żadnych informacji** o poprzednich żądaniach od tego samego klienta. To upraszcza architekturę serwerów, ale stwarza problem utrzymania kontekstu sesji użytkownika (np. zalogowania, zawartości koszyka). Problem ten rozwiązuje się za pomocą mechanizmów takich jak **ciasteczka (cookies)**, które są dołączane do żądań i pozwalają serwerowi zidentyfikować klienta.
3.  **Tekstowy:** Wiadomości HTTP (zarówno żądania, jak i odpowiedzi) są w dużej mierze czytelne dla człowieka, co ułatwia debugowanie.

**Struktura wiadomości HTTP:**

*   **Żądanie (Request):**
    *   **Linia startowa:** Zawiera trzy elementy: **metodę HTTP**, **adres URL zasobu** oraz **wersję protokołu**.
        *   `GET /index.html HTTP/1.1`
    *   **Nagłówki (Headers):** Pary klucz-wartość, które dostarczają dodatkowych informacji o żądaniu, np. `Host: www.example.com`, `User-Agent: Chrome`, `Accept-Language: pl`.
    *   **Opcjonalne ciało (Body):** Zawiera dane wysyłane do serwera, używane głównie w metodach `POST` i `PUT` (np. dane z formularza).

*   **Odpowiedź (Response):**
    *   **Linia statusu:** Zawiera **wersję protokołu**, **kod statusu** oraz jego **opis słowny**.
        *   `HTTP/1.1 200 OK`
    *   **Nagłówki (Headers):** Informacje o odpowiedzi, np. `Content-Type: text/html`, `Content-Length: 1234`, `Date: ...`.
    *   **Ciało (Body):** Właściwa treść odpowiedzi, czyli zasób, o który prosił klient (np. kod HTML strony, obrazek, dane JSON).

**Najważniejsze metody HTTP:**

*   **`GET`:** Prośba o pobranie zasobu. Powinna być operacją bezpieczną (nie modyfikuje stanu serwera).
*   **`POST`:** Wysłanie danych do serwera w celu ich przetworzenia (np. wysłanie formularza, utworzenie nowego zasobu).
*   **`PUT`:** Wysłanie danych w celu zaktualizowania (nadpisania) istniejącego zasobu.
*   **`DELETE`:** Usunięcie zasobu.
*   **`HEAD`:** Działa jak `GET`, ale serwer w odpowiedzi zwraca tylko nagłówki, bez ciała. Służy do sprawdzania metadanych zasobu bez jego pobierania.

**Najważniejsze kody statusu HTTP:**

*   **`2xx` (Success):** Żądanie zakończyło się sukcesem (np. `200 OK`).
*   **`3xx` (Redirection):** Wymagane jest dalsze działanie, aby ukończyć żądanie (np. `301 Moved Permanently` – zasób został trwale przeniesiony pod inny adres).
*   **`4xx` (Client Error):** Wystąpił błąd po stronie klienta (np. `404 Not Found` – serwer nie znalazł żądanego zasobu, `403 Forbidden` – brak uprawnień).
*   **`5xx` (Server Error):** Wystąpił błąd po stronie serwera (np. `500 Internal Server Error` – ogólny błąd serwera, `503 Service Unavailable` – serwer jest tymczasowo niedostępny).

**Ewolucja HTTP:**

*   **HTTP/1.1:** Standard przez wiele lat. Pozwala na utrzymywanie jednego połączenia TCP do wysłania wielu żądań (keep-alive), ale żądania muszą być obsługiwane sekwencyjnie.
*   **HTTP/2:** Wprowadził **multipleksowanie**, czyli możliwość jednoczesnego wysyłania wielu żądań i odpowiedzi w ramach jednego połączenia TCP, co znacznie przyspieszyło ładowanie stron.
*   **HTTP/3:** Zmienia warstwę transportową z TCP na **QUIC** (oparty na UDP), co rozwiązuje niektóre problemy HTTP/2 i jeszcze bardziej poprawia wydajność, zwłaszcza w niestabilnych sieciach.


## 42. Usługi warstwy transportu na przykładzie protokołu TCP.

### Szczegółowe wyjaśnienie

**Warstwa transportu w modelu OSI/ISO**

Warstwa transportu to **czwarta warstwa** modelu OSI. Jej fundamentalnym zadaniem jest zapewnienie **logicznej komunikacji "od końca do końca" (end-to-end)** między **aplikacjami** działającymi na różnych hostach. Podczas gdy warstwa sieci (niższa) zajmuje się dostarczaniem pakietów między hostami, warstwa transportu zajmuje się dostarczaniem danych między konkretnymi **procesami (aplikacjami)** na tych hostach.

Wyobraźmy sobie, że warstwa sieci to globalny system pocztowy, który dostarcza listy pod właściwy adres (adres IP). Warstwa transportu to usługa wewnątrz tego budynku pocztowego, która kieruje list do konkretnego adresata w danym mieszkaniu (numer portu) i decyduje, czy ma to być list polecony z potwierdzeniem odbioru (TCP), czy zwykła, szybka pocztówka (UDP).

**Główne usługi warstwy transportu:**

1.  **Segmentacja danych i ponowne składanie:** Dzieli strumień danych z warstwy aplikacji na mniejsze fragmenty (segmenty) po stronie nadawcy i składa je z powrotem w całość po stronie odbiorcy.
2.  **Adresowanie procesów (multipleksowanie/demultipleksowanie):** Każdej aplikacji przypisuje unikalny numer identyfikacyjny, zwany **numerem portu**. Dzięki temu wiele aplikacji na jednym hoście może jednocześnie korzystać z sieci. Warstwa transportu u nadawcy dodaje do segmentu port źródłowy i docelowy, a u odbiorcy na tej podstawie przekazuje dane do właściwej aplikacji.
3.  **Zapewnienie niezawodności (opcjonalnie):** Gwarantuje, że dane dotrą do celu w całości, bez błędów i we właściwej kolejności.
4.  **Kontrola przepływu (opcjonalnie):** Zapobiega "zalaniu" odbiorcy przez nadawcę, który wysyła dane szybciej, niż odbiorca jest w stanie je przetworzyć.

Warstwa transportu oferuje dwa główne protokoły, które realizują te usługi w różny sposób: **TCP** i **UDP**.

**Przykład: Protokół TCP (Transmission Control Protocol)**

TCP jest **połączeniowym, niezawodnym** protokołem, który stanowi podstawę dla większości usług internetowych, gdzie integralność danych jest kluczowa (np. WWW, e-mail, transfer plików).

**Charakterystyka i mechanizmy TCP:**

1.  **Połączeniowość (Connection-oriented):** Zanim jakiekolwiek dane zostaną wysłane, TCP musi najpierw ustanowić połączenie między klientem a serwerem. Odbywa się to za pomocą procesu zwanego **trójstopniowym uzgadnianiem (Three-Way Handshake)**:
    1.  **SYN:** Klient wysyła segment z flagą `SYN` (synchronize) i losowym numerem sekwencyjnym.
    2.  **SYN-ACK:** Serwer odpowiada segmentem z flagami `SYN` i `ACK` (acknowledgement), potwierdzając otrzymanie `SYN` klienta i wysyłając swój własny numer sekwencyjny.
    3.  **ACK:** Klient odsyła segment z flagą `ACK`, potwierdzając otrzymanie `SYN` od serwera. Połączenie jest ustanowione.

2.  **Niezawodność (Reliability):** TCP gwarantuje, że dane dotrą do celu. Realizuje to za pomocą kilku mechanizmów:
    *   **Numery sekwencyjne (Sequence Numbers):** Każdy bajt danych ma przypisany numer sekwencyjny. Pozwala to odbiorcy na ułożenie segmentów we właściwej kolejności, nawet jeśli dotarły w innej.
    *   **Potwierdzenia (Acknowledgements - ACK):** Odbiorca po otrzymaniu segmentu odsyła potwierdzenie (ACK) z numerem sekwencyjnym następnego bajtu, którego się spodziewa. Jeśli nadawca nie otrzyma potwierdzenia w określonym czasie (timeout), uznaje, że segment zaginął i dokonuje **retransmisji**.
    *   **Sumy kontrolne (Checksums):** Każdy segment zawiera sumę kontrolną, która pozwala odbiorcy wykryć, czy dane nie zostały uszkodzone w trakcie transmisji. Uszkodzone segmenty są odrzucane (i retransmitowane po upływie timeoutu).

3.  **Kontrola przepływu (Flow Control):**
    *   TCP używa mechanizmu **okna przesuwnego (sliding window)**. Odbiorca w każdym potwierdzeniu informuje nadawcę, ile ma jeszcze wolnego miejsca w swoim buforze (tzw. rozmiar okna odbiorczego). Nadawca nie może wysłać więcej danych, niż wynosi aktualny rozmiar okna odbiorcy, co zapobiega jego przepełnieniu.

4.  **Kontrola zatorów (Congestion Control):**
    *   TCP aktywnie stara się unikać powodowania zatorów w sieci. Zaczyna transmisję powoli (mechanizm **Slow Start**), a następnie dynamicznie dostosowuje szybkość wysyłania danych (rozmiar okna zatorowego) w zależności od warunków w sieci (np. na podstawie utraconych pakietów, które są sygnałem zatoru).

**Porównanie TCP vs UDP**

| Cecha | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
|---|---|---|
| **Typ połączenia** | **Połączeniowy** (wymaga handshake) | **Bezpołączeniowy** |
| **Niezawodność** | **Wysoka** (gwarantuje dostarczenie, kolejność i brak błędów) | **Niska** (brak gwarancji) |
| **Szybkość** | Wolniejszy (narzut na mechanizmy niezawodności) | **Szybszy** (minimalny narzut) |
| **Kontrola przepływu** | Tak (okno przesuwne) | Nie |
| **Kontrola zatorów** | Tak | Nie |
| **Nagłówek** | Większy (min. 20 bajtów) | Mniejszy (8 bajtów) |
| **Zastosowania** | WWW (HTTP), e-mail (SMTP), transfer plików (FTP), bazy danych | Streaming wideo/audio, gry online, telefonia internetowa (VoIP), DNS |

Podsumowując, TCP jest jak niezawodny kurier, który dba o to, by każda część przesyłki dotarła do adresata w idealnym stanie i we właściwej kolejności. UDP to szybki goniec, który po prostu rzuca paczki w kierunku adresata – niektóre mogą nie dotrzeć, inne mogą być uszkodzone, ale całość odbywa się bardzo szybko. Wybór między nimi zależy od wymagań aplikacji – czy ważniejsza jest niezawodność, czy szybkość i minimalne opóźnienia.


## 43. Protokoły rutingu warstwy sieci na przykładzie protokołu OSPF.

### Szczegółowe wyjaśnienie

**Warstwa sieci i rola routingu**

Warstwa sieci to **trzecia warstwa** modelu OSI. Jej głównym zadaniem jest **logiczne adresowanie** hostów (za pomocą adresów IP) oraz **routing (trasowanie)**, czyli proces znajdowania najlepszej ścieżki dla pakietów danych od hosta źródłowego do hosta docelowego w dużej, złożonej sieci (takiej jak Internet).

Urządzeniami, które podejmują decyzje o trasowaniu, są **routery**. Każdy router utrzymuje **tablicę routingu** – swoistą mapę sieci, która mówi mu, dokąd wysłać pakiet przeznaczony pod dany adres. Tablica ta może być budowana statycznie (ręcznie przez administratora) lub dynamicznie – i tu właśnie wkraczają **protokoły routingu**.

**Protokoły routingu** to zestawy reguł i algorytmów, które pozwalają routerom na automatyczną wymianę informacji o znanych im sieciach, budowanie spójnego obrazu topologii sieci i dynamiczne aktualizowanie swoich tablic routingu w odpowiedzi na zmiany (np. awarię jakiegoś łącza).

**Kategorie protokołów routingu**

Protokoły routingu dzielą się na dwie główne rodziny, różniące się sposobem działania:

1.  **Protokoły wektora odległości (Distance Vector):**
    *   **Jak działają:** Każdy router zna tylko swoich bezpośrednich sąsiadów i "wierzy na słowo" informacjom, które od nich otrzymuje. Okresowo wysyła do sąsiadów całą swoją tablicę routingu. Na podstawie tych informacji, każdy router wie, do których sieci można dotrzeć przez danego sąsiada i jaki jest "koszt" (metryka, np. liczba skoków) dotarcia do nich.
    *   **Wady:** Wolna zbieżność (czas potrzebny na rozpropagowanie informacji o zmianie w całej sieci), podatność na pętle routingu, duże obciążenie sieci (okresowe wysyłanie całych tablic).
    *   **Przykład:** **RIP** (Routing Information Protocol).

2.  **Protokoły stanu łącza (Link-State):**
    *   **Jak działają:** Każdy router buduje **pełną, kompletną mapę całej topologii sieci**. Robi to, rozgłaszając informacje tylko o stanie swoich własnych połączeń (łączy) do wszystkich innych routerów w sieci. Dzięki temu każdy router ma identyczny obraz sieci i na jego podstawie, używając **algorytmu Dijkstry (algorytm najkrótszej ścieżki)**, samodzielnie oblicza najlepsze trasy do wszystkich miejsc docelowych.
    *   **Zalety:** Szybka zbieżność, mniejsza podatność na pętle, bardziej efektywna komunikacja (wysyłane są tylko małe aktualizacje w momencie zmiany, a nie całe tablice).
    *   **Przykład:** **OSPF** (Open Shortest Path First).

**Przykład: Protokół OSPF (Open Shortest Path First)**

OSPF jest jednym z najpopularniejszych **wewnętrznych protokołów bramy (IGP - Interior Gateway Protocol)**, co oznacza, że jest używany do routingu wewnątrz jednego **systemu autonomicznego (AS)**, czyli sieci pod pojedynczą administracją (np. sieć firmowa, sieć dostawcy internetu).

**Charakterystyka OSPF:**

*   **Protokół stanu łącza:** Działa zgodnie z opisanym wyżej modelem – każdy router ma pełną mapę sieci i samodzielnie oblicza najlepsze ścieżki.
*   **Metryka "kosztu":** OSPF jako metrykę wykorzystuje **koszt**, który jest odwrotnie proporcjonalny do **przepustowości łącza**. Oznacza to, że preferowane są szybsze połączenia (np. 1 Gb/s) nad wolniejszymi (np. 100 Mb/s), nawet jeśli te drugie wymagałyby mniejszej liczby skoków. Daje to bardziej realistyczną ocenę "najlepszej" ścieżki.
*   **Hierarchiczna budowa (obszary - Areas):** Aby zwiększyć skalowalność i wydajność w dużych sieciach, OSPF pozwala na podzielenie systemu autonomicznego na mniejsze **obszary (areas)**. Wszystkie obszary muszą być połączone z centralnym **obszarem zerowym (area 0)**, zwanym **obszarem szkieletowym (backbone area)**.
    *   Routery wewnątrz jednego obszaru wymieniają się szczegółowymi informacjami o topologii tylko w ramach tego obszaru.
    *   Komunikacja między obszarami odbywa się za pośrednictwem **routerów granicznych obszaru (ABR - Area Border Routers)**, które przekazują zagregowane, uproszczone informacje o trasach. Taki podział znacznie zmniejsza liczbę informacji, które muszą być przetwarzane przez każdy router, i ogranicza zasięg problemów (awaria w jednym obszarze nie powoduje przeliczania tras w innych).
*   **Szybka zbieżność:** Dzięki rozsyłaniu małych, wyzwalanych zmianami aktualizacji (LSA - Link-State Advertisements) zamiast całych tablic, OSPF bardzo szybko reaguje na zmiany w topologii sieci.
*   **Bezklasowość:** OSPF jest protokołem bezklasowym, co oznacza, że w informacjach o trasach przesyła również maskę podsieci, co pozwala na efektywne wykorzystanie przestrzeni adresowej (VLSM - Variable Length Subnet Masking).

**Działanie OSPF w skrócie:**

1.  **Nawiązywanie sąsiedztwa:** Routery wysyłają pakiety "Hello" na swoich interfejsach, aby odkryć sąsiadów i nawiązać z nimi relację.
2.  **Wymiana baz danych:** Sąsiadujące routery wymieniają się swoimi bazami danych stanu łącza (LSDB), aby zsynchronizować swój obraz sieci.
3.  **Rozgłaszanie LSA:** Gdy router wykryje zmianę (np. awarię łącza, zmianę kosztu), generuje ogłoszenie o stanie łącza (LSA) i rozgłasza je do wszystkich innych routerów w swoim obszarze.
4.  **Uruchomienie algorytmu SPF:** Po otrzymaniu nowego LSA, każdy router aktualizuje swoją mapę topologii i ponownie uruchamia algorytm SPF (Dijkstry), aby obliczyć nowe, najlepsze ścieżki.
5.  **Aktualizacja tablicy routingu:** Na podstawie wyników algorytmu SPF, router aktualizuje swoją tablicę routingu.


## 44. Usługi warstwy łącza na przykładzie protokołu Ethernet lub protokołów z rodziny 802.11 (WiFi).

### Szczegółowe wyjaśnienie

**Warstwa łącza danych w modelu OSI/ISO**

Warstwa łącza danych to **druga warstwa** modelu OSI. Jej głównym zadaniem jest zapewnienie **niezawodnej transmisji danych w ramach jednego segmentu sieci lokalnej (LAN)**, czyli między urządzeniami podłączonymi do tego samego medium transmisyjnego (np. tego samego kabla, przełącznika, punktu dostępowego Wi-Fi).

Podczas gdy warstwa sieci zajmuje się globalnym adresowaniem i znajdowaniem drogi w całym Internecie, warstwa łącza danych skupia się na "ostatniej mili" – dostarczeniu danych do następnego urządzenia w sieci.

**Główne usługi warstwy łącza danych:**

1.  **Ramkowanie (Framing):** Odbiera pakiety z warstwy sieci i "opakowuje" je w jednostki zwane **ramkami (frames)**. Ramka posiada nagłówek i stopkę, które zawierają informacje sterujące.
2.  **Adresowanie fizyczne:** Używa **adresów fizycznych (MAC - Media Access Control)**, które są unikalnymi, 48-bitowymi identyfikatorami przypisanymi na stałe do każdej karty sieciowej na świecie. Adres MAC pozwala na jednoznaczne zidentyfikowanie konkretnego urządzenia w sieci lokalnej.
3.  **Kontrola dostępu do medium (Media Access Control - MAC):** W sieciach, gdzie wiele urządzeń dzieli to samo medium transmisyjne (np. wczesne wersje Ethernetu oparte na koncentratorach, sieci Wi-Fi), ta podwarstwa decyduje, które urządzenie i kiedy może nadawać, aby uniknąć **kolizji** (jednoczesnego nadawania przez kilka urządzeń).
4.  **Wykrywanie błędów:** Do stopki ramki dodawana jest **sekwencja sprawdzająca ramkę (FCS - Frame Check Sequence)**, najczęściej w postaci sumy kontrolnej CRC. Pozwala to odbiorcy zweryfikować, czy ramka nie została uszkodzona w trakcie transmisji. Uszkodzone ramki są odrzucane.

**Przykład 1: Protokół Ethernet**

Ethernet jest absolutnym standardem w **przewodowych sieciach lokalnych (LAN)**.

*   **Adresowanie:** Każda ramka Ethernet zawiera **docelowy adres MAC** i **źródłowy adres MAC**. Przełączniki (switche) sieciowe uczą się, które adresy MAC są dostępne na których ich portach i na tej podstawie inteligentnie przesyłają ramki tylko do właściwego portu docelowego (w przeciwieństwie do starych koncentratorów, które rozsyłały ramki na wszystkie porty).
*   **Format ramki:** Standardowa ramka Ethernet II zawiera m.in. adresy MAC, pole `EtherType` (identyfikujące protokół warstwy wyższej, np. IP) oraz dane (pakiet z warstwy sieci).
*   **Kontrola dostępu do medium:** We wczesnych, współdzielonych wersjach Ethernetu stosowano metodę **CSMA/CD (Carrier Sense Multiple Access with Collision Detection)**:
    1.  **Nasłuchuj medium (Carrier Sense):** Zanim zaczniesz nadawać, sprawdź, czy nikt inny nie nadaje.
    2.  **Jeśli wolne, nadawaj (Multiple Access):** Jeśli medium jest wolne, zacznij wysyłać ramkę.
    3.  **Wykrywaj kolizje (Collision Detection):** W trakcie nadawania cały czas nasłuchuj. Jeśli wykryjesz, że ktoś inny też zaczął nadawać (kolizja), natychmiast przestań, wyślij sygnał zagłuszający, odczekaj losowy czas i spróbuj ponownie od kroku 1.
    W nowoczesnych sieciach Ethernet opartych na przełącznikach, gdzie każde urządzenie ma dedykowane połączenie z przełącznikiem (full-duplex), problem kolizji praktycznie nie występuje i mechanizm CSMA/CD nie jest potrzebny.

**Przykład 2: Protokoły z rodziny 802.11 (Wi-Fi)**

802.11 to standard dla **bezprzewodowych sieci lokalnych (WLAN)**.

*   **Adresowanie:** Działa podobnie do Ethernetu, używając adresów MAC do identyfikacji urządzeń i punktów dostępowych (AP).
*   **Kontrola dostępu do medium:** W sieciach bezprzewodowych problem kolizji jest bardziej skomplikowany, ponieważ urządzenie nadające nie jest w stanie jednocześnie odbierać i nasłuchiwać kolizji (problem "ukrytej stacji"). Dlatego Wi-Fi używa innej metody: **CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)** – **unikanie kolizji**, a nie ich wykrywanie.
    1.  **Nasłuchuj medium (Carrier Sense):** Sprawdź, czy medium jest wolne.
    2.  **Jeśli wolne, odczekaj i zarezerwuj (Collision Avoidance):** Jeśli medium jest wolne, odczekaj jeszcze krótki, losowy czas. Następnie, opcjonalnie, wyślij krótką ramkę **RTS (Request to Send)** do punktu dostępowego, rezerwując medium na określony czas. Punkt dostępowy odpowiada ramką **CTS (Clear to Send)**, którą słyszą wszystkie inne stacje w zasięgu, informując je, aby nie nadawały przez ten czas.
    3.  **Nadawaj i czekaj na potwierdzenie:** Po otrzymaniu CTS (lub jeśli mechanizm RTS/CTS nie jest używany), stacja wysyła ramkę danych, a następnie oczekuje na **potwierdzenie (ACK)** od odbiorcy. Jeśli nie otrzyma ACK, uznaje, że doszło do kolizji lub błędu i próbuje retransmitować ramkę.

**Porównanie Ethernet vs Wi-Fi (w warstwie 2)**

| Cecha | Ethernet | Wi-Fi (802.11) |
|---|---|---|
| **Medium** | Przewodowe (skrętka miedziana, światłowód) | Bezprzewodowe (fale radiowe) |
| **Niezawodność medium** | Wysoka, mała podatność na zakłócenia | Niska, duża podatność na zakłócenia, tłumienie sygnału |
| **Kontrola dostępu** | CSMA/CD (w starych wersjach), obecnie niepotrzebna | **CSMA/CA** (unikanie kolizji) |
| **Potwierdzenia** | Brak potwierdzeń na poziomie warstwy 2 | **Wymagane potwierdzenia (ACK)** dla każdej ramki |
| **Bezpieczeństwo** | Fizyczne bezpieczeństwo medium | Wymaga silnych mechanizmów szyfrowania (WPA2/WPA3) |

## 45. Metody ochrony informacji stosowane w bankowości Internetowej.

### Szczegółowe wyjaśnienie

Bankowość internetowa jest celem numer jeden dla cyberprzestępców, dlatego stosuje się w niej wielowarstwowy, dogłębny model zabezpieczeń (defense in depth), który ma na celu ochronę informacji na każdym etapie – od uwierzytelnienia użytkownika, przez transmisję danych, aż po ich przetwarzanie i przechowywanie w systemach banku. Kluczowe metody ochrony to:

**1. Bezpieczne uwierzytelnianie użytkownika**

Celem jest pewne zweryfikowanie, że osoba logująca się do systemu jest faktycznie tym, za kogo się podaje.

*   **Wieloskładnikowe uwierzytelnianie (MFA - Multi-Factor Authentication):** To absolutny standard. Wymaga od użytkownika podania co najmniej dwóch z trzech rodzajów "dowodów" tożsamości:
    1.  **Coś, co wiesz:** Hasło, PIN.
    2.  **Coś, co masz:** Telefon komórkowy (do otrzymania kodu SMS lub potwierdzenia w aplikacji mobilnej), token sprzętowy.
    3.  **Coś, czym jesteś:** Dane biometryczne (odcisk palca, skan twarzy).
*   **Silna autoryzacja klienta (SCA - Strong Customer Authentication):** Wymóg prawny w Unii Europejskiej (dyrektywa PSD2), który nakazuje stosowanie MFA dla większości operacji bankowych online.
*   **Polityka silnych haseł:** Wymuszanie na użytkownikach tworzenia długich, skomplikowanych haseł i regularnej ich zmiany.
*   **Maskowanie hasła:** Podczas logowania system prosi o podanie tylko wybranych, losowych znaków z hasła, co utrudnia jego przechwycenie przez keyloggery.

**2. Szyfrowanie komunikacji**

Celem jest zapewnienie poufności i integralności danych przesyłanych między przeglądarką klienta a serwerem banku.

*   **Protokół TLS (Transport Layer Security):** Jest to następca SSL. Cała komunikacja z serwisem bankowości internetowej odbywa się za pośrednictwem szyfrowanego protokołu **HTTPS** (HTTP over TLS). TLS zapewnia trzy rzeczy:
    1.  **Szyfrowanie:** Dane są szyfrowane za pomocą klucza symetrycznego, unikalnego dla danej sesji, co uniemożliwia ich odczytanie przez osoby postronne (ochrona przed podsłuchem).
    2.  **Integralność:** Każda wiadomość jest opatrzona kodem uwierzytelniającym (MAC), który pozwala wykryć, czy nie została ona zmodyfikowana w trakcie przesyłania.
    3.  **Uwierzytelnienie serwera:** Przeglądarka, używając **certyfikatu cyfrowego serwera (certyfikat EV - Extended Validation)**, weryfikuje, że łączy się z autentycznym serwerem banku, a nie z fałszywą stroną phishingową. Certyfikat EV powoduje wyświetlenie nazwy banku na zielonym pasku adresu w przeglądarce.

**3. Ochrona po stronie serwera i aplikacji**

Celem jest zabezpieczenie systemów banku przed atakami z zewnątrz i wewnętrznymi.

*   **Firewalle (zapory sieciowe) i systemy wykrywania/zapobiegania włamaniom (IDS/IPS):** Filtrują ruch sieciowy i blokują próby nieautoryzowanego dostępu oraz znane wzorce ataków.
*   **Web Application Firewall (WAF):** Specjalizowana zapora, która chroni samą aplikację webową przed atakami takimi jak **SQL Injection** (wstrzykiwanie złośliwego kodu SQL) i **Cross-Site Scripting (XSS)** (wstrzykiwanie złośliwych skryptów do strony).
*   **Regularne audyty bezpieczeństwa i testy penetracyjne:** Banki zlecają zewnętrznym firmom etyczne ataki na swoje systemy w celu znalezienia i załatania luk w zabezpieczeniach.
*   **Szyfrowanie danych w spoczynku (Data at Rest):** Wrażliwe dane klientów (np. numery PESEL, hasła) są przechowywane w bazach danych w postaci zaszyfrowanej.

**4. Mechanizmy monitorowania i prewencji transakcyjnej**

Celem jest wykrywanie i blokowanie podejrzanych lub oszukańczych transakcji w czasie rzeczywistym.

*   **Limity transakcyjne:** Użytkownik może zdefiniować maksymalne kwoty dla pojedynczych przelewów i limity dzienne/miesięczne.
*   **Analiza behawioralna:** Systemy bankowe uczą się typowych zachowań klienta (np. pory logowania, typowe kwoty i odbiorcy przelewów). Każde odstępstwo od tego wzorca (np. logowanie z egzotycznego kraju, próba wykonania bardzo wysokiego przelewu do nowego odbiorcy) jest flagowane jako podejrzane i może wymagać dodatkowej weryfikacji.
*   **Powiadomienia i alerty:** Użytkownik otrzymuje natychmiastowe powiadomienia (SMS, push) o każdej operacji na jego koncie, co pozwala na szybką reakcję w przypadku oszustwa.

**5. Edukacja i świadomość użytkownika**

Najsłabszym ogniwem w łańcuchu bezpieczeństwa jest często sam człowiek. Dlatego banki prowadzą szeroko zakrojone akcje edukacyjne, uczulając klientów na:

*   **Phishing:** Nieklikanie w podejrzane linki w e-mailach i SMS-ach, które podszywają się pod bank.
*   **Ochronę danych logowania:** Nieudostępnianie nikomu haseł i kodów jednorazowych.
*   **Zasady bezpiecznego korzystania z komputera:** Używanie legalnego oprogramowania, antywirusa i regularne aktualizacje.


---

# Odpowiedzi "to the point" na obronę

## 41. Usługi i protokoły warstwy aplikacji na przykładzie protokołu HTTP.

Warstwa aplikacji to najwyższa warstwa modelu OSI, która dostarcza aplikacjom interfejs do sieci. Definiuje protokoły dla konkretnych usług, np. SMTP dla poczty, DNS dla nazw domen. Kluczowym przykładem jest **HTTP** – protokół usługi WWW. Działa on w modelu klient-serwer, jest bezstanowy i opiera się na żądaniach (np. `GET`, `POST`) i odpowiedziach z kodami statusu (np. `200 OK`, `404 Not Found`).

## 42. Usługi warstwy transportu na przykładzie protokołu TCP.

Warstwa transportu zapewnia komunikację "od końca do końca" między aplikacjami, używając **numerów portów**. Jej głównym protokołem jest **TCP (Transmission Control Protocol)**. Jest to protokół **połączeniowy i niezawodny**. Gwarantuje dostarczenie danych w całości i we właściwej kolejności dzięki mechanizmom takim jak **trójstopniowe uzgadnianie (handshake)**, **potwierdzenia (ACK)** i **retransmisje**. Stosuje się go tam, gdzie kluczowa jest integralność danych, np. w HTTP i SMTP.

## 43. Protokoły rutingu warstwy sieci na przykładzie protokołu OSPF.

Warstwa sieci odpowiada za routing, czyli wyznaczanie najlepszych ścieżek w sieci. Służą do tego protokoły routingu, które dynamicznie budują tablice routingu w routerach. Dzielą się na protokoły **wektora odległości** (jak RIP) i **stanu łącza**. Przykładem tych drugich jest **OSPF (Open Shortest Path First)**. W OSPF każdy router buduje pełną mapę sieci i na jej podstawie, używając algorytmu Dijkstry, oblicza najkrótsze ścieżki. Jako metrykę wykorzystuje koszt, zależny od przepustowości łącza.

## 44. Usługi warstwy łącza na przykładzie protokołu Ethernet lub protokołów z rodziny 802.11 (WiFi).

Warstwa łącza danych odpowiada za transmisję w sieci lokalnej (LAN) między urządzeniami w tym samym segmencie. Używa do tego **fizycznych adresów MAC**. W sieciach przewodowych standardem jest **Ethernet**, który w starych wersjach używał metody dostępu do medium **CSMA/CD** (wykrywanie kolizji). W sieciach bezprzewodowych **Wi-Fi (802.11)**, ze względu na specyfikę medium, stosuje się metodę **CSMA/CA** (unikanie kolizji) oraz mechanizm potwierdzeń (ACK) dla każdej ramki.

## 45. Metody ochrony informacji stosowane w bankowości Internetowej.

Bezpieczeństwo bankowości internetowej opiera się na modelu wielowarstwowym. Kluczowe metody to:
1.  **Silne uwierzytelnianie klienta (SCA)**, czyli **uwierzytelnianie wieloskładnikowe (MFA)**, wymagające np. hasła i kodu z telefonu.
2.  **Szyfrowanie całej komunikacji** za pomocą protokołu **HTTPS (TLS)**, co zapewnia poufność, integralność i uwierzytelnienie serwera.
3.  **Zabezpieczenia po stronie serwera**, takie jak WAF (Web Application Firewall) chroniący przed atakami SQL Injection i XSS.
4.  **Monitorowanie transakcji** i analiza behawioralna w celu wykrywania oszustw.

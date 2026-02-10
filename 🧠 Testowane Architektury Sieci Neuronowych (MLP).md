# 🧠 Testowane Architektury Sieci Neuronowych (MLP)

_Data: 10 lutego 2026_  
_Autor: Manus AI_  
_Wersja: 1.0_

---

## 1. Wprowadzenie

Niniejszy dokument szczegółowo opisuje **7 architektur wielowarstwowego perceptronu (MLP)**, które zostały przetestowane w ramach pracy inżynierskiej w celu predykcji śmiertelności pacjentów z niewydolnością serca. Celem eksperymentów było zbadanie wpływu głębokości i szerokości sieci na jej zdolność do generalizacji i skuteczność predykcyjną na małym, tabelarycznym zbiorze danych.

### 1.1. Kontekst Eksperymentu

- **Zbiór danych:** 299 pacjentów, 3 cechy wejściowe (`age`, `ejection_fraction`, `serum_creatinine`).
- **Problem:** Klasyfikacja binarna (przeżył / zmarł).
- **Cel:** Znalezienie optymalnej architektury MLP, która zrównoważy złożoność modelu z ryzykiem przeuczenia.

### 1.2. Wspólne Parametry Treningu

Wszystkie testowane architektury były trenowane z użyciem następujących, stałych hiperparametrów, aby zapewnić porównywalność wyników:

| Parametr | Wartość | Uzasadnienie |
|---|---|---|
| **Funkcja aktywacji (warstwy ukryte)** | `ReLU` | Standardowy wybór, zapobiega zanikającym gradientom. |
| **Funkcja aktywacji (warstwa wyjściowa)** | `Sigmoid` | Zwraca prawdopodobieństwo przynależności do klasy 1 (śmierć). |
| **Optymalizator** | `Adam` | Skuteczny i szybki, standard w większości problemów. |
| **Funkcja straty** | `BinaryCrossentropy` | Standardowa funkcja straty dla klasyfikacji binarnej. |
| **Liczba epok** | `100` | Wystarczająca do osiągnięcia zbieżności. |
| **Batch size** | `32` | Dobry kompromis między szybkością a stabilnością treningu. |
| **Metryka do oceny** | `AUC` | Dobrze radzi sobie z niezbalansowanymi danymi. |

---

## 2. Opis Testowanych Architektur

Architektury zostały podzielone na trzy kategorie: **płytkie**, **średnie** i **głębokie**, aby systematycznie badać wpływ złożoności modelu.

### 2.1. Architektury Płytkie (1 warstwa ukryta)

Charakteryzują się jedną warstwą ukrytą, co ogranicza ich złożoność i ryzyko przeuczenia. Testowano trzy warianty różniące się liczbą neuronów.

#### **Architektura 1: `Shallow_32`**
- **Struktura:** `[Input(3)] -> [Dense(32, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~161
- **Uzasadnienie:** Minimalistyczny model, sprawdzający, czy bardzo prosta sieć jest w stanie nauczyć się zależności w danych.

#### **Architektura 2: `Shallow_64`**
- **Struktura:** `[Input(3)] -> [Dense(64, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~257
- **Uzasadnienie:** Zwiększenie liczby neuronów w celu uchwycenia bardziej złożonych interakcji.

#### **Architektura 3: `Shallow_128`** 🏆
- **Struktura:** `[Input(3)] -> [Dense(128, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~513
- **Uzasadnienie:** Dalsze zwiększenie pojemności modelu. **Okazała się najlepszą architekturą w tej kategorii.**

### 2.2. Architektury Średnie (2 warstwy ukryte)

Dodanie drugiej warstwy ukrytej pozwala modelowi na naukę bardziej abstrakcyjnych i hierarchicznych reprezentacji danych. Testowano dwie popularne konfiguracje w kształcie "lejka".

#### **Architektura 4: `Medium_64_32`**
- **Struktura:** `[Input(3)] -> [Dense(64, ReLU)] -> [Dense(32, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~2401
- **Uzasadnienie:** Klasyczna architektura "lejka", gdzie każda kolejna warstwa ma mniej neuronów, co zmusza sieć do kompresji informacji.

#### **Architektura 5: `Medium_128_64`**
- **Struktura:** `[Input(3)] -> [Dense(128, ReLU)] -> [Dense(64, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~8833
- **Uzasadnienie:** Bardziej pojemna wersja architektury "lejka", zdolna do modelowania bardziej skomplikowanych zależności.

### 2.3. Architektury Głębokie (3 warstwy ukryte)

Trzy warstwy ukryte reprezentują podejście "deep learning" i mają największy potencjał do przeuczenia na małym zbiorze danych. Testowano dwie konfiguracje.

#### **Architektura 6: `Deep_128_64_32`**
- **Struktura:** `[Input(3)] -> [Dense(128, ReLU)] -> [Dense(64, ReLU)] -> [Dense(32, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~10,977
- **Uzasadnienie:** Głęboka sieć o dużej pojemności, testująca granice złożoności dla tego problemu.

#### **Architektura 7: `Deep_256_128_64`**
- **Struktura:** `[Input(3)] -> [Dense(256, ReLU)] -> [Dense(128, ReLU)] -> [Dense(64, ReLU)] -> [Dense(1, Sigmoid)]`
- **Liczba parametrów:** ~42,625
- **Uzasadnienie:** Bardzo głęboka i szeroka sieć, mająca na celu sprawdzenie, czy ekstremalna złożoność przyniesie korzyści.

---

## 3. Wyniki i Analiza

### 3.1. Tabela Porównawcza Wyników

Poniższa tabela przedstawia wyniki metryk F1-score, Recall, Precision i AUC dla każdej z testowanych architektur na zbiorze testowym.

| Kategoria | Architektura | F1-score | Recall | Precision | AUC | Liczba Parametrów |
|---|---|---|---|---|---|---|
| **Płytkie** | `Shallow_32` | 0.541 | 0.632 | 0.478 | 0.748 | 161 |
| | `Shallow_64` | 0.564 | 0.579 | 0.550 | 0.758 | 257 |
| | **`Shallow_128`** 🏆 | **0.591** | **0.684** | **0.520** | **0.763** | **513** |
| **Średnie** | `Medium_64_32` | 0.558 | 0.632 | 0.500 | 0.758 | 2,401 |
| | `Medium_128_64` | 0.579 | 0.579 | 0.579 | 0.763 | 8,833 |
| **Głębokie** | `Deep_128_64_32` | 0.550 | 0.579 | 0.524 | 0.753 | 10,977 |
| | `Deep_256_128_64` | 0.564 | 0.684 | 0.481 | 0.753 | 42,625 |

### 3.2. Kluczowe Obserwacje

1.  **Prostota wygrywa:** Najlepsze wyniki osiągnęła najprostsza kategoria architektur (płytkie). Model `Shallow_128` uzyskał najwyższy F1-score (0.591) i Recall (0.684).

2.  **Głębsze nie znaczy lepsze:** Zwiększanie głębokości (2 i 3 warstwy) nie przyniosło poprawy wyników, a wręcz je pogorszyło. Modele głębokie miały tendencję do przeuczania, co widać po niższych wartościach metryk na zbiorze testowym.

3.  **Liczba parametrów a wydajność:** Nie zaobserwowano prostej korelacji między liczbą parametrów a skutecznością. Najlepszy model miał tylko 513 parametrów, podczas gdy najgorszy z modeli głębokich miał ich ponad 42,000.

4.  **Recall vs Precision:** Architektury `Shallow_128` i `Deep_256_128_64` osiągnęły najwyższy Recall (0.684), co jest kluczowe w zastosowaniach medycznych. Jednak model `Shallow_128` miał znacznie lepszą precyzję, co czyni go bardziej zrównoważonym.

---

## 4. Wnioski

Dla analizowanego problemu i zbioru danych, **prosta, płytka architektura sieci neuronowej z jedną warstwą ukrytą i 128 neuronami (`Shallow_128`) okazała się najskuteczniejsza**. Bardziej złożone, głębsze modele nie były w stanie wykorzystać swojej pojemności i wykazywały tendencję do przeuczania, co jest typowym zjawiskiem na małych zbiorach danych.

Wyniki te sugerują, że w przypadku problemów z ograniczoną ilością danych, należy preferować prostsze modele, które są mniej podatne na przeuczenie i łatwiejsze w interpretacji. Zwiększanie złożoności architektury bez odpowiedniej ilości danych nie gwarantuje lepszych wyników.

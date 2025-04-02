# zaawansowane_metody_uczenia_maszynowego
# Laboratorium 1
## Opis projektu
Projekt składa się z kilku zadań związanych z analizą i manipulacją danymi za pomocą popularnych bibliotek NumPy oraz Pandas. Zadania obejmują operacje na tablicach NumPy, manipulację danymi w formacie DataFrame, generowanie wykresów za pomocą Matplotlib, a także wyciąganie wniosków z analiz statystycznych, takich jak macierz korelacji.

## Zadanie 1
### Opis
W tym zadaniu wczytujemy dane z pliku Excel przy użyciu biblioteki Pandas i przekształcamy je na tablicę NumPy. Następnie wykonujemy szereg operacji analitycznych, takich jak:
1. Obliczanie różnicy między tablicą zawierającą parzyste wiersze a tablicą z nieparzystymi wierszami.
2. Normalizacja danych poprzez odjęcie średniej i podzielenie przez odchylenie standardowe.
3. Obliczanie współczynnika zmienności i identyfikowanie kolumn o największym współczynniku zmienności.
4. Liczenie elementów większych od średniej w każdej kolumnie.
5. Znajdowanie kolumn z największymi wartościami oraz z największą liczbą elementów równych zero.
6. Porównanie sum elementów w wierszach o numerach parzystych i nieparzystych.
### Użyte biblioteki: 
1. Pandas
2. NumPy

## Zadanie 2
### Opis
To zadanie obejmuje kilka podstawowych operacji na tablicach NumPy:
1. Utworzenie tablicy jednowymiarowej zawierającej liczby od 1 do 20.
2. Slicing – wyodrębnienie elementów w zakresie od 5 do 15.
3. Utworzenie dwuwymiarowej tablicy (5x5) z losowymi liczbami całkowitymi z zakresu 0–50.
4. Obliczenie średniej, sumy i mediany dla tej tablicy.
5. Wykonanie operacji mnożenia elementów dwóch tablic.
### Użyte biblioteki:
1. NumPy

## Zadanie 3
### Opis
W tym zadaniu tworzymy obrazy w postaci dwuwymiarowych tablic NumPy:
1. Utworzenie "obrazu" (tablica 150x150) wypełnionego zerami i ustawienie centralnego regionu na wartość 255 (biały kwadrat).
2. Utworzenie gradientu, w którym wartości pikseli rosną liniowo od 0 do 255 w każdym wierszu.
3. Obliczenie średnich wartości pikseli dla obu obrazów (biały kwadrat i gradient).
### Użyte biblioteki:
1. NumPy
2. Matplotlib

## Zadanie 4
### Opis
W tym zadaniu tworzymy i manipulujemy DataFrame w bibliotece Pandas:
1. Utworzenie DataFrame z danymi o studentach, ocenach i grupach.
2. Sortowanie DataFrame według ocen malejąco.
3. Wyodrębnienie studentów z grupy "A".
4. Dodanie nowej kolumny "Status", która zależy od oceny studenta.
### Użyte biblioteki:
Pandas

## Zadanie 5
### Opis
Zadanie to polega na generowaniu wykresów matematycznych:
1. Generowanie wykresów funkcji na przedziale [-10, 10] z krokiem 0.03.
2. Rysowanie wykresów ciągłych dla różnych funkcji, takich jak funkcje trygonometryczne, wykładnicze, itp.
### Użyte biblioteki:
1. Matplotlib
2. NumPy

## Zadanie 6
### Opis
W tym zadaniu badamy korelację między danymi:
1. Wczytanie danych z pliku do DataFrame.
2. Obliczenie macierzy korelacji przy użyciu metody .corr().
3. Wizualizacja macierzy korelacji za pomocą wykresów punktowych (scatter plot) przy użyciu Matplotlib.
4. Analiza, jak wyglądają wykresy dla skorelowanych i nieskorelowanych danych oraz wnioskowanie o znaku współczynnika korelacji.
### Użyte biblioteki:
1. Pandas
2. Matplotlib
3. NumPy


# Laboratorium 2
## Opis projektu
Laboratorium 2 skupia się na analizie danych, wykrywaniu brakujących wartości oraz identyfikowaniu wartości odstających w danych. W ramach tego laboratorium zostaną wykonane operacje na plikach CSV, w tym m.in. importowanie danych, analiza brakujących danych, testowanie normalności, wizualizacja danych oraz transformacja danych.

## Zadanie 1
### Opis
W tym zadaniu pracujemy na pliku landtempssample.csv. Należy:
1. Wczytać dane z pliku, ustalając nazwy nagłówków, takie jak: 'ID_stacji', 'rok', 'miesiąc', 'srednia_temperatura', 'szerokosc_geograficzna', 'dlugosc_geograficzna', 'wysokosc', 'stacja', 'ID_panstwa', 'nazwa_panstwa'.
2. Połączyć kolumny 'miesiąc' i 'rok' w jeden obiekt typu data o nazwie 'data_pomiaru'.
3. Wyświetlić statystyki podsumowujące dla średniej miesięcznej temperatury.
4. Zidentyfikować brakujące dane w każdej kolumnie i obliczyć ich sumę.
5. Usunąć wiersze, w których brakuje wartości w kolumnie 'srednia_temperatura'.
### Działania:
1. Wczytanie danych z CSV z użyciem Pandas.
2. Łączenie kolumn i tworzenie nowej kolumny z datą.
3. Sprawdzanie brakujących danych.
4. Usuwanie wierszy z brakami.
### Użyte biblioteki:
Pandas

## Zadanie 2
### Opis
Na podstawie pliku covidtotalswithmissings.csv wykonaj następujące operacje:
1. Zdefiniuj listę zmiennych "totvars" i "demovars".
2. Sprawdź liczbę brakujących wartości w kolumnach zmiennych demograficznych.
3. Oblicz liczbę wierszy, które mają co najmniej trzy brakujące wartości w kolumnach demograficznych.
4. Wyświetl lokalizację oraz brakujące zmienne demograficzne dla pięciu pierwszych wierszy, które mają co najmniej trzy brakujące wartości.
5. Sprawdź, ile brakujących danych znajduje się w "totvars".
6. Oblicz liczbę wierszy z brakującą co najmniej jedną wartość w "totvars".
7. Wyświetl dane dla wierszy z brakującą wartością w "totvars".
8. Napraw brakujące dane w "totvars" za pomocą odpowiednich metod (np. uzupełnianie na podstawie liczby przypadków na milion).
### Działania:
1. Praca z danymi za pomocą Pandas.
2. Wykrywanie brakujących danych.
3. Uzupełnianie braków za pomocą odpowiednich metod.
### Użyte biblioteki:
Pandas

## Zadanie 3
### Opis
Pracując na pliku covidtotals.csv wykonaj następujące operacje:
1. Zdefiniuj zmienne "totvars" i "demovars".
2. Zmień format wyświetlania liczb zmiennoprzecinkowych na dwie cyfry po przecinku.
3. Oblicz kwantyle od 0% do 100% z krokiem co 10%.
4. Oblicz skośność (skewness) oraz kurtozę (kurtosis).
5. Stwórz metodę do testowania normalności dla zmiennych "total_cases", "total_deaths", "total_cases_pm", "total_deaths_pm".
6. Wyświetl wykresy kwantyl-kwantyl (QQ plot) dla zmiennych "total_cases" i "total_cases_pm".
7. Wyświetl wartości odstające dla kolumny "total_cases".
8. Oblicz kwantyle dla zmiennych "pop_density" i "gdp_per_capita".
9. Przeprowadź transformację logarytmiczną danych dotyczących COVID-19.
9. Wyświetl histogram dla przetransformowanych danych o łącznej liczbie przypadków COVID-19.
### Działania:
1. Obliczanie kwantyli, skośności, kurtozy.
2. Testowanie normalności.
3. Wyświetlanie wykresów QQ-plot i histogramów.
### Użyte biblioteki:
1. Pandas
2. NumPy
3. Scipy
4. Matplotlib
5. Seaborn

## Zadanie 4
### Opis
1. W tym zadaniu wykorzystujemy dane z plików landtemps2019avgs.csv oraz covidtotals.csv do analizy i wizualizacji:
2. Wybierz 10 losowych próbek danych dotyczących stacji meteorologicznych.
3. Wygeneruj histogram rozkładu średnich temperatur w stacjach meteorologicznych, dodając linię wskazującą średnią temperaturę.
4. Wykonaj analizę kwantyl-kwantyl (QQ plot) dla badania rozkładu danych.
5. Oblicz skośności i kurtozy dla danych dotyczących liczby przypadków COVID-19 na milion mieszkańców.
6. Narysuj histogramy przedstawiające liczbę przypadków COVID-19 na milion mieszkańców dla czterech wybranych regionów.
### Działania:
1. Losowanie próbek danych.
2. Tworzenie histogramów, wykresów QQ-plot.
3. Obliczanie skośności i kurtozy.
4. Wizualizacja danych.
### Użyte biblioteki:
1. Pandas
2. Matplotlib
3. Seaborn
4. NumPy


# Laboratorium 3
## Opis
Laboratorium to koncentruje się na analizie brakujących danych, imputacji oraz identyfikacji wartości odstających w zbiorach danych dotyczących COVID-19. Zajmiemy się przetwarzaniem danych w trzech głównych zadaniach: identyfikacja braków danych, imputacja danych oraz analiza wartości odstających w kontekście korelacji pomiędzy danymi. Poniżej znajdują się szczegółowe instrukcje dotyczące wykonania każdego zadania.

## Zadanie 1
### Opis
1. Wczytaj dane z pliku covidtotals.csv
2. Wyświetl podstawowe informacje o danych
3. Zidentyfikuj kolumny z brakującymi wartościami
4. Oblicz procent braków
5. Stwórz wykres słupkowy
### Działania
1. Wczytanie danych z pliku CSV.
2. Analiza brakujących danych za pomocą .isnull() i .sum().
3. Wykres słupkowy przedstawiający rozkład braków.
### Użyte biblioteki:
1. Pandas
2. Matplotlib lub Seaborn

## Zadanie 2
### Opis
1. Znajdź kolumny numeryczne, które zawierają braki
2. Wybierz dwie kolumny i oblicz średnią oraz medianę
3. Zastosuj imputację
4. Porównaj statystyki przed i po imputacji
### Działania
1. Wybór kolumn numerycznych z brakami.
2. Obliczenie średniej i mediany.
3. Imputacja brakujących danych.
4. Porównanie statystyk przed i po imputacji.
### Użyte biblioteki
Pandas

## Zadanie 3
### Opis
1. Przypisz dane do zmiennej covidtotalsonly
2. Podziel kolumny "total_cases" i "total_deaths" na pięć przedziałów kwantylowych
3. Wygeneruj tabelę przestawną
4. Zidentyfikuj nietypowe relacje
5. Oblicz średnią wartość w kolumnie hosp_beds
6. Wygeneruj wykres regresji
7. Wybierz wiersze z nietypowymi wartościami
8. Wygeneruj wykres regresji dla danych total_cases_pm i total_deaths_pm
### Działania
1. Wybór danych z ramki covidtotals.
2. Podział na przedziały kwantylowe.
3. Tabela przestawna.
4. Wykres regresji oraz analiza nietypowych wartości.
### Użyte biblioteki:
1. Pandas
2. Seaborn
3. Matplotlib


# Laboratorium 4
## Opis
W niniejszym laboratorium zajmiemy się analizą danych z pliku Walmart.csv z wykorzystaniem regresji liniowej oraz regresji Lasso. Celem jest przewidywanie sprzedaży na podstawie różnych cech, a także ocena jakości modelu. Poniżej znajdziesz szczegółowe kroki wymagane do realizacji każdego zadania.

## Zadanie 1
### Cel
Wykonanie analizy regresji liniowej w celu przewidywania wartości sprzedaży na podstawie różnych cech w zbiorze danych.
### Kroki do wykonania
1. Zweryfikuj poprawność danych
2. Sprawdź kolumny, ich typy i statystyki opisowe
3. Wykryj brakujące dane i uzupełnij je metodą imputacji
4. Wykryj i usuń duplikaty oraz sprawdź ekstremalne wartości (outliery)
5. Oblicz macierz korelacji i przedstaw ją jako heatmapę
6. Konwertuj kolumny daty do typu datetime oraz kolumny kategoryczne do category
7. Zastosuj kodowanie One-Hot lub Label Encoding
8. Ustal kolumnę Weekly_Sales jako cel (target), a resztę jako cechy (features)
9. Podziel dane na zbiór treningowy i testowy
10. Zainicjalizuj model regresji liniowej
11. Wytrenuj model na danych treningowych
12. Użyj wytrenowanego modelu do przewidywania wartości sprzedaży
13. Oceń jakość modelu
14. Zastosuj kroswalidację (k-fold cross-validation)
15. Analizuj wpływ cech na sprzedaż
### Działania
1. Wczytanie danych, czyszczenie, kodowanie.
2. Budowa modelu regresji liniowej.
3. Ocena jakości modelu oraz analiza cech wpływających na sprzedaż.
### Użyte biblioteki:
1. Pandas
2. Matplotlib / Seaborn
3. Scikit-learn

## Zadanie 2
### Cel
Użycie regresji Lasso do prognozowania sprzedaży i oceny jakości modelu
### Kroki do wykonania
1. Usuń obserwacje z brakującymi wartościami
2. Upewnij się, że kolumny z datą są przekonwertowane na typ datetime oraz zmienne kategoryczne mają odpowiedni typ
3. Zastosuj One-Hot Encoding
4. Wykonaj standaryzację cech za pomocą StandardScaler
5. Podziel dane na zbiór treningowy i walidacyjny
6. Użyj LassoCV do przeprowadzenia kroswalidacji
7. Wytrenuj model na zbiorze treningowym
8. Użyj wytrenowanego modelu do przewidywania sprzedaży na zbiorze walidacyjnym
9. Oblicz MSE, RMSE oraz R²
### Działania
1. Czyszczenie danych i przygotowanie do modelowania.
2. Budowa modelu regresji Lasso z kroswalidacją.
3. Ocena jakości modelu i prognozowanie sprzedaży.
### Użyte biblioteki:
1. Pandas
2. Scikit-learn


# Laboratorium 5
## Opis
W tym laboratorium skoncentrujemy się na implementacji oraz trenowaniu różnych modeli sieci neuronowych. Praca obejmuje klasyfikację różnych zbiorów danych przy użyciu sieci neuronowych, optymalizację hiperparametrów oraz zastosowanie technik regularizacji w celu uniknięcia przeuczenia.

## Zadanie 1
### Cel
Zaimplementowanie sieci neuronowej do klasyfikacji zbioru danych Iris przy użyciu biblioteki TensorFlow/Keras lub PyTorch.
### Kroki do wykonania
1. Wczytaj zbiór danych Iris
2. Podział danych na zbiór treningowy i testowy
3. Zbudowanie sieci neuronowej
4. Wytrenuj model
5. Ocena skuteczności modelu
### Działania
1. Wczytanie i przygotowanie danych.
2. Budowa sieci neuronowej.
3. Trenowanie i ocena modelu.
### Użyte biblioteki:
1. TensorFlow/Keras lub PyTorch
2. Scikit-learn

## Zadanie 2
### Cel
Eksperymentowanie z różnymi hiperparametrami w celu uzyskania najlepszego modelu do klasyfikacji obrazów z zestawu MNIST (ręcznie pisane cyfry 0-9).
### Kroki do wykonania
1. Wczytaj zbiór danych MNIST
2. Podział danych na zbiór treningowy i testowy
3. Eksperymentuj z różnymi wartościami hiperparametrów
4. Zbuduj i wytrenuj model
5. Porównaj wyniki
### Działania
1. Budowa różnych modeli z różnymi hiperparametrami.
2. Eksperymentowanie z sieciami o różnej głębokości i liczbie neuronów.
3. Ocena jakości wyników.
### Użyte biblioteki:
1. TensorFlow/Keras lub PyTorch
2. Matplotlib/Seaborn (do wizualizacji wyników)

## Zadanie 3
### Cel
Zaimplementowanie sieci neuronowej do klasyfikacji danych Fashion-MNIST oraz zastosowanie technik regularizacji (Dropout, L2 regularization) oraz augmentacji danych w celu uniknięcia przeuczenia.
### Kroki do wykonania
1. Wczytaj zbiór danych Fashion-MNIST
2. Podział danych na zbiór treningowy i testowy
3. Zastosowanie technik regularizacji
4. Budowa sieci neuronowej
5. Wytrenuj model i oceniaj efektywność regularizacji
### Działania
1. Implementacja sieci neuronowej z technikami regularizacji.
2. Trenowanie i ocena modelu w kontekście unikania przeuczenia.
3. Przeanalizowanie wpływu regularizacji na wynik.
### Użyte biblioteki:
1. TensorFlow/Keras lub PyTorch
2. Scikit-learn (do oceny modelu)

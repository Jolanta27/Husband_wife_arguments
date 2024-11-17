<<<<<<< HEAD
# Analiza Kłótni Między Małżonkami i Przewidywanie Czasu Trwania Kłótni

## Opis projektu

Celem tego projektu jest analiza danych dotyczących kłótni między małżonkami oraz przewidywanie czasu trwania kłótni na podstawie różnych cech. W projekcie wykorzystano trzy modele: regresję liniową, las losowy oraz wielowarstwowy perceptron (MLP). Wyniki modeli zostały zalogowane do MLflow, co umożliwia śledzenie i porównywanie różnych modeli.

## Dane

Dane pochodzą z pliku CSV `husband_wife_arguments.csv`, który zawiera informacje o kłótniach między małżonkami, takie jak:
- Data kłótni
- Czas trwania kłótni (w minutach)
- Temat kłótni
- Emocjonalny ton kłótni
- Typ rozwiązania kłótni
- Nastrój po kłótni
- Notatki dotyczące kłótni

## Przygotowanie danych

1. **Przekształcenie kolumny `Date`**: Kolumna `Date` została przekształcona na trzy nowe kolumny: `Year`, `Month` i `Day`.
2. **Uzupełnienie brakujących wartości**: Brakujące wartości w kolumnie `Mood Swing` zostały uzupełnione wartością `Cant say`.
3. **Kodowanie zmiennych kategorycznych**: Zmiennie kategoryczne zostały zakodowane za pomocą OneHotEncoder.
4. **Standaryzacja zmiennych numerycznych**: Zmiennie numeryczne zostały standaryzowane.

## Trenowanie modeli

Dane zostały podzielone na zbiory treningowy i testowy. Trzy modele zostały wytrenowane:
- **Regresja liniowa**
- **Las losowy**
- **MLP**

## Wyniki modeli

### Regresja liniowa
- **Mean Squared Error (MSE)**: 1.001
- **R-squared**: 0.0027

### Las losowy
- **Mean Squared Error (MSE)**: 1.172
- **R-squared**: -0.167

### MLP
- **Mean Squared Error (MSE)**: 2.564
- **R-squared**: -1.554

## Wnioski

Na podstawie wyników można stwierdzić, że regresja liniowa osiągnęła najlepsze wyniki spośród trzech testowanych modeli, chociaż wszystkie modele miały stosunkowo niskie wartości R-squared, co sugeruje, że mogą nie być dobrze dopasowane do danych. Możliwe jest, że inne cechy lub bardziej zaawansowane modele mogłyby poprawić wyniki.

## Wnioski dotyczące przewidywanego tematu

Analiza danych dotyczących kłótni między małżonkami pozwoliła na wyciągnięcie kilku interesujących wniosków:
- **Czas trwania kłótni**: Średni czas trwania kłótni wynosił około 33 minut, z dużą zmiennością w zależności od tematu i emocjonalnego tonu.
- **Tematy kłótni**: Najczęściej poruszane tematy to "Parenting Styles", "Money Management" i "Time Management".
- **Emocjonalny ton**: Emocjonalny ton kłótni miał znaczący wpływ na czas trwania kłótni. Kłótnie z tonem "Angry" i "Frustrated" były zazwyczaj dłuższe.
- **Rozwiązanie kłótni**: Kłótnie, które kończyły się "No Resolution" lub "Resolution Discussed", były zazwyczaj dłuższe niż te, które kończyły się "Compromise" lub "Apology".

## Logowanie wyników do MLflow

Wyniki modeli zostały zalogowane do MLflow, co umożliwia śledzenie i porównywanie różnych modeli.

## Uruchomienie projektu

1. **Klonowanie repozytorium**:
   ```sh
   git clone https://github.com/TwojeRepozytorium/husband_wife_arguments.git
   cd husband_wife_arguments
=======
No starter code is provided. Start from scratch!
>>>>>>> 87ab371ac2e431dce1f1943a68f8c98317287561

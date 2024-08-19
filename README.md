# AI-fitness-assistant

# 1. Wprowadzenie

Program ten wykorzystuje techniki wizji komputerowej do liczenia powtórzeń ćwiczeń na podstawie wideo. Korzysta z biblioteki MediaPipe do wykrywania pozycji ciała i śledzenia kluczowych punktów stawów, analizując ruchy w celu zliczania powtórzeń takich ćwiczeń jak przysiady, martwe ciągi i uginanie ramion.



# 2. Wymagania

Przed uruchomieniem programu upewnij się, że zainstalowane są następujące biblioteki:
  OpenCV: Do przechwytywania wideo i przetwarzania obrazów.
  
  MediaPipe: Do wykrywania pozycji ciała.
  
  NumPy: Do operacji numerycznych.
  
  Pandas: Do manipulacji danymi.
  
  Tensorflow: Do tworzenia modeli uczenia maszynowego.




# 3. Struktura programu

## Program jest podzielony na kilka sekcji:
#### Importowanie bibliotek:
W tej sekcji importowane są niezbędne biblioteki, takie jak cv2 (OpenCV), mediapipe, numpy i pandas.
#### Wykrywanie pozycji i wizualizacja:
  Model do szacowania pozycji ciała z MediaPipe jest używany do wykrywania kluczowych punktów na ciele. Sekcja ta przetwarza klatki wideo w celu identyfikacji stawów i kończyn, wizualizując je za pomocą narzędzi rysunkowych MediaPipe.

#### Wykrywanie pozycji i wizualizacja:
  Model do szacowania pozycji ciała z MediaPipe jest używany do wykrywania kluczowych punktów na ciele. Sekcja ta przetwarza klatki wideo w celu identyfikacji stawów i kończyn, wizualizując je za pomocą narzędzi rysunkowych MediaPipe.
        


#### Przygotowanie danych:
Program przygotowuje dane poprzez przechwytywanie i przetwarzanie klatek wideo. Śledzi pozycje stawów w czasie i wyodrębnia odpowiednie cechy do trenowania modelu uczenia maszynowego.
Sekcja ta zawiera kod do konwersji punktów kontrolnych pozycji na format odpowiedni do analizy, np. kąty między stawami lub odległości.

#### Logika liczenia powtórzeń:
Kluczowym elementem programu jest logika liczenia powtórzeń. Analizując zmiany w pozycjach stawów, program na podstawie stworzonego modelu ai identyfikuje aktualny stan powtórzenia (górny lub dolny) i odpowiednio zwiększa licznik powtórzeń.

 #### Wizualizacja:
Sekcja ta zajmuje się również wizualizacją procesu liczenia, nakładając licznik powtórzeń na klatki wideo.

   
# 4. Użytkowanie

## Aby użyć programu:

 #### Przechwytywanie wideo:
  Użyj kamery internetowej lub nagranego wcześniej wideo jako wejścia. Program przetwarza każdą klatkę, aby wykryć pozycje ciała.

  #### Uruchom wykrywanie pozycji:
  Program automatycznie wykryje pozycje kluczowych stawów i będzie śledził ich ruchy w czasie.
  #### Wybór mierzonego ćwiczenia:
  1-Uginanie ramion
  2-Przysiady
  3-Martwy ciąg

  #### Liczenie powtórzeń:
  W trakcie wykonywania ćwiczenia program będzie liczył powtórzenia na podstawie wykrytych wzorców ruchu.

  #### Wyświetlanie wyników:
  Wideo z nałożonym licznikiem powtórzeń zostanie wyświetlone lub zapisane jako wynik.
    

# 5. Wynik

## Program wyprowadza następujące wyniki:

  Licznik w czasie rzeczywistym: Wyświetlany bezpośrednio na strumieniu wideo.
    

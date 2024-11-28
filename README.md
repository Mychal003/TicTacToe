
# TicTacToe Game

## Opis
TicTacToe to klasyczna gra kółko i krzyżyk zaimplementowana w języku C++ z wykorzystaniem biblioteki **SFML** do obsługi graficznego interfejsu użytkownika. Gra umożliwia rozgrywkę na planszach o dowolnym rozmiarze, z dynamicznie dostosowanymi wymiarami i automatycznym przeciwnikiem opartym na algorytmie Minimax z optymalizacją alpha-beta.

## Funkcjonalności
- **Dowolny rozmiar planszy**: Możesz grać na planszach większych niż standardowe 3x3.
- **Dynamiczne rysowanie planszy**: Interfejs graficzny jest dostosowywany do wybranego rozmiaru planszy.
- **Algorytm Minimax z alpha-beta pruning**: Komputerowy przeciwnik jest inteligentny i przewiduje najlepszy ruch.
- **Tryb graficzny**: Gra wykorzystuje bibliotekę SFML do wyświetlania planszy i obsługi interakcji myszką.

## Wymagania
- System operacyjny Linux.
- Biblioteka **SFML** (Simple and Fast Multimedia Library).
- Kompilator obsługujący C++11 lub nowszy.

## Instalacja
1. Upewnij się, że masz zainstalowaną bibliotekę **SFML**:
   ```bash
   sudo apt update
   sudo apt install libsfml-dev
   ```

2. Sklonuj repozytorium lub skopiuj kod źródłowy.

3. Skopiuj odpowiednią czcionkę (np. DejaVuSans.ttf) do katalogu `/usr/share/fonts/truetype/dejavu/`, jeśli nie jest tam obecna.

4. Skompiluj projekt:
   ```bash
   g++ -o TicTacToe main.cpp -lsfml-graphics -lsfml-window -lsfml-system
   ```

## Uruchamianie
Uruchom grę poleceniem:
```bash
./TicTacToe
```
Następnie wprowadź rozmiar planszy, np. 3 dla 3x3, i rozpocznij rozgrywkę.

## Sterowanie
- Kliknij lewym przyciskiem myszy na wybrane pole, aby wykonać ruch.
- Gra automatycznie obsługuje ruchy komputera.

## Problemy i znane błędy
- **Czcionka**: Gra wymaga obecności czcionki DejaVuSans w określonej ścieżce. Jeśli gra nie uruchamia się poprawnie, upewnij się, że czcionka znajduje się w `/usr/share/fonts/truetype/dejavu/`.
- **Głębia rekursji**: Algorytm Minimax dla dużych plansz (np. 10x10) może być wolny. Został zaimplementowany limit głębokości dla poprawy wydajności.

## Plany rozwoju
- Dodanie możliwości gry dla dwóch graczy.
- Optymalizacja algorytmu dla plansz większych niż 5x5.
- Ulepszenie oprawy graficznej i dodanie animacji.

## Licencja
Projekt jest udostępniany na licencji MIT. Możesz korzystać z kodu w dowolnym celu, pod warunkiem zachowania oryginalnej informacji o autorze.

## Autor
Projekt stworzony przez Michała Pawlika w ramach projektu z projektowania i analizy algorytmów.

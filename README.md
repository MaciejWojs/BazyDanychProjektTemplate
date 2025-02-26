# Projekt Dokumentacji LaTeX

Ten projekt jest szablonem repozytorium do tworzenia dokumentacji w LaTeX. Zawiera predefiniowane ustawienia i pakiety, które ułatwiają pracę z dokumentami LaTeX, w tym wsparcie dla języka polskiego.

## Używanie w Codespace

Aby używać tego projektu w Codespace, wykonaj poniższe kroki:

1. **Utwórz Codespace**:
   - Przejdź do repozytorium na GitHub.
   - Kliknij przycisk "Code" i wybierz "Create Codespace on main".

2. **Konfiguracja środowiska**:
   - Po utworzeniu Codespace, środowisko zostanie automatycznie skonfigurowane na podstawie plików w folderze `.devcontainer`.
   - Plik `Dockerfile` zawiera instrukcje instalacji niezbędnych pakietów, takich jak LaTeX, biber, ghostscript, doxygen, graphviz, python3 i inkscape.
   - Plik `devcontainer.json` zawiera ustawienia specyficzne dla VS Code, takie jak motyw kolorów, narzędzia do budowania LaTeX oraz rozszerzenia.

3. **Budowanie dokumentu**:
   - Otwórz plik `dokument.tex` w edytorze.
   - Użyj polecenia `Ctrl+Alt+B` (lub odpowiedniego skrótu klawiszowego) do zbudowania dokumentu LaTeX.
   - Po zakończeniu budowania, wynikowy plik PDF będzie dostępny w panelu podglądu.

4. **Przesyłanie pliku PDF**:
   - Aby przesłać wygenerowany plik PDF, użyj skryptu `upload.sh`.
   - Otwórz terminal w Codespace i uruchom skrypt:
     ```bash
     ./upload.sh
     ```
   - Skrypt przesyła plik `dokument.pdf` oraz opcjonalnie `dokument-compressed.pdf` do zewnętrznego serwera i zwraca URL do pobrania.

## Struktura projektu

- `dokument.tex`: Główny plik dokumentu LaTeX.
- `preambula_pakiety.tex`: Plik z pakietami LaTeX.
- `preambula_ustawienia.tex`: Plik z ustawieniami LaTeX.
- `tex/`: Folder z rozdziałami dokumentu.
- `rys/`: Folder ze zdjęciami zawartymi w projekcie
- `.devcontainer/`: Folder z konfiguracją środowiska Codespace.

## Przydatne skróty klawiszowe

- `Ctrl+Alt+B`: Budowanie dokumentu LaTeX.
- `Ctrl+Shift+~`: Otwieranie terminala.
- `Ctrl+Alt+J`: Przeniesienie z kodu do PDF.
- `Ctrl+Click`: Przeniesienie z PDF do kodu.

## Dodatkowe informacje

Więcej informacji na temat używania LaTeX w VS Code można znaleźć w dokumentacji rozszerzenia [LaTeX Workshop](https://github.com/James-Yu/LaTeX-Workshop).

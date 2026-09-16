# Edytor kresek — wersja webowa (GitHub Pages)

Samodzielna wersja edytora, gotowa do wgrania na GitHub. Działa tak samo jak w Claude.

## Co wrzucić do repo (genso3/EdytorAdam)
- `index.html` — **cały program w jednym pliku** (logo CWL i skrypty pomocnicze wbudowane). Nadpisz nim stary `index.html` w katalogu głównym repo.
- `README.md` — opcjonalnie.

Nic więcej nie jest potrzebne — żadnych folderów, żadnych plików PDF.

## Jak wgrać (przez stronę GitHuba, bez żadnych narzędzi)
1. Pobierz oba pliki z tego projektu (przycisk pobierania pod tą wiadomością w czacie).
2. Wejdź na `https://github.com/genso3/EdytorAdam`.
3. **Add file → Upload files**, przeciągnij nowy `index.html` (i ewentualnie `README.md`) do okna.
4. Na dole wpisz krótki opis zmiany i kliknij **Commit changes** — GitHub podmieni plik o tej samej nazwie.
5. Strona `https://genso3.github.io/EdytorAdam/` odświeży się w ciągu ~1–2 minut.
6. Jeśli widzisz starą wersję — odśwież z pominięciem cache: **Ctrl+Shift+R**.

(Ustawienia Pages są już zrobione: Settings → Pages → Deploy from a branch, `main`, folder `/ (root)`.)

## Co jest w tej wersji
**Narzędzia:** Linia, Punkt, Szyk punktów, Wymiar, Gumka, Przytnij (+ Przesuń/panorama, zoom, obrót strony).

- **Szyk punktów** — przeciągasz linię, zostają same punkty w równym rozstawie. Zaznaczenie szyku pozwala zmienić liczbę punktów (−/+ lub wpisanie) albo wpisać rozstaw w jednostce kalibracji; „Rozbij na punkty” zamienia szyk na osobne punkty. Etykieta `n × rozstaw` i automatyczne wymiary rozstawu.
- **Wymiar** — ręczne wymiarowanie odcinków w jednostce kalibracji (wymaga wcześniejszej skali).
- **Punkt** — punkty asekuracyjne jako osobne typy w legendzie (kolor, rozmiar mm).
- **Przytnij** — wycięcie fragmentu rysunku do pola arkusza; „Anuluj przycięcie” wraca do całości. Przycięcie działa też w eksporcie wektorowym.
- **Zapisz roboczy / Otwórz roboczy** — kopia robocza (PDF + kreski + tabelka + kalibracja) do pliku, żeby wrócić do pracy bez ponownej kalibracji.
- **Zakładki** — kilka rysunków otwartych równocześnie, każdy z własną legendą, tabelką i formatem.
- **Automatyczny format arkusza A0–A4** wykrywany z wgranego PDF-a + ręczna zmiana formatu i orientacji (kreski i kalibracja przeliczane proporcjonalnie).
- **Typy kresek i punktów** w legendzie: nazwa, kolor, grubość/rozmiar w mm, linia ciągła lub kreskowana.
- **Skala i pomiar** długości, etykiety długości z regulacją wielkości.
- **Eksport PDF** — osadza stronę źródłową wektorowo (bez utraty jakości), dorysowuje ramkę, kreski, punkty, wymiary, tabelkę i logo; multistrona; wybór jakości eksportu.
- Tabelka rysunkowa WYSIWYG: legenda, pola Nazwa / Opracował / Projekt / Data, przełącznik ramki.
- Cofnij/Ponów (Ctrl+Z / Ctrl+Shift+Z), Wyczyść, Dopasuj.
- Języki interfejsu: polski, szwedzki, angielski.
- Poprawione odbicie tekstu z rysunków CAD (cyfry wymiarowe nie są w lustrzanym odbiciu) i szybkie renderowanie wektorowe (pomijanie „soft-mask”, który zawieszał przeglądarkę).

## Wymaga internetu
Silnik pdf.js, eksport PDF i czcionka z polskimi znakami ładują się z CDN — strona musi mieć dostęp do sieci. GitHub Pages to zapewnia.

## Uwaga
Edytor startuje pusty. Rysunek wczytujesz przyciskiem **+ PDF** lub **Otwórz PDF** na ekranie startowym.

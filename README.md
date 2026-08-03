# Edytor kresek — wersja webowa (GitHub Pages)

Samodzielna wersja edytora, gotowa do wgrania na GitHub. Działa tak samo jak w Claude.

## Co wrzucić do repo (genso3/EdytorAdam)
- `index.html` — **cały program w jednym pliku** (logo CWL i skrypty pomocnicze wbudowane). Nadpisz nim stary `index.html` w katalogu głównym repo.
- `README.md` — opcjonalnie.

Nic więcej nie jest potrzebne — żadnych folderów, żadnych plików PDF.

## Jak wgrać (najprościej, przez stronę GitHuba)
1. Wejdź do repo `EdytorAdam` → kliknij stary plik `index.html` → ikona ołówka (Edit).
2. Zamiast edytować: wróć do katalogu głównego, kliknij **Add file → Upload files**, przeciągnij nowy `index.html` i zatwierdź (**Commit changes**) — GitHub podmieni plik o tej samej nazwie.
3. Strona `https://genso3.github.io/EdytorAdam/` odświeży się w ciągu ~1–2 minut.
4. Jeśli widzisz starą wersję — odśwież z pominięciem cache: **Ctrl+Shift+R**.

(Ustawienia Pages są już zrobione: Settings → Pages → Deploy from a branch, `main`, folder `/ (root)`.)

## Co jest w tej wersji (nowości względem starej na GitHubie)
- **Automatyczny format arkusza A0–A4** wykrywany z wgranego PDF-a + ręczna zmiana formatu i orientacji (kreski i kalibracja przeliczane proporcjonalnie).
- Poprawione **odbicie tekstu** z rysunków CAD (cyfry wymiarowe nie są już w lustrzanym odbiciu) — w podglądzie i w eksporcie.
- Szybkie renderowanie wektorowe rysunków z CAD-a (pomijanie „soft-mask”, który zawieszał przeglądarkę).
- Eksport PDF osadza stronę źródłową wektorowo (bez utraty jakości), dorysowuje ramkę, kreski, tabelkę i logo.
- Tabelka rysunkowa WYSIWYG: legenda typów kresek, pola Nazwa / Opracował / Projekt / Data, przełącznik ramki.
- Skala i pomiar długości, typy kresek (kolor, grubość mm, ciągła/kreskowana), zoom, Cofnij/Ponów, multistrona.

## Wymaga internetu
Silnik pdf.js, eksport PDF i czcionka z polskimi znakami ładują się z CDN — strona musi mieć dostęp do sieci. GitHub Pages to zapewnia.

## Uwaga
Edytor startuje pusty. Rysunek wczytujesz przyciskiem **+ PDF** lub **Otwórz PDF** na ekranie startowym.

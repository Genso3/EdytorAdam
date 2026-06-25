# Edytor kresek — wersja webowa (GitHub Pages)

To jest samodzielna wersja edytora, gotowa do wgrania na GitHub. Działa tak samo jak w Claude.

## Zawartość
- `index.html` — cały edytor w jednym pliku (uruchamia się w przeglądarce).
- `uploads/PAB_P001227_II-A03.pdf` — przykładowy rysunek wczytywany na starcie.
- `uploads/logo-cwl.png` — logo CWL używane w tabelce eksportowanego PDF-a.

## Jak wgrać na GitHub Pages
1. Wrzuć całą zawartość tego folderu (`index.html` + folder `uploads/`) do repozytorium — najlepiej do katalogu głównego (root).
2. W ustawieniach repo: **Settings → Pages → Source = Deploy from a branch**, wybierz gałąź (np. `main`) i folder `/ (root)`.
3. Po chwili strona będzie pod adresem `https://<twój-login>.github.io/<repo>/`.

Ważne: zachowaj strukturę folderów — `index.html` musi mieć obok siebie folder `uploads/`, inaczej przykładowy rysunek i logo się nie wczytają.

## Wymaga internetu
Eksport PDF, czcionki (polskie znaki) i silnik pdf.js ładują się z CDN, więc strona musi mieć dostęp do sieci. GitHub Pages to zapewnia.

## Uwaga
Własny rysunek wczytujesz przyciskiem **+ PDF** — nie trzeba podmieniać pliku przykładowego.

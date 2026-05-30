# Santé Medica Petit — strona internetowa

Butikowa klinika kobieca w Gdańsku. Statyczna strona (HTML/CSS/JS), gotowa do
publikacji na GitHub Pages lub dowolnym hostingu plików statycznych.

## Struktura

```
index.html              — strona główna
assets/
  styles.css            — style (paleta, typografia, sekcje)
  main.js               — nawigacja, animacje, parallax, opinie
  pricing.js            — dane i renderowanie cennika
  image-slot.js         — komponent zdjęć (drag & drop)
  fonts/                — czcionki marki (De Lionist, Quasimoda)
  logos/                — logotypy SVG
  decor/                — dekoracje (arkada, ilustracje liniowe)
  photos/               — zdjęcia (wersje zoptymalizowane pod web)
```

## Publikacja na GitHub Pages

1. Utwórz nowe repozytorium na GitHub (np. `sante-medica-petit`).
2. Wgraj całą zawartość tego folderu do repozytorium:
   ```bash
   git init
   git add .
   git commit -m "Santé Medica Petit — website"
   git branch -M main
   git remote add origin https://github.com/UZYTKOWNIK/sante-medica-petit.git
   git push -u origin main
   ```
3. W repozytorium: **Settings → Pages**.
4. W sekcji **Build and deployment** → **Source** wybierz **Deploy from a branch**.
5. Branch: **main**, folder: **/ (root)**. Zapisz.
6. Po chwili strona będzie dostępna pod adresem
   `https://UZYTKOWNIK.github.io/sante-medica-petit/`.

## Edycja treści

- **Cennik** — edytuj tablicę `CENNIK` w `assets/pricing.js`.
- **Teksty** — bezpośrednio w `index.html`.
- **Zdjęcia** — podmień pliki w `assets/photos/` (zachowaj nazwy) lub na żywej
  stronie przeciągnij nowe zdjęcie na wybrane miejsce.
- **Kolory / typografia** — zmienne na górze `assets/styles.css` (`:root`).

## Uwaga

Mapa Google w sekcji Kontakt ładuje się z internetu — wymaga połączenia sieciowego.

# 🚀 QUICK START - Jak uruchomić stronę lokalnie

## Metoda 1: VSCode Live Server (NAJŁATWIEJSZA)

1. Otwórz folder projektu w VSCode
2. Zainstaluj rozszerzenie "Live Server" (jeśli nie masz)
3. Kliknij prawym przyciskiem na `index.html`
4. Wybierz "Open with Live Server"
5. ✅ Strona otworzy się w przeglądarce!

---

## Metoda 2: Python (jeśli masz Pythona)

```bash
# Otwórz terminal w folderze projektu
cd motocentrum-tyrtania

# Uruchom serwer
python -m http.server 8000

# Otwórz w przeglądarce:
# http://localhost:8000
```

---

## Metoda 3: Bezpośrednio w przeglądarce

**UWAGA**: Niektóre funkcje (np. fetch JSON) mogą nie działać!

1. Otwórz folder projektu
2. Przeciągnij `index.html` na przeglądarkę
3. LUB kliknij prawym → "Otwórz za pomocą" → Przeglądarka

---

## ✅ Test - Sprawdź czy działa:

- [ ] Logo wyświetla się
- [ ] 4 auta załadowały się w "Polecane oferty"
- [ ] Można kliknąć numer telefonu
- [ ] Mapa Google się ładuje
- [ ] Responsywność (zmień rozmiar okna)
- [ ] Hamburger menu na mobile

---

## 🌐 Następny krok: GitHub Pages

Gdy sprawdzisz że wszystko działa lokalnie:

1. Przeczytaj `DEPLOYMENT.md`
2. Wgraj na GitHub
3. Włącz GitHub Pages
4. Gotowe - strona online!

---

## 🆘 Problem?

**CSS się nie ładuje?**
- Sprawdź czy folder `css` jest w tym samym miejscu co `index.html`

**Auta się nie ładują?**
- Sprawdź czy folder `data` i plik `cars.json` są obecne
- Otwórz Console w przeglądarce (F12) i zobacz błędy

**Zdjęcia nie działają?**
- Sprawdź czy folder `images` jest obecny
- Upewnij się że ścieżki są poprawne

---

**Gotowe! Teraz możesz testować stronę lokalnie.** 🎉

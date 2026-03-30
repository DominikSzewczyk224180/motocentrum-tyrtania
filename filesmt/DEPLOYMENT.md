# 🚀 Jak postawić stronę online - KOMPLETNY PRZEWODNIK

## OPCJA 1: GitHub Pages (NAJSZYBSZA - 100% DARMOWA)

### Krok 1: Przygotuj konto GitHub
1. Jeśli nie masz konta, zarejestruj się na https://github.com
2. Zweryfikuj email

### Krok 2: Stwórz repozytorium
1. Kliknij "+" w prawym górnym rogu → "New repository"
2. Nazwa: `motocentrum-tyrtania`
3. Opis: "Strona internetowa Motocentrum Tyrtania"
4. Public (publiczne)
5. NIE dodawaj README (już masz)
6. Create repository

### Krok 3: Wgraj pliki
```bash
# Otwórz terminal w folderze projektu

# Inicjalizuj git
git init

# Dodaj wszystkie pliki
git add .

# Pierwszy commit
git commit -m "Initial commit - strona Motocentrum Tyrtania"

# Zmień nazwę brancha na main
git branch -M main

# Dodaj remote (ZAMIEŃ na swój link)
git remote add origin https://github.com/TWOJ-USERNAME/motocentrum-tyrtania.git

# Wyślij na GitHub
git push -u origin main
```

### Krok 4: Włącz GitHub Pages
1. Wejdź do swojego repo na GitHubie
2. Settings (na górze)
3. Po lewej: "Pages"
4. Source: "Deploy from a branch"
5. Branch: "main" + folder "/ (root)"
6. Save

### Krok 5: Gotowe!
Po 2-3 minutach strona będzie dostępna pod:
```
https://TWOJ-USERNAME.github.io/motocentrum-tyrtania/
```

---

## OPCJA 2: Railway.app (DO DYNAMICZNEJ STRONY Z BACKEND)

### Kiedy używać?
Gdy dodasz Flask backend i bazę danych - na razie NIE POTRZEBUJESZ!

### Krok 1: Załóż konto
1. Wejdź na https://railway.app
2. Sign up with GitHub
3. Autoryzuj Railway

### Krok 2: Deploy
1. Dashboard → "New Project"
2. "Deploy from GitHub repo"
3. Wybierz `motocentrum-tyrtania`
4. Railway automatycznie wykryje typ projektu

### Krok 3: Konfiguracja (jeśli będzie backend)
Stwórz plik `requirements.txt`:
```
Flask==3.0.0
gunicorn==21.2.0
```

Stwórz plik `Procfile`:
```
web: gunicorn app:app
```

### Krok 4: Custom domena
1. W Railway → Settings → Domains
2. "Generate Domain" (dostaniesz xxx.railway.app)
3. Lub dodaj swoją domenę

---

## OPCJA 3: Netlify (ALTERNATYWA DO GITHUB PAGES)

### Najszybsza metoda - Drag & Drop
1. Wejdź na https://netlify.com
2. Zarejestruj się
3. "Add new site" → "Deploy manually"
4. Przeciągnij cały folder projektu
5. Gotowe! Dostaniesz link typu: random-name.netlify.app

### Przez GitHub (lepsze)
1. "Add new site" → "Import from Git"
2. Wybierz GitHub
3. Wybierz repo `motocentrum-tyrtania`
4. Deploy

---

## 💰 KOSZTY - Porównanie

### GitHub Pages
- **Koszt**: 0 zł/miesiąc
- **Domena**: xxx.github.io (darmowa)
- **Limit**: Tylko statyczne strony HTML/CSS/JS
- **Idealny dla**: Demo i prezentacji

### Railway
- **Koszt**: 0 zł (500h darmowo/miesiąc) lub ~20 zł/m
- **Domena**: xxx.railway.app (darmowa)
- **Obsługa**: Backend, bazy danych
- **Idealny dla**: Finalna wersja z panelem admin

### Netlify
- **Koszt**: 0 zł/miesiąc
- **Domena**: xxx.netlify.app (darmowa)
- **Funkcje**: Formularze, funkcje serverless
- **Idealny dla**: Demo i prezentacji

---

## 🌐 WŁASNA DOMENA (motocentrumtyrtania.pl)

### Gdzie kupić?
1. **home.pl** - ~50 zł/rok (.pl)
2. **OVH.pl** - ~30 zł/rok (.pl)
3. **Cloudflare** - ~35 zł/rok (.com)

### Jak podpiąć do GitHub Pages?

#### Krok 1: Kup domenę
Załóż konto na home.pl i kup domenę

#### Krok 2: Stwórz plik CNAME
W głównym folderze projektu:
```
motocentrumtyrtania.pl
```

#### Krok 3: Dodaj do GitHub
```bash
git add CNAME
git commit -m "Add custom domain"
git push
```

#### Krok 4: DNS w home.pl
W panelu domeny → DNS → Dodaj rekordy:

**Typ A:**
```
@  →  185.199.108.153
@  →  185.199.109.153
@  →  185.199.110.153
@  →  185.199.111.153
```

**Typ CNAME:**
```
www  →  TWOJ-USERNAME.github.io
```

#### Krok 5: GitHub Settings
1. Repo → Settings → Pages
2. Custom domain: wpisz `motocentrumtyrtania.pl`
3. Save
4. ✅ Enforce HTTPS (po kilku minutach)

#### Krok 6: Czekaj
Propagacja DNS: 1-24h (zazwyczaj 1-2h)

---

## ✅ CHECKLIST PRZED POKAZANIEM KLIENTOWI

- [ ] Wszystkie zdjęcia załadowane
- [ ] Logo wyświetla się poprawnie
- [ ] Wszystkie linki działają
- [ ] Telefon jest klikalny
- [ ] Mapa Google działa
- [ ] Strona responsywna (sprawdź na telefonie)
- [ ] Opinie Google wyświetlone
- [ ] Statystyki są aktualne
- [ ] Footer ma prawidłowe dane
- [ ] Social media linki działają

---

## 🎯 PLAN PREZENTACJI DLA KLIENTA

### 1. Pokaż demo (GitHub Pages)
"Oto wersja demonstracyjna strony. Działa już online i możesz ją zobaczyć z dowolnego urządzenia."

### 2. Przejdź przez sekcje
- Hero: "Pierwsze wrażenie - eleganckie, profesjonalne"
- Oferty: "Automatycznie ładowane z bazy"
- Dlaczego my: "Podkreśla Wasze mocne strony"
- Opinie: "4.9 gwiazdek - to buduje zaufanie"
- Kontakt: "Łatwy kontakt i mapa"

### 3. Pokaż responsywność
Zmień rozmiar okna lub pokaż na telefonie

### 4. Przedstaw ofertę
"Co dostajesz:"
- Profesjonalna strona
- Własna domena (motocentrumtyrtania.pl)
- Hosting na rok
- Panel do zarządzania ofertami
- Szkolenie jak dodawać auta
- 3 miesiące wsparcia technicznego

"Cena: 2500 zł jednorazowo + 150 zł/rok hosting"

### 5. Kolejne kroki
"Jeśli się podoba, potrzebuję:"
- Decyzji (tak/nie)
- 2 tygodni na wdrożenie
- Dostępu do zdjęć aut (alta możesz je ściągać z OtoMoto)
- Opisów dla każdego auta

---

## 📞 WSPARCIE

Jeśli coś nie działa:
1. Sprawdź console w przeglądarce (F12)
2. Upewnij się że wszystkie pliki są na miejscu
3. Sprawdź czy ścieżki do plików są poprawne

## 🎓 DALSZY ROZWÓJ

Po akceptacji klienta:
1. Dodać stronę z pełną ofertą
2. Filtry i wyszukiwanie
3. Panel admina (Flask)
4. Formularz kontaktowy z emailem
5. Blog/aktualności (opcjonalnie)
6. Integracja z Facebook Pixel (tracking)

---

**Powodzenia z prezentacją! 🚀**

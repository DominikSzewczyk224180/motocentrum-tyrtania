# Motocentrum Tyrtania - Strona Internetowa

Profesjonalna strona internetowa dla komisu samochodowego Motocentrum Tyrtania w Rzuchowie.

## 📋 Funkcjonalności

- ✅ Responsywny design (desktop, tablet, mobile)
- ✅ Nowoczesny i elegancki wygląd
- ✅ Sekcja z polecany mi ofertami
- ✅ Dynamiczne ładowanie aut z JSON
- ✅ Opinie klientów z Google (4.9⭐)
- ✅ Sekcja "Dlaczego my"
- ✅ Integracja z Google Maps
- ✅ Smooth scroll i animacje
- ✅ Back to top button
- ✅ Mobile hamburger menu

## 🚀 Jak uruchomić lokalnie

### Metoda 1: Live Server (VSCode)
1. Zainstaluj rozszerzenie "Live Server" w VSCode
2. Otwórz folder projektu w VSCode
3. Kliknij prawym na `index.html` → "Open with Live Server"

### Metoda 2: Python SimpleHTTPServer
```bash
cd motocentrum-tyrtania
python -m http.server 8000
```
Następnie otwórz: http://localhost:8000

### Metoda 3: Bezpośrednio w przeglądarce
Po prostu otwórz plik `index.html` w przeglądarce (niektóre funkcje mogą nie działać)

## 📁 Struktura projektu

```
motocentrum-tyrtania/
├── index.html              # Strona główna
├── oferta.html            # Lista wszystkich aut (TODO)
├── o-nas.html             # O firmie (TODO)
├── kontakt.html           # Strona kontaktowa (TODO)
├── auto-details.html      # Szczegóły auta (TODO)
├── css/
│   └── style.css          # Główne style
├── js/
│   └── main.js            # JavaScript
├── images/
│   ├── cars/              # Zdjęcia aut
│   ├── logos/             # Logo firmy
│   ├── hero-bmw.png       # Zdjęcie hero
│   └── building.png       # Zdjęcie budynku
├── data/
│   └── cars.json          # Baza danych aut
└── README.md              # Ten plik
```

## 🎨 Kolorystyka

- **Złoty akcent**: #c9a961 (z logo)
- **Czarny/ciemny**: #1a1a1a
- **Tło jasne**: #f8f8f8
- **Białe**: #ffffff

## 📱 Sekcje strony głównej

1. **Hero Section** - Duże zdjęcie z nagłówkiem i statystykami
2. **Polecane oferty** - 4 najlepsze auta
3. **Dlaczego my** - 6 zalet komisu
4. **Opinie klientów** - 3 najlepsze opinie z Google
5. **Kontakt preview** - Mapa i podstawowe info
6. **Footer** - Nawigacja i dane kontaktowe

## 🔧 Następne kroki (TODO)

- [ ] Strona z pełną ofertą (oferta.html)
- [ ] Filtry i wyszukiwanie aut
- [ ] Strona szczegółów auta
- [ ] Strona O nas
- [ ] Strona Kontakt z formularzem
- [ ] Backend (Flask) do zarządzania ofertami
- [ ] Panel administratora

## 🌐 Deployment na GitHub Pages

1. **Stwórz repo na GitHubie**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TWOJ-USERNAME/motocentrum-tyrtania.git
git push -u origin main
```

2. **Włącz GitHub Pages**
- Wejdź do Settings → Pages
- Source: Deploy from branch
- Branch: main
- Folder: / (root)
- Save

3. **Strona będzie dostępna pod:**
`https://TWOJ-USERNAME.github.io/motocentrum-tyrtania/`

## 📊 Dane kontaktowe (w kodzie)

- **Adres**: Pstrązka 6, 44-285 Rzuchów
- **Telefon**: +48 733 944 449
- **Facebook**: [Link](https://www.facebook.com/p/Salon-Samochodowy-MOTOCENTRUM-TYRTANIA-100063584170987/)
- **Instagram**: [Link](https://www.instagram.com/motocentrum.tyrtania/)
- **Google Maps**: 4.9⭐ - 181 opinii

## 💡 Jak dodać nowe auto

Edytuj plik `data/cars.json`:

```json
{
  "id": 5,
  "brand": "BMW",
  "model": "Seria 3",
  "version": "320d xDrive",
  "year": 2020,
  "price": 135000,
  "mileage": 85000,
  "fuel": "Diesel",
  "transmission": "Automatyczna",
  "power": 190,
  "capacity": 1995,
  "drive": "4x4",
  "color": "Czarny",
  "doors": 4,
  "image": "images/cars/bmw-320d.png",
  "images": ["images/cars/bmw-320d.png"],
  "featured": true,
  "description": "Opis auta...",
  "equipment": ["Skóra", "Nawigacja", "..."]
}
```

## 🎓 Technologie

- HTML5
- CSS3 (Flexbox, Grid, Animations)
- Vanilla JavaScript (ES6+)
- Google Fonts (Montserrat, Open Sans)
- Google Maps Embed API

## 📞 Kontakt z deweloperem

Stronę stworzył: **Dominik**
Data Science & AI Student @ Breda University

---

**Wersja**: 1.0.0  
**Data**: Luty 2025  
**Status**: Demo - Gotowe do prezentacji klientowi

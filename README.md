# Sprelli — Platforma Korepetycji Online

**Sprelli** to nowoczesny marketplace edukacyjny łączący uczniów z zweryfikowanymi korepetytorami w Polsce. Platforma umożliwia rezerwację lekcji indywidualnych i grupowych, naukę przez interaktywne narzędzia oraz śledzenie postępów — wszystko w jednym miejscu.

---

## Czym jest Sprelli?

Sprelli to kompletna platforma edukacyjna, na której:

- **Uczniowie** (i rodzice) mogą znaleźć zweryfikowanego korepetytora, zarezerwować lekcję i płacić bezpiecznie przez internet
- **Korepetytorzy** budują swoją markę, zarządzają harmonogramem, sprzedają materiały edukacyjne i prowadzą lekcje bez żadnych zewnętrznych narzędzi
- **Szkoły i instytucje** mogą korzystać z platformy jako narzędzia do uzupełniania edukacji

Nasza misja: zdemokratyzować dostęp do wysokiej jakości korepetycji w Polsce.

---

## Dla uczniów

- **Szukaj i filtruj** nauczycieli według przedmiotu, poziomu, ceny i dostępności
- **Rezerwuj lekcje** indywidualne lub grupowe z weryfikowanymi korepetytorami
- **Ucz się online** w dedykowanym Pokoju Lekcyjnym z wideo, tablicą, czatem i quizami
- **Śledzij postępy** — XP, poziomy, seria dni nauki, osiągnięcia i cele
- **Rozwiązuj quizy i minigry** przypisane przez nauczyciela lub publiczne
- **Kupuj materiały edukacyjne** od nauczycieli z marketplace
- **Zarządzaj kontem rodzicielskim** — panel dla rodziców dzieci

---

## Dla korepetytorów

- **Profesjonalny profil** z opisem, stylami nauczania, certyfikatami i opiniami uczniów
- **Elastyczny harmonogram** — precyzyjna kontrola dostępności, przerwy między lekcjami, dni wolne
- **Lekcje indywidualne i grupowe** — pełne zarządzanie, rezerwacje, anulowania, przeniesienia
- **Pokój Lekcyjny** z wideokonferencją, wspólną tablicą, materiałami i quizami na żywo
- **Marketplace materiałów** — sprzedawaj PDFy, notatki, ćwiczenia bezpośrednio uczniom
- **Tworzenie quizów i minigier** dla swoich uczniów (6 typów gier edukacyjnych)
- **Weryfikacja tożsamości i kwalifikacji** — badge zaufania widoczny na profilu
- **Panel statystyk** — zarobki, liczba uczniów, oceny, historia lekcji
- **Program subskrypcji** — plany rozszerzające możliwości i obniżające prowizję

---

## Pokój Lekcyjny (LessonRoom)

Własna, wbudowana przestrzeń do prowadzenia lekcji online:

| Narzędzie | Opis |
|-----------|------|
| **Wideo** | Połączenie audio-wideo w czasie rzeczywistym |
| **Tablica** | Współdzielona tablica do rysowania i pisania, eksport do PNG |
| **Czat** | Wbudowany czat tekstowy |
| **Quizy** | Nauczyciel wysyła quiz, uczeń rozwiązuje na żywo |
| **Materiały** | Udostępnianie plików w trakcie lekcji |
| **Minigry** | 6 typów interaktywnych gier edukacyjnych |
| **Timer** | Odliczanie czasu lekcji widoczne dla nauczyciela |

Lekcja grupowa obsługuje wielu uczestników z dynamiczną wyceną per osoba.

---

## System Gamifikacji

Nauka na Sprelli to też zabawa. Platforma posiada pełny system motywacyjny:

- **XP (punkty doświadczenia)** za ukończone lekcje, quizy, serie dni nauki
- **9 poziomów** — od Początkującego do Kolosa Edukacji
- **Streak** — seria kolejnych dni aktywności z nagrodami XP za milestone'y (3, 7, 14, 30, 60, 100 dni)
- **Osiągnięcia** — odznaki w 6 kategoriach (lekcje, quizy, materiały, seria, społeczność, kamienie milowe)
- **Cele nauki** — nauczyciel wyznacza cele z kamieniami milowymi, uczeń je realizuje
- **Tablice wyników** i publiczne profile z przypiętymi osiągnięciami

---

## Stos Technologiczny

Sprelli zbudowane jest na nowoczesnym, sprawdzonym stosie technologicznym:

**Frontend**
- Next.js 16 (App Router) + React 19 + TypeScript 5
- Tailwind CSS 4 — responsywny design, dark mode
- PWA — instalowalna aplikacja na telefonach

**Backend**
- Python + FastAPI — wydajne asynchroniczne API
- PostgreSQL — relacyjna baza danych
- Redis — sesje, kolejki zadań, WebSocket pub/sub
- JWT authentication z automatycznym odświeżaniem tokenów

**Infrastruktura**
- Hosting frontend: Vercel (CDN globalny)
- Hosting backend: Railway (auto-scaling)
- Storage plików: AWS S3 (region Europa)
- Płatności: Stripe (karty, BLIK)
- Email transakcyjny: Resend
- CI/CD: GitHub Actions (testy automatyczne przy każdym PR)

**Bezpieczeństwo**
- HTTPS + HSTS
- Pełna zgodność z RODO / UODO
- Rate limiting na endpointach rejestracji i logowania
- Content Security Policy
- Blokada botów AI (ochrona treści)

---

## Zgodność Prawna

Platforma działa w pełnej zgodności z polskim i europejskim prawem:

- **RODO** — eksport danych, usunięcie konta, zarządzanie zgodami marketingowymi
- **CMP (Cookie Consent)** — granularne zarządzanie cookies z zapisem preferencji
- **Regulamin**, Polityka Prywatności, Warunki dla Korepetytorów, Polityka Cookies — kompletna dokumentacja prawna
- **Prawo odstąpienia od umowy** — widoczne przy każdej rezerwacji zgodnie z ustawą o usługach elektronicznych
- **Obsługa sporów** — wbudowany system reklamacji i zwrotów

---

## Skala Projektu

- **50+ stron** i podstron w aplikacji
- **2 panele użytkownika** (uczeń + korepetytor) z pełną integracją API
- **Panel administracyjny** z narzędziami moderacji, analityki, wypłat i marketingu
- **25 landing page'y** przedmiotowych i miejskich pod SEO
- **Blog edukacyjny** z artykułami dla uczniów i rodziców
- **15+ szablonów email** transakcyjnych (weryfikacja, rezerwacja, przypomnienia, faktury)
- **6 typów minigier** edukacyjnych z edytorem dla nauczycieli
- **Program poleceń (referral)** z kodami i bonusami XP

---

## Status

Platforma jest aktywnie rozwijana i przygotowywana do launchu na rynek polski.

**Kontakt:** kontakt@sprelli.com  
**Strona:** [sprelli.com](https://sprelli.com)

---

*SPRELLI Sp. z o.o. — ul. Marszałkowska 58, 00-545 Warszawa*

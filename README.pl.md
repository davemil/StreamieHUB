<p align="right">
  <a href="README.md">🇬🇧 English</a>
</p>

<p align="center">
  <img src="assets/banner.png" alt="StreamieHUB Banner" width="600" />
</p>

<h1 align="center">StreamieHUB</h1>

<p align="center">
  <strong>Lekka aplikacja desktopowa do streamowania na Twitch, YouTube i Kick</strong><br>
  Alerty, overlaye, chat bot, punkty kanalu, giveawaye, donacje - wszystko w jednej apce.
</p>

<p align="center">
  <a href="https://github.com/dondaiku/StreamieHUB/releases/latest"><img src="https://img.shields.io/github/v/release/dondaiku/StreamieHUB?style=for-the-badge&color=7c3aed" alt="Najnowsza wersja"></a>
  <a href="https://github.com/dondaiku/StreamieHUB/releases"><img src="https://img.shields.io/github/downloads/dondaiku/StreamieHUB/total?style=for-the-badge&color=7c3aed" alt="Pobrania"></a>
  <img src="https://img.shields.io/badge/platforma-Windows-blue?style=for-the-badge" alt="Platforma">
  <img src="https://img.shields.io/badge/licencja-proprietary-gray?style=for-the-badge" alt="Licencja">
</p>

---

## Czym jest StreamieHUB?

StreamieHUB to darmowa, lokalna aplikacja desktopowa dla streamerow - lekka alternatywa dla StreamElements, Streamlabs czy Mix It Up. Wszystko dziala na Twoim PC, bez otwierania przegladarki.

<p align="center">
  <img src="assets/screenshot-dashboard.png" alt="StreamieHUB Dashboard" width="800" />
</p>

## Funkcje

| Modul | Opis |
|-------|------|
| **Alerty** | Powiadomienia wizualne i dzwiekowe na followsy, suby, bitsy, raidy, donacje |
| **Chat Bot** | Wlasne komendy, timery, moderacja - dziala na Twitch, YouTube i Kick |
| **BiBot** | Mapuj bitsy/donacje na akcje - odtwarzaj dzwieki, animacje, naciskaj klawisze |
| **Punkty kanalu** | Wlasna waluta, sklep, redempcje, ranking |
| **Giveaway** | Wejscie slowem kluczowym, kolo fortuny, loteria - losuj na zywo |
| **Death Counter** | Licznik smierci w grach wyswietlany na overlayu |
| **Overlaye** | Alert box, chat, cele, lista eventow - dodaj jako OBS Browser Source |
| **Donacje** | Przyjmuj tipy przez Stripe z wlasna strona donacji |

## Platformy

<p align="center">
  <img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" alt="Twitch">
  <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube">
  <img src="https://img.shields.io/badge/Kick-53FC18?style=for-the-badge&logo=kick&logoColor=black" alt="Kick">
</p>

- **Twitch** - EventSub (suby, bitsy, followsy, raidy) + czat przez tmi.js
- **YouTube** - Live Streaming API (czat, Super Chaty)
- **Kick** - WebSocket API (czat, eventy)

## Instalacja

1. Wejdz w [**Releases**](https://github.com/dondaiku/StreamieHUB/releases/latest)
2. Pobierz `StreamieHUB-Setup-x.x.x.exe`
3. Uruchom instalator - gotowe

> **Wymagania:** Windows 10/11 z WebView2 (preinstalowany na nowoczesnym Windowsie).

## Jak dzialaja overlaye

StreamieHUB uruchamia lokalny serwer na Twoim PC. Dodaj overlaye do OBS jako Browser Source:

```
http://localhost:3200/overlay/alerts
http://localhost:3200/overlay/chat
http://localhost:3200/overlay/goals
http://localhost:3200/overlay/deathcounter
http://localhost:3200/overlay/eventlist
http://localhost:3200/overlay/giveaway
```

Wszystkie overlaye aktualizuja sie w czasie rzeczywistym przez Socket.IO - zero opoznienia.

## Stack technologiczny

- **Desktop:** [Tauri v2](https://v2.tauri.app/) (Rust + WebView2)
- **UI:** React + TypeScript + Tailwind CSS + shadcn/ui
- **Overlaye:** React + Framer Motion (serwowane jako strony localhost)
- **Backend:** Node.js + Socket.IO (komunikacja real-time, integracje platform)
- **Baza danych:** SQLite (lokalna, zero konfiguracji)

## Free vs Pro

StreamieHUB jest **darmowy** z hojnymi limitami. Zaawansowani uzytkownicy moga przejsc na **Pro** po nieograniczone mozliwosci.

| | Free | Pro |
|---|---|---|
| Wszystkie moduly | Tak | Tak |
| Wlasne komendy | 20 | Bez limitu |
| Aktywne overlaye | 3 | Bez limitu |
| Wlasne alerty | 5 | Bez limitu |
| Watermark na overlayach | Tak | Nie |
| Prowizja od donacji | 3% | 1% |
| Szablony premium | - | Tak |
| Priorytetowe wsparcie | - | Tak |

## Zgloszenia bledow i pomysly

Znalazles buga? Masz pomysl na funkcje? Otworz [Issue](https://github.com/dondaiku/StreamieHUB/issues) lub zacznij [Dyskusje](https://github.com/dondaiku/StreamieHUB/discussions).

## Autor

Stworzone przez **DON DAIKU** - [Twitch](https://twitch.tv/dondaiku) | [Twitter/X](https://x.com/dondaiku)

---

<p align="center">
  <sub>StreamieHUB &copy; 2026 DON DAIKU. Wszelkie prawa zastrzezone.</sub>
</p>

<div align="center">

# 🎯 FocusFlow

Osobisty asystent produktywności oparty na technice Pomodoro — zadania, dziennik skupienia, dźwięki ambient i statystyki, wszystko w jednej aplikacji webowej.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3.0-7952B3?logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![Font Awesome](https://img.shields.io/badge/Font%20Awesome-6.4.0-528DD7?logo=fontawesome&logoColor=white)](https://fontawesome.com/)

**[Polski](#-polski) | [English](#-english)**

</div>

---

## 🇵🇱 Polski

### Spis treści
- [O projekcie](#o-projekcie)
- [Funkcje](#funkcje)
- [Stack technologiczny](#stack-technologiczny)
- [Wymagania](#wymagania)
- [Instalacja](#instalacja)
- [Uruchomienie](#uruchomienie)
- [Użycie](#użycie)
- [Struktura projektu](#struktura-projektu)
- [Współtworzenie](#współtworzenie)
- [Licencja](#licencja)
- [Kontakt](#kontakt)

### O projekcie

FocusFlow to lekka, w pełni frontendowa aplikacja webowa, która działa jak osobisty trener produktywności. Zamiast blokować rozpraszacze, wspiera świadome zarządzanie czasem przy pomocy techniki Pomodoro, listy zadań z priorytetami, dziennika skupienia oraz kojących dźwięków w tle. Wszystkie dane (zadania, wpisy dziennika, statystyki, ustawienia timera) są przechowywane lokalnie w przeglądarce (`localStorage`) — bez konieczności logowania czy backendu.

Projekt jest przeznaczony dla każdego, kto chce zwiększyć swoją koncentrację i produktywność podczas pracy lub nauki, korzystając z prostego narzędzia webowego działającego zarówno na desktopie, jak i na smartfonie.

### Funkcje

- ⏱️ **Timer Pomodoro** — konfigurowalne cykle pracy/przerwy z wizualnym licznikiem (kołowy pasek postępu) i dźwiękiem po zakończeniu cyklu.
- ✅ **Lista zadań (To-Do)** — dodawanie, edycja, usuwanie i oznaczanie zadań jako wykonane, z priorytetami (wysoki/średni/niski) i sortowaniem.
- 📓 **Dziennik skupienia** — notatki tekstowe po każdej sesji, z historią wpisów posortowaną wg daty.
- 🎧 **Ambient Sound** — odtwarzacz dźwięków tła (deszcz, fale, kawiarnia, las, ogień, wiatr) z regulacją głośności dla każdego dźwięku niezależnie.
- 📊 **Statystyki** — liczba ukończonych cykli Pomodoro, wykonanych zadań i łączny czas pracy.
- 💾 **Eksport / import danych** — kopia zapasowa wszystkich danych do pliku JSON i możliwość jej przywrócenia.
- 🔔 **Powiadomienia przeglądarkowe** — alerty o końcu cyklu pracy/przerwy (Notification API).
- 📱 **Responsywny interfejs** — układ dostosowany do telefonów, tabletów i desktopów.

### Stack technologiczny

- **HTML5 / CSS3 / JavaScript (Vanilla JS)** — bez frameworków SPA i bez kroku budowania.
- **Bootstrap 5.3.0** (CDN) — layout i komponenty UI.
- **Font Awesome 6.4.0** (CDN) — ikony.
- **Web APIs** — `localStorage` (dane), `Notification API` (powiadomienia), `HTMLAudioElement` (dźwięki ambient).

### Wymagania

- Dowolna nowoczesna przeglądarka (Chrome, Firefox, Edge, Safari).
- Serwer HTTP do serwowania plików statycznych, np. Apache z pakietu **XAMPP** (zalecane, ponieważ projekt znajduje się w `htdocs`), albo dowolny inny lokalny serwer plików statycznych.

### Instalacja

Aplikacja nie wymaga instalacji zależności — to statyczny zestaw plików HTML/CSS/JS.

```bash
# 1. Sklonuj repozytorium do katalogu htdocs XAMPP
git clone https://github.com/MrPrompt24/FocusFlow.git

# 2. Upewnij się, że Apache w XAMPP jest uruchomiony
```

### Uruchomienie

Po uruchomieniu Apache w XAMPP otwórz aplikację w przeglądarce pod adresem:

```
http://localhost/FocusFlow/index.html
```

Alternatywnie plik `index.html` można otworzyć bezpośrednio w przeglądarce (część funkcji, np. powiadomienia, może wymagać serwowania przez `http://`).

### Użycie

1. Ustaw długość cyklu pracy i przerwy w panelu Timera i kliknij **Start**.
2. Dodawaj zadania w zakładce **Zadania**, przypisując im priorytet.
3. Po zakończonej sesji zapisz refleksje w zakładce **Dziennik**.
4. W zakładce **Dźwięki** włącz wybrany dźwięk ambient i dostosuj głośność.
5. W zakładce **Statystyki** śledź postępy oraz eksportuj/importuj kopię zapasową danych.
6. Włącz powiadomienia przeglądarkowe, aby otrzymywać alerty o końcu cyklu.

### Struktura projektu

```
FocusFlow/
├── index.html          # Główny plik aplikacji (timer, zadania, dziennik, dźwięki, statystyki)
├── pomoc.html           # Strona pomocy
├── o-aplikacji.html     # Strona "O aplikacji"
├── sounds/              # Pliki audio dla trybu Ambient Sound
├── FocusFlow.png        # Grafika/logo aplikacji
├── fav.png              # Favicon
├── LICENSE              # Licencja MIT
└── README.md            # Ten plik
```

### Współtworzenie

Pull requesty są mile widziane. W przypadku większych zmian najpierw otwórz issue, aby omówić proponowane zmiany.

### Licencja

Ten projekt jest objęty licencją MIT — zobacz plik [LICENSE](LICENSE).

### Kontakt

Autor: **MrPrompt** — repozytorium: [github.com/MrPrompt24/FocusFlow](https://github.com/MrPrompt24/FocusFlow)

---

## 🇬🇧 English

### Table of Contents
- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Running the App](#running-the-app)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

### About

FocusFlow is a lightweight, fully front-end web application that acts as a personal productivity coach. Instead of blocking distractions, it supports mindful time management through the Pomodoro technique, a priority-based to-do list, a focus journal, and calming ambient sounds. All data (tasks, journal entries, stats, timer settings) is stored locally in the browser (`localStorage`) — no login or backend required.

It's built for anyone who wants to boost their focus and productivity while working or studying, using a simple web tool that works on both desktop and mobile.

### Features

- ⏱️ **Pomodoro Timer** — configurable work/break cycles with a visual circular progress indicator and a completion sound.
- ✅ **To-Do List** — add, edit, delete, and complete tasks, with priority levels (high/medium/low) and sorting.
- 📓 **Focus Journal** — text notes after each session, with a date-sorted entry history.
- 🎧 **Ambient Sound** — background sound player (rain, ocean waves, café, forest, fire, wind) with independent volume control per sound.
- 📊 **Statistics** — completed Pomodoro cycles, completed tasks, and total work time.
- 💾 **Data Export / Import** — back up all data to a JSON file and restore it later.
- 🔔 **Browser Notifications** — alerts when a work/break cycle ends (Notification API).
- 📱 **Responsive UI** — layout adapted for phones, tablets, and desktops.

### Tech Stack

- **HTML5 / CSS3 / Vanilla JavaScript** — no SPA framework, no build step.
- **Bootstrap 5.3.0** (CDN) — layout and UI components.
- **Font Awesome 6.4.0** (CDN) — icons.
- **Web APIs** — `localStorage` (data), `Notification API` (alerts), `HTMLAudioElement` (ambient sounds).

### Requirements

- Any modern browser (Chrome, Firefox, Edge, Safari).
- An HTTP server to serve static files, e.g. Apache from the **XAMPP** stack (recommended, since the project lives in `htdocs`), or any other local static file server.

### Installation

No dependency installation is required — this is a static HTML/CSS/JS bundle.

```bash
# 1. Clone the repository into your XAMPP htdocs folder
git clone https://github.com/MrPrompt24/FocusFlow.git

# 2. Make sure Apache is running in XAMPP
```

### Running the App

With Apache running in XAMPP, open the app in your browser at:

```
http://localhost/FocusFlow/index.html
```

Alternatively, `index.html` can be opened directly in a browser (some features, like notifications, may require serving over `http://`).

### Usage

1. Set the work/break cycle length in the Timer panel and click **Start**.
2. Add tasks in the **Tasks** tab, assigning a priority to each one.
3. After a session, write your reflections in the **Journal** tab.
4. In the **Sounds** tab, turn on an ambient sound and adjust its volume.
5. In the **Stats** tab, track your progress and export/import a data backup.
6. Enable browser notifications to get alerts when a cycle ends.

### Project Structure

```
FocusFlow/
├── index.html          # Main app file (timer, tasks, journal, sounds, stats)
├── pomoc.html           # Help page
├── o-aplikacji.html     # "About" page
├── sounds/              # Audio files for Ambient Sound mode
├── FocusFlow.png        # App artwork/logo
├── fav.png              # Favicon
├── LICENSE              # MIT License
└── README.md            # This file
```

### Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

### License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

### Contact

Author: **MrPrompt** — repository: [github.com/MrPrompt24/FocusFlow](https://github.com/MrPrompt24/FocusFlow)

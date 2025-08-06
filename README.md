# CRON → Proxmox Schedule Converter (English)

A modern, user-friendly converter from CRON expressions to Proxmox schedules (systemd calendar events), fully compliant with the official [Proxmox Calendar Events documentation](https://pve.proxmox.com/wiki/Calendar_Events).

## Features

- **Convert CRON (5 fields) to Proxmox/systemd calendar event format**
- **Modern, responsive UI** (gradients, cards, icons, copy buttons)
- **Popular backup schedules** – ready-to-use, clickable examples
- **User-friendly UX** – hints, validation, error handling
- **Easy result copying**

## Demo

![Screenshot](demo.png)

## Popular backup schedule examples

| CRON                | Description                                 |
|---------------------|---------------------------------------------|
| `0 2 * * *`         | Every day at 2:00 AM                        |
| `0 3 * * 0`         | Every Sunday at 3:00 AM                     |
| `0 */4 * * *`       | Every 4 hours, every day                    |
| `0 1 1 * *`         | First day of the month at 1:00 AM           |
| `0 23 * * 1-5`      | Monday to Friday at 11:00 PM                |
| `*/15 8-18 * * 1-5` | Every 15 minutes during work hours (Mon-Fri) |
| `0 0 * * 6,0`       | Weekends at midnight                        |
| `0 0 1 1 *`         | Once a year, January 1st at midnight        |

## How to use?

1. Open the `cron2proxmox.html` file in your browser (no backend or installation required).
2. Enter a CRON expression (5 fields) or select an example from the list.
3. Click **Generate** – you'll get a Proxmox schedule ready to use.
4. Copy the generated expression with a single click.

## Example usage

- **CRON:** `*/15 8-9 * * 1-5`
- **Proxmox:** `mon..fri 8..9:0/15`

- **CRON:** `0 8-16/2 * * *`
- **Proxmox:** `8,10,12,14,16:0`

## Compatibility

- Supports typical CRON cases, ranges, steps, lists, weekdays, months.
- Output is compatible with [systemd calendar events](https://man7.org/linux/man-pages/man7/systemd.time.7.html) and Proxmox documentation.

## Inspiration

Project inspired by the needs of IT administrators and Proxmox documentation.

## License

Public Domain – free for any use.

---

# CRON → Proxmox Schedule Converter (Polski)

Nowoczesny, wygodny konwerter wyrażeń CRON na harmonogramy Proxmox (systemd calendar events), zgodny z dokumentacją Proxmox: [Proxmox Calendar Events](https://pve.proxmox.com/wiki/Calendar_Events).

## Funkcje

- **Konwersja CRON (5 pól) na format Proxmox/systemd calendar event**
- **Nowoczesny, responsywny interfejs** (gradienty, karty, ikony, przyciski kopiowania)
- **Popularne harmonogramy backupów** – gotowe przykłady do kliknięcia
- **Przyjazny UX** – podpowiedzi, walidacja, obsługa błędów
- **Łatwe kopiowanie wyniku**

## Demo

![Zrzut ekranu](demo.png)

## Przykłady popularnych harmonogramów backupów

| CRON                | Opis                                      |
|---------------------|--------------------------------------------|
| `0 2 * * *`         | Codziennie o 2:00 w nocy                   |
| `0 3 * * 0`         | W każdą niedzielę o 3:00                   |
| `0 */4 * * *`       | Co 4 godziny, codziennie                   |
| `0 1 1 * *`         | Pierwszego dnia miesiąca o 1:00            |
| `0 23 * * 1-5`      | Od poniedziałku do piątku o 23:00          |
| `*/15 8-18 * * 1-5` | Co 15 minut w godzinach pracy (pon-pt)     |
| `0 0 * * 6,0`       | W weekendy o północy                       |
| `0 0 1 1 *`         | Raz w roku, 1 stycznia o północy           |

## Jak używać?

1. Otwórz plik `cron2proxmox.html` w przeglądarce (nie wymaga backendu ani instalacji).
2. Wprowadź wyrażenie CRON (5 pól) lub wybierz przykład z listy.
3. Kliknij **Generuj** – otrzymasz harmonogram Proxmox gotowy do użycia.
4. Skopiuj wygenerowane wyrażenie jednym kliknięciem.

## Przykładowe użycie

- **CRON:** `*/15 8-9 * * 1-5`
- **Proxmox:** `mon..fri 8..9:0/15`

- **CRON:** `0 8-16/2 * * *`
- **Proxmox:** `8,10,12,14,16:0`

## Zgodność

- Obsługuje typowe przypadki CRON, zakresy, kroki, listy, dni tygodnia, miesiące.
- Wynik jest zgodny z [systemd calendar events](https://man7.org/linux/man-pages/man7/systemd.time.7.html) i dokumentacją Proxmox.

## Inspiracja

Projekt inspirowany potrzebami administratorów IT oraz dokumentacją Proxmox.

## Licencja

Domena publiczna – do dowolnego użytku.

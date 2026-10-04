[English](README.md) · **Polski**

# bartz-kancelaria.pl

Strona internetowa jednoosobowej kancelarii w Płocku. Projekt, wykonanie
i opieka: Witold Woźniak.

**[bartz-kancelaria.pl →](https://bartz-kancelaria.pl)**

| Czerwiec 2025 | Październik 2026 |
| --- | --- |
| ![Strona w czerwcu 2025](screenshots/before-desktop.jpg) | ![Strona w październiku 2026](screenshots/after-desktop.jpg) |

## Zadanie

Klientką jest moja mama. Justyna Bartz jest radcą prawnym i stałą mediatorką
z listy Prezesa Sądu Okręgowego w Płocku. Przez dziesięć lat orzekała jako
sędzia, a w 2008 roku otworzyła własną kancelarię.

Strona ma dwóch czytelników:

- **Ktoś w kłopocie.** Rozwód, śmierć bliskiej osoby, spór. Często pierwszy
  raz u prawnika, czyta z telefonu, wieczorem. Strona ma jedno zadanie: żeby
  zadzwonił albo napisał.
- **Instytucja**, która sprawdza kancelarię przed podpisaniem umowy. Ma
  zobaczyć poważną kancelarię.

Mój pierwszy nagłówek odrzuciła jako „bardziej coach niż radca” i miała rację:
żadnego słowa w nim nie dało się sprawdzić. Stąd zasada dla każdego zdania na
stronie: zostaje tylko, jeśli da się sprawdzić, że jest prawdziwe. Żadnych
haseł, żadnych obietnic wyniku. Tego samego wymaga etyka zawodowa.

## Co z tego wyszło

- **Zero JavaScriptu.** Dwadzieścia stron czystego HTML-a i jeden arkusz
  stylów. Nic się nie doładowuje, nic się nie psuje, nic nie śledzi.
- **Czytelna dla każdego.** Kontrast tekstu spełnia WCAG AAA (7:1). Każda
  strona przechodzi automatyczny test dostępności przy każdej zmianie, a błąd
  oznacza czerwony build.
- **Dokumenty mediacyjne online.** Osiem dokumentów, których używa
  w mediacjach. Każdy jako strona z wypełnionym przykładem i PDF do druku,
  powstały z tego samego tekstu. Cztery z tych PDF-ów to formularze do
  wypełnienia na komputerze.
- **Bez ciasteczek, bez śledzenia.** Czcionki są na naszym serwerze, a mapa
  jest narysowana z danych OpenStreetMap i podana jako zwykły obrazek, więc
  żadne dane odwiedzających nie trafiają do Google. Polityka prywatności może
  to uczciwie napisać.
- **Lekka.** Około 300 kB na stronę, głównie dwa kroje pisma.
- **Tania w utrzymaniu.** Przy zmianie treści nie muszę nawet zaglądać do
  kodu: mówię agentowi AI, co zmienić, testy to sprawdzają i gotowe. Nowa cena
  czy numer telefonu to kilka sekund mojej pracy.

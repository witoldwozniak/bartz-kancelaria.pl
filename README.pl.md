[English](README.md) · **Polski**

# bartz-kancelaria.pl

Strona internetowa Kancelarii Radcy Prawnego Justyny Bartz, jednoosobowej
kancelarii w Płocku. Projekt, wykonanie i utrzymanie: Witold Woźniak.

**[bartz-kancelaria.pl →](https://bartz-kancelaria.pl)**

| Czerwiec 2025 | Październik 2026 |
| --- | --- |
| ![Strona w czerwcu 2025](screenshots/before-desktop.jpg) | ![Strona w październiku 2026](screenshots/after-desktop.jpg) |

## Zadanie

Klientką jest moja mama, Justyna Bartz: radca prawny i stała mediatorka z listy
Prezesa Sądu Okręgowego w Płocku. Przez dziesięć lat orzekała jako sędzia, a od
2008 roku prowadzi własną kancelarię.

Strona ma dwóch odbiorców:

- **Klient indywidualny**, często pierwszy raz u prawnika, w sprawie rozwodu,
  spadku albo sporu, zwykle czytający na telefonie. Strona ma mu ułatwić
  telefon albo wiadomość.
- **Instytucja**, która sprawdza kancelarię przed podpisaniem umowy. Dla niej
  strona ma przedstawić wiarygodną, profesjonalną kancelarię.

Każde zdanie na stronie musi dać się sprawdzić. Strona nie obiecuje wyników
i nie używa haseł reklamowych, zgodnie z zasadami etyki radcy prawnego.

## Rezultaty

- **Bez JavaScriptu.** Dwadzieścia stron statycznego HTML-a i jeden arkusz
  stylów.
- **Dostępność.** Kontrast tekstu spełnia WCAG AAA (7:1).
- **Dokumenty mediacyjne.** Osiem dokumentów używanych w jej mediacjach. Każdy
  jest opublikowany jako strona z wypełnionym przykładem i jako PDF do druku,
  generowany z tego samego źródła. Cztery z tych PDF-ów to formularze do
  wypełnienia na komputerze.
- **Prywatność.** Bez ciasteczek i bez śledzenia. Czcionki są serwowane razem
  ze stroną, a mapa jest narysowana z danych OpenStreetMap i podana jako
  statyczny obraz. Strony nie pobierają niczego z innych domen.
- **Waga.** Około 300 kB na stronę, w większości czcionki.
- **Testy.** Przy każdej zmianie zestaw testów end-to-end sprawdza wszystkie
  dwadzieścia stron: dostępność, treść, nawigację, metadane SEO i pliki PDF.
- **Utrzymanie.** Zmiany treści nie wymagają otwierania kodu: edycję
  wprowadza agent AI, a testy ją weryfikują. Zmiana numeru telefonu czy
  jednego zdania zajmuje kilka sekund.

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
- **Utrzymanie.** Klientka nie chciała sama zarządzać stroną, więc nie ma
  panelu administracyjnego; stronę utrzymuję ja. Zmiany treści nie wymagają
  otwierania kodu: edycję wprowadza agent AI, a testy ją weryfikują. Zmiana
  numeru telefonu czy jednego zdania zajmuje kilka sekund.

## Przebieg

- **Punkt wyjścia.** Poprzednią stronę (wyżej, czerwiec 2025) wykonała inna
  firma, w pakiecie z abonamentem na hosting i utrzymanie, który kosztował
  więcej, niż strona wymagała. Zaproponowałem nowy projekt i rezygnację z tego
  abonamentu.
- **Brief.** Wywiad projektowy w lipcu 2026 roku określił dwóch odbiorców, ton
  i listę rzeczy, których na stronie nie będzie: Temidy, młotków, zdjęć
  stockowych, obietnic wyniku ani wyskakujących okien.
- **Projekt i teksty.** Klientka dała mi pełną swobodę w projekcie
  i w większości tekstów. Jej własne teksty ze starej strony zostały, poprawiona jest tylko
  typografia.
- **Akceptacja.** Nowe teksty omówiliśmy zdanie po zdaniu. Ostateczne
  brzmienie, z jej poprawkami, zatwierdziła we wrześniu 2026 roku. Do tego
  czasu podgląd strony był dostępny tylko po zalogowaniu.
- **Hosting.** Strona tymczasowo działa bezpłatnie na Cloudflare Pages.
  Domena, hosting i poczta przechodzą do jednego dostawcy, tańszego i z lepszym
  wsparciem.

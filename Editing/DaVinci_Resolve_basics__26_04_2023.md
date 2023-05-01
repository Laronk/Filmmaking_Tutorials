# DaVinci Resolve basics, 26.04.2023

## 1. Baza danych i pliki projektu

* Resolve ma bezę danych projektów.
* Bazy danych mogą być zapisane na nośnikach zewnętrznych, ale nośniki z exFAT źle działają.
* Nie ma pojedyńczych plików projektowych zapisanych jak w Premiere.

---

## 2. Zakładki

* Media - importowanie folderów / plików
* Cut - szybka edycja (pomijalne)
* Edit - standardowa edycja
* Fusion - efekty specjalne
* Fairlight od audio, można głośność tracków zmieniać, dodaje efekty jak  Voice Isolation, tu jest EQ
* Delivery - tu ustawiamy In/Out range, format: MP4, Quality: Restrict to 40 000 (dla 4K), 15 000 (FHD)

---

## 3. Framerate timeline-u

ustawiany na stałe przy jego tworzeniu. Ustawiamy fps jak w nagraniach, które będziemy edytować, lub ich wielokrotność.

---

## 4. Inspector klipów

w prawym górnym rogu.

---

## 5. Dynamic zoom

zoom, ramki do ustawienia wielkości

---

## 6. Stabilizacja

“stability” jest ok

---

## 7. Selekcja

Dwa kliknięcia na klip w media pool otwiera klip w podglądzie, po zaznaczeniu Input i Output przerzucamy klikając “insert” (F9 jest domyślnie, 0 też wygodne)

---

## 8. Narzędzia - skróty klawiszowe

* B - Razer
* Ctrl/Command+B - cięcie na głowicy
* D - zmienia widoczność klipu
* Alt/Option+Y (A w premiere) - odznaczanie ścieżek ma tu wpływ

---

## 9. Dip to black/white

Uzyskujemy poprzez zaczemy na końcach klipów.
W analogiczny sposób fade na audio.

---

## 10. Nest-owanie

Nest z premiere w DaVinci nazywa się coumpound clip.

---

## 11. Color

Nie koloruje się adjustment layers, lecz całe klipy w zakładce Colors.

Pracujemy na węzłach (nodes).

Drzewko przepływu zmian od lewej do prawej.
Kolorowanie zależy od materiału z konkretnej kamery,

Alt/Option+S - dodaj nowy node

**Mateusz poleca taką kolejność:**

    I. NR - Redukcja szumów (Temporal NR: Frames 1, better, wartości ok 12) <— zamula gdy jest włączona, więc na czas montażu wyłączamy 


    II. WB - Balans bieli - odpowiada za to czy żółty czy niebieski obraz - Ustawić scopes na Vectorscope, show… i dociągnąć Offset, żeby plama była na środku


    III. EXP - Ekspozycja - ciemniej/jaśniej:
    (Primaries - Color Wheels: Lift - rozjaśnia ciemne elementy (tony 0-20), Gamma odpowiada za midtones (20-70), Gain tones powyżej 70, Offset - balans bieli poprawia 


    IV. CONT - Kontrast - suwaczek lub na krzywej “curves” i robić słynną S 


    V. SAT - saturacja - suwaczek (do 50-60), gdy konkretny kolor chcemy podrasować to w krzywych
    

    VI. LUT/CST - profil kolorystyczny, który narzucamy

    VII. SHARP - wyostrzenie - ikonka kropelki, i suwaczek do 48 max

Można dodać node, zrobić maskę po kształcie, itd,

Można dodać node, zrobić maskę po kolorze, itd.

Node się wyłącza i włącza Ctrl/Command.

Node’y można kopiować z kipu na klip. !!! UWAGA KOPIUJE STABILZACJĘ TEŻ !!!

Można klikać na obraz i robić “grab still” i rzucić na inne klipy.

Można wyłączyć efekty kolorowania dla płynnego podglądu - tęczowe kółeczko nad obrazem.

---

## 12. POCKET + DaVinci Resolve

1. Wrzucić “Color space transform” z efektów i wybrać pocketowe ustawienia

Gallery - drugi przycisk myszy - preserver camera raw settings gdy z pocketa psuje balans bieli

---

1. Po pobraniu programu

warto w ustawieniach parę rzeczy zrobić:

* Master settings:

  * UHD można ustawić jako domyślne jak w 4k zazwyczaj montujemy

  * 25 fps

* Color Management:

  * Color science: DaVinci YRGB

  * Timeline Color space - Rec709A dla Mac’ów!

---

## 13. Przenoszenie projektu

File > Export Project jako … > .drp

można wyeksportować sobie na MINEowych Macach

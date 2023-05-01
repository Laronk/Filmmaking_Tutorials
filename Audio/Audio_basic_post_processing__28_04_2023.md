# Szkolenie z dźwięku - Bartek Bieżca, 28.04.2023

## Czym jest dźwięk

* fala akustyczna
* sygnał ciągły analogowy - przy nagrywaniu audio
* sygnał cyfrowy - przetwarzanie audio (sygnał dyskretny, próbkowania)

---

## Zapis cyfrowy dźwięku

### Charakterystyka

* Częstotliwość próbkowania (48 kHz)
  * im więcej, tym lepiej
  * ilość informacji w nagraniu

* Rozdzielczość bitowa (najczęściej pracujemy na 24 bit lub 32 bit)

---

## Waveform - adobe audition

### skala w dB (Decybele)

* skala logarytmiczna
* wyskalowana do zera (> 0 przester, utrata informacji najgłośniejszych)
* przesterowane audio jest nie do uratowania (nie ma informacji)

### Analiza częstotliwościowa

* wykonywane przez transformatę foriera
* pokazuje częstotliwości i ich ilość / udział (głośność) w nagraniu

### Szum

* noise floor
* nie istnieją urządzenia bez szumu
* unikać jak ognia (moża dodać w post produkcji jeśli trzeba)

---

## Post processig audio

### kompresja

* dokładanie saturacji sygnału
* wycinanie częstotliwości
* "podbijanie" częstotliwości

### filtracja - Eqalizer

* zakres słyszalny dla człowieka (teoretyczny): 20 kHz - 20 000 kHz
* kształtowanie barwy głosu

### procesory dynamiczne

* rozpiętość dynamiczna - przedział głośności danego audio
* kompresor - zmiana różnic między najcichszym i najgłośniejszym dźwiękiem (wpływa na barwę głosu)

---
---

## **Program do obróbki audio - adobe audition**

* tryb multitrack - tryb pracy w sesji
* sesja - plik projektowy
* ślad - audio na ścieżce

### Tryb wave form

* selekcja audio
* przygotowanie materiału do pracy
* praca destruktywna - nadpisuje plik audio
* skalowanie głośności nie jest destruktywne o ile nie ma przesteru

### Tryb multitrack

### Tools

* V - move
* R - żyletka
* Shift+E - usuwanie pustych kanałów
* zaznaczanie i loopback (zapętlanie - odtwarzanie w pętli)
* Ctrl+Shift+D - wygodne przemapowanie narzędzia "Silence" - wklejenie zer (brak wartości - cisza bez szumu) w zaznaczenie

### Track effects - efekty na samych ścieżkach

* transformacja informacji audio - efekty
* processig szeregowy
* kolejność załączonych efektów ma znaczenie

### Clip effects (efekt samego klipu)

### Struktura folderów tworzona przez audition

* Backup - stany sesji
* Imported Files - pliki zaimportowane
* Merged Files

### Organizacja pracy

* dodatkowy folder "Raw" - backup surowych plików audio
* nazywanie ścieżek (Lektor, Aktor_1, Aktor_2, Muzyka_1, etc.)
* kolorowanie ścieżek
* fade-in i fade-ot na śladach

---

## **Workflow - lektor**

Selekcja

* stworzenie nowej sesji (stereo, 24bit)
* wycięcie (wyciszenie oddechów)
* wybranie take-ów
* eliminacja niechcianych pomyłek etc.

Edycja

1. Hard limiter (konkretny kompresor z ratio dążącym do nieskońsczoności)
   * -1:-1.5 dB
2. De-ess (2 slidery)
3. Kompresja dynamiczna
4. Parametric eqalizer - zestaw filtrów (kształtowanie barwy głosu)
   * Low cut / High pass (filtr zaporowy)
   * Band pass (wybiórcza częstotliwość)
   * Shelf (półka)
   * High cut / Low pass (filtr zaporowy)

### Efekt track

#### Dynamics

* **Kompresor**
  * **ratio** - ratio przyciszenia (1 - nie przycisza)
  * **tresold** - poziom od którego przyciszamy
  * attack - bardziej zaawansowane
  * release - bardziej zaawansowane
  * makeup - kompensacja zmniejszonej głośności przez kompresor (do wysłyszenia)

---

### Przedziały (logiczne - prostota identyfikacji) dźwięku słyszalnego

1. < 500
2. \> 500 < 2000
3. \> 2500

---

### Skala Lufs-owa (niższe częstotliwści są postrzegalnie głośniejsze dla ludzkiego ucha)

* -19:-16 LUFS - **lektor**
* -14 LUFS - **muzka**

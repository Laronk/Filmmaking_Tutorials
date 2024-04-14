# Jak zrealizować streama 101

## 1. Wymyślić cel streama

np. studio pogodowe

## 2. Zapotrzebowanie na ludzi

obstawa streama

* Realizator audio
* Realizator video
* Stage hand
* Operatorzy kamer
* Reżyser (na małych produkcjach można bez)
* Scenografia - team

## 3. Ogólne potrzeby

* Przygotować hosta - komputer spinający wszystko razem

* Dużo ekranów - co najmniej 3 dla komfortowej pracy

## 4. Połączenie urządzeń

* PC Host - wszystko do konfiguracji streama
* VMix - mixer audio/video (funkcje podobne do ATM-a), łatwiej robić audio i overlay-e, streamowanie do wielu platform naraz

* PC Host (VMix) <- USB -> ATM-8
* Wyjście ATM <- HDMI -> Monitor gółwny poglądowy ("Multiview")
* PC Host (VMix) <- USB -> Audio mixer
* Kamery <- HDMI/SDI -> ATM
* Mixer Audio <- ETH -> Router (Sieć z PC Host)

## 5. Konfiguiracja urządzeń

### 1. Konfiguracja ATM-a

   1.1. "General" ATM wprowadza opuźnienie urządzeń input

   1.2. "Audio" Ustwaiwamy standard rozdzielczości video kamer

   1.3. "Multiview" Można ustawić standard audio, ale lepiej puścić to przez dedykowany mixer

   1.4. "Labels" Ustawienie wedle potrzeby

   1.5. Ustawienie kluczowania koloru

    Panel konfiguracyjny -> Properties -> Upstream Key -> Gamma

   1.6. Ustawienie klucza transmisyjnego do streamu 

    Panel konfiguracyjny -> Output -> Live Stream -> Key

   1.7. Stills - stałe klatki

    Ustawiamy zdjęcia i grafiki (nie video) do pokzaywania na streamie. Dobre miejsce do ustawienia żródeł do kluczowania.

### 2. Konfiguracja Mixera X-Air

 2.1. Skonfigurować wyjścia i wejścia audio

    Main - L/R 

 2.2. Ponazywać szyny audio (dla komfortu i szybkości pracy)

### 3. Konfiguracja VMix-a

 3.1. Konfiguracja ścieżek dźwiękowych
 
    Settings -> Audio Outputs

 3.2. Konfiguracja opuźnienia audio

    Audio jest przetwarzane z regóły szybciej niż video, więc należy je opuźnić przed rozpoczęciem transmisji.

 3.3. Konfiguracja outputu streama pod różne platformy

* Facebook - 128kbps, Full HD 6Mb/s

## 6. VMix

* VMix - darmowy 60-dniowy trial, lub 50 dolarów / miesiąc subskrypcja premium

* Ustawienie paneli video: po lewej "Preview", po prawej "Program".

* Po lewej stronie na dole okna są wszystkie wejścia (media, kamery, etc.) z jakich będziemy korzystać.
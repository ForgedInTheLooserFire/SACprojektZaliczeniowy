PODZIAŁ PROJEKTU NA 2 OSOBY (OPCJA A – xdotool)

OSOBA 1 — ATAK (BadUSB – symulacja HID)



„Jak wygląda atak i dlaczego jest groźny”



Zakres odpowiedzialności:



Ta osoba udowadnia, że atak jest możliwy.



Co dokładnie robi:

1️⃣ Przygotowanie środowiska



VM z Linuxem (ofiara)



instalacja xdotool



2️⃣ Symulacja BadUSB (ATAK)



payloady typu:



xdotool type "BadUSB simulation works"



xdotool key ctrl+alt+t

xdotool type "whoami"

xdotool key Return

//jakiś wirus można wymyslić



3️⃣ Pokazanie cech BadUSB



bardzo szybkie wpisywanie

brak interakcji użytkownika

automatyczne skróty klawiszowe



4️⃣ Dokumentacja



screeny „przed / po”



opis payloadu



wniosek: system ufa HID bez weryfikacji



📝 Jak OSOBA 1 pisze w sprawozdaniu:



„Część atakująca projektu skupiała się na symulacji zachowania urządzenia BadUSB poprzez emulację klawiatury HID. Wykazano możliwość automatycznego wykonywania poleceń bez wiedzy użytkownika.”



OSOBA 2 — OBRONA



„Jak to wykryć, ograniczyć lub zablokować”



Zakres odpowiedzialności:



Ta osoba pokazuje, że system da się zabezpieczyć.



Co dokładnie robisz:

1️⃣ Analiza zagrożenia



dlaczego HID jest zaufany



dlaczego BadUSB jest trudny do wykrycia



porównanie: człowiek vs HID



2️⃣ Obrona — DETEKCJA



Skupiasz się na:



nieludzkiej szybkości wpisywania



sekwencjach skrótów (CTRL+ALT+T)



braku aktywności myszy



opisujesz mechanizm



podajesz scenariusze wykrycia



3️⃣ Obrona — PREWENCJA



Opisujesz:



USBGuard (whitelist HID)



blokadę nowych klawiatur



polityki użytkownika (least privilege)



4️⃣ Obrona — OGRANICZENIE SKUTKÓW



brak auto-login



brak sudo



brak autostartu



📝 Jak TY piszesz w sprawozdaniu:



„Część obronna projektu koncentruje się na wykrywaniu i ograniczaniu skutków ataku BadUSB poprzez analizę zachowania wejścia HID oraz mechanizmy kontroli urządzeń USB.”



JAK TO POŁĄCZYĆ W JEDEN PROJEKT

STRUKTURA SPRAWOZDANIA (IDEALNA)



1️⃣ Wstęp

– czym jest BadUSB



2️⃣ Część atakująca (OSOBA 1)

– symulacja HID

– payloady

– efekty



3️⃣ Część obronna (OSOBA 2)

– detekcja

– prewencja

– ograniczenie skutków



4️⃣ Analiza porównawcza

– dlaczego obrona jest trudna

– trade-off security vs usability



5️⃣ Wnioski


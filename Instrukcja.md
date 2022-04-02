# Gwiezdni_Zule_Dla-Linuxa
Witaj w Instrukcji Instalacji Gwiezdnych Żuli Na linuxie! Jest to cięższe niż na innych systemach ale dasz sobie radę jeżeli będziesz postępował krok po kroku z naszymi instukcjami!

1. Pobierz wszystkie pliki z tego repozytorium (możesz pominąć Instrukcje)
2. Zainstaluj Wine:
Preferowany sposób instalacji Wine na komputerze z systemem Linux to strona internetowa WineHQ . Oferuje prosty proces 
do naśladowania i rezygnuje z wielu bardziej złożonych kroków, które w innym przypadku mogłyby być związane z innymi metodami.
Instrukcje instalacji dla Mint / Ubuntu można znaleźć na ich stronie wiki pod adresem: https://wiki.winehq.org/Ubuntu
3. Postępujmy zgodnie z prostymi krokami wymienionymi tam pod nagłówkiem „Instalowanie pakietów WineHQ”.
Będziemy musieli uruchomić wiersze kodu, które widzimy w szarych polach pojedynczo, używając terminala. Jeśli znasz wiersz poleceń w systemie Windows,
terminal w systemie Linux jest podobny. W Mint możesz znaleźć Terminal w sekcji „Administracja” w menu głównym lub w sekcji „Wszystkie aplikacje”. Lub możesz 
otworzyć okno terminala, używając domyślnego skrótu klawiaturowego: CTRL + ALT + T w dowolnym momencie.
Jeśli nie masz żadnego doświadczenia z tego rodzaju rzeczami, to w porządku. Wszystko, co musimy zrobić, to dokładnie powtórzyć to, co jest pokazane 
na stronie wiki WineHQ i zadziała. Możesz wpisać go ręcznie w terminalu podczas odwoływania się do strony internetowej, ale ta metoda jest podatna na 
błędy wynikające z błędnego wpisania.
Bardziej niezawodnym sposobem jest użycie funkcji kopiowania i wklejania na komputerze. Zwykle możesz to zrobić za pomocą poleceń klawiaturowych CTRL + C
(kopiuj) i CTRL + V (wklej) , ale w terminalu te skróty klawiaturowe pełnią zupełnie inne funkcje, więc zamiast tego będziesz chciał skorzystać z menu prawego
przycisku myszy do kopiowania i wklejania do okna terminala.
Po otwarciu strony wiki WineHQ i przygotowaniu okna terminala skopiujemy i wkleimy zawartość w szarych polach, a następnie wykonamy kod po jednej linii na raz. 
Będziesz musiał mieć uprawnienia administratora, aby wprowadzić te zmiany na swoim komputerze, więc podczas wykonywania tych czynności zostaniesz poproszony o podanie hasła. Będziesz także potrzebować dostępu do Internetu, aby pobrać niezbędne pliki.
Zacznij więc od skopiowania linii z pierwszego szarego pola:
sudo dpkg - add-architecture i386
Wklej tę linię do terminala za pomocą menu prawego przycisku myszy, a następnie naciśnij klawisz Enter, aby uruchomić tę linię kodu. Wprowadź hasło administratora 
po monicie i naciśnij klawisz Enter, aby potwierdzić.
Po zakończeniu ponownie zobaczysz ten sam pusty monit, który widziałeś na początku podczas pierwszego otwierania terminala, i dzięki temu wiesz, że jest gotowy do 
wprowadzenia następnego wiersza.
Następnie skopiuj i wklej następujący wiersz samodzielnie do terminala:
wget -nc https://dl.winehq.org/wine-builds/winehq.key
I tak jak poprzednio, naciśnij Enter, aby go uruchomić. Po zakończeniu tego kroku powtórz proces z następną linią w dół:
sudo apt-key add winehq.key
I ponownie naciśnij klawisz Enter. Jeśli w dowolnym momencie komputer poprosi o potwierdzenie wprowadzonych zmian, naciskając klawisz T / N, po prostu naciśnij
klawisz Y i ponownie naciśnij klawisz Enter, aby kontynuować proces instalacji.
W następnym zestawie pól, w których jest napisane „Dodaj repozytorium”, wystarczy uruchomić tylko jeden wiersz odpowiadający używanej wersji Linuksa.
Na przykład, jeśli jest to Ubuntu 18.04 lub Linux Mint 19.x (w tym przypadku x może wynosić 1, 2 lub 3), chcesz uruchomić wiersz w polu „Użyj tego polecenia:”,
który odpowiada temu, be: sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ bionic main' dla tych wersji odpowiednich systemów operacyjnych.
Jeśli nie masz pewności, którego numeru wersji Linuksa używasz, w Linux Mint możesz znaleźć te informacje, przechodząc do menu głównego i pod „Preferencjami”
wybierając aplikację „Informacje o systemie”. W wyświetlonym oknie pojawi się nazwa i wersja systemu operacyjnego. Może nie wyświetlać numeru .x po przecinku w Linux Mint, ale po prostu użyj odpowiedniego głównego numeru wersji. Więc Linux Mint 19 użyłby repozytorium 19.x, a dla Linux Mint 20, 20.x byłoby tym, którego chcesz użyć.
Po dodaniu repozytorium dla twojej wersji systemu operacyjnego, następnie będziesz chciał uruchomić wiersz:
sudo apt update
Po zakończeniu tego procesu ostatnim krokiem na stronie wiki WineHQ jest informacja o instalacji „jednego z poniższych pakietów”. Zalecałbym używanie „Oddziału 
stabilnego”, aby uzyskać najbardziej wiarygodne ogólne wrażenia.
To wszystko, czego potrzebujesz do podstawowych kroków instalacji Wine. Powinien zostać zainstalowany w tym momencie, jeśli wszystko poszło dobrze i możesz 
bezpiecznie zamknąć okno terminala. Teraz będziesz chciał pobrać plik .exe , który uruchamia oprogramowanie Windows, które próbujesz uruchomić.

[Caly punkt 3 jest opisany w artykule nie napisanym przeze mnie: https://ichi.pro/pl/jak-grac-w-gry-rpg-maker-w-systemie-linux-przy-uzyciu-wine-23587095084547]

4. Za pomocą programu Wine uruchom Grę na Linuxie!

System organizacji wydarze� 

1. Opis projektu:

Projekt System organizacji i  wydarze�  ma na celu stworzenie platformy, kt�ra pozwala u�ytkownikom przegl�da� wydarzenia, tworzy�, edytowa� i usuwa� nowe wydarzenia, a tak�e list� go�ci, kt�ra pokazuje, kto mo�e uczestniczy� w wydarzeniach. 

*Funkcje
-Tworzenie nowych wydarze�
-Edycja szczeg��w wydarzenia
-Zapraszanie go�ci
-Monitorowanie post�pu wydarzenia
-Usuwanie organizacji zdarze�

2. Rejestracja i autoryzacja:

Nowi u�ytkownicy b�d� mogli za�o�y� konto,Zalogowani u�ytkownicy b�d� r�wnie� mogli tworzy� wydarzenia i organizacje, dodawa� daty, listy go�ci, edytowa� i usuwa� je, wprowadzaj�c swoje dane.

3.Dodaj now� organizacj� i wydarzenie:

Zarejestrowani u�ytkownicy mog� doda� nowe wydarzenie i organizacj�.Dodawanie organizacji i wydarzenia, nazwy wydarzenia, daty wydarzenia i listy go�ci.

4.Edytowa� i usuwa� organizacje i wydarzenia :

Zarejestrowani u�ytkownicy b�d� mogli modyfikowa� i usuwa� zaplanowane wydarzenia.Zmienia�, aktualizowa� i ca�kowicie usuwa� dane organizacji i wydarze�.

5.Przegl�danie wydarze� i organizacji :

Przegl�da� wydarzenia i organizacje, u�ytkownicy b�d� mogli przegl�da� zaplanowane wydarzenia.

W skr�cie System i  organizacji wydarze� pozwala u�ytkownikom tworzy�, usuwa�, zarz�dza� i monitorowa� r�ne wydarzenia. U�ytkownicy mog� zaprasza� go�ci i �ledzi� ich udzia�.

6.U�yte technologie:

app.js
Jest to g��wny punkt wej�cia aplikacji. Konfiguruje serwer Express, ��czy si� z baz� danych MongoDB za pomoc� Mongoose.

user.js
Definiuje schemat danych u�ytkownika w MongoDB przy u�yciu Mongoose. 

event.js
Definiuje schemat danych zdarze� w MongoDB przy u�yciu Mongoose. 

authController.js
Zawiera logik� uwierzytelniania i autoryzacji u�ytkownik�w.

/eventController.js
Zawiera logik� zarz�dzania zdarzeniami.

authRoutes.js
Definiuje trasy zwi�zane z uwierzytelnianiem u�ytkownik�w (logowanie, rejestracja, wylogowanie).

routes/eventRoutes.js
Definiuje trasy zwi�zane z zarz�dzaniem zdarzeniami (przegl�danie, tworzenie, aktualizacja, usuwanie zdarze�).

login.ejs
Szablon EJS dla strony logowania.

views/register.ejs
Szablon EJS dla strony rejestracji. 

views/events.ejs
Szablon EJS dla strony wydarze�.

views/editEvent.ejs
Szablon EJS do edycji istniej�cego wydarzenia.

views/newEvent.ejs
Szablon EJS do tworzenia nowego wydarzenia.

public/css/styles.css
(Opcjonalnie) Plik CSS do stylizacji szablon�w EJS.

package.json
Ten plik zawiera metadane dotycz�ce projektu oraz list� zale�no�ci i skrypt�w projektu.

package-lock.json
Ten plik jest automatycznie generowany przez npm i zawiera dok�adne wersje zainstalowanych zale�no�ci

Instalacja :

Sklonuj repozytorium:
-git clone 
WA�NE
Po sklonowaniu, aby uruchomi� ten projekt nale�y zainstalowa�:

-Pobieranie MongoDB https://www.mongodb.com/try/download/community i zainstaluj go.
*Aby uruchomi� aplikacj�, nale�y zainstalowa� dodatkowe paczki:
-npm init -y
-npm install express mongoose body-parser express-session helmet bcrypt ejs
-npm install --save-dev nodemon
*Po zainstalowaniu paczek, uruchom aplikacj� za pomoc� polecenia:
-npm start

Aplikacja b�dzie dost�pna pod adresem :
http://localhost:3000

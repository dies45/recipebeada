# Dokumentáció

## Követelményanalízis

Feladat: 
Első beadandóként  egy kis  webes alkalmazás elkészítése a cél szerveroldali technológiák segítségével. 
A feladatnak mininálisan tartalmaznia kell:

- legalább két modellt, egy-sok kapcsolatban
- legalább 1 űrlapot
- legalább 1 listázó oldalt
- legyen lehetőség új felvételére
- legyen lehetőség meglévő szerkesztésére
- legyen lehetőség meglévő törlésére
- legyenek benne csak hitelesítés után elérhető funkciók
- perzisztálás fájlba történjen
- közzététel Herokun

Választott feladat: Receptek és hozzávalók

Funkcionális elvárások:
- A felhaszáló recepteket szeretne tároli, erre szolgál az új recept hozzáadása.
- A felvett recepteket meg kell jeleníteni, későbbi olvasásra.
- A recepteket meg lehessen tekinteni és módosításokat lehessen hozzáírni, hogy minél jobb legyen.
- A recepteket lehessen törölni is.
- Bejelentkezés után lehessen hozzáférni a receptekhez.
- A főoldalon legyen rövid tájékoztató.

Nem funkcionális elvárások:
- Felhasználóbarát elrendezés
- Gyors működés
- Biztonságos működés: jelszavak tárolása

Használatieset-modell:

Szerepkörök:
- vendég: a főoldalhoz, a regisztrációhoz, és a bejelentkezés oldalakhoz fér hozzá, de recepteket megtekinteni és rögzíteni nem tud
- felhasználó: a vendég szerepkörén túl recepteket tud hozzáadni, módosítani és törölni

Használati eset diagram:



Folyamat menete:

Főoldal->Bejelenkezés->Saját receptek->Új recept hozzáadása

##Tervezés

Architektúra terv:

Oldaltérkép:

Publikus:
- Főoldal
- Regisztráció
- Bejelentkezés

Felhasználó:
- Főoldal
- Bejelentkezés/Kilépés
- Receptek: Új recept hozzáadása/törlése, Recept megtekintése/módosítás hozzáfűzése

Végpontok:

- get/ : főoldal
- get/login : bejelentkező oldal
- post/login : bejelentkezési adatok bevitele
- get/signup : regisztrációs oldal
- post/signup : regisztrációs adatok elküldése
- get/list : receptek megjelenítése
- get/new : új recept felvétele
- post/new : recept adatainak felküldése
- get/:id : recept adatai
- post/:id/comment : módosítás hozzáadása



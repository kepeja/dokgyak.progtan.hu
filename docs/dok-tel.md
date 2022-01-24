---
sidebar_position: 2
---

Telepítés
=========



Igényelt szoftverek
-------------------

Előzetesen telepíteni kell gépünkre:
- [node.js](https://nodejs.org/)
- [yarn](https://yarnpkg.com/)
- [git](https://git-scm.com/) - ha szeretnénk **git**-alapú tárolást, változat-követést...


Induló honlaphely létrehozása
-----------------------------

1. Parancssorban abba a mappába kell lépni, amin belül szeretnénk létrehozni a honlapot tartalmazó mappát.

1. Az alábbi parancs létrehozza a honlaphelyet:  
  ``` title="parancssorban:"
  npx create-docusaurus@latest [name] [template]
  npx create-docusaurus@latest honlapnev classic
  ```
  A fenti parancs hatására létrejön a `[honlapnev]` mappa és benne az induló honlap állományai, mappaszerkezete.


Fejlesztői honlap-kiszolgáló
----------------------------

A fejlesztést jelentősen könnyíti - ha a változtatások java részét önműködően frissítve láthatjuk egy böngészőben.  
Ehhez indítsuk el a honlap-kiszolgálót a `[honlapnev]` mappából!

``` title="parancssor, [honlapnev] mappában:"
yarn start
```
A honlap néhány másodperc múlva rendelkezésre áll a `localhost:3000/` címen.


Verziókövetés, GitHub
---------------------

Állítsuk be a **git** számára, hogy ez a mappa egy helyi *repo* lesz!:

``` title="parancssor, [honlapnev] mappában:"
git init
git add .
git commit -m "Első commit"
```

Ezek után töltsük fel a mappa tartalmát a [GitHub](https://github.com)-on előzőleg létrehozott üres *repo*-ba! Ehhez a **GitHub**-on megtaláljuk a szükséges parancsokat, pl.:

``` title="parancssor, [honlapnev] mappában:"
git remote add origin https://github.com/user/ures-repo.git
git branch -M main
git push -u origin main
```

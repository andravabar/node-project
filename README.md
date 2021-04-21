# Node-project ja lisarakenduse loomine
#### 2020∕21 projekt nr 3 "Node-project ja sellel lisarakenduse loomine" toimus ajavahemikul 03.02 - 05.02.2021.

**Projektijuht:** Markus Rätsep (TAK-19)

Meie tiim **"Word?"** jagunes kahte tiimi tulenevalt kursuse alustamise aastast, kas 2019 (ehk II kursus) või 2020 (ehk I kursus). 

**TA(K)-19 tiim:** 
Markus Rätsep TAK-19 / Erki Tammeaid TAK-19 / Laura Lepik TAK-19 / Mikk Lehtsaar TA-19 

**TA-20 tiim:**
Timo Pirn TA-20 / Andra Vabar TA-20 / Mattias A. Kaerma TA-20

## Kust me pärit oleme?
Kõik tiimi liikmed on pärit Eestist ning õpivad Kuressaare Ametikoolis tarkvara arenduse erialal.

## Projekti idee ja eesmärk
Projekti eesmärk oli etteantud Node.js ja Socket.io koodibaasi peale luua edasiarendatud rakendus, mis kasutab klient-server tehnoloogiat. 
Tiim **Word?** valis selleks kõrvalrakenduseks sõna arvamise mängu, mida saab chati-keskkonnas mängida teiste chatis olevate liikmetega.

## Projekti kõrvalrakenduse lühikirjeldus
Kõrvalrakenduseks sai valitud online sõna arvamise mäng kahe inimese vahel, kus mõlemal mängijal on kasutada terve tähistiku jagu tähti, arvamaks ära arvuti poolt randomly valitud sõna. Ära arvatav sõna kuvatakse ekraanil täht haaval nii, et igale tähele on eraldatud üks kriipsuke. Võidab see mängija, kes arvab sõna ära enne teist mängijat, arvestades asjaoluga, et valesti võib tähti pakkuda kokku 5 korda.

### Vahe eesmärgid
**Esimine kursus - TA-20**
 - Aru saada klient-server rakenduse tööpõhimõtetest
 - Analüüsi põhjal wireframe koostamine ja testimine
 - Disainireeglite loomine
 - Eelneva põhjal HTML ja CSS loomine
 - Testimine
 
**Teine kursus - TAK-19 ja TA-19**
 - Esimese kursuse juhendamine ja abistamine
 - Back-end ehk andmebaas ja server
 - JavaScript

## Suhtluskanalid: 
- Slack
- Teams

## Töövahendid ja lingid: 
- Github
- VS Code
- Figma [Wireframe](https://www.figma.com/proto/Live3cD0KFTNqMM44Go2nt/Wireframe?node-id=497%3A792&scaling=scale-down)


## Küsimused projekti kohta
 - Kas oleksid tahtnud täita mingit muud ülesannet selles meeskonnas
 - Üks pehme oskus, mida õppisin ja endas arendasin
 - Üks tehniline oskus, mida õppisin ja endas arendasin

**Markus Rätsep:**
1. Kuna ma ei ole Javascriptis kõige suurem käpp, siis mulle meeldis et sain ennast veel arendada selles.
2. Õppisin läbi teamsi suhtlemist ja koostöö tegemist.
3. Sain socket.io ja node js kohta rohkem teada ja kuidas neid täpsemalt kasutada.

**Erki Tammeaid:**
1. Ma olen rahul endale määratud ülesandega, kuigi javascripti ma kõige rohkem ei oska.
2. Õppisin paremini koostööd tegema ja abivajajaid aitama nii kontaktis, kui ka Teamsi vahendusel.
3. Sain node.js-i kohta natukene rohkem teada.

**Laura Lepik:**

**Mikk Lehtsaar:**

**Timo Pirn:**
1. Olen rahul määratud ülesandega. Selle projektiga ei oleks tahtnud alustada JavaScriptiga tutvumist, sest natuke liiga keeruline.
2. Tiimiga suhtlemist.
3. Terminali ja Gitiga töötamist.

**Andra Vabar:**
1. Olin rahul endale seatud ülesandega selles meeskonnas.
2. Sain veelkord kinnitust, et mulle meeldib tiim vestlusesse haarata ja iga viimne kui üks liige arutlema panna, võttes endale nö moderaatori rolli. Arendasin endas kindlasti kuulamise oskust, teisalt õppisin, kuidas enda ideid paremini selgemaks ja arusaadavamaks teha teistele.
3. Github'ga seotud oskusi sai arendatud - kuidas uut versiooni endale branchida, muudatusi teha ning seejärel repository pushida.

**Mattias A. Kaerma:**
1. Esimesel päeval ma puudusin ja kui jõudsin teiselpäeval kooli siis liitusin ma jälle figma tiimiga, kuna seal oli vaja veidikene abi siis otsustasin sinna jääda. Olen oma ülessandega rahul
2. Õppisin täitma korrektselt readme.md faili
3. Jällegi kujundamise osa, ja ekraanide linkimine Figmas

---------------------------------------------------------------

**Stack**
- Node JS / JS / npm
- Express (Node JS framework)
- Socket.io
- Redis

--------------------------------

**How to run**

This how to explains how to run this project on Ubuntu server.

1. Update your system
```
sudo apt update && sudo apt -y upgrade
```
2. Install the most recent version of Nodejs and npm (node packet manager). We use this repository because the normal Ubuntu repository has very old version.
```
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```
3. Test Nodejs
```
node -v
```
4. Test npm
```
npm -v
```
5. Install nodemon globally
```
sudo npm install -g nodemon
```
6. Install Redis
```
sudo apt install redis-server
```
7. Update redis.conf file. Find `supervised no` line and change to `supervised systemd` since Ubuntu uses the systemd init system.
```
sudo nano /etc/redis/redis.conf
```
8. Start Redis
```
sudo service redis-server start
```
9. Clone the repository
```
git clone https://github.com/kuressaareametikool/node-project
```
10. Change directory to project folder
```
cd node-project
```
11. Install modules
```
npm install
```
12. Run server
```
nodemon server.js
```

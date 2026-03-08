# Podatki

Podatke sem pridobil iz spletnega mesta Keggle. Celotna podatkovna zbirka vsebuje 14 csv datotek, vendar po vsej verjetnosti ne bom uporabil vseh, jih bom pa vseeno opisal.


#### circuits
Vsebuje podatke o progah.

- circuitId: ID proge
- circuitRef: poenostavljeno ime proge
- name: celotno ime proge
- location: mesto, v katerem se proga nahaja
- country: država, v katerem se proga nahaja
- lat: latitude
- lng: longitude
- alt: altitude
- url: povezava do wikipedia strani proge


#### constructor_results
Podatki rezultatov konstruktorjev.

- constructorResultsId: ID
- raceId: ID dirke
- constructorId: ID konstruktorja
- points: točke
- status: status rezultata


#### constructor_standings
Lestvica konstruktorjev po vsaki dirki.

- constructorStandingsId: ID
- raceId: ID dirke
- constructorId: ID konstruktorja
- points: št. točk
- position: uvrstitev na lestvici
- positionText: v string formatu
- wins: št. zmag

#### constructors
Podatki o konstruktorjih

- constructorId: ID konstruktorja
- constructorRef: referenčno ime konstruktorja
- name: dejansko ime konstruktorja
- nationality: Država ekipe
- url: povezava do wikipedie

#### driver_standings
Lestvica voznikov po vsaki dirki.

- driverStandingsId: ID
- raceId: ID dirke
- driverId: ID voznika
- points: št. točk
- position: uvrstitev na lestvici
- positionText: v string formatu
- wins: št. zmag

#### drivers
Podatki o voznikih

- driverId: ID voznika
- driverRef: referenca voznika
- number: številka voznika
- code: 3 črkovna koda voznika (običajno prve 3 črke priimka)
- forename: ime
- surname: priimek
- dob: datum rojstva
- nationality: državljanstvo
- url: povezava do wikipedie

#### lap_times
Časi krogov

- raceId: ID dirke
- driverId: ID voznika
- lap: krog
- position: položaj dirkača
- time: čas
- milliseconds: čas v milisekundah

#### pit_stops
Časi postankov

- raceId: ID dirke
- driverId: ID voznika
- stop: številka postanka
- lap: krog
- time: čas proge
- duration: čas postanka
- milliseconds: v milisekundah

#### qualifying
Kvalifikacije

- qualifyId: ID kvalifikacij
- raceId: ID dirke
- driverId: ID voznika
- constructorId: ID konstruktorja
- number: številka voznika
- position: pozicija
- q1: čas v q1 (1. del kvalifikacij)
- q2: čas v q2 (2. del kvalifikacij)
- q3: čas v q3 (3. del kvalifikacij)

#### races
Dirke

- raceId: ID dirke
- year: leto dirke
- round: številka dirke v letu
- circuitId: ID proge
- name: ime dirke
- date: datum dirke
- time: UTC čas dirke
- url: povezava do wikipedie

Naslednji stolpci so tudi del te datoteke, vendar ker se prvič uporabijo leta 2021 jih ne bom uporabljal (verjetno jih tudi v nobenem primeru ne bi uporabil)
- fp1_date
- fp1_time
- fp2_date
- fp2_time
- fp3_date
- fp3_time
- quali_date
- quali_time
- sprint_date
- sprint_time

#### results
Podatki rezultatov voznikov.

- resultId: ID rezultata
- raceId: ID dirke
- driverId: ID voznika
- constructorId: ID konstruktorja
- number: številka voznika
- grid: začetni položaj
- position: končni položaj
- positionText: v tekstu
- positionOrder: končni položaj za vse voznike (tudi tiste, ki niso končali dirke)
- points: točke
- laps: št. krogov
- time: končni čas
- milliseconds: v milisekundah
- fastestLap: kateri krog je bil najhitrejši
- rank: rank najhitrejšega kroga
- fastestLapTime: čas najhitrejšega kroga
- fastestLapSpeed: najvišja dosežena hitrost najhitrejšega kroga (v mph)
- statusId: ID statusa

#### seasons
Leta

- year: leto sezone
- url: link do wikipedie

#### sprint_results
Rezultati šprint dirk

- resultId: ID rezultata
- raceId: ID dirke
- driverId: ID voznika
- constructorId: ID konstruktorja
- number: številka voznika
- grid: začetni položaj
- position: končni položaj
- positionText: v tekstu
- positionOrder: končni položaj za vse voznike (tudi tiste, ki niso končali dirke)
- points: točke
- laps: št. krogov
- time: končni čas
- milliseconds: v milisekundah
- fastestLap: kateri krog je bil najhitrejši
- fastestLapTime: čas najhitrejšega kroga
- statusId: ID statusa

#### status
Možni statusi dirkačev

- statusID: ID statusa
- status: status
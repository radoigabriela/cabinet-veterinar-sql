# Proiect 5 – Cabinet Veterinar (SQL)

Acest proiect a fost realizat în cadrul unui seminar practic și are ca scop proiectarea completă a unei baze de date relaționale pentru un cabinet veterinar.

## Cerința temei

Am fost rugată să creez o bază de date care să ajute un cabinet veterinar să își gestioneze activitatea. Baza trebuia să includă informații despre:

- proprietarii animalelor
- pacienți (animalele tratate)
- consultațiile medicale
- tratamentele aplicate

Am pornit de la analiza conceptuală (identificarea entităților și a relațiilor), am trecut la modelarea logică (ER-diagramă, cardinalități), apoi am implementat schema în MySQL Workbench și am exportat-o în fișier `.sql`.

De asemenea, schema a fost normalizată până la forma 3 (3NF), astfel încât să nu existe dependențe tranzitive și să fie păstrată integritatea datelor.

## Ce conține proiectul

- `CE_2_203_Radoi_GabrielaBianca_CabinetVeterinar.sql` – scriptul SQL complet
- `CE_2_203_Radoi_GabrielaBianca_CabinetVeterinar.mwb` – modelul grafic realizat în MySQL Workbench
- (opțional) imaginea cu ER-diagrama și cerințele PDF, dacă sunt încărcate

## Relațiile principale

- Un **proprietar** poate avea mai mulți **pacienți**
- Un **pacient** poate avea mai multe **consultații**
- O **consultație** poate conține mai multe **tratamente**

## Normalizare (3NF)

Fiecare tabel are o cheie primară clară, toate atributele depind direct de cheie, iar structura evită orice dependențe tranzitive. Relațiile sunt bine definite prin chei externe, păstrând integritatea referențială.

## Tehnologii folosite

- MySQL Workbench
- SQL standard

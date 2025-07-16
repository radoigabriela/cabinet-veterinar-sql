# Proiect 5 – Cabinet Veterinar (SQL)

Acest repository conține o bază de date relațională pentru un cabinet veterinar, construită pentru a ilustra procesul complet de proiectare și implementare a unei soluții de gestiune.

### Modelul de bază acoperă:

- proprietarii animalelor
- pacienții (animalele tratate)
- consultațiile medicale
- tratamentele aplicate

Proiectul a fost dezvoltat etapizat: de la analiza conceptuală (identificarea entităților și relațiilor), la modelarea logică (diagrama ER și definirea cardinalităților), până la implementarea efectivă în MySQL Workbench.

Datele au fost structurate conform regulilor de normalizare (până la forma normală 3), pentru a asigura integritatea informațiilor și a evita redundanțele.

### Fișiere incluse

- CE_2_203_Radoi_GabrielaBianca_CabinetVeterinar.sql – scriptul SQL complet pentru crearea bazei de date
- CE_2_203_Radoi_GabrielaBianca_CabinetVeterinar.mwb – modelul vizual realizat în MySQL Workbench
 
### Relațiile dintre entități

- Un **proprietar** poate deține mai mulți **pacienți**
- Un **pacient** poate avea mai multe **consultații**
- O **consultație** poate include mai multe **tratamente**

Relațiile sunt gestionate prin chei externe, astfel încât fiecare tabel păstrează legătura logică cu celelalte fără pierderi de informație.

### Normalizare (Forma Normală 3)

Structura bazei de date respectă următoarele principii:

- fiecare tabel are o cheie primară unică
- toate atributele depind direct de cheia primară
- nu există dependențe tranzitive între coloane

Astfel, baza de date este coerentă și eficientă din punctul de vedere al integrității și stocării.

### Tehnologii folosite

- MySQL Workbench
- SQL (interogări standard)

Proiectul este util pentru înțelegerea modului în care se poate construi o bază de date funcțională, clar organizată și ușor de întreținut, într-un context practic inspirat din realitate.

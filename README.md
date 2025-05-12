# Metrika proizvoda
File Calculator.java ima 188 linija koda

File Start.java ima 26 linija koda

Zbirno ceo projekat ima 214 linija koda (LOC)

# Staticka analiza fajla Start.java
fajl – broj linije koda – zapažanje

Start.java – linija 1 – Klasa Start nije ni u jednom paketu; trebala bi da bude u nekom nazvanom paketu

Start.java – linija 6 – Ime promenljive 'Expression' se ugalvnom pise malim slovima u Java jeziku; trebalo bi da bude 'expression'

# Staticka analiza fajla Calculator.java
fajl – broj linije koda – zapažanje

Calculator.java - linija 1 - Klasa Calculator nije ni u jednom paketu; trebala bi da bude u nekom nazvanom paketu

Calculator.java - linija 4 - Klasa Calculator sadrži samo statičke metode i promenljive, ali nema eksplicitno definisan privatni konstruktor. U ovom obliku, moguće je kreirati instancu klase, iako to nije potrebno

Calculator.java - linija 18 - promeniti ime string-a ToString kako ne bi doslo da zabune sa metodom toString

Calculator.java - linija 24 - Ime stringa 'Run' se ugalvnom pise malim slovima u Java jeziku; trebalo bi da bude 'run'

Calculator.java - linija 70 - Promenljiva textResult se koristi samo da bi čuvala rezultat izraza Float.toString(finalResult) – a zatim se odmah vraća. To je nepotrebno i povećava dužinu i složenost koda bez neke koristi

Calculator.java - linija 74 - Ime promenljive 'Calculate' se ugalvnom pise malim slovima u Java jeziku; trebalo bi da bude 'calculate'

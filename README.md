Calculator.java

LOC 134

Broj cvorova (n):34 Broj bridova (e):40

C=E-N+2=40-43+2=4 Ciklomatska sloyenost iznosi 4

Kngnitivnu slozenost, mozemo primetiti da metoda evulateExpression ima nekoliko grananja i petljikoje bi mogle otezati citanje i razumevanje koda.
Metode Calculate ima mnogo grananja, sto takodje moze povecati kognitivnu sloznost.

Staticka analiza:

Linije 12-16: Staticki simboli su dobro definisani i koriste se konvecionalno.
Linije 28-58: Metoda evulateExpression ima dugacak blok koda koji bi mogao biti refaktorisan u manje metode radi bolje citljivosti i odrzavanja.
Linije 60-86: Metode Calculate takodje ima dugacak blok koda koji bi mogao biti refaktorisan na slican nacin.

Podtoji potencijal za dodavanje komentara radi boljeg objasnjenja slozenih delova logike.

Code smells:

Staticke promenljive finalResult: Staicke promenljive se cesto izbegavaju , posebno ako nisu potrebne.
Treba koristiti lokalne promenljive unutar metode gdeje to moguce.
Koristenje Stringa za matematicke operacije.
Metoda ToString u unutrasnjoj klasi Operations vraca string koji presdstavlja simbole matematickih operacija.
Dugacke metode:Metode evulateExpression i Calculate su relativno duge i slozenost otezava odrzavanje i razumevaje koda.
Nepotrebno koristenje ToString.
Nesigurna upotreba try-catch bloka.
U metodi evulateExpression koristi se try-catch blok bez preciznog navodjenja izuzetaka koji se hvataju.
Treba specifirati izuzetke.
Nekonzistentna upotreba zagrada u kontrolnim strukturama.
U nekim delovima koda nema zagrada oko blokova koda u if i else konstrukcijama sto moze dovesti do problema sa citljivoscu i potencijalno uvodjenje greske. Start.java

LOC 19 

Broj cvorova (n):3 Broj bridova (e):2

C=E-N+2=2-3+2=1 Ciklomatska slozenost 1

Program je jednostavan, sa jednom petljom i jednim grananjem sto znaci da ce kognitivna slozenost biti niska upravo zbog jednostavnosti strukture i logike.

Staticka analiza:

Ovaj kod deluje ispravno i obavlja ocekivane funkcionalnosti.
Medjutim postoji nekliko mesta gde se moze dodati provera kako bi se poboljsalo rukovanje potencijalnim greskama.

Code Smells:

Linije 9-19: Otvaranje novog Scanner-a unutar petlja moze izbeci kreiranjem objekta Scanner jednom izvan petlje i ponovo ga koristiti.


# Prezentacija projekta – Analiza faktora sreće po državama

## Uvod

U ovom projektu analizirali smo povezanost ekonomskih i društvenih faktora s indeksom sreće stanovništva koristeći podatke iz World Happiness Reporta za 2016. godinu.

Cilj projekta bio je primijeniti statističke metode koje smo učili na kolegiju, kako bismo analizirali stvarne podatke i vidjeli što utječe na sreću država. Posebno nas je zanimalo postoji li povezanost između ekonomskog faktora, odnosno BDP-a po stanovniku, i indeksa sreće.

Podatke smo analizirali koristeći programski jezik R u okruženju RStudio.

---

## Opis podataka

Dataset sadrži podatke za 157 država i uključuje više faktora koji utječu na indeks sreće.

Glavna varijabla koju smo analizirali je Happiness Score, što predstavlja numeričku procjenu razine sreće stanovništva neke države.

Osim toga, dataset uključuje i druge varijable kao što su:

- Economy (GDP per Capita) – ekonomski faktor
- Family – obiteljska podrška
- Health – očekivani životni vijek
- Freedom – sloboda donošenja odluka
- Trust – povjerenje u vladu
- Generosity – velikodušnost

Ove varijable omogućuju analizu različitih faktora koji mogu utjecati na sreću.

---

## Deskriptivna statistika

Prvo smo izračunali mjere centralne tendencije. To su mjere koje nam govore koja je tipična ili prosječna vrijednost u skupu podataka.

### Aritmetička sredina

Aritmetička sredina je zapravo ono što svakodnevno zovemo prosjek. Dobije se tako da zbrojimo sve vrijednosti i podijelimo s njihovim brojem.

U našem slučaju aritmetička sredina indeksa sreće iznosi:

5.382

To znači da prosječna država ima indeks sreće oko 5.38.

### Medijan

Medijan je srednja vrijednost kada sve podatke sortiramo od najmanjeg do najvećeg. Drugim riječima, to je vrijednost koja dijeli podatke na dva jednaka dijela.

U našem slučaju medijan iznosi:

5.314

To znači da polovica država ima indeks sreće manji od te vrijednosti, a polovica veći.

### Mod

Mod je vrijednost koja se najčešće pojavljuje u skupu podataka.

U našem slučaju mod iznosi:

6.379

To znači da se ta vrijednost najčešće pojavljuje među državama.

Usporedbom ovih mjera možemo vidjeti da distribucija nije savršeno simetrična, ali nema velikih odstupanja.

---

## Mjere raspršenja

Dok mjere centralne tendencije govore gdje se nalazi prosjek, mjere raspršenja govore koliko su podaci rašireni oko tog prosjeka.

### Varijanca

Varijanca mjeri koliko se vrijednosti u prosjeku razlikuju od srednje vrijednosti.

U našem slučaju varijanca iznosi:

1.303

To znači da postoji određena razina razlika između država.

### Standardna devijacija

Standardna devijacija je slična varijanci, ali je izražena u istoj jedinici kao originalni podaci, pa ju je lakše interpretirati.

U našem slučaju standardna devijacija iznosi:

1.142

To znači da indeks sreće tipično odstupa od prosjeka za oko jednu jedinicu.

To pokazuje da postoje umjerene razlike u sreći između država.

---

## Empirijska vjerojatnost

Empirijska vjerojatnost predstavlja procjenu vjerojatnosti na temelju stvarnih podataka, odnosno promatranjem koliko se puta neki događaj dogodio.

U našem slučaju promatrali smo kolika je vjerojatnost da slučajno odabrana država ima indeks sreće veći od prosjeka.

Dobivena vrijednost je:

0.497

To znači da oko 49.7% država ima indeks sreće veći od prosjeka.

To ima smisla jer prosjek obično dijeli podatke približno na dva dijela.

---

## Uvjetna vjerojatnost i nezavisnost

Uvjetna vjerojatnost predstavlja vjerojatnost nekog događaja uz uvjet da se dogodio neki drugi događaj.

U našem slučaju promatrali smo vjerojatnost da država ima iznadprosječan indeks sreće uz uvjet da pripada regiji Western Europe.

Dobivena vrijednost iznosi:

0.905

To znači da oko 90.5% država u toj regiji ima iznadprosječan indeks sreće.

Budući da je ta vrijednost znatno veća od ukupne vjerojatnosti, možemo zaključiti da regija i indeks sreće nisu nezavisni.

Drugim riječima, regija ima značajan utjecaj na razinu sreće.

---

## Empirijska distribucijska funkcija

Empirijska distribucijska funkcija pokazuje koliki udio podataka ima vrijednost manju ili jednaku nekoj određenoj vrijednosti.

Na primjer, dobili smo:

F(6) = 0.701

To znači da oko 70.1% država ima indeks sreće manji ili jednak 6.

Ova funkcija nam pomaže razumjeti raspodjelu podataka.

---

## Zakon velikih brojeva i centralni granični teorem

Zakon velikih brojeva kaže da što uzmemo veći uzorak, to će prosjek tog uzorka biti bliži stvarnom prosjeku populacije.

Centralni granični teorem kaže da distribucija sredina uzoraka teži normalnoj distribuciji, čak i ako originalni podaci nisu normalno distribuirani.

Ovi teoremi objašnjavaju zašto možemo koristiti uzorak za zaključivanje o populaciji.

---

## Korelacija između BDP-a i indeksa sreće

Korelacija mjeri koliko su dvije varijable međusobno povezane.

Vrijednost korelacije može biti između -1 i 1.

U našem slučaju korelacija iznosi:

0.790

To znači da postoji jaka pozitivna povezanost između BDP-a po stanovniku i indeksa sreće.

Drugim riječima, države s većim BDP-om po stanovniku imaju tendenciju imati veći indeks sreće.

Važno je naglasiti da korelacija ne znači uzročnost, nego samo povezanost.

---

## Testiranje statističke hipoteze

Statistički test koristimo kako bismo provjerili vrijedi li neka pretpostavka o populaciji.

U našem slučaju testirali smo je li prosječni indeks sreće veći od 5.

Dobivena p-vrijednost bila je manja od 0.001.

To znači da je vrlo mala vjerojatnost da je rezultat dobiven slučajno.

Zbog toga odbacujemo nul-hipotezu i zaključujemo da je prosječni indeks sreće statistički značajno veći od 5.

---

## Zaključak

U ovom projektu primijenili smo statističke metode na stvarne podatke kako bismo analizirali indeks sreće država.

Zaključili smo da:

- prosječni indeks sreće iznosi oko 5.38  
- postoje umjerene razlike između država  
- geografska regija ima značajan utjecaj  
- postoji jaka povezanost između BDP-a i sreće  
- statistički test potvrđuje da je prosječni indeks sreće veći od 5  

Projekt pokazuje kako statistika omogućuje analizu stvarnih društvenih podataka i donošenje zaključaka na temelju podataka.

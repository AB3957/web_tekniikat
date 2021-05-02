Harjoitus 3: HTML- ja CSS-perusteita jatkuu

Tässä harjoituksessa opit

CSS-syntaksin eli kielen määrittelyn
Määrittelemään ulkoisen tyylitiedoston, joka on voimassa koko sivustoosi
Perusmuotoilujen tekeminen tyylitiedoston avulla, kommentoinnin tyylitiedostoon
Tyyliluokan ja tyylitunnisteen käytön
Eri tapojen vaikutusalueet: Selaimen oletusmääritykset->Tyylitiedosto->dokumentin sisäiset <head>-osion määrittelyt ->html-elementtikohtaiset määrittelyt
Validaattorin käytön

Alla muutamia vinkkejä, tee määritykset ensin <head>-osioon dokumentin sisälle:

Tee uusi html-dokumentti ja anna <title>-elementiksi nimi "Asiakkaat -taulukko".
Kopioi ylhäältä muotoilematon taulukko sivupohjaasi.
Kopio koodista käsin se vielä toiseen kertaan sivullesi ja määritä taulukon tunnisteeksi (id) "Asiakkaat".
Tallenna dokumentti harj3-hakemistoon nimelle: asiakkaat_taulukko.html
Määritä <head>-osioon tyylit voimaan ja määrittele sen sisälle seuraavat tyylimääritykset.
Määritä sivulle ylä- ja vasen marginaali 50px (body-määreeseen margin-top ja margin-left)
Määritä tyyleissä (id ja #) juuri tähän Asiakkaat -taulukkoon liittyvät yleiset muotoilut (eivät siis vaikuta oletustaulukon määrityksiin (vinkki: #Asiakkaat {.....}),
kirjasinlajiksi "Helvetica, Arial, sans-serif" ja
reunukset yksinkertaisiksi (oletus on kaksikertainen piirto) vinkki: "border-collapse".
Määritä Asiakkaat -taulukolle otsikkorivi (th-elementit sarakkeille: Yritys, Yhteyshenkilö, Maa)
Muotoile yhteiset tyylit Asiakkaat -taulukon otsikkoriville ja -taulukon soluille: reunat, tausta sekä välistys tekstille soluun asettumiseksi (backround-color, border, padding 3-7px)
Määritä Asiakkaat -taulukon otsikkoriville seuraavat määritykset
taustaväri vaalean sininen
kirjasinkoko 1.2em,
tekstiväri vaalea,
hivenen isompi välistys solussa ylös ja alas (5px)
Määritä vaihtoehtoinen hyvin vaalean sinertävä tyyliluokka Asiakkaat -taulukon riveille ja sen soluille ja kutsu joka toista riviä tällä luokalla.
Voit kokeilla kohtaan 11 myös yleistä määritystä parillisille ja parittomille riveille taulukossa, jolloin ei erikseen tarvitse kutsua tyyliluokkaa joka toisella rivillä:

table#Asiakkaat tr:nth-child(even) {
background-color: #eee;
}
table#Asiakkaat tr:nth-child(odd) {
background-color:#fff;
}
# Decision Intelligence — Prattin decision pathways -malli

Liittyy kaavioon: `decision-pathways-pratt.drawio`

Dr. Lorien Pratt on tekoälyn ja koneoppimisen pioneeri, joka tunnetaan
muun muassa siirto-oppimisen (transfer learning) kehittäjänä. Hän on
yksi Decision Intelligence (DI) -käsitteen luojista ja Quantellia-yhtiön
päätieteilijä. Pratt on kuvannut DI:n perusajatuksen yksinkertaisesti:
kyse on siitä, miten toiminnasta päästään lopputuloksiin. DI yhdistää
inhimillisen päätöksenteon dataan, malleihin ja koneoppimiseen sen sijaan,
että data jätettäisiin irralleen itse päätöksestä.

Mallin ydin on **Causal Decision Diagram (CDD)** — kausaalinen
päätöskaavio, joka tekee näkyväksi sen syy-seurausketjun, jonka kautta
päätöksentekijän toiminta johtaa tavoiteltuihin lopputuloksiin. Tästä
ketjusta Pratt käyttää nimitystä **action-to-outcome pathway** eli
toiminnasta lopputulokseen kulkeva polku. Kaavio luetaan vasemmalta
oikealle: vasemmalla ovat päätöksentekijän käytettävissä olevat valinnat
ja ulkoiset reunaehdot, oikealla tavoiteltu lopputulos, ja niiden välissä
on kausaalinen ketju, johon data ja koneoppiminen kiinnittyvät.

## Mallin elementit

### Päätösvivut (Levers)

Vivut ovat päätöksentekijän hallinnassa olevia, toisensa poissulkevia
valintoja. Yksittäinen valinta (choice) on osa laajempaa vipua (lever),
joka koostuu joukosta vaihtoehtoisia valintoja. Vivuista syntyy toiminta
(action) — esimerkiksi päätös nostaa markkinointibudjettia tai muuttaa
hinnoittelua. Olennaista on, että vivut ovat juuri niitä asioita, joista
päätöksentekijällä on päätösvalta, toisin kuin ulkoisista tekijöistä.

### Ulkoiset tekijät (Externals)

Ulkoiset tekijät vaikuttavat lopputulokseen, mutta eivät ole
päätöksentekijän hallinnassa annetulla hetkellä. Tällaisia ovat
esimerkiksi markkinatilanne, sää, kilpailijoiden toiminta tai
lainsäädäntö. Ne ovat ketjun annettuja reunaehtoja: malli ottaa ne
huomioon, mutta päätöksentekijä ei voi niitä säätää.

### Välimuuttujat (Intermediates)

Välimuuttujat ovat syy-seurausketjun välivaiheita toiminnan ja
lopputuloksen välillä. Ne ovat vivuilla ja ulkoisilla tekijöillä
tuotettua tietoa — esimerkiksi laskettu riskipisteet, kysyntäennuste tai
muu johdettu suure. Ketjut voivat olla monivaiheisia: yksi välimuuttuja
voi vaikuttaa kausaalisesti toiseen ennen kuin lopputulos syntyy. Juuri
välimuuttujien kohdalla, ketjun keskellä, data, analytiikka ja
koneoppimismallit kiinnittyvät päätökseen. Pratt kuvaa tämän kohdan
toiminnasta lopputulokseen kulkevan polun keskelle: siellä, missä
suhdetta toiminnan ja seurauksen välillä ei tunneta, tarvitaan
data-analytiikkaa tai koneoppimista.

### Riippuvuudet (Dependencies)

Riippuvuudet ovat kaavion nuolia, jotka ilmaisevat elementtien välisen
syy-seuraussuhteen — sen, miten muutos yhdessä elementissä vaikuttaa
toiseen. Riippuvuus voi olla yksinkertainen oletettu suhde tai
koneoppimismallin kuvaama yhteys; jälkimmäistä Pratt merkitsee kaavioissaan
linkin kohdalla olevalla kolmiolla. Riippuvuudet ovat se rakenne, joka
tekee CDD:stä enemmän kuin prosessikaavion: ne mallintavat syytä ja
seurausta, eivät ainoastaan tapahtumien järjestystä.

### Lopputulokset ja tavoite (Outcomes, Objective)

Lopputulokset ovat toiminnan mitattavia seurauksia. Tavoite (Objective)
on se mitattava päämäärä, jota vasten lopputuloksia arvioidaan. Kun päätös
toistuu, mitatut lopputulokset muodostavat opetusdataa
koneoppimismalleille — tämä on se kohta, jossa DI ja datatiede kytkeytyvät
toisiinsa ja jossa malli oppii ajan myötä.

## Syy-seurausketju on mallin ydin

Aivan kuten tasapainotetussa tuloskortissa, myös CDD:ssä arvo ei ole
yksittäisissä laatikoissa vaan niitä yhdistävässä kausaalisessa
logiikassa. CDD eroaa tavanomaisesta päätöspuusta tai prosessikaaviosta
juuri siinä, että se painottaa toiminnan ja mitattavan lopputuloksen
välistä syy-seuraussuhdetta. Prattin mukaan CDD vastaa ihmisen
luonnollista tapaa hahmottaa päätöksiä ja keventää siten kognitiivista
kuormaa: se vapauttaa ajattelukapasiteettia itse päätöksen kannalta
olennaisiin, monimutkaisiin kysymyksiin.

Malli kytkeytyy myös iteratiiviseen Observe–Orient–Decide–Act (OODA)
-silmukkaan: lopputuloksia havainnoidaan, ne palautetaan opetusdataksi, ja
päätöstä tarkennetaan ajan myötä. Kaaviossa tämä on kuvattu katkoviivalla
palautuvana nuolena lopputuloksista takaisin ketjun alkuun. Simulaatio
puolestaan tuottaa mallista aineiston, joka tekee näkyväksi, mihin
lopputuloksiin eri vivun asetukset todennäköisesti johtavat.

Kaaviossa asettelu noudattaa Prattin alkuperäistä vasemmalta oikealle
kulkevaa polkua: vasemmalla päätöksentekijän hallinnassa olevat vivut ja
hänen ulottumattomissaan olevat ulkoiset tekijät, keskellä välimuuttujien
muodostama syy-seurausketju datan ja koneoppimisen kytkentäkohtana, ja
oikealla tavoiteltu lopputulos arvioituna mitattavaa tavoitetta vasten.

## Lähteet

- Pratt, L. 2019. *Link: How Decision Intelligence Connects Data, Actions,
  and Outcomes for a Better World.* Bingley: Emerald Publishing.
- Pratt, L. & Malcolm, N. E. 2023. *The Decision Intelligence Handbook:
  Practical Steps for Evidence-Based Decisions in a Complex World.*
  Sebastopol, CA: O'Reilly Media.
- Pratt, L. *Lorien Pratt's blog — Decision Intelligence, Agile Applied
  AI, Machine Learning.* https://www.lorienpratt.com/ (mm. kirjoitukset
  kausaalisista päätöskaavioista ja "A Framework for How Data Informs
  Decisions").
- Quantellia / OpenDI. *Decision Intelligence -käsitteistö* (Levers,
  Externals, Intermediates, Dependencies, Outcomes). https://www.opendi.org/

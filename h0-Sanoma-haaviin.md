# h0 - Sanoma haaviin

Ensimmäinen tehtäväni on vangita ja analysoida verkkoliikennettä. On monta eri tapaa, joten listataan yleisimmät.

## Tapa 1: Selaimen kehittäjäntyökalu

Selaimen kehittäjäntyökalusta löytyy mm. Network -välilehti, josta voidaan tarkistaa verkkoliikennettä. Muun muassa, päivitetyään tätä Githubin -verkkosivua tuli seuraavat verkkoliikenteen raportti (katso alla olevaan kuvaan).

![Jansson_Tunkistestaus_laksy_h0_Network_01](https://github.com/user-attachments/assets/9391fd27-0259-42f0-9903-3258a4782dcc)

Huomioi, että tämä verkkoliikenteen rapportti on Microsoft Edge -selaimesta. Tehtäväannossa mainittu Firefox Web tools Network pitää tulostaa samalaiset tulokset:

![Jansson_Tunkistestaus_laksy_h0_Network_02](https://github.com/user-attachments/assets/22567129-d1b0-4e0e-aee0-ee7988320e0a)

Analysoidaan Firefoxin kehittäjäntyökalun verkkoliikenteen raporttia, koska se tulosti enemmän tietoja ja on selkeämpi rakenne.

Huomaamme heti, että kaikki kuvassa olevassa verkkoliikenteiden status ovat 200, mikä kertoo loistavas, virhettömästä verkkoliikenteen lähetys.

Metoodit ovat GET, mikä tarkoittaa domainit (eli verkkosivut) ja niiden tiedostot *hakeavat* dataa.
Sitten huomaamme, että suurin osa, erityisesti githubassets -sivustot, ovat tyypiltään javascript -koodausskriptejä.

Kun taas itse github.com -pääsivusto on HTML -tiedostoa 

## Referenences



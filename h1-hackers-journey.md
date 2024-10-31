# h1 - Hacker's journey

**Päivistys 30.10.2024**: Tehtäväni on vielä kesken,
koska Tero Karvisen kurssin sivuston mukaan,
kohdassa Läksyt -luvussa (https://terokarvinen.com/tunkeutumistestaus/),
läksyjen linkki piti lähettää viimeistään 24 h ennen seuraava luento,
ts. viimeistään torstaina 31.10.2024 klo 08:15.

Palautin URL:in Laksuun hyvissä ajoin, koska minulla on muu meno
torstaina 31.10.2024 klo 8:00.

Tässä tehtävässä tutustuumme porttiskannaukseen ja rakennamme oma hakkerilabraa.

---

## x) Tiivistelmiä aiheesta eri lähdeistä.

### 1. Herrasmieshakkerit - Valkohattuhakkerit, vieraana Iiro Uusitalo (Jakso 1, 01.10.2019)

![Jansson_Tunkistestaus_laksy_h1_x_tiivistelmät_01](https://github.com/user-attachments/assets/0d06ff9c-ebd5-44a3-b13d-6fac1d0cee3f)

Podcastin jountajat Mikko Hyppönen ja Tomi Tuominen, virallisesti Suomen tietoturvakentän wirallset 

wanhukset (heidän sanojensa mukaan), saavat tälle jaksolle vieraaksi Iiro Uusitalo. He keskustelevat

mm. bug bounty-ohjelmista, Team Whackista sekä valkohattuhakkeriryhmästä Team Rotista ja ryhmän 

järjestimistä ilmaisista murtotestauksista.

#### Kommenteja
- Podcastin ensimmäisessä jaksossa he vielä pohtivat sopivaa heidän kartanostudiolle.
Yleisö pystyi lähettämään ehdouksia hashtagilla #hakkerit.

-- Viikon uutisia

I) Simjack uhka on vakavampi kuin Simswap. Asiasta huomioi Twitter entisen toimitusjohtaja.
    
* Uutinen koski SAT:een lisäysominaisuuden olevaan havoittuvuuden, joka ei ole esinny
monessa paikoissa eikä suuren osa väestöstä. Eli haavoittuvuus koski lähinnä hyvin tarkkaan ja rajattuun ryhmään. 
    
* Podcastissa huomioittiin, että teleoperattorin vaihto on hyvin erilaista Amerikassa verrattuna Suomeen.
    
* Tomi Tuominen kritisoi podcastissa, että uutiseen reagointiin liian herkkäästi. Hän toivosi 
uutislähettäjiltä harkkinavaraisempaa viestintää ja parempaa taustatietojen tarkistusta,
ts. lähdekriitisyyttä. 
    
* Hän kommentoi koko jutun ns. "pelko uutisointi", eli tehtiin kärpäsestä härän.
Häntä kismitti erityisesti faktojen liiotellua markkinatarkoituksiin.

II) Linux Malware haittaohjelma on Attacklandscape uudemman rapportin mukaan
  pääsyt ohi, ts. edelläkävellyt, Microsoft Malware.

* Historiallinen hetki.
    
* Uutinen on todella merkkitävä, sillä monet IoT laitteet, kuten Telnet,
käyttävät Linuxia.
    
* Tämä on ollut Linuxissa pitkään ollut ja toivottu määränpää.
    
* "Simple as the Best" ja "Done as the Best".

III) Pohjois-Korean pääkaupungissa Pyongyangissa järjestettään virtuaalivaluuta, "blockchain cryptocurrency" konferenssi.
Ihmeellistä, miten raskasti sanktiottu maa oli yhtäkkiä kiinnostunut kryptovaluutasta.

-- Viikon vierashaastattelu. Iiro Uusitalo, ulkomaassa tunnetaan paremman "Liro" L -merkkillä.

** Hän on erkioistunut erityisesti Linux ja Infra ("lähellä omaa sydäntä").

** Jountajat ottivat ylös TeamWhale, eli Ylessä tuotettu dokumenttisarja, jossa
kuvailtiin mahdollisimman hyvin realistisesti hakkerointia. Mikko Hyppönen
kehui sarjasta kommentilla "oikeesti toteuttu oikealla työkalulla".

** Iiro mainitisi Team Rot (saksan sanasta "punainen"), joka perustui
yhdessä Pasilan Hacklabissa. Hän sanoi, että tiimin meinikki oli niin hyvä
että kaveriryhmä jatkoi toiminnansa tapahtuman jälkeen. Ryhmä on aktiivinen myös
vapaa-aikana.

** Team Rot koostuu kuusi monipuolista asiantuntjoita / osamispuolia, mm. Pythonilla SQL Injektiota, "Reversaus" (?), Webbend testauksia,
Linux & Infra, jne.

** Kuntahaaste, joka oli kunnalle ja kaupungille järjest "tempaus" Twitterin avoimilla kirjeellä. Tempauksessa yritettiin murtotestaus
tiettyyn kuntaan, koska monissa kunnissa on samaanlaisia sovelluksia. Kun yksi kunta hyökätään, niin muut kunnat hyötyvät.
Tempaukseen osallistui vain yhdeksän kuntaa, koska suuren osan kuntaryhmästä pelkäsivät jo pelkästä hankeesta "missä hakkerit hakkeroi
kuntapalvelimeen". Toisin sanoen, hanke oli liian riskimäistä kunnalle, vaikka halutiinkin parantaa heidän palvelimia 
(sana "hakkeri" on muutoinkin keskusdessamme musta tahrama ja taboo sana). Tyypillistä suomalaista epävarmuuta
ja varovaisuutta, erityisesti ilmaisista palveluista. Lisäksi kunnat valitti, miksi viestitti Twitterissä, eikä
suoraan heille.

** Lisäksi he ovat järjestämä korkeakoululle kouluhaaste, samaa idea kuin kuntahaaste. Tällä kerta, löytyneet haavoituksista ilmoitetaan julkisesti.

** Keskusteltiin backboundista / bookboundista. Iiro hyvin huomioi, että suljetut ohjelmistot ovat suosittelevempaa, sillä julkiset ohjelmistot
kuka vaan (mm. tietoturvatutkija) voi osallistua. Suljettuihin pääse vaan kutsun tai oikeudet backbound -järjestäjiltä.
F-Secure backbound oli Suomalaisia ensimmäisiä julkaistettu backbound (vaati kovaa "matuureja"). Backboundissa
on paljon korjattavaa, mukaan lukien bugeja jotka eivät ole tietoturvauhkia.

** Mikko oli iloinen Iiro kommentista miten bookbound mainostetaan ja mikä on se tosi elämässä (26:00 - 26:40 aikakohta).

** "Recon" -vaihe backboundissa kasvaa koko ajan, ensimmäinen löytäjä saa suuren pottin.

** Ajankohdassa 29:30 Iiro kysyi jountajilta, miten he ylläpitävät heidän osaamista. Mikon mukaan "hujarisyndrooma"
on hyvin yleistä tässä alalla. Kurinalaisuus ja ajankäyttö optimointi on Mikon mukaan paras ratkaisu.
Mikko itse lukee joka päivä 2 - 300 työkaluista liittyvää artikkeleita (taitolaji). Ei ole oikopolkkua.
Jokainen pitää kehittää oman ihmisarvon. Tomi sanoi puolestaan, että omat isot asettetut tavoitteet motivoi osaamista.
Mikko myös suosittelee lukea monipuolista, eikä vain yhtä kirjaa (eikä yhtä osa-alueeta). Esim. hän lukee
muun muassa kasinosta (ja heidän työntekjöiden epäluotamusta muihin), vaikka olisi itse IT ja tietoturvan asiantuntija.

** Hovimestari suositus: Iiro suosittelee yksilöllistä verkkotunnusta sähköpostiosoiteen palvelujen rekisteröintiin.
Lisäksi suositelttin "Irtoviiksi mies" kirja.

Lähteet: 

https://www.withsecure.com/fi/whats-new/podcasts/herrasmieshakkerit

|-> https://podcasts.apple.com/fi/podcast/valkohattuhakkerit-vieraana-iiro-uusitalo-0x01/id1479000931?i=1000451871015

---
---

### 2. Tutkimusartikkeli kybertappoketjusta.

![Jansson_Tunkistestaus_laksy_h1_x_tiivistelmät_02](https://github.com/user-attachments/assets/84c3b9cc-0f81-470b-a83d-28cfb6352406)


Tutkimusartikkelissa Eric M. Mutchins ym. esittävät/kertovat ...

Lähde: Hutchins, E. M., Cloppert, M. J., Amin, R. M. s.a. Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains. Lockheed Martin Corporation.  Luettavissa: https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf. Luettu: .

---
---

### 3. The Art of Hacking -videokokoelma.

![Jansson_Tunkistestaus_laksy_h1_x_tiivistelmät_03](https://github.com/user-attachments/assets/de9d9b53-cb64-4641-b3ae-611fe33c6dcf)

The Art of Hacking on kurssivideosarja, joka opastaa ja autaa opiskelijaa tietoturvan urakehityksessä. Opiskelija opii fundamentalit liityen eetiset hakkerointia ja tunkeutumistestauksen tekniikat. Tehtäväannon mukaan keskitymme sarjasta neljänteen oppituntiin: aktiivinen havannointi / kohdetiedostelu (eng. active recon).

#### Kommenteja
* Pitää ymmärtää passivinen recon ja aktiivinen recon erovaisuudet.
--> Passiivinen recon ei lähetä mitään paketteja suoraan kohdistetuun ympäristöön. On näkymätön lokitiedostolle (porttiskannaus).
--> Aktiivinen recon lähetää informaatioita kohdistetuun verkkoon. Hälyttää, kun joku tarkistaa lokitiedostot (porttiskannaus).
Tekee enemmän skannauksia kuten haavoittuvuus skannaukset, tällöin suoritaa enemmän toimintaa kuin pasiivinen (ts. paljon meluisempaa).

* Kohdeita on liian paljon ja on vain rajatettu aikaa. Kohdetiedostelu on avain, jolla voimme kohdistaa ääretön datasta oikeat systeemit ja palveluita mihin voimme hyökätä.

* Kohdetiedostelun metoodit ovat porttiskannaus, web palvelun arvostelu (Web Service Review) ja haavoittuvuus skannaus.

* Työkaluita on useita: Nmap, Masscan ja Udprotoscanner porttiskannaukselle, EyeWitness web palvelun arvosteluun, ja OpenVAS + Nikto haavoituvuus skannaukselle (sekä verkko että web palvelun). Videossa tehtiin myös harjoituksia (demoja).

Lähde:https://www.oreilly.com/videos/the-art-of/9780135767849/9780135767849-SPTT_04_00/

---
---

### 4. Finlex: Tietomuron vahingonkorvaus.

![Jansson_Tunkistestaus_laksy_h1_x_tiivistelmät_04](https://github.com/user-attachments/assets/2ed76bfb-6f4b-44cb-b2e5-344337f4f055)

Kyseessä on Suomen lain mukaan tietomurron yrityksen tunnusmerkistön täyttämisestä.
Kyseessä on vahingonkorvauksen sovittelemisesta.

Lähde:
https://finlex.fi/fi/oikeus/kko/kko/2003/20030036

---
---

## a) Kali Linux asennus Virtualboxiin.

Tehtävään suositeltiin Kali Linuxia Virtualboxissa käyttöä.

### Live iso -levykuva.

Koska Tero Karvisen Tunkeutumistestaus -sivustossa oleva linkki
https://cdimage.kali.org/kali-2021.1/kali-linux-2021.1-live-amd64.iso
on mennyt vanhaksi, joudun asentamaan suoraan Kalin orgaanisaation sivustolta,
https://www.kali.org/get-kali/#kali-live.

Linkin mukaan pitää asentaa live-amd64.iso -levykuvan versio Kali Linuxista,
joka näkyy alla olevassa kuvassa:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_01](https://github.com/user-attachments/assets/d5ee44e4-4648-466d-a0e6-7f4154993e03)

Toisin sanoen, meidän täytyy asentaa Linux Kaliin johonkin ulkoiseen muistivälineen kuten CD-ROM tai muistitikku.
Linux Foundation -sivuston Jack Wallen kirjottajan mukaan, Live Boot on siinä hyvä valinta, että voimme ajaa
Linuxin distrot muistivälineissä ilman minkäälaista muokausta tai tarvetta pääkoneen kiintolevyyn.

Koska ajomme suorittaa tunkeutumistestauksia Kali Linux, niin ymmärrän tietoturvan ja -suojan näkökulmasta
miksi opettaja suosittelee Live Boot -versio Kalista (mm. ettei minun laptopin kiintolevy kärsii vahingossa).
Lähde: https://www.linux.com/training-tutorials/live-booting-linux/.

### Formattointi käytössä oleva muistitikku.

Minulla sattui vanha Linux Mint -muistitikku, jonka pitkään aikaan käytänyt (sanotaan noin 2 vuotta).
Kyseessä on SanDisk 3.2Gen1 USB -muistikku. Koska muistitikkussa on jo Linux Mint distro,
joudun formattoimaan kokonaan muistitikkua.

Formattoinissa tapahtui semmoinen vika, että USB esintyy kaksi USB -ajuria (USB Driver D:/ ja E:/).
Google haulla sain seuraavan opastus, miten voin korjata vian Powershellissä:
https://gist.github.com/krisbolton/fc34ee629721d979f9f4275cba8dcfe5
Ohjeet korjaasi minun ongelmaani. Nyt USB:ssä on vain yksi USB -ajuri (USB Driver E:/).
Formattoin vielä yhden kerran USB -muistivälineen.
Virus-skannasin myös muistitikun F-Securen Safe avulla. Ei yhtäkään haitallista tiedostoja ja dataa.

Alla olevassa kuvassa on minun suoritus noudetuaan kyseiseen ohjeen:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_02](https://github.com/user-attachments/assets/4464671c-f096-4eb8-9b52-665a14fef55b)

Uusien lähteiden mukaan, kuten Sagar Sharma It's FOSS -sivustolta (https://itsfoss.com/virtualbox-boot-from-usb/), 
Virtualbox pystyy nykyään ajaa Live Boot iso -kuvakeet suoraan muistitikusta. Tämä oli uutta minulle,
koska aiemmassa Linux -kurssissa käytimme nimeomaan .ova tai itse Virtualbox version Linuxista (tarkkaan ottaen Ubuntu Server).

### Asennan vihdoin Kalin muistitikkuun.

Asennan vihdoin Linux Kalin Live Boot -version, ns. https://cdimage.kali.org/kali-2024.3/kali-linux-2024.3-live-amd64.iso,
muistitikkulleni. Se on kooltaan lähes 4,3 GB, mikä kyllä mahtuu 57 GB vapaa olevaan muistitikulle.

Kun Kali Linuxin iso -kuvakeen on ladattu "Downloads" -kansioon, niin konfiguroin sitä ensin
Oracle VM Virtualboxissa (Version 7.0.12 r 159484 (Qt5.15.2), 2023 Oracle) Tero Karvisen Linux
Debian asennusohjeen mukaisesti (https://terokarvinen.com/2021/install-debian-on-virtualbox/).
Varmistin myös toiselta lähteeltä kuten Nakivo Team, miten asennetaan Kali Linux
Virtualboxiin (https://www.nakivo.com/blog/how-to-install-kali-linux-on-virtualbox/).

Alla olevat kuvat todistavat tarkkaan Kali -asennuksen muistitikulleni

#### I) Luodaan uuden virtuaalikoneen.
Nimetään oikea tarkka nimen virtuaalikoneelle, kuten TeroKarvinenTunkeutumisTestausKaliLinux.
Tallenetaan se muistitikun virtualkoneiden hakemistoon, ja tuodaan ladatun live iso -kuvakeen
Kali Linuxista. Kuten Debian asennusohjeessa huomioitiin, "Skip Unattended Installation"
pitää olla valittu.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_03](https://github.com/user-attachments/assets/be7249db-64f4-43ac-9ead-dc937e038eaf)

#### II) Konfiguroidaan prosessin ja muistin.
Laitetaan noin 1 CPU ja 4000 MB Teron ohjeiden ja suosituksien mukaan.
Muut jätetään silleen (ts. ei muokata).

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_04](https://github.com/user-attachments/assets/fe2c8140-041a-4f54-9ade-7862bbeca72e)

#### III) Konfiguroidaan kiintolevyä.
Ohjeiden mukaan kiintolevyssä pitää olla minimi 20 GB, kun taas Teron ohjestuksessa
suositeltiin 60 GB. Noudataan Teron ohjeeta.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_05](https://github.com/user-attachments/assets/fcecd805-3d30-43ba-a03d-43dce6c8f779)

#### IV) Tarkistetaan yhteenveto ja hyväksytään painamalla "Finish".

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_06](https://github.com/user-attachments/assets/560adf21-1add-40d9-9f70-6cbabaa53501)


Näköjään Virtualbox kaatui kokonaan ennen kun pystyin asentamaan virtuaalikoneen.
Joudun toistamaan edelliset vaiheet uudestaan.

Toisen yrityksen jälkeen saimme luotuaan Kali Linux Live virtuaalikoneen,
nimeltään TeroKarvinenTunkeutumisTestausKaliLinux. Tässä auttoi sekin,
että ladattu Kali Live ISO -kuvake on myös muistitikkussa.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_07](https://github.com/user-attachments/assets/fed2f502-0e65-42be-9eea-4e5ea4feee23)

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_08](https://github.com/user-attachments/assets/e20a2148-f0cd-4dd6-a60a-2d152871694e)

Huomautus, että tallensin vahingossa virtuaalikoneen C:/ -kiintolevyyn vaikka se piti tallentaa muistitikkuun.
Onneksi ongelma pystyttiin helposti ratkaista painamalla hiiren oikealla "TeroKarvinenTunkeutumisTestausKaliLinux"
nimikettä Virtualboxia ja painaa "Move" taulukkosta. Se siirtää kaikki Virtualbox -tiedostot uuteen paikaan,
ja jättää vanhan paikan tyhjäksi.

Kun TeroKarvinenTunkeutumisTestausKaliLinux -virtuaalikone on nyt muistitikkussa, voin aina poista se Virtualbox taulukosta,
painamalla "Remove only" ja tuoda se uudestaan muistitikkusta klikkamalla "Add" (huomaa, että "Import" hakee vain .ova -tiedostot.
Minun tallentama virtuaalikone on .vbox -tiedosto!). Nyt voin rauhassa nukkua, ettei koneeni kiintolevyssä pyörii 
eikä fyysisesti tallenettu Kali Linuxin Live -virtuaalikone tunkeutumistestauken työkaluineen.

Koska **TeroKarvinenTunkeutumisTestausKaliLinux** on todella pitkä nimike joka kirjoituksessa,
lyhennän se jatkossa nimellä **TT Kali Linux** (TT tule tunkeutumistestauksesta).

### Käynnistetään Kali Linux.
Ajatessaan TT Kali Linux painamalla "Start" Virtualboxissa (katso kuva toiseksi edellinen kuva),
ilmestyy seuraava valikkonäyttö:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_09](https://github.com/user-attachments/assets/e8463fac-84b0-425b-87cf-5ad6ad31ddfb)

Valitsemme valikkosta ensimmäisen vaihtoehdon, "Live system (amd64)". Kestää hetken kun se käynnistyy.

Kun se on valmis, pääsin seuraavaan graafisen käyttöliitymään:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_10](https://github.com/user-attachments/assets/f7a32521-7011-4164-b077-1f5e25a65730)

## b) Verkkojen täydellinen irrotus TT Kali Linux -virtuaalikoneesta.

Ennen kun rupean aloita testauksen, Tero huomioi tärkeän Valkamon artikkelin lukemista
(tämä olisi pitänyt lukee, ennen kun olisin asentanut yhtäkään virtuaalikonetta):
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_11](https://github.com/user-attachments/assets/3d5cf22b-69fd-406c-8dff-16bd46bf4ddd)

Lähde: https://tuomasvalkamo.com/PenTestCourse/week-2/

Artikkelissa mainitiin tärkeät kohdat:
- **Pitää aina testata ja irota kaikki netit ennen todellista testausta!**
Artikkelissa mainitiin päätavat jolla varmistetaan että netti todella pois irrottu, mikä on myös tehtäväannon b -vaihe:
A) **Varmista TT Kali Linuxin Network asetuksesta (Virtualboxista), että
verkot ovat poistettu, ts. ruksa pois "Cable Connected".**

Avaan TT Kali Linuxin Network asetukset sillä välin kun se pyörii.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_11](https://github.com/user-attachments/assets/32c35945-f14e-446c-9c57-4539ad2d15f2)

Kuvasta näemme, että TT Kali Linux on vielä yhdistetty NAT -verkostoon, koska "Cable Connected" vielä päällä.
Laitan pois päältä ruksamalla sen pois.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_12](https://github.com/user-attachments/assets/c584890a-e507-4cb3-8981-83619a06acc8)


B) **Varmista omasta host-koneesta, että siltäkin on otettu kaikki netit pois!**
Tämä koskee sekä Ethernet että Wifi verkot. Minun täytyy tarkistaa sekä järjestelmähallinnasta Settings > Network & Internet,
alla oikeassa olevaa nettiyhteys pikakuvake että Powershellillä TestConnection, tarkkaan ottaen kommennolla
    Test-Connection -TargetName www.google.com -Traceroute

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_13](https://github.com/user-attachments/assets/cbb25a10-f244-479e-844b-8f8de425dab8)
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_14](https://github.com/user-attachments/assets/bc66611e-b314-456e-bc2e-cb0fd1c5f672)
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_15](https://github.com/user-attachments/assets/e6e6a3d9-fa15-4bc6-81e2-07cfc546772e)

Triplatarkistin Test-Connection kommentoa.

Lähde: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/test-connection?view=powershell-7.4

C) **ping 8.8.8.8** ja **ping www.google.com**
Kun kummastakaan ei tulee yhteyksiä, esim. "ping www.google.com: Temporary failure in name resolution" (Kali Linux)
ja "ping: unknown host www.google.com" (Metasploitable 2) niin nettiyhteys on pois suljettu.
Jos tulee yksikin yhteyslähetys, en saa missään nimessä tehdä testausta.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_16](https://github.com/user-attachments/assets/7199c377-d03a-4e71-ac0f-6add6438dea2)

Kuvasta näkee, että olen pinganut moneen kertaan (laskujen mukaan yli 6-8 kertaa) sekä 8.8.8.8 että www.google.com,
enkä saanut kummasta responsia. Eli verkko on suljettu pois TT Kali Linux virtuaalikoneesta ja saan suoritaa testausta.

Huomaa, että jatkoin kirjoittamista vasta kun suoritin testaukseen loppuun. Githubin on pois käytöstä,
kun suljin kaikki netit koneestani.

## c) Testaa nmap -kommentoa ja analysoi.

Kun olin aivan varmana, että kaikki netit ovat irrottu pois koneestani, suoritin seuraava porttiskannauksen kommentoa TT Kali Linuxissa:
    nmap -A localhost

Alla olevassa kuvassa näkyy tulokset:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_17](https://github.com/user-attachments/assets/57796dd2-4130-4d66-bd84-ce9a6a6103fe)

Kuvasta analysoin, ettei porttiskannaus pystynyt löytämään yhtäkään DNS palvelimia. Tämä on tarkoituskin, sillä
se todistaa virtuaalikoneessa ei ole toimivaa nettiä ja tällöin ei pääse mihinkään ulkoiseen palvelimeen.
Porttiskannaus ilmoittaa, että localhost (127.0.0.1) pääkone (host) on päällä (0,00044 sekunnilla viivellä).
Sitten porttiskannaus löysi muita osoitteet localhostille (joka ei ole skannattu)
mm. ::1, joka pikaisella Google haulla mukaan on kompressoitu formaatti IPV6 loopback
osoite (0:0:0:0:0:0:0:1). Toisin sanoen, se on IPV6 -osoiteversio localhostista
(joka on IPV4:ssä tuttu 127.0.0.1 -osoite).

Kaikki 1000 skannatut portit localhost ovat huomiotta tilassa eikä esittää
1000 suljetuja tcp porteja. Eli nmap -porttiskannauksen kommento pystyi 
skannamaan vain yhden 1 IP-osoiteen eli localhosti (jonka käyttää tällä yksi host -kone)
0,86 sekunnissa, mikä oli nopee. Mutta tämä oli tarkoituskin, koska meillä kaikki netti
pois päältä.

## d) Kahden daemon (demoniin) porttiskannauksen.
Tämä jäi valettavasti väliin, sillä pystyn asentamaan daemonit vain verkkon kautta.
Tämä tarkoitti, että joudun lopetamaan koko testauksen, asentaa kaikki netit takaisin
ja sitten käynnistä TT Kali TT uudestaan, asentaa demoniit, jne.

Tämä ei tekee hyvää minun pakko-oireinen häiriölleni. Lisäksi minulla ei ole paljonkaan
kokemusta daemonista, joten en lyhyessä ajassa pystynyt keksimään hyviä demonia.
Yritin kokeilla Someshwaran M. opastusta, mutta se osoittautui työläksi.
Lähde: https://somesh-rokz.medium.com/how-to-create-daemons-in-linux-with-a-simple-hello-world-bash-example-e739dea78284

Keskityn sen sijaan Metasploitable testaukseen.

## e) Metasploitable asennus.
Noudatin Valkamon ohjestusta asennettessaan Metasploitable 2.

Päivistys 31.10.2024, klo 22.21: En ehtinyt suorittaa Metasploitable asennuksen, sillä
Helgan Club Tuvalla oli klo 17 maissa torstaina 31.10.2024 Halloween tapahtuma,
johon lupaudin olemaan apukätenä tapahtuman järjestyksessä.
Pahoittelut.






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
-

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

### II) Konfiguroidaan prosessin ja muistin.
Laitetaan noin 1 CPU ja 4000 MB Teron ohjeiden ja suosituksien mukaan.
Muut jätetään silleen (ts. ei muokata).

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_04](https://github.com/user-attachments/assets/fe2c8140-041a-4f54-9ade-7862bbeca72e)

### III) Konfiguroidaan kiintolevyä.
Ohjeiden mukaan kiintolevyssä pitää olla minimi 20 GB, kun taas Teron ohjestuksessa
suositeltiin 60 GB. Noudataan Teron ohjeeta.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_05](https://github.com/user-attachments/assets/fcecd805-3d30-43ba-a03d-43dce6c8f779)

### IV) Tarkistetaan yhteenveto ja hyväksytään painamalla "Finish".

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_06](https://github.com/user-attachments/assets/560adf21-1add-40d9-9f70-6cbabaa53501)


Näköjään Virtualbox kaatui kokonaan ennen kun pystyin asentamaan virtuaalikoneen.
Joudun toistamaan edelliset vaiheet uudestaan.

Toisen yrityksen jälkeen saimme luotuaan Kali Linux Live virtuaalikoneen,
nimeltään TeroKarvinenTunkeutumisTestausKaliLinux. Tässä auttoi sekin,
että ladattu Kali Live ISO -kuvake on myös muistitikkussa.

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_07](https://github.com/user-attachments/assets/fed2f502-0e65-42be-9eea-4e5ea4feee23)

![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_08](https://github.com/user-attachments/assets/e20a2148-f0cd-4dd6-a60a-2d152871694e)




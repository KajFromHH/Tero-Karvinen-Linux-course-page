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

Koska Tero Karvisen Tunkeutumistestaus -sivustossa oleva linkki
https://cdimage.kali.org/kali-2021.1/kali-linux-2021.1-live-amd64.iso
on mennyt vanhaksi, joudun asentamaan suoraan Kalin orgaanisaation sivustolta,
https://www.kali.org/get-kali/#kali-live.

Linkin mukaan pitää asentaa live-amd64.iso -levykuvan versio Kali Linuxista,
joka näkyy alla olevassa kuvassa:
![Jansson_Tunkistestaus_laksy_h1_a_kalin_asennus_01](https://github.com/user-attachments/assets/d5ee44e4-4648-466d-a0e6-7f4154993e03)


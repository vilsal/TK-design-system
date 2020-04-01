
# Stat.fi Beta Design System <!-- omit in toc -->

## Sisällysluettelo <!-- omit in toc -->
- [Typografia](#typografia)
- [Kuvat](#kuvat)
  - [Hero-kuvat](#hero-kuvat)
- [Ikonit](#ikonit)
- [Värit](#v%c3%a4rit)
- [Sivupohja](#sivupohja)
  - [Navigaatio-palkki](#navigaatio-palkki)
  - [Megamenu](#megamenu)
  - [Sisältöalue](#sis%c3%a4lt%c3%b6alue)
  - [Sivuston tausta](#sivuston-tausta)
  - [Tekstipalsta](#tekstipalsta)
  - [Blokit](#blokit)
  - [Footer](#footer)
- [Komponentit](#komponentit)
  - [Jakoviiva](#jakoviiva)
  - [Haitari](#haitari)
    - [Haitarin ikonien tyylit](#haitarin-ikonien-tyylit)
  - [Kuviot](#kuviot)
  - [Laajennuspaneeli](#laajennuspaneeli)
  - [Linkit](#linkit)
    - [Sisäiset linkit](#sis%c3%a4iset-linkit)
    - [Negatiivi](#negatiivi)
    - [Linkki tekstin seassa](#linkki-tekstin-seassa)
    - [Linkit ikonilla](#linkit-ikonilla)
    - [Ulkoinen linkki](#ulkoinen-linkki)
  - [Murupolku](#murupolku)
  - [Painikkeet](#painikkeet)
    - [Ensisijainen painike](#ensisijainen-painike)
    - [Toisijainen painike](#toisijainen-painike)
    - [Kolmassijainen painike](#kolmassijainen-painike)
    - [Negatiivi-painike](#negatiivi-painike)
    - [Painikkeet mobiilissa](#painikkeet-mobiilissa)
  - [Pudotusvalikot](#pudotusvalikot)
    - [Yhden valinnan](#yhden-valinnan)
    - [Useamman valinnan (multi select)](#useamman-valinnan-multi-select)
  - [Pääkohdat](#p%c3%a4%c3%a4kohdat)
  - [Tagit](#tagit)
    - [Tyyppi-tagi](#tyyppi-tagi)
  - [Taulukot](#taulukot)
  - [Videot](#videot)

## Typografia
Fontteina käytetään Googlen ilmaisia fontteja. Vaikka osa fonttien ko'oista on tässä ilmoitettu pikseleinä, ne tulee toteuttaa suhteellisina arvoina (em tai rem). 

| Taso             | Font                     | Font-size     | Font-family                                                    |
| ---------------- | ------------------------ | ------------- | -------------------------------------------------------------- |
| Leipäteksti      | Source Sans Pro, regular | 16px/1rem     | Source Sans Pro, Arial, Verdana, Lucida, Helvetica, Sans-serif |
| Leipäteksti, iso | Source Sans Pro, regular | 18px          |
| H1               | Barlow, regular          | 34px          |
| H2               | Barlow, regular          | 28px          |
| H3               | Barlow, regular          | 22px          |
| H4               | Barlow, medium           | 16px          |
| H5               | Barlow, medium           | 14px          |
| Ingressi         | Barlow regular           | 17px/1.255rem |
| Introteksti      | Barlow, medium           | 14px          |


## Kuvat
### Hero-kuvat
Mobiilissa hero-kuva ulottuu näytön laidasta laitaan. Mobiilinäytöllä näkyy täysikokoisesta kuvasta rajattu tietty kohta. (Kohta määritellään myöhemmin tarkemmin.)

Desktopissa hero-kuva ulottuu näytön laidasta laitaan kunnes kuvan koko tulee vastaan. Sen jälkeen kuvan vasemmalle ja oikealle puolelle tulee marginaalit. Kuva-alueen korkeus pysyy samana koko ajan ja kuva rajautuu korkeudesta näytön koon kasvaessa. 
	
Hero-kuviksi valitaan sellaisia, jotka toimivat monessa koossa. 

## Ikonit

Ikoneina käytetään (jo aiemmin käytössä olleita) Font Awesomen ja IcoMoonin ilmaisia ikonikirjastoja. 

## Värit
Väreinä käytetään Tilastokeskuksen väripalettia. (Värien kontrastitarkistusta pitää tehdä ja palettia päivittää!) 

## Sivupohja
	
### Navigaatio-palkki
| Max-width | Sisältöalueen leveys | Background-color |
| --------- | -------------------- | ---------------- |
| 2500px    | 1200px               | #0073b0          |

Navigaatio-palkin taustan leveys on näytön/selainikkunan laidasta laitaan 2500px asti. Siitä ylöspäin navipalkin oikealle ja vasemmalle puolelle tulee marginaalit. 
*Poikkeus:* 
Jos ollaan sivulla, jossa on bannerikuva (aiheen ja tarkennetun aiheen sivuilla): navipalkin tausta on näytön laidasta laitaan kunnes bannerikuvan rajat tulevat vastaan: navipalkki loppuu siinä missä bannerikuvakin. 

Navipalkin sisältöalue on leveydeltään 1200px eli sama kuin muukin sisältöalue. Navipalkin sisältö pysyy sisältöalueen sisällä, se ei leviä taustan mukana näytön koon kasvaessa. Navipalkin sisältö on samassa linjassa sivun muun sisällön kanssa eli alkaa vasemmassa laidassa samasta kohdasta kuin sivuston muukin sisältö. 

| Font          | Font-size | Color     | Font-variant | Text-decoration | Padding                                                                      |
| ------------- | --------- | --------- | ------------ | --------------- | ---------------------------------------------------------------------------- |
| Barlow medium | 1.1rem    | valkoinen | normal       | none            | padding-left ja padding-right: 1.5rem, padding-top ja padding-bottom: 1.2rem |
			
Navigaatiopalkin painikkeiden välissä on ohuet pystyviivat, viivojen korkeus sama kuin navipalkin korkeus: 
| Width | Color   |
| ----- | ------- |
| 1px   | #338fc0 |

Navipalkin sisällön tasaus: vasen. Sisältö ei levity tasaisesti koko navipalkin alueelle vaan on tasattu sisältöalueen vasempaan laitaan. 

### Megamenu
Megamenun sisältö keskitetty vasempaan laitaan.  

### Sisältöalue
Pikseleistä lasketaan rem-arvot tai %-osuudet. 

|             | Leveys | Palstoja max | Sisällön tasaus |
| ----------- | ------ | ------------ | --------------- |
| **Desktop** | 1200px | 3            | vasen           |
| **Mobiili** |        | 1            | vasen           |

Sisältöalueen maksimileveys desktopissa on 1200px. Sisältöalueen sisältö on tasattu vasemmalle. Sisältöalue on jaettu desktopissa maksimissaan kolmeen palstaan ja mobiilissa yhteen palstaan. Desktopin kolme palstaa asettuvat responsiivisesti allekkain näytön/selainikkunan pienentyessä. 

### Sivuston tausta
| Background|
| ----- |
| valkoinen, 2% musta |


	
### Tekstipalsta
|             | Width |
| ----------- | ----- |
| **Desktop** | 555px |
| **Mobiili** |       |

### Blokit
|             | Background-color    | Margin        | Padding                                                                                                                                |
| ----------- | ------------------- | ------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Desktop** | valkoinen, 2% musta | 2.5rem (40px) | 2.5rem (40px)                                                                                                                          |
| **Mobiili** | valkoinen, 2% musta | 2.5rem (40px) | **Padding-top** ja **padding-bottom**: puolet desktopin paddingista. **Padding-left** ja **padding-right**: 1/4 desktopin paddingista. |

### Footer 

| Max-width | Sisältöalueen leveys | Background-color |
| --------- | -------------------- | ---------------- |
| 2500px    | 1200px               | #0073b0          |
		
Footerin tausta ulottuu aina laidasta laitaan, sekä isoissa että pienissä näytöissä/selainikkunoissa. 
Isoissa desktop-näytöissä 2500px leveyteen asti koko näytön levyinen, siitä ylöspäin tulee marginaalit. Eli footerin tausta käyttäytyy deskarissa kuten yläpalkin ja navipalkin tausta. 
	
Footerin sisältöalue on leveydeltään 1200px eli sama kuin muukin sisältöalue.

Neljä palstaa: ensimmäisessä Tilastokeskuksen logo, kolme muuta linkkipalstoja. Tarvittaessa näytön/selainikkunan pienentyessä palstat hyppäävät kokonaan toiselle riville ensimmäisen rivin palstojen alle. 

## Komponentit

### Jakoviiva
Ensisijaisesti eri osioiden erottamiseen toisistaan tulee käyttää tyhjää tilaa. Niissä tilasteissa, joissa tyhjää tilaa ei voida käyttää, käytetään jakoviivoja.  

![Jakoviiva](images/divider.png)

| Height | Color   |
| ------ | ------- |
| 1px    | #aaaaaa |

Jakoviivoja voidaan käyttää asioiden ryhmittelyyn asettamalla niitä eri ryhmien väliin, esim menuissa. 

Jakoviivoilla voidaan myös erottaa saman kokonaisuuden/toisiinsa liittyviä asioita toisistaan. 

![Jakoviiva erottamassa toisiinsa liittyviä asioita.](images/divider_example1.png)

### Haitari 

Haitari-rakenteella saadaan lyhennetty sivun pituutta. Haitarin sisällön tulee muodostaa yhtenäinen kokonaisuus. 

![Avattu haitari-elementti, mobiiliversio.](images/haitari.png)

Haitari on enintään kaksi tasoa syvä. Sisempi taso on sisennetty ensimmäisen alle, tällä ilmaistaan haitarin hierarkinen rakenne. Suljettujen kohtien kohdalla on plus-ikoni, joka muuttuu miinus-ikoniksi kun kohta avataan. Avatun kohdan alle tulee jakoviiva. 

Plus-ja miinus-ikonit ovat suurempia ja tummempia ensimmäisellä tasolla ja pienempiä ja vaaleampia syvemmällä tasolla. Myös tällä kerrotaan visuaalisesti hierarkiasta. 

#### Haitarin ikonien tyylit

| Hierarkiataso | Height | Width | Color    |
| ------------- | ------ | ----- | -------- |
| Ensimmäinen   | 15px   | 15px  | #0073b0  |
| Toinen        | 11px   | 11px  | #338FC0F |

### Kuviot

|             | Font |
| ----------- | ---- |
| **Otsikko** | H4   |

### Laajennuspaneeli 
(Eng. expansion panel)

Esim. Videon käsikirjoitus -laajennuspaneeli

| Font | 
| ---------- | 
| Leipäteksti    | 
	
### Linkit

Kaikki linkit toimivat näppäimistökäytössä vain enterillä. 

#### Sisäiset linkit

| Tila           | Font        | Text-decoration | Color   | Muuta                                 |
| -------------- | ----------- | --------------- | ------- | ------------------------------------- |
| **Tavallinen** | Leipäteksti | none            | #006CA5 |                                       |
| **Hover**      |             | underline       | #0039a6 | Kursori muuttuu kädeksi linkin päällä |
| **Focus**      |             | underline       | #0039a6 | Reunus: 2px, #0073b0                  |
| **Vierailtu**  |             | none            | #551A8B |                                       |

Tavallinen-tila:
![Tavallinen linkki.](images/link.png)

Hover-tila:
![Linkin hover-tila.](images/hover_link.png)

Focus-tila:
![Kohdistettuna oleva linkki.](images/focus_link.png)

Vierailtu-tila:
![Vierailtu linkki.](images/visited_link.png)

#### Negatiivi

Negatiivinen linkki on linkki tummalla taustalla. 

| Tila           | Font        | Text-decoration | Color     | Muuta                                 |
| -------------- | ----------- | --------------- | --------- | ------------------------------------- |
| **Tavallinen** | Leipäteksti | none            | valkoinen |                                       |
| **Hover**      |             | underline       | valkoinen | Kursori muuttuu kädeksi linkin päällä |
| **Focus**      |             | underline       | valkoinen | Reunus: 2px, valkoinen                |
| **Vierailtu**  |             | none            | valkoinen |                                       |

Tavallinen-tila:
![Tavallinen negatiivinen linkki.](images/negative_link.png)

Hover-tila:
![Negatiivinen linkki hover-tilassa.](images/negative_hover_link.png)

Focus-tila:
![Negatiivinen linkki kohdistettuna.](images/focus_negative_link.png)

Vierailtu-tila:
![Vierailtu negatiivinen linkki.](images/negative_link.png)


#### Linkki tekstin seassa

Tekstin seassa, eli p-elementin sisällä, olevat linkit alleviivataan aina. Muissa linkeissä ei ole alleviivausta. 

| Tila           | Font        | Text-decoration |
| -------------- | ----------- | --------------- |
| **Tavallinen** | Leipäteksti | underline       |


![Tekstin seassa olevat linkit alleviivataan.](images/linkkip.png)

#### Linkit ikonilla

![Linkkejä ikonien kanssa.](images/icons_link.png)

Ikoni tulee linkin eteen (poikkeuksena ulkoinen linkki, jossa ikoni tulee tekstin jälkeen) ja on samanvärinen kuin linkin teksti. Ikoni on osa linkkiä. 

![Nuoli linkin perässä korostaa sitä, että linkistä tapahtuu jotain.](images/linkki_nuoli.png)

![Nuoli linkin perässä, negatiivinen linkki.](images/negative_link_icon.png)

Yksittäisessä erillään olevassa linkissä linkin perässä oleva nuoli korostaa, että linkistä tapahtuu jotain. Nuoli on aina linkin perässä. Nuoli-ikoni ei ole osa linkkiä, siitä klikkaamalla ei tapahdu mitään. 

![Linkillä voi olla kaksi ikonia.](images/link_kaksi_ikonia.png)

Linkeillä voi olla myös kaksi ikonia. Ikonit asettuvat silloin joko linkkitekstin molemmille puolille tai peräkkäin tekstin jälkeen (ks. ulkoinen linkki). 

| Ikoni                | Color     |
| -------------------- | --------- |
| **Nuoli**            | #0073b0   |
| **StatFin/database** | #f59a23   |
| **Muu**              | musta     |
| **Negatiivi**        | valkoinen |

#### Ulkoinen linkki

![Ulkoiseen palveluun vievä linkki.](images/ulkoinen_link.png)

Ulkoiseen palveluun vievän linkin perässä on ulkoisen linkin ikoni. Tämä ikoni on osa linkkiä. Linkin tekstissä tulee kertoa, että linkki vie toiseen palveluun. 

![Ulkoiseen palveluun vievä linkki.](images/ulkoinen_link_kaksi_ikonia.png)

Ulkoisella linkillä voi olla myös kaksi ikonia. Ikonit asettuvat silloin peräkkäin. 

### Murupolku

 Murupolun osat viimeistä lukuunottamatta ovat linkkejä ja ne noudattavat H5-otsikkotason fonttia sekä tavallisen linkin tyyliä. Murupolun viimeinen kohta ei ole linkki. 
 
 Osiot erotetaan toisistaan /-merkillä. 
	
Vaikka murupolku noudattaa H5-tason fonttia, se ei ole semanttisesti H5-tason otsikko vaan navigaatio-elementti. 

| Murupolun osa | Font           | Font-size | Color   | Text-decoration |
| ------------- | -------------- | --------- | ------- | --------------- |
| Linkki        | Barlow, medium | 14px      | #006ca5 | none            |
| Viimeinen     | Barlow, medium | 14px      | musta   | none            |

**Murupolku desktopissa** 

Desktopissa näytetään murupolussa kaikki tasot: 

![Murupolku desktopissa.](images/murupolku.png)
	
**Murupolku mobiilissa**

Mobiilissa matalilla sivuston hierarkian tasoilla (n. kaksi ensimmäistä tasoa) näytetään normaali murupolku: 

![Murupolku mobiilissa ylemmillä hierarkian tasoilla.](images/murupolku_mobiili1.png)

Syvämmällä hierarkian tasoilla murupolussa näytetään vain linkki yhtä tasoa hierarkiassa ylemmäs. Näin estetään murupolun rivittyminen mobiilissa. Esim. tilastojulkistus-sivun murupolussa näkyy vain linkki tilaston sivulle:

![Murupolku mobiilissa syvemmillä hierarkian tasoilla.](images/murupolku_mobiili2.png)

|                                             | Murupolun muoto                                                              |
| ------------------------------------------- | ------------------------------------------------------------------ |
| **Desktop**                                 | Tilastotieto / Suomalaisten matkailu / Tilastojulkistus / Taulukko |
| **Mobiili (matalilla hierarkian tasoilla)** | Tilastotieto / Suomalaisten matkailu                               |
| **Mobiili (syvillä hierarkian tasoilla)**   | < Tilastojulkistus                                                 |

### Painikkeet

![Painikkeiden eri tilat.](images/buttons.png)

**Yhteiset ominaisuudet**
|Font|Border-radius|Min-width|Min-height|Focus-kehys|
|-|-|-|-|-|
|Source Sans Pro, regular, 16px/1rem|5px|80px|40px|2px, #0073b0|

#### Ensisijainen painike

![Ensisijaisen painikkeen eri tilat.](images/primary_buttons.png)

|Tila|Color|Background-color|Border|Box-shadow|
|-|-|-|-|-|
|**Tavallinen**|valkoinen|#0073b0|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Selected/pressed**|valkoinen|#0073b0|-|2px, 2px, 5px, rgba(5,3,112,0.35) inset|
|**Disabled**|#666666|#f2f2f2|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Hover**|valkoinen|#338fc0|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Focus**|valkoinen|#338fc0|-|2px, 2px, 5px, rgba(102,102,102,0.35)|

#### Toisijainen painike

![Toissijaisen painikkeen eri tilat.](images/secondary_buttons.png)

|Tila|Color|Background-color|Border|Box-shadow|
|-|-|-|-|-|
|**Tavallinen**|#0073b0|valkoinen|#0073b0|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Selected/pressed**|#0073b0|valkoinen|#0073b0|2px, 2px, 5px, rgba(102,102,102,0.35) inset|
|**Disabled**|#7f7f7f|valkoinen|#aaaaaa|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Hover**|#0073b0|#f2f2f2|#0073b0|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Focus**|#0073b0|#f2f2f2|#0073b0|2px, 2px, 5px, rgba(102,102,102,0.35)|

#### Kolmassijainen painike

![Kolmassijaisen painikkeen eri tilat.](images/tertiary_buttons.png)

|Tila|Color|Background-color|Border|Box-shadow|
|-|-|-|-|-|
|**Tavallinen**|#0073b0|#f2f8fb|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Selected/pressed**|#0073b0|#f2f8fb|-|2px, 2px, 5px, rgba(102,102,102,0.35) inset|
|**Disabled**|#666666|#f2f2f2|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Hover**|musta|#f2f8fb|-|2px, 2px, 5px, rgba(102,102,102,0.35)|
|**Focus**|musta|#f2f8fb|-|2px, 2px, 5px, rgba(102,102,102,0.35)|

#### Negatiivi-painike

![Negatiivi-painikkeen eri tilat.](images/negative_buttons.png)

|Tila|Color|Background-color|Border|Box-shadow|
|-|-|-|-|-|
|**Tavallinen**|#0073b0|valkoinen|#0073b0|4px, 4px, 5px, rgba(85,85,85,0.35)|
|**Selected/pressed**|#0073b0|valkoinen|#0073b0|2px, 2px, 5px, rgba(102,102,102,0.35) inset|
|**Disabled**|#7f7f7f|valkoinen|#aaaaaa|4px, 4px, 5px, rgba(85,85,85,0.35)|
|**Hover**|#0073b0|#f2f2f2|#0073b0|4px, 4px, 5px, rgba(85,85,85,0.35)|
|**Focus**|?|?|?|?|

#### Painikkeet mobiilissa

![Painikkeet mobiilissa.](images/buttons_mobile.png)

Mobiilissa painikkeet ovat lähes täysleveitä lukuunottamatta niiden oikealle ja vasemmalle puolelle jääviä marginaaleja. 

### Pudotusvalikot 

(Eng. dropdown)

Pudotusvalikoilla on aina label. 

#### Yhden valinnan

#### Useamman valinnan (multi select)	

### Pääkohdat

Pääkohdat, esim. tilastojulkistuksen sivulla. 

Fontti: ingressi-tyyli, #00B2A9

Sisennys: riippuva sisennys eli teksti sisentyy palleron oikealle puolelle, kaikki rivit samassa linjassa. 

Pallon väri: #00B2A9

Vasen pystyviiva: #00B2A9. Pystyviivaa ei ole mobiilissa.

### Tagit

#### Tyyppi-tagi
= Tyyppitagi Tilasto-, Tilastojulkistus- ja Muutoksia tässä tilastossa -sivujen yläosassa. 

Fontti: Barlow medium 14px, #333333

### Taulukot
Otsikon fontti: H4-tyyli
Fontti: Barlow Semi Condensed regular

Sarake- ja riviotsikoiden fonttityyli: Barlow Semi Condensed SemiBold

Solun padding-left ja padding-right: 10px

Solun padding-top ja padding-bottom: 8px

### Videot
Otsikon fontti: H4-tyyli



	


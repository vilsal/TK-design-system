
# Stat.fi Beta Design System

Sisällysluettelo:
[Typografia](#typografia)
[Kuvat](#kuvat)
[Ikonit](#ikonit)
[Värit](#värit)
[Sivupohjat](#sivupohjat)
[Komponentit](#komponentit)

## Typografia
Fontteina käytetään Googlen ilmaisia fontteja. 
### Otsikot
Fontti: Barlow
H1 Barlow, regular 34px
H2 Barlow, regular 28px
H3 Barlow, regular 22px
H4 Barlow, medium 16px
H5 Barlow, medium 14px
	
### Leipäteksti
Fontti: Source Sans Pro, regular 16px = 1rem
Font-family: Source Sans Pro, Arial, Verdana, Lucida, Helvetica, Sans-serif;
	
### Ingressi
Fontti: Barlow regular, 17px/1.255rem

### Sivun esittelyteksti 
Aihe- ja ilmiö-sivuilla
Fontti: Barlow regular, 17px/1.255rem
	
### Kuvion, taulukon ja videon otsikko
Fontti: H4-tyyli
	
### Yhteystiedot/Asiantuntijat-blokki
Titteli: leipätekstin tyyli
Nimi: Source Sans Pro regular, 18px
Puhelinnumero: leipätekstin tyyli

## Kuvat
### Herokuvat
Mobiilissa näytön laidasta laitaan, tietty kohta (määritellään tarkemmin) kuvasta rajattu näkymään. 

Desktopissa näytön laidasta laitaan kunnes kuvan koko tulee vastaan. Kuva-alueen korkeus pysyy samana koko ajan ja kuva rajautuu korkeudesta näytön koon kasvaessa. 
	
Kuviksi valitaan sellaisia, jotka toimivat monessa koossa. 

## Ikonit

## Värit

## Sivupohjat
	
### Navigaatio-palkki
#### Navigaatio-palkin tausta
Taustan väri: #0073b0
			
Navigaatio-palkin taustan leveys on näytön/selainikkunan laidasta laitaan 2500px asti. Siitä ylöspäin tulee marginaalit. 
*Poikkeus:* 
Jos ollaan sivulla, jossa on bannerikuva (aiheen ja tarkennetun aiheen sivuilla): navipalkin tausta on näytön laidasta laitaan kunnes bannerikuvan rajat tulevat vastaan: navipalkki loppuu siinä missä bannerikuvakin. 
			
#### Navigaatio-palkin sisältö
Fontti: Barlow medium, 1.1rem, valkoinen, pienaakkoset, ei alleviivausta 
Fontin padding-left ja padding-right: 1.5rem 
Fontin padding-top ja padding-bottom: 1.2rem 
			
Navigaatiopalkin painikkeiden välissä on ohuet 1px #338fc0 pystyviivat, viivojen korkeus sama kuin navipalkin korkeus. 
			
Navipalkin sisältöalue on leveydeltään 1200px eli sama kuin muukin sisältöalue. Navipalkin sisältö pysyy sisältöalueen sisällä, se ei leviä taustan mukana näytön koon kasvaessa. 

Sisällön tasaus: vasen. Sisältö ei levity tasaisesti koko navipalkin alueelle vaan pysyy vasemmassa laidassa. 
Navipalkin sisältö alkaa vasemmassa laidassa samasta kohdasta kuin sivuston muukin sisältö eli ne ovat samassa linjassa. 

### Megamenu
Megamenun sisältö keskitetty vasempaan laitaan. 
Megamenujen sisällöissä (linkeissä) alleviivaus. 

### Sisältöalue
Pikseleistä lasketaan rem-arvot tai %-osuudet. 
		
Sisältöalueen sisältö on tasattu vasemmalle. 
	
Desktop: 
Sisältöalueen leveys: 1200px
Sisältöalue on jaettu desktopissa maksimissaan kolmeen palstaan. 
		
Mobiili:
Mobiilissa on vain yksi palsta. Desktopin kolme palstaa asettuvat responsiivisesti allekkain näytön/selainikkunan pienentyessä. 

### Tausta
Koko sivuston background: valkoinen, 2% musta
	
### Tekstipalsta
Desktop: 
Tekstipalstan leveys: 555px

Mobiili: 

### Blokit
Taustaväri: valkoinen, 2% musta

Desktop:
Marginaali: 40px; 2.5rem
Padding: 40px; 2.5rem

Mobiili:
Marginaali: noudattaa toistaiseksi desktopin marginaaleja. 
Padding-top ja padding-bottom: puolet desktopin paddingista. 
Padding-left ja padding-right: 1/4 desktopin paddingista. 

### Footer
Footerin tausta ulottuu aina laidasta laitaan, sekä isoissa että pienissä näytöissä/selainikkunoissa. 
Isoissa desktop-näytöissä 2500px leveyteen asti koko näytön levyinen, siitä ylöspäin tulee marginaalit. Eli footerin tausta käyttäytyy deskarissa kuten yläpalkin ja navipalkin tausta. 
	
Footerin sisältöalue on leveydeltään 1200px eli sama kuin muukin sisältöalue. 
	
Footerin tausta tk-sininen: #0073b0 
Footerin linkit linkkityyleillä. 
		
Neljä palstaa: ensimmäisessä Tilastokeskuksen logo, kolme muuta linkkipalstoja. Tarvittaessa näytön/selainikkunan pienentyessä palstat hyppäävät kokonaan toiselle riville ensimmäisen rivin palstojen alle. 

## Komponentit

### Laajennuspaneeli (expansion panel)
Esim. Videon käsikirjoitus -laajennuspaneeli
Fontti: Source Sans Pro, regular 16px
	
### Linkit
Kaikki linkit alleviivataan, myös murupolun ja megamenun linkit. 
	
#### Sisäinen linkki
Fontti: leipätekstin tyyli, alleviivattu
Väri: #0073b0; R0 G115 B176

#### Ulkoinen linkki:
Tyyliltään sama kuin sisäinen linkki. Linkin perässä on ulkoisen linkin ikoni. Linkin tekstissä tulee kertoa, että linkki vie toiseen palveluun. 

### Murupolku
Murupolun viimeinen kohta ei ole linkki. Muut kohdat ovat ja ne ovat siksi alleviivattuja. 
	
Fontti: H5-tyylit. Semanttisesti ei H5-tason otsikko vaan navigaatio-elementti. 
	
Desktop: 
Kaikki tasot näkyvissä: 
Etusivu >  Liikenne ja matkailu >  Suomalaisten matkailu > Tilastojulkistus
	
Mobiili: 
Korkealla sivuston hierarkian tasolla näytetään normaali murupolku: 
Etusivu > Liikenne ja matkailu
Syvän hierarkian tasolla murupolussa näytetään vain linkki edelliselle tasolle. Esim. tilastojulkistus-sivun murupolussa näkyy linkki tilaston sivulle: 
< Suomalaisten matkailu

### Painikkeet

### Pudotusvalikot (dropdownit)
Pudotusvalikoilla on aina label. 

#### Yhden valinnan:

#### Useamman valinnan (multi select):

### Pääkohdat tilastojulkistuksessa
Fontti: ingressi-tyyli, #00B2A9
Sisennys: riippuva sisennys eli teksti sisentyy palleron oikealle puolelle, kaikki rivit samassa linjassa. 
Pallon väri: #00B2A9
Vasen pystyviiva: #00B2A9. Pystyviivaa ei ole mobiilissa. 	

### Taulukot
Fontti: Barlow Semi Condensed regular
Sarake- ja riviotsikoiden fonttityyli: Barlow Semi Condensed SemiBold
Solun padding-left ja padding-right: 10px
Solun padding-top ja padding-bottom: 8px

### Tyyppi-tagi
= Tyyppitagi Tilasto-, Tilastojulkistus- ja Muutoksia tässä tilastossa -sivujen yläosassa. 
Fontti: Barlow medium 14px, #333333
	


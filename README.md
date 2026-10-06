# Episode Player

Yksinkertainen selainsoitin MP3-tiedostoille ja podcasteille. Soitin muistaa, mihin kohtaan jäit, joten voit pysäyttää kuuntelun ja jatkaa myöhemmin samasta kohdasta, vaikka seuraavana päivänä.

**Osoite:** https://ehken.github.io/player/

## Ominaisuudet

- Toisto ja tauko
- Hyppy 20 sekuntia taakse- tai eteenpäin
- Kelauspalkki
- Toistonopeus 0,8×–2×
- **Muistaa kohdan:** sijainti tallentuu 5 sekunnin välein ja aina kun toisto pysähtyy, esimerkiksi kun otat kuulokkeet pois
- **Viimeisimmät:** lista viimeisimmistä jaksoista ja kohdista, joihin jäit
- Kuulokkeiden ja lukitusnäytön painikkeet toimivat (play/tauko, ±20 s)
- Pikanäppäimet tietokoneella: `välilyönti` = toisto/tauko, `←` `→` = 20 s

## Käyttö

1. Avaa https://ehken.github.io/player/
2. Liitä MP3-tiedoston osoite kenttään ja paina **Load**.
3. Kuuntele. Kun avaat soittimen myöhemmin uudelleen, valitse jakso **Recent**-listasta, niin toisto jatkuu siitä, mihin jäit.

Puhelimessa kannattaa lisätä soitin aloitusnäyttöön, niin se aukeaa kuin sovellus.

## Kirjanmerkki: jakso suoraan artikkelista soittimeen

Monella sivulla podcast-jakson MP3-osoite ei näy suoraan, varsinkaan jos jakso on maksumuurin takana. Kirjanmerkki hoitaa tämän puolestasi. Kun painat sitä sivulla, jolla jakso on, se etsii sivulta jakson MP3-osoitteen ja avaa sen suoraan soittimessa.

**Miksi kirjanmerkki?** Maksumuurin takana MP3-osoite näkyy vain kirjautuneelle käyttäjälle. Siksi haun täytyy tapahtua sinun omassa selaimessasi, jossa olet jo kirjautunut. Kirjanmerkki ei lähetä tunnuksiasi tai muita tietoja minnekään, vaan se vain lukee MP3-osoitteen avoimelta sivulta ja avaa sen soittimessa.

### Kirjanmerkin koodi

Kopioi koko rivi:

```
javascript:(()=>{let u=[...document.querySelectorAll('audio,audio source')].map(e=>e.currentSrc||e.src).find(s=>/\.mp3/i.test(s));if(!u){const m=document.documentElement.innerHTML.match(/https?:(?:\\?\/){2}[^"'\s<>]+?\.mp3[^"'\s<>]*/i);if(m)u=m[0]}if(!u){alert('MP3-linkkiä ei löytynyt. Paina ensin play sivun soittimessa ja kokeile uudelleen.');return}u=u.replace(/\\\//g,'/').replace(/&amp;/g,'&');location.href='https://ehken.github.io/player/?url='+encodeURIComponent(u)})()
```

### Asennus

**iPhone (Brave tai Safari)**
1. Avaa mikä tahansa sivu ja lisää se kirjanmerkkeihin.
2. Avaa kirjanmerkit, paina uutta kirjanmerkkiä pitkään ja valitse **Muokkaa**.
3. Korvaa kirjanmerkin osoite yllä olevalla koodilla.

**Android (Chrome)**
1. Lisää mikä tahansa sivu kirjanmerkkeihin.
2. Muokkaa kirjanmerkkiä ja korvaa sen osoite yllä olevalla koodilla.

**Tietokone (Chrome, Brave, Edge, Safari)**
1. Näytä kirjanmerkkipalkki (Chromessa ja Bravessa `Ctrl/Cmd + Shift + B`).
2. Klikkaa palkkia hiiren oikealla painikkeella → **Lisää sivu** / **Add page**.
3. Liitä kirjanmerkin osoitteeksi yllä oleva koodi.

Jos sama selain on synkronoitu tietokoneen ja puhelimen välillä (esim. Brave Sync tai Chrome Sync), kirjanmerkki siirtyy puhelimeen itsestään.

### Käyttö

1. Avaa sivu, jolla podcast-jakso on. Jos jakso on maksumuurin takana, varmista, että olet kirjautunut.
2. Käynnistä kirjanmerkki:
   - **iPhone:** avaa kirjanmerkit ja napauta kirjanmerkkiä.
   - **Android Chrome:** kirjoita osoiteriville kirjanmerkin nimi ja valitse se ehdotuksista. Kirjanmerkkilistasta napauttaminen ei toimi Chromessa.
   - **Tietokone:** klikkaa kirjanmerkkiä kirjanmerkkipalkista.
3. Soitin aukeaa ja lataa jakson. Paina play.

### Jos se ei toimi

- **"MP3-linkkiä ei löytynyt":** paina ensin play sivun omassa soittimessa ja käynnistä kirjanmerkki sitten uudelleen. Joillain sivuilla äänitiedoston osoite ilmestyy vasta toiston alkaessa.
- **Ei tapahdu mitään:** tarkista, että kirjanmerkin osoite alkaa sanalla `javascript:` ja että koodi on kopioitu kokonaan. Jotkin selaimet poistavat `javascript:`-alun liitettäessä, joten kirjoita se tarvittaessa käsin.
- **Et ole kirjautunut:** maksumuurin takana olevaa jaksoa ei löydy ilman kirjautumista.

## Yksityisyys

- Kuunteluhistoria ja kohdat tallentuvat **vain omaan selaimeesi**, eikä niitä lähetetä minnekään. Muut soittimen käyttäjät eivät näe historiaasi.
- Historia säilyy, kunnes tyhjennät selaimen tiedot. iPhonen Safarissa sivuston tiedot voivat poistua, jos sivulla ei käy 7 päivään. Aloitusnäyttöön lisätyssä soittimessa tätä rajoitusta ei ole.
- Eri laitteet eivät jaa historiaa: puhelimella ja tietokoneella on kummallakin oma historiansa.

## Tekniikka

Yksi HTML-tiedosto (`index.html`), jossa ei ole palvelinta, kirjastoja eikä seurantaa. Soitin toimii GitHub Pagesissa. Jakson voi avata suoraan linkillä muodossa `https://ehken.github.io/player/?url=<MP3-osoite>`.

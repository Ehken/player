# Episode Player

Yksinkertainen selainsoitin MP3-tiedostoille ja podcasteille. Soitin muistaa, mihin kohtaan jäit, joten voit pysäyttää kuuntelun ja jatkaa myöhemmin samasta kohdasta, vaikka seuraavana päivänä.

**Osoite:** https://ehken.github.io/player/

## Ominaisuudet

- Toisto ja tauko, kelauspalkki
- Hyppy taakse- tai eteenpäin, pituus valittavissa: 10, 15, 20 tai 30 s
- Toistonopeus 0,8×–2×
- **Muistaa kohdan:** sijainti tallentuu 5 sekunnin välein ja aina kun toisto pysähtyy, esimerkiksi kun otat kuulokkeet pois
- **Palaa hieman taaksepäin:** kun jatkat yli 2 minuutin tauon jälkeen, toisto alkaa 10 sekuntia aiemmasta kohdasta
- **Jatka kuuntelua -lista:** jaksot, edistymispalkki ja jäljellä oleva aika
- **Soittolista (valinnainen):** yhteinen jaksolista useammalle laitteelle, uudet jaksot merkitään **New**
- Merkitse jakso kuunnelluksi tai poista se listalta (poiston voi perua)
- Jakson voi lisätä listalle kuuntelematta sitä heti
- Asennettavissa puhelimen aloitusnäyttöön omalla kuvakkeella
- **MP3-linkin kopiointi:** soivan jakson suoran MP3-linkin voi kopioida ja avata missä tahansa muussa soittimessa
- Kuulokkeiden ja lukitusnäytön painikkeet toimivat
- Pikanäppäimet tietokoneella: `välilyönti` = toisto/tauko, `←` `→` = hyppy

## Käyttö

### Jakson lisääminen

1. Avaa https://ehken.github.io/player/
2. Kopioi MP3-tiedoston osoite leikepöydälle.
3. Paina oikean yläkulman **+**-painiketta. Alhaalta aukeaa **Add an episode** -paneeli.
4. Paina **Paste**, niin osoite liitetään kenttään. Voit myös painaa kenttää pitkään ja valita Liitä.
5. Valitse jompikumpi:
   - **Play now** aloittaa jakson heti. Jos jakso oli jo kesken, se jatkuu siitä kohdasta.
   - **Add to list** tallentaa jakson **Continue listening** -listalle myöhempää varten. Meneillään oleva toisto ei keskeydy.
6. Sulje paneeli tarvittaessa **✕**-painikkeesta tai napauttamalla paneelin ulkopuolelle.

Jakson voi lisätä myös suoraan sivulta kirjanmerkillä, katso [Kirjanmerkki](#kirjanmerkki-jakso-suoraan-sivulta-soittimeen).

### Toisto

- **Iso painike keskellä:** toisto ja tauko.
- **Vasen ja oikea kaarinuoli:** hyppy taakse- ja eteenpäin. Nuolessa näkyvä numero on hypyn pituus sekunteina.
- **Kelauspalkki:** vedä palkkia, niin pääset haluamaasi kohtaan. Vasemmalla näkyy kulunut aika, oikealla jäljellä oleva aika.
- **Speed:** napauta vaihtaaksesi toistonopeutta järjestyksessä 1× → 1,2× → 1,5× → 1,75× → 2× → 0,8×.
- **Skip:** napauta vaihtaaksesi hypyn pituutta järjestyksessä 10 → 15 → 20 → 30 s. Sama pituus on käytössä kuulokkeiden ja lukitusnäytön painikkeissa.

- **MP3 link:** kopioi soittimessa olevan jakson suoran MP3-linkin leikepöydälle. Linkin voi liittää esimerkiksi VLC:hen, podcast-sovellukseen tai selaimen osoiteriville, jos haluat kuunnella jakson jossain muualla.

Nopeus ja hypyn pituus tallentuvat, joten ne ovat samat, kun avaat soittimen seuraavan kerran.

### Kuuntelun jatkaminen

- Sijainti tallentuu automaattisesti. Kun avaat soittimen uudelleen, viimeisin kesken oleva jakso on valmiina siinä kohdassa, mihin jäit. Paina play.
- Jos taukoa on ollut yli 2 minuuttia, toisto alkaa 10 sekuntia aiemmasta kohdasta, jotta muistat, mihin jäit.
- Kun jakso loppuu (tai jäljellä on alle 30 sekuntia), se merkitään kuunnelluksi.

### Continue listening -lista

Listalla näkyvät viimeisimmät 12 jaksoa uusimmasta vanhimpaan. Jokaisesta jaksosta näkyy edistymispalkki, jäljellä oleva aika ja prosentti.

- **Avaa jakso:** napauta jakson nimeä. Toisto alkaa siitä, mihin jäit.
- **Merkitse kuunnelluksi:** napauta **✓**. Jakso saa merkinnän **Listened**. Napauta **✓** uudelleen, niin merkintä poistuu ja jakso alkaa seuraavalla kerralla alusta.
- **Poista listalta:** napauta **✕**. Jos poistit vahingossa, paina alareunaan ilmestyvää **Undo**-painiketta muutaman sekunnin sisällä.
- **Current** tarkoittaa soittimessa juuri nyt olevaa jaksoa, **Playing** sitä, joka parhaillaan soi.

### Pikanäppäimet (tietokone)

- `välilyönti`: toisto/tauko
- `←` / `→`: hyppy taakse / eteen

### Aloitusnäyttöön

Kun soitin on aloitusnäytöllä, se aukeaa omana sovelluksenaan ilman selaimen osoiteriviä.

**iPhone, Safari**
1. Avaa https://ehken.github.io/player/
2. Paina **Jaa**-painiketta (neliö ja nuoli ylös).
3. Valitse **Lisää Koti-valikkoon** ja paina **Lisää**.

**iPhone, Brave**
1. Avaa https://ehken.github.io/player/
2. Paina osoiterivin **⋯**-valikkoa ja valitse **Jaa**.
3. Valitse **Lisää Koti-valikkoon** ja paina **Lisää**.

**Android, Chrome**
1. Avaa https://ehken.github.io/player/
2. Paina oikean yläkulman **⋮**-valikkoa.
3. Valitse **Asenna sovellus** tai **Lisää aloitusnäytölle**.

**Huom. iPhonessa** aloitusnäytöltä avattu soitin pitää oman listansa, erillään selaimesta. Kirjanmerkki avaa jaksot aina selaimessa, joten niiden kohdat ja lista näkyvät selaimessa, eivät aloitusnäytön sovelluksessa. Jos käytät kirjanmerkkiä, käytä soitinta myös selaimessa.

## Soittolista (valinnainen)

Soittimeen voi yhdistää soittolistan, jonka jaksot näkyvät kaikilla siihen yhdistetyillä laitteilla. Kun soittolistalle lisätään jakso, se ilmestyy muille laitteille automaattisesti merkinnällä **New**. Soitin toimii täysin myös ilman soittolistaa.

Soittolista ei ole osa tätä repoa. Se on erillinen, yksityinen palvelu, jonka osoitteen ja avaimet saat soittolistan ylläpitäjältä. Soittimeen tallentuvat vain yhteystiedot, ja nekin vain omalle laitteellesi.

### Soittolistan yhdistäminen

**Linkillä (helpoin)**
1. Avaa soittolistan ylläpitäjältä saamasi linkki laitteella, jolla haluat kuunnella.
2. Soitin ilmoittaa **Playlist connected**, ja jaksot näkyvät otsikon **Playlist** alla.
3. Lisää soitin halutessasi aloitusnäyttöön (katso [Aloitusnäyttöön](#aloitusnäyttöön)). Avaa linkki ensin selaimessa ja lisää soitin vasta sitten aloitusnäyttöön.

**Käsin**
1. Paina yläkulman **säätimet**-kuvaketta (kaksi liukusäädintä).
2. Täytä **Playlist address** ja **Read key**.
3. Täytä **Write password** vain, jos tällä laitteella saa lisätä jaksoja soittolistalle. Kuuntelulaitteilla kenttä jätetään tyhjäksi.
4. Paina **Save**.

### Soittolistan käyttö

- Jaksot on ryhmitelty ohjelmittain, uusin ensin. Jokaisesta jaksosta näkyy jakson tunnus, julkaisupäivä ja edistyminen.
- **New** tarkoittaa jaksoa, jota ei ole vielä avattu tällä laitteella. Kun laite yhdistetään ensimmäistä kertaa, olemassa olevia jaksoja ei merkitä uusiksi.
- Napauta jaksoa, niin toisto alkaa. Kuuntelukohta tallentuu laitekohtaisesti, eli jokaisella kuuntelijalla on oma kohtansa.
- Soitin tarkistaa uudet jaksot, kun se avataan tai tuodaan näkyviin (enintään 5 minuutin välein). Viimeksi ladattu lista näkyy myös ilman verkkoyhteyttä.
- Jos ohjelmalla on yli 5 jaksoa, loput saa näkyviin painikkeella **Show all**.

### Jaksojen lisääminen soittolistalle

Toimii vain laitteella, jolle on tallennettu kirjoitussalasana.

- **Kirjanmerkillä:** avaa jakson sivu ja paina kirjanmerkkiä. Soitin kysyy **Save to playlist?**. Tarkista otsikko ja ohjelman nimi ja valitse **Save & play**, tai **Just play**, jos et halua lisätä jaksoa.
- **Soittimessa:** paina **+**, liitä MP3-osoite, täytä **Title** ja **Show** ja paina **Save to playlist**.

Samaa jaksoa ei voi lisätä kahdesti.

### Soittolistan jakaminen toiselle laitteelle

1. Paina säätimet-kuvaketta laitteella, jossa soittolista on jo yhdistetty.
2. Kohdassa **Share link** on valmis linkki. Paina **Copy** ja avaa linkki toisella laitteella.

Jakolinkissä on vain lukuavain, ei koskaan kirjoitussalasanaa. Jaa linkki vain niille, joille soittolista on tarkoitettu.

### Soittolistan poistaminen laitteelta

Säätimet → **Disconnect**. Soittolista ja sen tiedot poistuvat siltä laitteelta. Kuuntelukohdat säilyvät.

## Kirjanmerkki: jakso suoraan sivulta soittimeen

Monella sivulla podcast-jakson MP3-osoite ei näy suoraan, varsinkaan jos jakso on maksumuurin takana. Kirjanmerkki hoitaa tämän puolestasi. Kun painat sitä sivulla, jolla jakso on, se etsii sivulta jakson MP3-osoitteen ja avaa sen suoraan soittimessa.

**Miksi kirjanmerkki?** Maksumuurin takana MP3-osoite näkyy vain kirjautuneelle käyttäjälle. Siksi haun täytyy tapahtua sinun omassa selaimessasi, jossa olet jo kirjautunut. Kirjanmerkki ei lähetä tunnuksiasi minnekään. Se lukee avoimelta sivulta jakson MP3-osoitteen, otsikon ja julkaisupäivän ja avaa ne soittimessa. Tiedot kulkevat linkin `#`-merkin jälkeen, joten ne eivät päädy GitHubin palvelimelle.

### Kirjanmerkin koodi

Kopioi koko rivi:

```
javascript:(()=>{let u=[...document.querySelectorAll('audio,audio source')].map(e=>e.currentSrc||e.src).find(s=>/\.mp3/i.test(s));if(!u){const m=document.documentElement.innerHTML.match(/https?:(?:\\?\/){2}[^"'\s<>]+?\.mp3[^"'\s<>]*/i);if(m)u=m[0]}if(!u){alert('MP3-linkkiä ei löytynyt. Paina ensin play sivun soittimessa ja kokeile uudelleen.');return}u=u.replace(/\\\//g,'/').replace(/&amp;/g,'&');const q=s=>document.querySelector(s),t=(q('meta[property="og:title"]')||{}).content||(q('h1')||{}).textContent||document.title,p=(q('meta[property="article:published_time"]')||{}).content||(q('time[datetime]')||{}).dateTime||'';location.href='https://ehken.github.io/player/#'+new URLSearchParams({url:u,title:t.trim(),published:p,article:location.href.split('#')[0]})})()
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
3. Soitin aukeaa, ja jakso on valmiina siinä kohdassa, mihin jäit (uusi jakso alusta). Paina play.
4. Jos soittimeen on yhdistetty soittolista ja laitteelle on tallennettu kirjoitussalasana, soitin kysyy **Save to playlist?**. Tarkista otsikko ja ohjelman nimi ja valitse **Save & play**, tai **Just play**, jos et halua lisätä jaksoa soittolistalle.

### Jos se ei toimi

- **"MP3-linkkiä ei löytynyt":** paina ensin play sivun omassa soittimessa ja käynnistä kirjanmerkki sitten uudelleen. Joillain sivuilla äänitiedoston osoite ilmestyy vasta toiston alkaessa.
- **Ei tapahdu mitään:** tarkista, että kirjanmerkin osoite alkaa sanalla `javascript:` ja että koodi on kopioitu kokonaan. Jotkin selaimet poistavat `javascript:`-alun liitettäessä, joten kirjoita se tarvittaessa käsin.
- **Et ole kirjautunut:** maksumuurin takana olevaa jaksoa ei löydy ilman kirjautumista.

## Yksityisyys

- Kuunteluhistoria ja kohdat tallentuvat **vain omaan selaimeesi**, eikä niitä lähetetä minnekään. Muut soittimen käyttäjät eivät näe historiaasi.
- Historia säilyy, kunnes tyhjennät selaimen tiedot. iPhonen Safarissa sivuston tiedot voivat poistua, jos sivulla ei käy 7 päivään. Aloitusnäyttöön lisätyssä soittimessa tätä rajoitusta ei ole.
- Eri laitteet eivät jaa historiaa: puhelimella ja tietokoneella on kummallakin oma historiansa.

## Tekniikka

Yksi HTML-tiedosto (`index.html`) sekä kuvakkeet ja `manifest.webmanifest` aloitusnäyttöä varten. Ei palvelinta, kirjastoja eikä seurantaa. Soitin toimii GitHub Pagesissa. Jakson voi avata suoraan linkillä muodossa `https://ehken.github.io/player/#url=<MP3-osoite>`.

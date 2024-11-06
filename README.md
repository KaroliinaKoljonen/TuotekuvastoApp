1. HomeController.cs
  Controller, joka hakee tiedot products.json-tiedostosta ja välittää ne käyttöliittymälle. Se toimii välikätenä tietolähteen (products.json) ja käyttöliittymän (Product.cshtml) välillä.  Product()-metodi käyttää GetProducts()-metodia hakemaan tuotetiedot, jotka palautetaan Product.cshtml-näkymälle.

2. products.json
  Tietolähde, joka sisältää tuotetiedot JSON-muodossa. Tiedostosta luetaan tuotetiedot, jotka deserialisoidaan HomeControllerissa listaksi Product-olioita.

3. Product.cs
  Malli, joka määrittelee tuotteen ominaisuudet (nimi, hinta, kuvaus, kuva). Kuvaa tuotteen tietorakenteen ja muotoilee nimen ja hinnan näkymää varten.

4. Product.cshtml
   Näkymä, joka vastaa tuotteiden näyttämisestä käyttöliittymässä. Luo HTML-kortit tuotteista käyttäen niiden tietoja, kuten nimeä, hintaa ja kuvausta, ja näyttää ne käyttäjälle.

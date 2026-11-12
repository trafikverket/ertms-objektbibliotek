# ERTMS-objektbibliotek – version 6.0

Objektbibliotek för ERTMS med 3D-geometrier, 2D-celler, objektlista (feature definitions) och attributlista.
Ni hittar publicerade versioner under [Releases](https://github.com/trafikverket/ertms-objektbibliotek/releases) på Trafikverkets GitHub.

## Kompatibilitet

ERTMS-objektbibliotek från version 6.0 och uppåt är anpassat för leverans mot systemet Sophie. Projekt som ska leverera till BIS måste använda version 5.0 eller lägre.


## Innehåll

ERTMS-objektbibliotek består av dessa delar som distribueras tillsammans med denna readme-fil.

* **ERTMS_6.0_3D.cel:** 3D-representation av järnvägsobjekt.
* **ERTMS_6.0_2D.cel:** 2D-symboler/celler för ritningar.
* **featureDefinitions-v6.0.csv:** Lista över objekt som ingår i biblioteket, med koppling till geometrier och celler för grafisk representation samt till attributset. Semikolonseparerad och kodad i UTF-8 med BOM.
* **propertySets-v6.0.csv:** Attributset som kopplas till objekten. Semikolonseparerad och kodad i UTF-8 med BOM.
* **Katalog Objektbiblioteket v6.0.pdf:** Förteckning över alla feature definitions med beskrivning och bilder på 2D-celler samt 3D-geometrier.


### Kopplingen mellan feature definitions och attribut

Varje feature definition använder ett generellt propertyset för sin objekttyp: SpotLocationEntity för punktobjekt och LinearLocationEntity för längdsträckta objekt. Där det är relevant kopplas dessutom objektspecifika egenskaper till respektive feature definition. Vissa objekt har därför bara det generella propertysetet och saknar objektspecifika egenskaper.


## Format

Geometrier och celler levereras som .cel-filer.

Om ett projekt har behov av geometrier och celler i .dwg-format kan ni kontakta förvaltningen, [se denna sida för kontaktinformation](https://earum.sp.trafikverket.se/sites/20260113073637/home/Sidor/ERTMS-objektbibliotek.aspx) (kräver behörighet).


## Revideringshistorik

För tidigare versioner av biblioteket har revideringsdokument tagits fram som listar ändringarna mellan versionerna. Version 6.0 innebär en så omfattande förändring att den räknas som ett nytt bibliotek, och något revideringsdokument finns därför inte för denna version. Planen är att revideringsdokument tas fram från och med nästa release.
# ERTMS-objektbibliotek

Objektbibliotek för ERTMS med 3D-geometrier, 2D-celler, objektlista (Feature Definitions) och attributlista.

## Innehåll

Biblioteket har tidigare distribuerats utanför GitHub, senast som version 5.0. Första versionen i detta repo planeras bli **v6.0.0**. Äldre versioner finns därför inte i repots historik.

| Del | Format | Beskrivning |
|-----|--------|-------------|
| 3D-geometrier | `.dgn` | 3D-representation av järnvägsobjekt |
| 2D-celler | `.dgn` | 2D-symboler/celler för ritningar |
| Feature Definitions | `.csv` | Lista över objekt som ingår i biblioteket, med koppling till geometrier och celler för grafisk representation samt till attributset |
| Attributlista | `.csv` | Attributset som kopplas till objekten |

## Branchstrategi

- **`main`** innehåller den senaste godkända, skarpa versionen av biblioteket.
- **`dev`** innehåller pågående arbete. Innehållet här kan vara ofullständigt, ändras löpande och är **inte** godkänt för skarp användning.
- **`release/{major}.{minor}`** (t.ex. `release/1.0`) innehåller en specifik version av biblioteket och används för buggfixar av den versionen.

Ändringar görs i `dev` (eller i feature-brancher som mergas till `dev`). När en ny version är granskad och klar mergas den till `main`, och en release-branch skapas vid behov. Buggfixar för tidigare versioner görs i respektive release-branch.

## Versionering

Skarpa versioner märks med taggar, t.ex. `v1.0.0`. Varje tagg avser en specifik, godkänd version av biblioteket. Buggfixar ger ny patch-version (`v1.0.1`), nya eller ändrade objekt ger ny minor- eller major-version.
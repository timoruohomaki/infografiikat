# CLAUDE.md

Tämä tiedosto ohjeistaa Claudea (ja muita tekoälyavustajia) tämän repositorion infografiikkojen tuottamisessa ja ylläpidossa.

## Repositorion tarkoitus

Repositorio sisältää infografiikkaelementtejä, jotka tukevat **oikeushallinnon tiedolla johtamisen viitearkkitehtuurin** dokumentointia. Painopiste on johtamisen tuessa: johtamisen viitekehysten sekä tiedon ja kontekstin roolin kuvaamisessa.

## Kohdeympäristö

- **Kohdedokumentti:** PDF, taitettu **valkoiselle pohjalle**.
- **Seuraus suunnitteluun:** Kaikkien graafisten elementtien tulee toimia vaaleaa taustaa vasten — riittävä kontrasti, ei vaaleaa tekstiä vaalealla pohjalla.
- **Tulostettavuus:** Värimaailman on säilyttävä luettavana myös mustavalkotulostuksessa. Varmistetaan riittävä sävyero, ei pelkästään väriin perustuvaa erottelua.

## Tiedostomuodot ja työnkulku

1. **Lähdetiedostot** tehdään ja säilytetään `draw.io`-muodossa (`.drawio`), jotta ne ovat jatkossa muokattavissa.
2. **Vientitiedostot** tuotetaan tarvittaessa `.svg`-muotoon (ensisijainen, skaalautuva) tai `.png`-muotoon dokumenttiin liittämistä varten.
3. Yksi käsitteellinen kokonaisuus = yksi lähdetiedosto. Vältetään ylisuuria, monta asiaa sekoittavia kaavioita.
4. Tiedostonimet kuvaavia ja yhtenäisiä (esim. `johtamisen-viitekehys-strateginen.drawio`).

## Visuaaliset suunnitteluperiaatteet

### Värit
- Vaalea tai valkoinen tausta.
- Tekstit tummia (esim. lähes musta `#1A1A2E`).
- Korostusväreissä suositaan hillittyä, asiantuntevaa palettia: tummansininen, petrooli, ja varautunut korostusväri vain harkitusti.
- Riittävä kontrastisuhde: vähintään WCAG AA, mieluiten AAA leipätekstille.

### Typografia ja luettavuus
- Selkeä, ammattimainen ulkoasu — kyseessä on julkishallinnon viitearkkitehtuuridokumentti.
- Tekstin minimikoko valitaan niin, että se on luettavissa PDF:ssä myös pienennettynä.

### Saavutettavuus
- Ei pelkkään väriin perustuvaa tiedonvälitystä (huomioidaan värisokeus).
- Selkeät otsikoinnit ja looginen lukujärjestys.

## Kielelliset konventiot

- **Ensisijainen kieli:** suomi.
- Termistö julkishallinnon ja kokonaisarkkitehtuurin vakiintuneen sanaston mukaista (JHS-suositukset, viitearkkitehtuurikäytännöt).
- **Lukuformaatit:** tuhaterotin on piste (`.`) ja desimaalierotin pilkku (`,`). Esim. `1.250,75`.
- Päivämäärät ja kellonajat ISO 8601 / RFC 3339 -muodossa (esim. `2026-05-21`).

## Versionhallinta

- Commit-viestit selkeitä ja kuvaavia, suomeksi.
- Lähdetiedostot (`.drawio`) versioidaan aina; vientitiedostot voidaan tarvittaessa generoida uudelleen lähteestä.

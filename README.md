# Snidex Studio 3.3

Demonstration av ett internt projekt- och beredningsverktyg. Publicerad öppen demo: https://jsall77.github.io/snidex-studio/ . Källorna och exempeldata innehåller ingen verklig kundorder.

Starta `python3 -m http.server 5177 --directory dist`. Ingen installation eller byggkedja krävs. För en självständig HTML-fil används `../package_standalone.py` från arbetsytans rot (lokala absoluta arbetsvägar i paketeringsverktyget).

## Version 3.3

- Zoom mot pekaren, dubbelklick för detaljvy, panorering med Shift/högerdrag eller Flytta vy samt tvåfingersgester. Piltangenter flyttar, +/- zoomar, 0 återställer. Kameraläget ändrar inte projektdata eller kundbildens utsnitt.
- Egen innerprofil direkt under standardvalen; fungerande avsnittsgenvägar i bred och smal layout.
- 40 sekunders svensk textad introduktionsfilm med animerade markeringar på riktiga skärmbilder, och läsbar textversion.

## Version 3.2

- Grafisk profil från användarens tillhandahållna logotypsida: RGB244/163/0, #F4A300, svart och vitt.
- Grundlogotyp på ljusa ytor, negativ på svart och helsvart på andra underlag; symbol och ordmärke behåller proportionerna och får avskilt friutrymme.
- Samma logotyp-/färgbehandling i gränssnitt, kundalbum, produktionsförslag och HTML-exporter. Typografi är inte specificerad i utdraget; Montserrat/Helvetica behålls.

## Version 3.1

- Tydlig måttpanel med karmdjup och separata önskemål för huvud-/innerbåge, ytterbåge i kopplad konstruktion, synliga karm-/bågbredder, post/tvärpost samt glasfals.
- Numeriskt märkt Snitt-vy och uppdaterad principgeometri; null betyder okänt mått, aldrig ett påstått standardmått.
- Profilsatser kräver uttrycklig `frameDepths`-tillämpning och matchning mot begärda `sectionDimensions` innan profil-/kaplistor kan beräknas. Egna källnoteringar verifierar inte en profil.
- Rättningar av låsta fältval vid mallbyte, lokala postcentrum i beredning och fältspecifika glas-/beslagsönskemål i kundalbum.
- Konstruktionsmått följer projekt, delad konfiguration, kundalbum och produktionsförslag.

## Genomfört

- SA KFI, ST KFI, SA EFI och tre fönsterdörrsystem. Rektangulärt, runt, ellips-/cirkelsegment och separat högerhöjd för snedform.
- Globalt rutnät samt lokalt rekursivt fältträd med stabila ID, måttsatta postcentrum, delning/sammanslagning och individuella öppnings-/konstruktionsönskemål.
- Spröjs per fält: system, bredd, båge/glasnivå, isolerrutespalt och egna centrum. Logiska glasdelar visas som principgeometri.
- Träslag, täckmålning, bets/lasyr, klarlack, glans och 215 ungefärliga RAL CLASSIC-skärmprover med sparad RAL-kod.
- Snidex Original/Traditionell ytterprofil, Slät/Pärla/Fas innerprofil samt egna namngivna profiler som redigerbara punktkonturer och faktisk illustrativ 3D-geometri.
- Best Glass och Press Glass samt namngivna specialglas, krav, skikt, spalter, beläggning och databladreferenser per fält.
- Winkhaus/ASSA som beslagssystemönskemål, separat handtagsinköpskälla (Snidex/Beslagskonsulten), 20 artikelreferenser med källor och fem verkliga produktfoton. Fyra fotoanpassade handtagsformer, detaljzoom och föreslagen Snidexprofilering.
- Antal, littera, rum/plan/fasad, fästa mallar, skapa liknande, ändra sparad position, mängdändringar, individuella/grupperade lås, ångra/gör om och tangentbordsnavigering.
- Projektimport/export, utförandelänkar, A/B-jämförelse, lokalt fotomontage, fryst lokal granskningsnotering och projektbundet dokumentarkiv.
- Kundalbum och produktionsförslag i PDF/HTML/JSON, med mängder, positionsrevisioner och dokument-ID. Äldre dokumentversioner kan återskapas från lokalt sparade ögonblicksbilder.
- Import av versionsmärkt masterdata, begränsade deklarativa formler/regler, villkorade receptlistor/pris, granskningspaket med SHA-256 och idempotensnyckel samt matchning av manuellt importerad kvittens.

## Produktionsgräns

Ingen verklig Snidex-masterdata, produktionsprislista, verifierad profilsats, glas-/beslagsmappning eller Archimede-adapter har levererats. Profiler, beslag, trästruktur och färger är illustrativa. Ett känt leverantörsnamn innebär inte artikelkompatibilitet. Egna profiler och glas är konstruktionsförfrågningar.

Alla beräknade listor kräver uttryckligt importerade recept. Tomt/ofullständigt/otillämpligt bibliotek ger null och kontrollpunkter. Egna profiler, ändrade glasönskemål och omappade beslag får inte ärva ett vanligt recept. Importens `verified:true` är importörens uppgift. Inga lokala godkännanden eller kvittenser kan frisläppa produktion. Inga CNC-filer eller native Archimede-importfiler skapas.

## Lagring och delning

GitHub Pages är öppet och har ingen inloggning. Projekt, masterdata, dokumentarkiv och ångrahistorik lagras lokalt i webbläsaren, inte på en gemensam server. Exportera projektfiler för säkerhetskopia. Delningslänkar innehåller bara fönsterkonfiguration, inte projekt-/kundmetadata. Fasadfoton hålls i sidans minne och skickas inte iväg. Skärmen skickar inga order/offertförfrågningar.

Intern drift med gemensamma projekt, behörigheter, central attest och autentiserad ERP-återrapportering kräver en separat server och verifierad integration.

## Verifiering

Kör med Node: `check-model.mjs`, `check-model-v3.mjs`, `check-preparation.mjs`, `check-production-v3.mjs`, `check-project-v3.mjs`. Testerna omfattar 192 + 432 + 1152 geometri-/beredningsfall samt meningsfulla scen-, regel-, recept-, lås-, import-, mängd-, hash- och kvittensfall. Separata presentations-/material-/glaseditortester finns i arbetsytans `work/`. PDF-exempel provgenereras i riktig webbläsare och renderas för visuell kontroll.

Den grafiska profilen följer nu användarens tillhandahållna logotypsida; tidigare webbobserverade färger har ersatts. Originalbilder och logga attribueras Snidex. Montserrat distribueras under OFL. Three.js, pdf-lib och RAL-skärmdatans MIT-licenser medföljer under assets. RAL-datan är en oberoende ungefärlig skärmpalett, inte RAL:s licensierade digitalbibliotek. Fysiskt kulörprov behövs före order.

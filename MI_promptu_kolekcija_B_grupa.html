<!DOCTYPE html>
<html lang="lv">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>MI promptu kolekcija · B grupa · pašvaldības</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.3.1/umd/react.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.3.1/umd/react-dom.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/7.24.7/babel.min.js"></script>
<style>
  :root {
    --purple: #AC61C8;
    --purple-dark: #7A3C8E;
    --purple-light: #EFD9F5;
    --teal: #00C992;
    --teal-light: #D4F5E9;
    --orange: #FF8225;
    --orange-light: #FFE4D1;
    --blue: #02B2FE;
    --blue-light: #D4F0FF;
    --dark: #1A1A2E;
    --grey: #6B6B7B;
    --grey-light: #F2F2F5;
    --grey-border: #E0E0E5;
    --white: #FFFFFF;
    --red: #C5283D;
    --red-light: #F8D7DA;
    --green: #3E8E3E;
    --yellow: #FFF3CD;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #FAFAFB;
    color: var(--dark);
    line-height: 1.5;
  }
  h1, h2, h3, h4 { font-family: "Arial Black", Arial, sans-serif; }
  button { font-family: inherit; cursor: pointer; }
  input, textarea, select { font-family: inherit; font-size: 14px; }
  textarea { resize: vertical; }
  ::-webkit-scrollbar { width: 10px; height: 10px; }
  ::-webkit-scrollbar-track { background: var(--grey-light); }
  ::-webkit-scrollbar-thumb { background: var(--grey); border-radius: 5px; }
  ::-webkit-scrollbar-thumb:hover { background: var(--purple-dark); }
  @media print {
    .no-print { display: none !important; }
    body { background: white; }
  }
</style>
</head>
<body>
<div id="root"></div>

<script type="text/babel" data-type="module">
const { useState, useMemo, useEffect, useRef } = React;

// ============================================================
// DATU MODELIS — 15 ŠABLONI
// ============================================================

const TEMPLATES = [
  {
    nr: 1, posms: "Plānošana", nosaukums: "Audita risku karte projektam",
    kad: "Audita plānošanas posmā, kad jāidentificē galvenie riski konkrētam pašvaldības projektam vai jomai",
    karkass: `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādam objektam:

OBJEKTS: [pašvaldības projekta vai jomas apraksts]
BUDŽETS/APJOMS: [summa vai darbības apjoms]
ATBILDĪGĀ STRUKTŪRA: [pašvaldības dienests vai iestāde]
LAIKA POSMS: [audita aptverošais periods]

Lūdzu, palīdzi sastādīt risku karti:
1. Identificē 5-7 galvenos riskus šim objekta tipam pašvaldības kontekstā
2. Katram riskam: aprakstu, iespējamību (zema/vidēja/augsta), ietekmi
3. Norādi, kuri riski prasa neatkarīgu datu pārbaudi (piem. ģeotelpiskie dati)
4. Norādi, kuri riski iespējami saistīti ar valsts iestāžu kompetenci

Strukturē kā tabulu ar iespēju filtrēt pēc prioritātes.`,
    joma: "Mežs/vide",
    paraugs: `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādam objektam:

OBJEKTS: Saldus pašvaldības meža apsaimniekošanas process 2024. gadā
BUDŽETS/APJOMS: 145 ha kopējā ciršanas platība, ieņēmumi ~280 000 EUR
ATBILDĪGĀ STRUKTŪRA: Saldus pašvaldības meža apsaimniekošanas dienests
LAIKA POSMS: 01.01.2024 – 31.12.2024

Lūdzu, palīdzi sastādīt risku karti:
1. Identificē 5-7 galvenos riskus šim objekta tipam pašvaldības kontekstā
2. Katram riskam: aprakstu, iespējamību (zema/vidēja/augsta), ietekmi
3. Norādi, kuri riski prasa neatkarīgu datu pārbaudi (piem. ģeotelpiskie dati)
4. Norādi, kuri riski iespējami saistīti ar valsts iestāžu kompetenci

Strukturē kā tabulu ar iespēju filtrēt pēc prioritātes.`,
    fields: [
      { key: "objekts", label: "Objekts", placeholder: "Piem. Saldus pašvaldības meža apsaimniekošanas process 2024" },
      { key: "apjoms", label: "Budžets/apjoms", placeholder: "Piem. 145 ha, ieņēmumi ~280 000 EUR" },
      { key: "struktura", label: "Atbildīgā struktūra", placeholder: "Piem. Pašvaldības meža apsaimniekošanas dienests" },
      { key: "periods", label: "Laika posms", placeholder: "Piem. 01.01.2024 – 31.12.2024" },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādam objektam:

OBJEKTS: ${f.objekts}
BUDŽETS/APJOMS: ${f.apjoms}
ATBILDĪGĀ STRUKTŪRA: ${f.struktura}
LAIKA POSMS: ${f.periods}

Lūdzu, palīdzi sastādīt risku karti:
1. Identificē 5-7 galvenos riskus šim objekta tipam pašvaldības kontekstā
2. Katram riskam: aprakstu, iespējamību (zema/vidēja/augsta), ietekmi
3. Norādi, kuri riski prasa neatkarīgu datu pārbaudi (piem. ģeotelpiskie dati)
4. Norādi, kuri riski iespējami saistīti ar valsts iestāžu kompetenci

Strukturē kā tabulu ar iespēju filtrēt pēc prioritātes.`,
  },
  {
    nr: 2, posms: "Plānošana", nosaukums: "Pierādījumu avotu identifikācija",
    kad: "Kad zināms, kas jāpārbauda, bet jāidentificē, kādi datu avoti var sniegt pierādījumus",
    karkass: `Esmu pašvaldības iekšējais auditors. Man jāpārbauda šāds apgalvojums:

APGALVOJUMS: [pašvaldības ziņojuma vai dokumenta apgalvojums]
KONTEKSTS: [īsa situācijas apraksts]

Lūdzu, palīdzi identificēt pierādījumu avotus:
1. Iekšējie pašvaldības avoti (dokumenti, sistēmas, ieraksti)
2. Valsts iestāžu publiskie reģistri un datu bāzes (norādi konkrētus)
3. Atvērtie ģeotelpiskie un statistikas dati
4. Trešo pušu avoti (mediji, NVO ziņojumi, akadēmiski pētījumi)

Katram avotam: kā tam piekļūt, cik uzticams, kādi ir ierobežojumi.
Sakārto secībā no neatkarīgākā līdz mazāk neatkarīgajam.`,
    joma: "Iepirkumi/būvniecība",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man jāpārbauda šāds apgalvojums:

APGALVOJUMS: "Skolas piebūves būvdarbi (līgums Nr. PB-2024-018, summa 487 500 EUR) izpildīti pilnā apjomā saskaņā ar tehnisko specifikāciju un nodoti ekspluatācijā 30.09.2024."
KONTEKSTS: Pašvaldības būvvaldes ziņojums apliecina pieņemšanu. Auditā pārbaudu, vai apgalvojums atbilst faktiskajai izpildei.

Lūdzu, palīdzi identificēt pierādījumu avotus:
1. Iekšējie pašvaldības avoti (dokumenti, sistēmas, ieraksti)
2. Valsts iestāžu publiskie reģistri un datu bāzes (norādi konkrētus)
3. Atvērtie ģeotelpiskie un statistikas dati
4. Trešo pušu avoti (mediji, NVO ziņojumi, akadēmiski pētījumi)

Katram avotam: kā tam piekļūt, cik uzticams, kādi ir ierobežojumi.
Sakārto secībā no neatkarīgākā līdz mazāk neatkarīgajam.`,
    fields: [
      { key: "apgalvojums", label: "Apgalvojums", placeholder: "Pašvaldības ziņojuma apgalvojums, ko jāpārbauda", multiline: true },
      { key: "konteksts", label: "Konteksts", placeholder: "Īss situācijas apraksts" },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man jāpārbauda šāds apgalvojums:

APGALVOJUMS: ${f.apgalvojums}
KONTEKSTS: ${f.konteksts}

Lūdzu, palīdzi identificēt pierādījumu avotus:
1. Iekšējie pašvaldības avoti (dokumenti, sistēmas, ieraksti)
2. Valsts iestāžu publiskie reģistri un datu bāzes (norādi konkrētus)
3. Atvērtie ģeotelpiskie un statistikas dati
4. Trešo pušu avoti (mediji, NVO ziņojumi, akadēmiski pētījumi)

Katram avotam: kā tam piekļūt, cik uzticams, kādi ir ierobežojumi.
Sakārto secībā no neatkarīgākā līdz mazāk neatkarīgajam.`,
  },
  {
    nr: 3, posms: "Plānošana", nosaukums: "Sadarbības iestādes noteikšana",
    kad: "Audita plānošanas posmā, kad jāizprot, ar kuru valsts iestādi būs jāsadarbojas",
    karkass: `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādā jomā:

JOMA: [audita joma vai konkrēts objekts]
PAŠVALDĪBAS DARBĪBA: [ko tieši pašvaldība dara šajā jomā]
IESPĒJAMIE PĀRKĀPUMI: [kāda veida nesakritības varētu konstatēt]

Lūdzu, palīdzi noteikt:
1. Kuras valsts iestādes ir kompetentas šajā jomā?
2. Kāds ir kompetenču sadalījums starp tām?
3. Ar kuru iestādi jāsadarbojas, ja konstatēju pārkāpumu?
4. Kādi ir formālie sadarbības veidi (informēšana, pieprasījums, sūdzība)?
5. Kāda informācija no pašvaldības iestādei būs vajadzīga?

NB: Ja neesi pārliecināts par kompetenču sadalījumu, norādi to skaidri — es pārbaudīšu pirmavotos.`,
    joma: "Vide/teritorijas plānošana",
    paraugs: `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādā jomā:

JOMA: Pašvaldības zemes detālplānojumu izstrāde un saskaņošana
PAŠVALDĪBAS DARBĪBA: Pašvaldība pieņem detālplānojumus, kas maina zemes lietošanas mērķi un būvniecības nosacījumus īpašumiem aizsargājamās dabas teritoriju buferzonās
IESPĒJAMIE PĀRKĀPUMI: Detālplānojumi pieņemti bez vides ietekmes novērtējuma vai bez konsultācijas ar atbildīgajām valsts iestādēm

Lūdzu, palīdzi noteikt:
1. Kuras valsts iestādes ir kompetentas šajā jomā?
2. Kāds ir kompetenču sadalījums starp tām?
3. Ar kuru iestādi jāsadarbojas, ja konstatēju pārkāpumu?
4. Kādi ir formālie sadarbības veidi (informēšana, pieprasījums, sūdzība)?
5. Kāda informācija no pašvaldības iestādei būs vajadzīga?

NB: Ja neesi pārliecināts par kompetenču sadalījumu, norādi to skaidri — es pārbaudīšu pirmavotos.`,
    fields: [
      { key: "joma", label: "Joma", placeholder: "Audita joma vai konkrēts objekts" },
      { key: "darbiba", label: "Pašvaldības darbība", placeholder: "Ko tieši pašvaldība dara šajā jomā", multiline: true },
      { key: "parkapumi", label: "Iespējamie pārkāpumi", placeholder: "Kāda veida nesakritības varētu konstatēt", multiline: true },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Plānoju auditu šādā jomā:

JOMA: ${f.joma}
PAŠVALDĪBAS DARBĪBA: ${f.darbiba}
IESPĒJAMIE PĀRKĀPUMI: ${f.parkapumi}

Lūdzu, palīdzi noteikt:
1. Kuras valsts iestādes ir kompetentas šajā jomā?
2. Kāds ir kompetenču sadalījums starp tām?
3. Ar kuru iestādi jāsadarbojas, ja konstatēju pārkāpumu?
4. Kādi ir formālie sadarbības veidi (informēšana, pieprasījums, sūdzība)?
5. Kāda informācija no pašvaldības iestādei būs vajadzīga?

NB: Ja neesi pārliecināts par kompetenču sadalījumu, norādi to skaidri — es pārbaudīšu pirmavotos.`,
  },
  {
    nr: 4, posms: "Konstatējums", nosaukums: "Konstatējuma 4-elementu strukturēšana",
    kad: "Kad savākti pierādījumi un nepieciešams strukturēts konstatējuma formulējums (B grupas standarts: Fakts/Pierādījums/Ietekme/Sadarbība)",
    karkass: `Esmu pašvaldības iekšējais auditors. Man ir audita atklājumi, ko jāstrukturē kā formālu konstatējumu.

ATKLĀJUMI BRĪVĀ FORMĀ:
[apraksti atklājumus brīvā formā — kas, kur, kad, cik]

PĀRBAUDĪTIE PIERĀDĪJUMI:
[uzskaiti pierādījumus, kurus pārbaudīji]

Lūdzu, strukturē šo kā formālu pašvaldības audita konstatējumu ar 4 elementiem:

1. FAKTS — kāds ir konstatētais fakts (neitrāli, bez vērtējuma)
2. PIERĀDĪJUMS — kā tas pierādīts (datu avots, metode, datums)
3. IETEKME — kādi ir reālie vai potenciālie zaudējumi/riski
4. SADARBĪBA — vai un ar kuru valsts iestādi nepieciešama formāla sadarbība

Lieto auditora valodu — precīzu, bez emocijām, ar skaitļiem un datumiem.`,
    joma: "Mežs/vide",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man ir audita atklājumi, ko jāstrukturē kā formālu konstatējumu.

ATKLĀJUMI BRĪVĀ FORMĀ:
Saldus pašvaldības mežā cirsts vairāk nekā plānā un VMD saskaņojumā. Plāns un saskaņojums — 45 ha. Sentinel-2 attēli no 2024.04. un 2024.10. salīdzinājumā ar LVM ĢeoTĪmekļa kvartālu robežām rāda, ka cirsti 67 ha. Pārsniegums — 22 ha kvartālos 409-01 un 409-02. Pašvaldības gada ziņojumā teikts "saskaņā ar plānu".

PĀRBAUDĪTIE PIERĀDĪJUMI:
- Sentinel-2 satelītu attēli (Copernicus, 03.04.2024 un 12.10.2024)
- LVM ĢeoTĪmekļa kvartālu robežu dati (publiski pieejami)
- Saldus pašvaldības meža apsaimniekošanas plāns 2024 (iekšējais dokuments)
- VMD ciršanas saskaņojums Nr. SA-2024-0148 (publiski pieejams)
- Pašvaldības 2024. gada saimnieciskās darbības ziņojums

Lūdzu, strukturē šo kā formālu pašvaldības audita konstatējumu ar 4 elementiem:

1. FAKTS — kāds ir konstatētais fakts (neitrāli, bez vērtējuma)
2. PIERĀDĪJUMS — kā tas pierādīts (datu avots, metode, datums)
3. IETEKME — kādi ir reālie vai potenciālie zaudējumi/riski
4. SADARBĪBA — vai un ar kuru valsts iestādi nepieciešama formāla sadarbība

Lieto auditora valodu — precīzu, bez emocijām, ar skaitļiem un datumiem.`,
    fields: [
      { key: "atklajumi", label: "Atklājumi brīvā formā", placeholder: "Apraksti atklājumus — kas, kur, kad, cik", multiline: true, rows: 5 },
      { key: "pieradijumi", label: "Pārbaudītie pierādījumi", placeholder: "Uzskaiti pierādījumus, kurus pārbaudīji", multiline: true, rows: 5 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man ir audita atklājumi, ko jāstrukturē kā formālu konstatējumu.

ATKLĀJUMI BRĪVĀ FORMĀ:
${f.atklajumi}

PĀRBAUDĪTIE PIERĀDĪJUMI:
${f.pieradijumi}

Lūdzu, strukturē šo kā formālu pašvaldības audita konstatējumu ar 4 elementiem:

1. FAKTS — kāds ir konstatētais fakts (neitrāli, bez vērtējuma)
2. PIERĀDĪJUMS — kā tas pierādīts (datu avots, metode, datums)
3. IETEKME — kādi ir reālie vai potenciālie zaudējumi/riski
4. SADARBĪBA — vai un ar kuru valsts iestādi nepieciešama formāla sadarbība

Lieto auditora valodu — precīzu, bez emocijām, ar skaitļiem un datumiem.`,
  },
  {
    nr: 5, posms: "Konstatējums", nosaukums: "Pierādījumu novērtēšana",
    kad: "Kad savākti vairāki pierādījumi un nepieciešams novērtēt to uzticamību un pietiekamību",
    karkass: `Esmu pašvaldības iekšējais auditors. Man ir savākti pierādījumi konstatējumam.

KONSTATĒJUMS: [īsi formulēts konstatējums]

PIERĀDĪJUMI:
1. [pierādījuma 1 apraksts un avots]
2. [pierādījuma 2 apraksts un avots]
3. [pierādījuma 3 apraksts un avots]

Lūdzu, izvērtē pierādījumus pēc kritērijiem:

1. UZTICAMĪBA — vai avots ir neatkarīgs un autoritatīvs?
2. PIETIEKAMĪBA — vai pierādījumu daudzums un kvalitāte ir pietiekama konstatējuma pamatošanai?
3. RELEVANCE — vai pierādījums tieši pamato konstatējumu?
4. AKTUALITĀTE — vai pierādījums attiecas uz audita periodu?

Katram pierādījumam: vērtējums (1-5 skalā) un komentārs.
Beigās: vai pierādījumu kopums ir pietiekams, vai jāmeklē vēl, un kādi tieši.`,
    joma: "Sociālie pakalpojumi",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man ir savākti pierādījumi konstatējumam.

KONSTATĒJUMS: Pašvaldības sociālā dienesta GMI pabalstu piešķiršanas procesā 2024. gadā 14% gadījumu (47 no 336) trūkst pilna ienākumu deklarēšanas dokumentācija saskaņā ar MK noteikumiem Nr. 809.

PIERĀDĪJUMI:
1. Sociālā dienesta klientu lietu izlases pārbaude (n=336, izlases metode — sistemātiska, intervāls 5)
2. MK noteikumu Nr. 809 prasību saraksts (publisks normatīvais akts)
3. SOPA sistēmas izvilkums par GMI lēmumiem 01.01.2024-31.12.2024
4. Sociālā dienesta vadītāja paskaidrojuma raksts (datēts 15.02.2026)
5. VID datu pieprasījuma žurnāls (iekšējs sociālā dienesta dokuments)

Lūdzu, izvērtē pierādījumus pēc kritērijiem:

1. UZTICAMĪBA — vai avots ir neatkarīgs un autoritatīvs?
2. PIETIEKAMĪBA — vai pierādījumu daudzums un kvalitāte ir pietiekama konstatējuma pamatošanai?
3. RELEVANCE — vai pierādījums tieši pamato konstatējumu?
4. AKTUALITĀTE — vai pierādījums attiecas uz audita periodu?

Katram pierādījumam: vērtējums (1-5 skalā) un komentārs.
Beigās: vai pierādījumu kopums ir pietiekams, vai jāmeklē vēl, un kādi tieši.`,
    fields: [
      { key: "konstatejums", label: "Konstatējums", placeholder: "Īsi formulēts konstatējums", multiline: true, rows: 3 },
      { key: "pieradijumi", label: "Pierādījumu saraksts", placeholder: "Uzskaiti pierādījumus ar avotiem", multiline: true, rows: 6 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man ir savākti pierādījumi konstatējumam.

KONSTATĒJUMS: ${f.konstatejums}

PIERĀDĪJUMI:
${f.pieradijumi}

Lūdzu, izvērtē pierādījumus pēc kritērijiem:

1. UZTICAMĪBA — vai avots ir neatkarīgs un autoritatīvs?
2. PIETIEKAMĪBA — vai pierādījumu daudzums un kvalitāte ir pietiekama konstatējuma pamatošanai?
3. RELEVANCE — vai pierādījums tieši pamato konstatējumu?
4. AKTUALITĀTE — vai pierādījums attiecas uz audita periodu?

Katram pierādījumam: vērtējums (1-5 skalā) un komentārs.
Beigās: vai pierādījumu kopums ir pietiekams, vai jāmeklē vēl, un kādi tieši.`,
  },
  {
    nr: 6, posms: "Konstatējums", nosaukums: "Ietekmes kvantifikācija",
    kad: "Kad jāaprēķina vai jāapraksta konstatējuma ietekme — finansiālā, reputācijas, juridiskā",
    karkass: `Esmu pašvaldības iekšējais auditors. Man jāizvērtē konstatējuma ietekme.

KONSTATĒJUMS: [īsi formulēts konstatējums]
APJOMS: [skaitļi — summas, daudzumi, procenti]

Lūdzu, palīdzi kvantificēt ietekmi 4 dimensijās:

1. FINANSIĀLĀ IETEKME (tiešie zaudējumi, potenciālie zaudējumi, ietaupījumu zudums)
2. JURIDISKĀ IETEKME (iespējamie pārkāpumi, soda risks, atbildības jautājumi)
3. REPUTĀCIJAS IETEKME (sabiedrības uzticības risks, mediju intereses iespējamība)
4. OPERATĪVĀ IETEKME (procesa pārtraukumi, resursu novirzīšana, sistēmiskās korekcijas)

Katrai dimensijai — konkrēti aprēķini vai pamatoti aplēses ar pieņēmumiem.`,
    joma: "Iepirkumi/būvniecība",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man jāizvērtē konstatējuma ietekme.

KONSTATĒJUMS: Pašvaldības iepirkumā Nr. PI-2024-031 par sociālā centra renovāciju (līgumsumma 612 000 EUR) konstatēts, ka 3 piedāvājumu izvērtēšanas kritēriji (kvalitatīvie) atšķiras no iepirkuma nolikumā publicētajiem. Uzvarētājs izvēlēts ar atšķirīgo kritēriju kopumu.
APJOMS: Līgumsumma 612 000 EUR. Otrā piedāvājuma summa — 587 000 EUR (par 25 000 EUR mazāk). Trešā piedāvājuma summa — 599 000 EUR.

Lūdzu, palīdzi kvantificēt ietekmi 4 dimensijās:

1. FINANSIĀLĀ IETEKME (tiešie zaudējumi, potenciālie zaudējumi, ietaupījumu zudums)
2. JURIDISKĀ IETEKME (iespējamie pārkāpumi, soda risks, atbildības jautājumi)
3. REPUTĀCIJAS IETEKME (sabiedrības uzticības risks, mediju intereses iespējamība)
4. OPERATĪVĀ IETEKME (procesa pārtraukumi, resursu novirzīšana, sistēmiskās korekcijas)

Katrai dimensijai — konkrēti aprēķini vai pamatoti aplēses ar pieņēmumiem.`,
    fields: [
      { key: "konstatejums", label: "Konstatējums", placeholder: "Īsi formulēts konstatējums", multiline: true, rows: 3 },
      { key: "apjoms", label: "Apjoms", placeholder: "Skaitļi — summas, daudzumi, procenti", multiline: true, rows: 2 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man jāizvērtē konstatējuma ietekme.

KONSTATĒJUMS: ${f.konstatejums}
APJOMS: ${f.apjoms}

Lūdzu, palīdzi kvantificēt ietekmi 4 dimensijās:

1. FINANSIĀLĀ IETEKME (tiešie zaudējumi, potenciālie zaudējumi, ietaupījumu zudums)
2. JURIDISKĀ IETEKME (iespējamie pārkāpumi, soda risks, atbildības jautājumi)
3. REPUTĀCIJAS IETEKME (sabiedrības uzticības risks, mediju intereses iespējamība)
4. OPERATĪVĀ IETEKME (procesa pārtraukumi, resursu novirzīšana, sistēmiskās korekcijas)

Katrai dimensijai — konkrēti aprēķini vai pamatoti aplēses ar pieņēmumiem.`,
  },
  {
    nr: 7, posms: "Konstatējums", nosaukums: "Klasifikācija pēc smaguma",
    kad: "Kad ir vairāki konstatējumi un tie jāklasificē pēc smaguma audita ziņojumam",
    karkass: `Esmu pašvaldības iekšējais auditors. Man ir [N] konstatējumi audita ziņojumam.

KONSTATĒJUMI:
1. [konstatējums 1 ar īsu aprakstu un ietekmi]
2. [konstatējums 2 ar īsu aprakstu un ietekmi]
3. [konstatējums 3 ar īsu aprakstu un ietekmi]

Lūdzu, klasificē katru konstatējumu pēc smaguma:

KRITISKS — tūlītēja rīcība nepieciešama, būtiska finansiāla vai juridiska ietekme, sistēmiska problēma
BŪTISKS — nepieciešama mērķtiecīga rīcība, vidēja ietekme, varētu kļūt sistēmisks
VIDĒJS — process jāuzlabo, ierobežota ietekme, lokāla problēma
ZEMS — process jāmonitorē, niecīga ietekme, atsevišķs gadījums

Katram konstatējumam:
- Klasifikācija
- Pamatojums (kāpēc šis līmenis, ne augstāks/zemāks)
- Ieteicamais reaģēšanas laiks (nedēļas/mēneši)
- Vai jāinformē pašvaldības dome formāli vai darba kārtībā`,
    joma: "Nekustamais īpašums",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man ir 4 konstatējumi audita ziņojumam par pašvaldības nomas līgumiem.

KONSTATĒJUMI:
1. 7 nomas līgumiem (no 89 pārbaudītajiem) nav noteikta indeksācijas kārtība — pašvaldības zaudējumi pēdējos 3 gados aplēsti 14 200 EUR
2. 1 nomas līgums (telpas Brīvības ielā 12) nav reģistrēts zemesgrāmatā, kaut ir spēkā kopš 2019. gada
3. 23 nomas līgumiem nomas maksa zem tirgus vērtības (vidēji par 18%), pamatojums dokumentos nav atrodams. Iespējami nepieļaujama valsts atbalsta riski
4. 2 nomas līgumiem nomnieki ir nepilnīgi izpildījuši remontdarbu pienākumus, bet pašvaldība nav piedzinusi sankcijas (līgumcena 8 400 EUR)

Lūdzu, klasificē katru konstatējumu pēc smaguma:

KRITISKS — tūlītēja rīcība nepieciešama, būtiska finansiāla vai juridiska ietekme, sistēmiska problēma
BŪTISKS — nepieciešama mērķtiecīga rīcība, vidēja ietekme, varētu kļūt sistēmisks
VIDĒJS — process jāuzlabo, ierobežota ietekme, lokāla problēma
ZEMS — process jāmonitorē, niecīga ietekme, atsevišķs gadījums

Katram konstatējumam:
- Klasifikācija
- Pamatojums (kāpēc šis līmenis, ne augstāks/zemāks)
- Ieteicamais reaģēšanas laiks (nedēļas/mēneši)
- Vai jāinformē pašvaldības dome formāli vai darba kārtībā`,
    fields: [
      { key: "konstatejumi", label: "Konstatējumi (numerēts saraksts)", placeholder: "1. Konstatējums...\n2. Konstatējums...\n3. Konstatējums...", multiline: true, rows: 8 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man ir konstatējumi audita ziņojumam.

KONSTATĒJUMI:
${f.konstatejumi}

Lūdzu, klasificē katru konstatējumu pēc smaguma:

KRITISKS — tūlītēja rīcība nepieciešama, būtiska finansiāla vai juridiska ietekme, sistēmiska problēma
BŪTISKS — nepieciešama mērķtiecīga rīcība, vidēja ietekme, varētu kļūt sistēmisks
VIDĒJS — process jāuzlabo, ierobežota ietekme, lokāla problēma
ZEMS — process jāmonitorē, niecīga ietekme, atsevišķs gadījums

Katram konstatējumam:
- Klasifikācija
- Pamatojums (kāpēc šis līmenis, ne augstāks/zemāks)
- Ieteicamais reaģēšanas laiks (nedēļas/mēneši)
- Vai jāinformē pašvaldības dome formāli vai darba kārtībā`,
  },
  {
    nr: 8, posms: "Rekomendācijas", nosaukums: "Rekomendāciju variantu ģenerēšana",
    kad: "Pamata pielietojums — kad ir gatavs konstatējums un nepieciešami vairāki rekomendāciju varianti",
    karkass: `Esmu iekšējais auditors pašvaldībā. Man ir audita konstatējums:

FAKTS: [iekopē fakta tekstu]
PIERĀDĪJUMS: [iekopē pierādījuma aprakstu]
IETEKME: [iekopē ietekmes aprakstu]

Lūdzu, piedāvā 3 rekomendāciju variantus:
1. Tūlītēja rīcība pašvaldības iekšienē (1-2 nedēļās)
2. Sistēmiska uzlabošana pašvaldības procesā (3-6 mēnešos)
3. Sadarbība ar valsts iestādi (kuru iestādi un kā)

Katram variantam: kam adresēta, izpildes laiks, sagaidāmais rezultāts.`,
    joma: "Mežs/vide",
    paraugs: `Esmu iekšējais auditors pašvaldībā. Man ir audita konstatējums:

FAKTS: Saldus pašvaldības mežā cirsts 67 ha (VMD saskaņojums 45 ha) — pārsniegums 22 ha.
PIERĀDĪJUMS: Sentinel-2 (2024.04. un 2024.10.) un LVM ĢeoTĪmekļa kvartālu analīze. Kvartāli 409-01 un 409-02 cirsti bez VMD saskaņojuma.
IETEKME: Pārvaldes ziņojuma apgalvojums "saskaņā ar plānu" nav patiess. Risks atkārtotai ciršanai bez saskaņojuma.

Lūdzu, piedāvā 3 rekomendāciju variantus:
1. Tūlītēja rīcība pašvaldības iekšienē (1-2 nedēļās)
2. Sistēmiska uzlabošana pašvaldības procesā (3-6 mēnešos)
3. Sadarbība ar valsts iestādi (kuru iestādi un kā)

Katram variantam: kam adresēta, izpildes laiks, sagaidāmais rezultāts.`,
    fields: [
      { key: "fakts", label: "Fakts", placeholder: "Konstatētais fakts ar skaitļiem", multiline: true, rows: 2 },
      { key: "pieradijums", label: "Pierādījums", placeholder: "Kā fakts pierādīts", multiline: true, rows: 2 },
      { key: "ietekme", label: "Ietekme", placeholder: "Reālie vai potenciālie zaudējumi/riski", multiline: true, rows: 2 },
    ],
    template: (f) => `Esmu iekšējais auditors pašvaldībā. Man ir audita konstatējums:

FAKTS: ${f.fakts}
PIERĀDĪJUMS: ${f.pieradijums}
IETEKME: ${f.ietekme}

Lūdzu, piedāvā 3 rekomendāciju variantus:
1. Tūlītēja rīcība pašvaldības iekšienē (1-2 nedēļās)
2. Sistēmiska uzlabošana pašvaldības procesā (3-6 mēnešos)
3. Sadarbība ar valsts iestādi (kuru iestādi un kā)

Katram variantam: kam adresēta, izpildes laiks, sagaidāmais rezultāts.`,
  },
  {
    nr: 9, posms: "Rekomendācijas", nosaukums: "Rekomendācijas SMART uzlabošana",
    kad: "Kad ir gatavs rekomendācijas pirmais variants, bet jāuzlabo precizitāte un izpildāmība",
    karkass: `Esmu pašvaldības iekšējais auditors. Man ir šāda audita rekomendācija:

[iekopē rekomendāciju]

Lūdzu, izvērtē šo rekomendāciju pēc 4 kritērijiem:
1. SMART — vai mērķis ir specifisks, izmērāms, sasniedzams, relevants, ar termiņu?
2. Skaidrība — vai pašvaldības adresāts viennozīmīgi sapratīs, kas jādara?
3. Izpildāmība — vai tas ir reāli iespējams pašvaldības resursu ietvaros?
4. Verificējamība — vai pēc termiņa varēs pārbaudīt izpildi?

Norādi konkrētus uzlabojumus katrā kritērijā. Beigās — pārformulē rekomendāciju.`,
    joma: "Teritorijas plānošana",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man ir šāda audita rekomendācija:

"Pašvaldības būvvaldei jāuzlabo detālplānojumu izstrādes process un jāievieš stingrāka kontrole pār vides aspektiem aizsargājamās teritorijās."

Lūdzu, izvērtē šo rekomendāciju pēc 4 kritērijiem:
1. SMART — vai mērķis ir specifisks, izmērāms, sasniedzams, relevants, ar termiņu?
2. Skaidrība — vai pašvaldības adresāts viennozīmīgi sapratīs, kas jādara?
3. Izpildāmība — vai tas ir reāli iespējams pašvaldības resursu ietvaros?
4. Verificējamība — vai pēc termiņa varēs pārbaudīt izpildi?

Norādi konkrētus uzlabojumus katrā kritērijā. Beigās — pārformulē rekomendāciju.`,
    fields: [
      { key: "rekomendacija", label: "Rekomendācija", placeholder: "Iekopē rekomendāciju, ko gribi uzlabot", multiline: true, rows: 4 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man ir šāda audita rekomendācija:

"${f.rekomendacija}"

Lūdzu, izvērtē šo rekomendāciju pēc 4 kritērijiem:
1. SMART — vai mērķis ir specifisks, izmērāms, sasniedzams, relevants, ar termiņu?
2. Skaidrība — vai pašvaldības adresāts viennozīmīgi sapratīs, kas jādara?
3. Izpildāmība — vai tas ir reāli iespējams pašvaldības resursu ietvaros?
4. Verificējamība — vai pēc termiņa varēs pārbaudīt izpildi?

Norādi konkrētus uzlabojumus katrā kritērijā. Beigās — pārformulē rekomendāciju.`,
  },
  {
    nr: 10, posms: "Rekomendācijas", nosaukums: "Rekomendāciju prioritizēšana",
    kad: "Kad ir vairākas rekomendācijas un jāzin, kurā secībā tās jāievieš",
    karkass: `Man ir [N] audita rekomendācijas pašvaldības projektam. Lūdzu, palīdzi prioritizēt.

REKOMENDĀCIJAS:
1. [iekopē rekomendāciju 1]
2. [iekopē rekomendāciju 2]
3. [iekopē rekomendāciju 3]

KRITĒRIJI prioritizēšanai pašvaldības kontekstā:
- Riska smagums (kāds zaudējums, ja nereaģējam)
- Pašvaldības spēja izpildīt patstāvīgi (vai vajag valsts iestādes iesaisti)
- Izpildes ātrums un izmaksas

Katrai rekomendācijai novērtē 1-5 skalā un piedāvā ieviešanas secību ar pamatojumu.`,
    joma: "Mežs/vide",
    paraugs: `Man ir 3 audita rekomendācijas Saldus pašvaldības meža projektam. Lūdzu, palīdzi prioritizēt.

REKOMENDĀCIJAS:
1. Veikt mežaudzes atjaunošanu kvartālos 409-01 un 409-02 (12 ha + 10 ha) 6 mēnešu laikā.
2. Ieviest obligātu LVM ĢeoTĪmekļa pārbaudi pirms katras ciršanas darbu sākšanas.
3. Pieprasīt no VMD oficiālu atzinumu par 22 ha pārkāpumu un iespējamām sekām.

KRITĒRIJI prioritizēšanai pašvaldības kontekstā:
- Riska smagums (kāds zaudējums, ja nereaģējam)
- Pašvaldības spēja izpildīt patstāvīgi (vai vajag valsts iestādes iesaisti)
- Izpildes ātrums un izmaksas

Katrai rekomendācijai novērtē 1-5 skalā un piedāvā ieviešanas secību ar pamatojumu.`,
    fields: [
      { key: "rekomendacijas", label: "Rekomendāciju saraksts", placeholder: "1. Rekomendācija...\n2. Rekomendācija...\n3. Rekomendācija...", multiline: true, rows: 6 },
    ],
    template: (f) => `Man ir audita rekomendācijas pašvaldības projektam. Lūdzu, palīdzi prioritizēt.

REKOMENDĀCIJAS:
${f.rekomendacijas}

KRITĒRIJI prioritizēšanai pašvaldības kontekstā:
- Riska smagums (kāds zaudējums, ja nereaģējam)
- Pašvaldības spēja izpildīt patstāvīgi (vai vajag valsts iestādes iesaisti)
- Izpildes ātrums un izmaksas

Katrai rekomendācijai novērtē 1-5 skalā un piedāvā ieviešanas secību ar pamatojumu.`,
  },
  {
    nr: 11, posms: "Rekomendācijas", nosaukums: "Adresāta noteikšana",
    kad: "Kad nav skaidrs, kas pašvaldībā vai valsts iestādē ir atbildīgs par rekomendācijas izpildi",
    karkass: `Man ir audita konstatējums:

[iekopē konstatējumu]

Un piedāvātā rekomendācija:

[iekopē rekomendāciju]

Lūdzu, palīdzi noteikt pašvaldības kontekstā:
1. Kurš pašvaldības darbinieks vai dienests ir tieši atbildīgs?
2. Kāda valsts iestāde (NKMP, VARAM, VMD, LVĢMC, IZM, LM) ir saistīta ar šo jautājumu?
3. Vai pašvaldības dome jāinformē formāli vai darba kārtībā?
4. Vai sabiedrība jāinformē (publiskās intereses) vai tas ir tikai iekšējs jautājums?

Norādi precīzus iestāžu un dienestu nosaukumus.`,
    joma: "Sociālie pakalpojumi",
    paraugs: `Man ir audita konstatējums:

"Pašvaldības sociālā dienesta GMI pabalstu piešķiršanas procesā 14% gadījumu trūkst pilna ienākumu deklarēšanas dokumentācija saskaņā ar MK noteikumiem Nr. 809."

Un piedāvātā rekomendācija:

"Sociālajam dienestam 3 mēnešu laikā jāizstrādā un jāievieš dokumentu pilnības kontrolsaraksts pirms GMI lēmuma pieņemšanas."

Lūdzu, palīdzi noteikt pašvaldības kontekstā:
1. Kurš pašvaldības darbinieks vai dienests ir tieši atbildīgs?
2. Kāda valsts iestāde (NKMP, VARAM, VMD, LVĢMC, IZM, LM) ir saistīta ar šo jautājumu?
3. Vai pašvaldības dome jāinformē formāli vai darba kārtībā?
4. Vai sabiedrība jāinformē (publiskās intereses) vai tas ir tikai iekšējs jautājums?

Norādi precīzus iestāžu un dienestu nosaukumus.`,
    fields: [
      { key: "konstatejums", label: "Konstatējums", placeholder: "Iekopē konstatējumu", multiline: true, rows: 3 },
      { key: "rekomendacija", label: "Rekomendācija", placeholder: "Iekopē rekomendāciju", multiline: true, rows: 3 },
    ],
    template: (f) => `Man ir audita konstatējums:

${f.konstatejums}

Un piedāvātā rekomendācija:

${f.rekomendacija}

Lūdzu, palīdzi noteikt pašvaldības kontekstā:
1. Kurš pašvaldības darbinieks vai dienests ir tieši atbildīgs?
2. Kāda valsts iestāde (NKMP, VARAM, VMD, LVĢMC, IZM, LM) ir saistīta ar šo jautājumu?
3. Vai pašvaldības dome jāinformē formāli vai darba kārtībā?
4. Vai sabiedrība jāinformē (publiskās intereses) vai tas ir tikai iekšējs jautājums?

Norādi precīzus iestāžu un dienestu nosaukumus.`,
  },
  {
    nr: 12, posms: "Sadarbība", nosaukums: "Sadarbības procedūra ar valsts iestādi",
    kad: "Kad konstatējums prasa formālu sadarbību ar VMD, VARAM, NKMP, LVĢMC u.c.",
    karkass: `Esmu pašvaldības iekšējais auditors. Mans konstatējums prasa sadarbību ar valsts iestādi.

KONSTATĒJUMS: [iekopē konstatējumu]
VALSTS IESTĀDE: [piem. VMD]

Lūdzu, palīdzi sagatavot sadarbības procedūru:
1. Kāda formāla informācija pašvaldībai jāiesniedz iestādei?
2. Kāds ir paredzamais reaģēšanas laiks no iestādes puses?
3. Kādi dokumenti pašvaldībai jāuzkrāj pirms iesnieguma?
4. Kāda ir iestādes iespējamā reakcija (lēmuma veidi)?
5. Kā pašvaldība var sekot līdzi sadarbības procesam?

Strukturē atbildi kā pašvaldības iekšējo procedūru ar atbildīgo personu lomām.`,
    joma: "Mežs/vide",
    paraugs: `Esmu pašvaldības iekšējais auditors. Mans konstatējums prasa sadarbību ar valsts iestādi.

KONSTATĒJUMS: Saldus pašvaldības mežā cirsts 22 ha vairāk, nekā saskaņots ar VMD. Kvartāli 409-01 un 409-02 cirsti bez atļaujas.
VALSTS IESTĀDE: VMD (Valsts meža dienests)

Lūdzu, palīdzi sagatavot sadarbības procedūru:
1. Kāda formāla informācija pašvaldībai jāiesniedz iestādei?
2. Kāds ir paredzamais reaģēšanas laiks no iestādes puses?
3. Kādi dokumenti pašvaldībai jāuzkrāj pirms iesnieguma?
4. Kāda ir iestādes iespējamā reakcija (lēmuma veidi)?
5. Kā pašvaldība var sekot līdzi sadarbības procesam?

Strukturē atbildi kā pašvaldības iekšējo procedūru ar atbildīgo personu lomām.`,
    fields: [
      { key: "konstatejums", label: "Konstatējums", placeholder: "Iekopē konstatējumu", multiline: true, rows: 3 },
      { key: "iestade", label: "Valsts iestāde", placeholder: "Piem. VMD, VARAM, NKMP, LVĢMC, IUB" },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Mans konstatējums prasa sadarbību ar valsts iestādi.

KONSTATĒJUMS: ${f.konstatejums}
VALSTS IESTĀDE: ${f.iestade}

Lūdzu, palīdzi sagatavot sadarbības procedūru:
1. Kāda formāla informācija pašvaldībai jāiesniedz iestādei?
2. Kāds ir paredzamais reaģēšanas laiks no iestādes puses?
3. Kādi dokumenti pašvaldībai jāuzkrāj pirms iesnieguma?
4. Kāda ir iestādes iespējamā reakcija (lēmuma veidi)?
5. Kā pašvaldība var sekot līdzi sadarbības procesam?

Strukturē atbildi kā pašvaldības iekšējo procedūru ar atbildīgo personu lomām.`,
  },
  {
    nr: 13, posms: "Sadarbība", nosaukums: "Vēstule/e-pasts valsts iestādei",
    kad: "Kad jāsagatavo formāls iesniegums vai informēšanas vēstule valsts iestādei",
    karkass: `Esmu pašvaldības iekšējais auditors. Man jāsagatavo vēstule valsts iestādei par audita atklājumu.

ADRESĀTS: [iestādes nosaukums un struktūrvienība]
TĒMA: [īsi par ko vēstule]
KONSTATĒJUMS: [iekopē konstatējumu]
PIEPRASĪJUMA TIPS: informēšana / atzinuma pieprasījums / sūdzība / sadarbības lūgums

Lūdzu, sagatavo vēstules projektu, ņemot vērā:
1. Latvijas valsts pārvaldes komunikācijas standartus (formāls tonis, bet ne sausi birokrātisks)
2. Pašvaldības un valsts iestādes attiecības — kā partneri, ne pretinieki
3. Skaidru pieprasījumu vai informāciju — ko sagaidām no iestādes
4. Pievienojamo dokumentu sarakstu

Struktūra: virsraksts, ievads, faktu izklāsts, juridiskais pamats (ja attiecināms), pieprasījums, kontaktinformācija.

NB: Sagatavo projektu, ko parakstīs pašvaldības izpilddirektors vai juridiski atbildīgā persona — ne pats auditors.`,
    joma: "Iepirkumi/būvniecība",
    paraugs: `Esmu pašvaldības iekšējais auditors. Man jāsagatavo vēstule valsts iestādei par audita atklājumu.

ADRESĀTS: Iepirkumu uzraudzības birojs (IUB)
TĒMA: Informēšana par konstatētu nesakritību iepirkuma procedūrā
KONSTATĒJUMS: Pašvaldības iepirkumā Nr. PI-2024-031 par sociālā centra renovāciju (līgumsumma 612 000 EUR) konstatēts, ka 3 piedāvājumu izvērtēšanas kritēriji atšķiras no iepirkuma nolikumā publicētajiem. Iekšējais audits ir noslēgts 12.03.2026.
PIEPRASĪJUMA TIPS: Informēšana ar iespēju saņemt IUB skaidrojumu par piemērojamām normām

Lūdzu, sagatavo vēstules projektu, ņemot vērā:
1. Latvijas valsts pārvaldes komunikācijas standartus (formāls tonis, bet ne sausi birokrātisks)
2. Pašvaldības un valsts iestādes attiecības — kā partneri, ne pretinieki
3. Skaidru pieprasījumu vai informāciju — ko sagaidām no iestādes
4. Pievienojamo dokumentu sarakstu

Struktūra: virsraksts, ievads, faktu izklāsts, juridiskais pamats (ja attiecināms), pieprasījums, kontaktinformācija.

NB: Sagatavo projektu, ko parakstīs pašvaldības izpilddirektors vai juridiski atbildīgā persona — ne pats auditors.`,
    fields: [
      { key: "adresats", label: "Adresāts", placeholder: "Iestādes nosaukums un struktūrvienība" },
      { key: "tema", label: "Tēma", placeholder: "Īsi par ko vēstule" },
      { key: "konstatejums", label: "Konstatējums", placeholder: "Iekopē konstatējumu", multiline: true, rows: 3 },
      { key: "tips", label: "Pieprasījuma tips", placeholder: "informēšana / atzinuma pieprasījums / sūdzība / sadarbības lūgums" },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Man jāsagatavo vēstule valsts iestādei par audita atklājumu.

ADRESĀTS: ${f.adresats}
TĒMA: ${f.tema}
KONSTATĒJUMS: ${f.konstatejums}
PIEPRASĪJUMA TIPS: ${f.tips}

Lūdzu, sagatavo vēstules projektu, ņemot vērā:
1. Latvijas valsts pārvaldes komunikācijas standartus (formāls tonis, bet ne sausi birokrātisks)
2. Pašvaldības un valsts iestādes attiecības — kā partneri, ne pretinieki
3. Skaidru pieprasījumu vai informāciju — ko sagaidām no iestādes
4. Pievienojamo dokumentu sarakstu

Struktūra: virsraksts, ievads, faktu izklāsts, juridiskais pamats (ja attiecināms), pieprasījums, kontaktinformācija.

NB: Sagatavo projektu, ko parakstīs pašvaldības izpilddirektors vai juridiski atbildīgā persona — ne pats auditors.`,
  },
  {
    nr: 14, posms: "Sadarbība", nosaukums: "Audita kopsavilkums domei",
    kad: "Kad audita ziņojums gatavs un nepieciešams kopsavilkums pašvaldības domes sēdei",
    karkass: `Esmu pašvaldības iekšējais auditors. Audita ziņojums gatavs un jāsagatavo kopsavilkums domes sēdei.

AUDITA TĒMA: [audita tēma]
PERIODS: [audita periods]
GALVENIE KONSTATĒJUMI: [3-5 konstatējumi]
GALVENĀS REKOMENDĀCIJAS: [3-5 rekomendācijas]

Lūdzu, sagatavo kopsavilkumu (max 1 lpp.) domes sēdei ar:
1. Audita kontekstu (1 rindkopa)
2. Galvenajiem atklājumiem (3-5 punkti)
3. Riskiem, ja netiek rīkots
4. Galvenajām rekomendācijām (sarakstā, ar prioritāti)
5. Piedāvātajiem domes lēmumiem

Tonis — informējošs, ne aizstāvošs vai apsūdzošs. Cipari un fakti, ne emocijas.
Valoda — pieejama domniekiem, kas nav specializējušies šajā jomā.`,
    joma: "Nekustamais īpašums",
    paraugs: `Esmu pašvaldības iekšējais auditors. Audita ziņojums gatavs un jāsagatavo kopsavilkums domes sēdei.

AUDITA TĒMA: Pašvaldības nomas līgumu portfeļa pārvaldība
PERIODS: 01.01.2022 – 31.12.2024
GALVENIE KONSTATĒJUMI: 89 aktīvi nomas līgumi, kopējā gada nomas maksa 187 000 EUR. 23 līgumiem (26%) nomas maksa zem tirgus vērtības par 18%. 7 līgumiem nav indeksācijas — zaudējumi 14 200 EUR. 1 līgums nav reģistrēts zemesgrāmatā kopš 2019. 2 līgumiem sankcijas (8 400 EUR) nav piedzītas.
GALVENĀS REKOMENDĀCIJAS: Inventarizācija 6 mēnešos, nomas maksas metodika ar tirgus atsauci, neregistrētā līguma reģistrācija 30 dienās, sankciju piedziņa.

Lūdzu, sagatavo kopsavilkumu (max 1 lpp.) domes sēdei ar:
1. Audita kontekstu (1 rindkopa)
2. Galvenajiem atklājumiem (3-5 punkti)
3. Riskiem, ja netiek rīkots
4. Galvenajām rekomendācijām (sarakstā, ar prioritāti)
5. Piedāvātajiem domes lēmumiem

Tonis — informējošs, ne aizstāvošs vai apsūdzošs. Cipari un fakti, ne emocijas.
Valoda — pieejama domniekiem, kas nav specializējušies šajā jomā.`,
    fields: [
      { key: "tema", label: "Audita tēma", placeholder: "Piem. Pašvaldības nomas līgumu portfeļa pārvaldība" },
      { key: "periods", label: "Periods", placeholder: "Piem. 01.01.2022 – 31.12.2024" },
      { key: "konstatejumi", label: "Galvenie konstatējumi", placeholder: "3-5 konstatējumi", multiline: true, rows: 4 },
      { key: "rekomendacijas", label: "Galvenās rekomendācijas", placeholder: "3-5 rekomendācijas", multiline: true, rows: 4 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Audita ziņojums gatavs un jāsagatavo kopsavilkums domes sēdei.

AUDITA TĒMA: ${f.tema}
PERIODS: ${f.periods}
GALVENIE KONSTATĒJUMI: ${f.konstatejumi}
GALVENĀS REKOMENDĀCIJAS: ${f.rekomendacijas}

Lūdzu, sagatavo kopsavilkumu (max 1 lpp.) domes sēdei ar:
1. Audita kontekstu (1 rindkopa)
2. Galvenajiem atklājumiem (3-5 punkti)
3. Riskiem, ja netiek rīkots
4. Galvenajām rekomendācijām (sarakstā, ar prioritāti)
5. Piedāvātajiem domes lēmumiem

Tonis — informējošs, ne aizstāvošs vai apsūdzošs. Cipari un fakti, ne emocijas.
Valoda — pieejama domniekiem, kas nav specializējušies šajā jomā.`,
  },
  {
    nr: 15, posms: "Atskats", nosaukums: "Audita procesa pašrefleksija",
    kad: "Pēc audita pabeigšanas — lai izvērtētu pašu auditora darbu un identificētu uzlabojumus nākamajiem auditiem",
    karkass: `Esmu pašvaldības iekšējais auditors. Tikko pabeidzu auditu un vēlos veikt strukturētu pašrefleksiju.

AUDITA TĒMA: [audita tēma]
ILGUMS: [cik nedēļas/mēneši]
GALVENIE IZAICINĀJUMI: [ar ko bija grūti tikt galā]
KAS NOGĀJA LABI: [kas bija stiprākā audita daļa]

Lūdzu, palīdzi strukturēt pašrefleksiju 5 jomās:
1. PIERĀDĪJUMU SAVĀKŠANA
2. ANALĪZE UN SECINĀJUMI
3. KOMUNIKĀCIJA
4. LAIKA PĀRVALDĪBA
5. PROFESIONĀLĀ ATTĪSTĪBA

Strukturē kā tabulu ar konkrētām darbībām katrā jomā.`,
    joma: "Universāls",
    paraugs: `Esmu pašvaldības iekšējais auditors. Tikko pabeidzu auditu un vēlos veikt strukturētu pašrefleksiju.

AUDITA TĒMA: Pašvaldības meža apsaimniekošanas process 2024. gadā
ILGUMS: 4 mēneši (no plānošanas līdz ziņojuma iesniegšanai)
GALVENIE IZAICINĀJUMI: Pirmo reizi izmantoju ģeotelpiskos rīkus (Sentinel-2, LVM ĢeoTĪmeklis). Sākumā nesapratu, kā lasīt NDVI vērtības. Sadarbība ar VMD bija lēna — atbilde uz pieprasījumu nāca 6 nedēļās.
KAS NOGĀJA LABI: Atklājums bija pamatots ar neatkarīgiem datiem (satelītu attēli), ne tikai ar pašvaldības iekšējiem dokumentiem. Tas padarīja konstatējumu neapstrīdamu.

Lūdzu, palīdzi strukturēt pašrefleksiju 5 jomās:
1. PIERĀDĪJUMU SAVĀKŠANA
2. ANALĪZE UN SECINĀJUMI
3. KOMUNIKĀCIJA
4. LAIKA PĀRVALDĪBA
5. PROFESIONĀLĀ ATTĪSTĪBA

Strukturē kā tabulu ar konkrētām darbībām katrā jomā.`,
    fields: [
      { key: "tema", label: "Audita tēma", placeholder: "Piem. Pašvaldības meža apsaimniekošanas process 2024" },
      { key: "ilgums", label: "Ilgums", placeholder: "Piem. 4 mēneši" },
      { key: "izaicinajumi", label: "Galvenie izaicinājumi", placeholder: "Ar ko bija grūti tikt galā", multiline: true, rows: 3 },
      { key: "labi", label: "Kas nogāja labi", placeholder: "Kas bija stiprākā audita daļa", multiline: true, rows: 3 },
    ],
    template: (f) => `Esmu pašvaldības iekšējais auditors. Tikko pabeidzu auditu un vēlos veikt strukturētu pašrefleksiju.

AUDITA TĒMA: ${f.tema}
ILGUMS: ${f.ilgums}
GALVENIE IZAICINĀJUMI: ${f.izaicinajumi}
KAS NOGĀJA LABI: ${f.labi}

Lūdzu, palīdzi strukturēt pašrefleksiju 5 jomās:
1. PIERĀDĪJUMU SAVĀKŠANA
2. ANALĪZE UN SECINĀJUMI
3. KOMUNIKĀCIJA
4. LAIKA PĀRVALDĪBA
5. PROFESIONĀLĀ ATTĪSTĪBA

Strukturē kā tabulu ar konkrētām darbībām katrā jomā.`,
  },
];

// Krāsu palete
const POSMS_COLOR = {
  "Plānošana": { bg: "var(--blue-light)", border: "var(--blue)", text: "#0277A0" },
  "Konstatējums": { bg: "var(--orange-light)", border: "var(--orange)", text: "#A04500" },
  "Rekomendācijas": { bg: "var(--teal-light)", border: "var(--teal)", text: "#005A40" },
  "Sadarbība": { bg: "var(--purple-light)", border: "var(--purple)", text: "var(--purple-dark)" },
  "Atskats": { bg: "var(--grey-light)", border: "var(--grey)", text: "var(--dark)" },
};

const JOMAS = [
  "Visas jomas", "Mežs/vide", "Iepirkumi/būvniecība", "Sociālie pakalpojumi",
  "Nekustamais īpašums", "Teritorijas plānošana", "Vide/teritorijas plānošana", "Universāls"
];

const POSMI = ["Visi posmi", "Plānošana", "Konstatējums", "Rekomendācijas", "Sadarbība", "Atskats"];

const CHECKLIST = [
  { kat: "FAKTI", jaut: "Vai MI piesauca konkrētus skaitļus, datumus, normatīvos aktus? Pārbaudi pirmavotos." },
  { kat: "IESTĀDES", jaut: "Vai MI piedāvā kontaktu ar konkrētu valsts iestādi? Pārbaudi, vai šī iestāde reāli ir atbildīga par šo jautājumu (MI bieži kļūdās par VMD/VARAM kompetenču sadalījumu)." },
  { kat: "TERMIŅI", jaut: "Vai piedāvātie termiņi ir reāli pašvaldības resursu ietvaros? Vai termiņš atbilst normatīvajiem aktiem?" },
  { kat: "PROCEDŪRAS", jaut: "Vai MI piedāvātā sadarbības procedūra ar valsts iestādi atbilst reālai praksei? Pārbaudi pašvaldības iekšējos noteikumos." },
  { kat: "RISKI", jaut: "Vai MI nav pieminējis riskus, kas varētu rasties no rekomendācijas izpildes? Vai tu pats redzi tos?" },
  { kat: "AVOTI", jaut: "Vai MI norādīja avotus uz konkrētiem normatīviem vai dokumentiem? Pārbaudi, vai tie reāli eksistē un vai MI tos pareizi citē." },
  { kat: "KONFLIKTI", jaut: "Vai MI atbilde nav pretrunā ar pašvaldības iepriekšējiem lēmumiem vai politikām?" },
  { kat: "ALTERNATĪVAS", jaut: "Vai MI piedāvātais variants ir vienīgais? Vai jautājums par citām alternatīvām dotu citas atbildes?" },
  { kat: "VALODA", jaut: "Vai MI atbildes valoda ir piemērota audita ziņojumam? Vai jāpārformulē formālāk vai konkrētāk?" },
  { kat: "ATBILDĪBA", jaut: "Vai MI atbildē nav slēptu pieņēmumu par atbildību? Vai pašvaldības darbinieki, kas lasīs ziņojumu, sapratīs precīzi?" },
];

const QUALITY_PRINCIPLES = [
  { p: "LOMA", v: "'Pastāsti par audita rekomendācijām'", l: "'Esmu pašvaldības iekšējais auditors. Lūdzu sniedz rekomendācijas...'" },
  { p: "KONTEKSTS", v: "'Kā uzlabot iepirkuma procesu?'", l: "'Pašvaldības iepirkumā konstatētas X nesakritības. Budžets 612 000 EUR. Jautājums — kā uzlabot procesu?'" },
  { p: "KONKRĒTI DATI", v: "'Mežā cirsts daudz vairāk nekā plānots'", l: "'Mežā cirsts 67 ha, plānoti 45 ha (VMD saskaņojums). Pārsniegums 22 ha kvartālos 409-01, 409-02.'" },
  { p: "STRUKTŪRA", v: "'Kas man jādara tālāk?'", l: "'Strukturē atbildi 3 daļās: 1) Tūlītēja rīcība (1-2 ned.), 2) Sistēmiska uzlabošana (3-6 mēn.), 3) Sadarbība ar VMD.'" },
  { p: "OUTPUT FORMĀTS", v: "Bez specifikācijas", l: "'Strukturē kā tabulu ar kolonnām: Risks | Iespējamība | Ietekme | Reaģēšanas laiks. Maks. 7 rindas.'" },
  { p: "OGRANIČOJUMI", v: "Bez ierobežojumiem", l: "'Ja neesi pārliecināts par X, norādi to skaidri — es pārbaudīšu pirmavotos. Neizdomā konkrētus skaitļus.'" },
];

// ============================================================
// KOMPONENTES
// ============================================================

function CopyButton({ text, label = "Kopēt" }) {
  const [copied, setCopied] = useState(false);
  const handleCopy = () => {
    if (!text) return;
    navigator.clipboard.writeText(text).then(() => {
      setCopied(true);
      setTimeout(() => setCopied(false), 2000);
    }).catch(() => {
      // Fallback
      const ta = document.createElement('textarea');
      ta.value = text;
      document.body.appendChild(ta);
      ta.select();
      try { document.execCommand('copy'); setCopied(true); setTimeout(() => setCopied(false), 2000); } catch {}
      document.body.removeChild(ta);
    });
  };
  return (
    <button
      onClick={handleCopy}
      style={{
        background: copied ? 'var(--green)' : 'var(--purple)',
        color: 'white',
        border: 'none',
        padding: '8px 16px',
        borderRadius: '6px',
        fontWeight: 'bold',
        fontSize: '13px',
        transition: 'background 0.2s',
      }}
    >
      {copied ? '✓ Nokopēts' : label}
    </button>
  );
}

function Header({ activeTab, setActiveTab }) {
  const tabs = [
    { id: 'sakums', label: 'Sākums' },
    { id: 'sabloni', label: 'Šabloni' },
    { id: 'darba_lapa', label: 'Mana darba lapa' },
    { id: 'izvertesana', label: 'MI izvērtēšana' },
    { id: 'kvalitate', label: 'Promptu kvalitāte' },
  ];
  return (
    <header style={{ background: 'white', borderBottom: '1px solid var(--grey-border)', position: 'sticky', top: 0, zIndex: 100 }}>
      <div style={{ maxWidth: '1200px', margin: '0 auto', padding: '16px 24px' }}>
        <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center', marginBottom: '12px' }}>
          <div>
            <h1 style={{ margin: 0, color: 'var(--purple-dark)', fontSize: '22px' }}>MI promptu kolekcija</h1>
            <p style={{ margin: '4px 0 0 0', color: 'var(--grey)', fontSize: '13px', fontStyle: 'italic' }}>
              B grupa · pašvaldības iekšējie auditori · VI modulis
            </p>
          </div>
        </div>
        <nav style={{ display: 'flex', gap: '4px', flexWrap: 'wrap' }} className="no-print">
          {tabs.map(t => (
            <button
              key={t.id}
              onClick={() => setActiveTab(t.id)}
              style={{
                padding: '10px 18px',
                background: activeTab === t.id ? 'var(--purple)' : 'transparent',
                color: activeTab === t.id ? 'white' : 'var(--dark)',
                border: '1px solid ' + (activeTab === t.id ? 'var(--purple)' : 'var(--grey-border)'),
                borderRadius: '6px',
                fontWeight: activeTab === t.id ? 'bold' : 'normal',
                fontSize: '14px',
                transition: 'all 0.2s',
              }}
            >
              {t.label}
            </button>
          ))}
        </nav>
      </div>
    </header>
  );
}

function Sakums({ setActiveTab }) {
  return (
    <div style={{ maxWidth: '900px', margin: '0 auto', padding: '32px 24px' }}>
      <div style={{
        background: 'var(--purple-light)',
        border: '2px solid var(--purple)',
        borderRadius: '8px',
        padding: '24px',
        marginBottom: '32px',
        textAlign: 'center',
      }}>
        <h2 style={{ color: 'var(--purple-dark)', margin: '0 0 12px 0', fontSize: '20px' }}>
          MI rīks dod struktūru — pašvaldības auditors saglabā spriedumu un atbildību
        </h2>
        <p style={{ margin: 0, color: 'var(--purple-dark)', fontWeight: 'bold', fontSize: '15px' }}>
          Pašvaldības konstatējums + valsts iestādes datu apstiprinājums = uzticams pierādījums
        </p>
      </div>

      <div style={{ background: 'var(--red-light)', border: '1px solid var(--red)', borderRadius: '8px', padding: '20px', marginBottom: '24px' }}>
        <h3 style={{ margin: '0 0 16px 0', color: 'var(--red)', fontSize: '16px' }}>PIRMS IEVADI DATUS MI RĪKĀ</h3>
        <ul style={{ margin: 0, paddingLeft: '20px', lineHeight: 1.8 }}>
          <li><strong>NEKAD</strong> neievadi sensitīvus datus (personas datus, slepenus dokumentus, klasificētu informāciju)</li>
          <li><strong>ANONIMIZĒ</strong> iestāžu un projektu nosaukumus, ja tie nav publiski. Pašvaldībai īpaši — projekta vadītāju vārdus</li>
          <li><strong>PĀRBAUDI</strong>, vai tava pašvaldība atļauj MI rīku izmantošanu darba uzdevumiem</li>
          <li><strong>IZVĒRTĒ</strong> MI atbildi pirms iekļaušanas audita ziņojumā — ar 'MI izvērtēšana' kontrolsarakstu</li>
          <li><strong>DOKUMENTĒ</strong> kuru MI rīku lietoji, kāds bija prompts, kāda bija atbilde — audita pierādījumu pakas daļa</li>
        </ul>
      </div>

      <h3 style={{ color: 'var(--purple-dark)', marginTop: '32px' }}>Kas ir šajā kolekcijā</h3>
      <div style={{ display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(280px, 1fr))', gap: '16px', marginTop: '16px' }}>
        {[
          { title: 'Šabloni', desc: '15 promptu šabloni — 5 audita posmos. Skaties karkasu (tukšu) vai aizpildītu paraugu no 5 jomām.', tab: 'sabloni' },
          { title: 'Mana darba lapa', desc: 'Aizpildi savus konstatējuma datus — sistēma ģenerē gatavu promptu, ko kopēt MI rīkā.', tab: 'darba_lapa' },
          { title: 'MI izvērtēšana', desc: '10 punktu kontrolsaraksts MI atbildes pārbaudei pirms iekļaušanas audita ziņojumā.', tab: 'izvertesana' },
          { title: 'Promptu kvalitāte', desc: 'Ja MI atbilde nav apmierinoša — bieži problēma ir promptā. 6 principi labākam promptam.', tab: 'kvalitate' },
        ].map((card, i) => (
          <div key={i} onClick={() => setActiveTab(card.tab)} style={{
            background: 'white',
            border: '1px solid var(--grey-border)',
            borderRadius: '8px',
            padding: '20px',
            cursor: 'pointer',
            transition: 'all 0.2s',
          }}
            onMouseEnter={e => { e.currentTarget.style.borderColor = 'var(--purple)'; e.currentTarget.style.transform = 'translateY(-2px)'; }}
            onMouseLeave={e => { e.currentTarget.style.borderColor = 'var(--grey-border)'; e.currentTarget.style.transform = 'translateY(0)'; }}
          >
            <h4 style={{ margin: '0 0 8px 0', color: 'var(--purple-dark)' }}>{card.title}</h4>
            <p style={{ margin: 0, fontSize: '13px', color: 'var(--grey)' }}>{card.desc}</p>
          </div>
        ))}
      </div>

      <h3 style={{ color: 'var(--purple-dark)', marginTop: '32px' }}>15 šabloni pa audita posmiem</h3>
      <div style={{ display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(180px, 1fr))', gap: '12px', marginTop: '16px' }}>
        {Object.keys(POSMS_COLOR).map(posms => {
          const count = TEMPLATES.filter(t => t.posms === posms).length;
          const c = POSMS_COLOR[posms];
          return (
            <div key={posms} style={{
              background: c.bg,
              borderLeft: `4px solid ${c.border}`,
              padding: '16px',
              borderRadius: '4px',
            }}>
              <div style={{ fontWeight: 'bold', color: c.text, fontSize: '14px' }}>{posms}</div>
              <div style={{ fontSize: '24px', fontWeight: 'bold', color: c.text, fontFamily: 'Arial Black' }}>{count}</div>
              <div style={{ fontSize: '11px', color: 'var(--grey)' }}>šablon{count === 1 ? 's' : 'i'}</div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

function Sabloni() {
  const [filterPosms, setFilterPosms] = useState("Visi posmi");
  const [filterJoma, setFilterJoma] = useState("Visas jomas");
  const [search, setSearch] = useState("");
  const [view, setView] = useState("karkass");
  const [expandedNr, setExpandedNr] = useState(null);

  const filtered = useMemo(() => {
    return TEMPLATES.filter(t => {
      if (filterPosms !== "Visi posmi" && t.posms !== filterPosms) return false;
      if (filterJoma !== "Visas jomas" && t.joma !== filterJoma) return false;
      if (search && !(`${t.nosaukums} ${t.kad}`).toLowerCase().includes(search.toLowerCase())) return false;
      return true;
    });
  }, [filterPosms, filterJoma, search]);

  return (
    <div style={{ maxWidth: '1100px', margin: '0 auto', padding: '24px' }}>
      <div style={{ marginBottom: '24px' }}>
        <h2 style={{ color: 'var(--purple-dark)', margin: '0 0 8px 0' }}>15 šabloni</h2>
        <p style={{ margin: 0, color: 'var(--grey)', fontSize: '14px' }}>
          Filtrē pēc posma vai jomas. Klikšķini uz šablona, lai redzētu pilnu tekstu.
        </p>
      </div>

      <div style={{ display: 'flex', gap: '12px', flexWrap: 'wrap', marginBottom: '20px', background: 'white', padding: '16px', borderRadius: '8px', border: '1px solid var(--grey-border)' }} className="no-print">
        <div style={{ flex: '1 1 200px' }}>
          <label style={{ display: 'block', fontSize: '12px', fontWeight: 'bold', marginBottom: '4px', color: 'var(--grey)' }}>POSMS</label>
          <select value={filterPosms} onChange={e => setFilterPosms(e.target.value)} style={{ width: '100%', padding: '8px', borderRadius: '4px', border: '1px solid var(--grey-border)' }}>
            {POSMI.map(p => <option key={p}>{p}</option>)}
          </select>
        </div>
        <div style={{ flex: '1 1 200px' }}>
          <label style={{ display: 'block', fontSize: '12px', fontWeight: 'bold', marginBottom: '4px', color: 'var(--grey)' }}>JOMA</label>
          <select value={filterJoma} onChange={e => setFilterJoma(e.target.value)} style={{ width: '100%', padding: '8px', borderRadius: '4px', border: '1px solid var(--grey-border)' }}>
            {JOMAS.map(j => <option key={j}>{j}</option>)}
          </select>
        </div>
        <div style={{ flex: '2 1 200px' }}>
          <label style={{ display: 'block', fontSize: '12px', fontWeight: 'bold', marginBottom: '4px', color: 'var(--grey)' }}>MEKLĒT</label>
          <input type="text" value={search} onChange={e => setSearch(e.target.value)} placeholder="Meklē šablonā..." style={{ width: '100%', padding: '8px', borderRadius: '4px', border: '1px solid var(--grey-border)' }} />
        </div>
        <div>
          <label style={{ display: 'block', fontSize: '12px', fontWeight: 'bold', marginBottom: '4px', color: 'var(--grey)' }}>SKATS</label>
          <div style={{ display: 'flex', borderRadius: '4px', overflow: 'hidden', border: '1px solid var(--grey-border)' }}>
            <button onClick={() => setView("karkass")} style={{ padding: '8px 14px', background: view === 'karkass' ? 'var(--purple)' : 'white', color: view === 'karkass' ? 'white' : 'var(--dark)', border: 'none', fontSize: '13px' }}>Karkass</button>
            <button onClick={() => setView("paraugs")} style={{ padding: '8px 14px', background: view === 'paraugs' ? 'var(--purple)' : 'white', color: view === 'paraugs' ? 'white' : 'var(--dark)', border: 'none', fontSize: '13px' }}>Paraugs</button>
          </div>
        </div>
      </div>

      <div style={{ marginBottom: '12px', fontSize: '13px', color: 'var(--grey)' }}>
        Atrasti: <strong>{filtered.length}</strong> no {TEMPLATES.length} šabloniem
      </div>

      <div style={{ display: 'flex', flexDirection: 'column', gap: '12px' }}>
        {filtered.map(t => {
          const c = POSMS_COLOR[t.posms];
          const expanded = expandedNr === t.nr;
          const text = view === 'karkass' ? t.karkass : t.paraugs;
          return (
            <div key={t.nr} style={{
              background: 'white',
              border: '1px solid var(--grey-border)',
              borderLeft: `4px solid ${c.border}`,
              borderRadius: '6px',
              overflow: 'hidden',
            }}>
              <div onClick={() => setExpandedNr(expanded ? null : t.nr)} style={{
                padding: '14px 18px',
                cursor: 'pointer',
                display: 'flex',
                gap: '16px',
                alignItems: 'center',
              }}>
                <div style={{
                  background: c.border, color: 'white', fontWeight: 'bold',
                  width: '36px', height: '36px', display: 'flex', alignItems: 'center', justifyContent: 'center',
                  borderRadius: '50%', fontSize: '14px', flexShrink: 0,
                }}>{t.nr}</div>
                <div style={{ flex: 1, minWidth: 0 }}>
                  <div style={{ display: 'flex', gap: '8px', flexWrap: 'wrap', alignItems: 'center', marginBottom: '4px' }}>
                    <span style={{ background: c.bg, color: c.text, fontSize: '11px', fontWeight: 'bold', padding: '2px 8px', borderRadius: '10px' }}>{t.posms}</span>
                    <span style={{ background: 'var(--grey-light)', color: 'var(--grey)', fontSize: '11px', padding: '2px 8px', borderRadius: '10px' }}>{t.joma}</span>
                  </div>
                  <div style={{ fontWeight: 'bold', fontSize: '15px', color: 'var(--dark)' }}>{t.nosaukums}</div>
                  <div style={{ fontSize: '12px', color: 'var(--grey)', fontStyle: 'italic', marginTop: '2px' }}>{t.kad}</div>
                </div>
                <div style={{ color: 'var(--grey)', fontSize: '20px', flexShrink: 0 }}>
                  {expanded ? '▾' : '▸'}
                </div>
              </div>
              {expanded && (
                <div style={{ padding: '0 18px 18px 18px', borderTop: '1px solid var(--grey-border)' }}>
                  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center', marginTop: '14px', marginBottom: '8px' }}>
                    <div style={{ fontSize: '12px', fontWeight: 'bold', color: 'var(--grey)' }}>
                      {view === 'karkass' ? 'KARKASS — kopē un aizpildi vietas ar [kvadrātiekavām]' : `AIZPILDĪTS PARAUGS — joma: ${t.joma}`}
                    </div>
                    <CopyButton text={text} />
                  </div>
                  <pre style={{
                    background: '#F8F8FA',
                    border: '1px solid var(--grey-border)',
                    borderRadius: '4px',
                    padding: '14px',
                    margin: 0,
                    whiteSpace: 'pre-wrap',
                    fontFamily: '"Consolas", monospace',
                    fontSize: '12.5px',
                    lineHeight: 1.6,
                  }}>{text}</pre>
                </div>
              )}
            </div>
          );
        })}
      </div>
    </div>
  );
}

function DarbaLapa() {
  const [selectedNr, setSelectedNr] = useState(8);
  const [fields, setFields] = useState({});

  const template = TEMPLATES.find(t => t.nr === selectedNr);

  // Reset fields when template changes
  useEffect(() => {
    const initialFields = {};
    template.fields.forEach(f => { initialFields[f.key] = ""; });
    setFields(initialFields);
  }, [selectedNr]);

  const handleFieldChange = (key, value) => {
    setFields(prev => ({ ...prev, [key]: value }));
  };

  // Aizvieto tukšos laukus ar [aizpildi šeit] norādēm
  const filledFields = useMemo(() => {
    const result = {};
    template.fields.forEach(f => {
      result[f.key] = fields[f.key]?.trim() || `[${f.label.toLowerCase()} — aizpildi šo lauku]`;
    });
    return result;
  }, [fields, template]);

  const generatedPrompt = useMemo(() => {
    return template.template(filledFields);
  }, [filledFields, template]);

  const allFilled = template.fields.every(f => fields[f.key]?.trim());
  const c = POSMS_COLOR[template.posms];

  return (
    <div style={{ maxWidth: '1100px', margin: '0 auto', padding: '24px' }}>
      <div style={{ marginBottom: '24px' }}>
        <h2 style={{ color: 'var(--purple-dark)', margin: '0 0 8px 0' }}>Mana darba lapa</h2>
        <p style={{ margin: 0, color: 'var(--grey)', fontSize: '14px' }}>
          Izvēlies šablonu, aizpildi laukus, kopē ģenerēto promptu MI rīkā.
        </p>
      </div>

      <div style={{ background: 'white', border: '1px solid var(--grey-border)', borderRadius: '8px', padding: '20px', marginBottom: '20px' }}>
        <div style={{ display: 'flex', alignItems: 'center', gap: '12px', marginBottom: '16px' }}>
          <div style={{ background: 'var(--purple)', color: 'white', borderRadius: '50%', width: '28px', height: '28px', display: 'flex', alignItems: 'center', justifyContent: 'center', fontWeight: 'bold', fontSize: '14px' }}>1</div>
          <h3 style={{ margin: 0, color: 'var(--purple-dark)' }}>Izvēlies šablonu</h3>
        </div>
        <select value={selectedNr} onChange={e => setSelectedNr(Number(e.target.value))} style={{ width: '100%', padding: '12px', borderRadius: '6px', border: '2px solid var(--purple)', fontSize: '14px', fontWeight: 'bold' }}>
          {TEMPLATES.map(t => (
            <option key={t.nr} value={t.nr}>
              {t.nr}. [{t.posms}] {t.nosaukums}
            </option>
          ))}
        </select>
        <div style={{ marginTop: '10px', padding: '10px 14px', background: c.bg, borderLeft: `3px solid ${c.border}`, borderRadius: '4px', fontSize: '13px', color: c.text }}>
          <strong>Kad lietot:</strong> {template.kad}
        </div>
      </div>

      <div style={{ background: 'white', border: '1px solid var(--grey-border)', borderRadius: '8px', padding: '20px', marginBottom: '20px' }}>
        <div style={{ display: 'flex', alignItems: 'center', gap: '12px', marginBottom: '16px' }}>
          <div style={{ background: 'var(--purple)', color: 'white', borderRadius: '50%', width: '28px', height: '28px', display: 'flex', alignItems: 'center', justifyContent: 'center', fontWeight: 'bold', fontSize: '14px' }}>2</div>
          <h3 style={{ margin: 0, color: 'var(--purple-dark)' }}>Aizpildi laukus</h3>
        </div>
        <div style={{ display: 'flex', flexDirection: 'column', gap: '14px' }}>
          {template.fields.map(f => (
            <div key={f.key}>
              <label style={{ display: 'block', fontWeight: 'bold', fontSize: '13px', marginBottom: '6px', color: 'var(--dark)' }}>{f.label}</label>
              {f.multiline ? (
                <textarea
                  value={fields[f.key] || ""}
                  onChange={e => handleFieldChange(f.key, e.target.value)}
                  placeholder={f.placeholder}
                  rows={f.rows || 3}
                  style={{
                    width: '100%', padding: '10px',
                    borderRadius: '6px',
                    border: '2px solid var(--teal)',
                    background: fields[f.key]?.trim() ? 'white' : 'var(--teal-light)',
                    fontSize: '13px', fontFamily: 'Arial, sans-serif',
                  }}
                />
              ) : (
                <input
                  type="text"
                  value={fields[f.key] || ""}
                  onChange={e => handleFieldChange(f.key, e.target.value)}
                  placeholder={f.placeholder}
                  style={{
                    width: '100%', padding: '10px',
                    borderRadius: '6px',
                    border: '2px solid var(--teal)',
                    background: fields[f.key]?.trim() ? 'white' : 'var(--teal-light)',
                    fontSize: '13px',
                  }}
                />
              )}
            </div>
          ))}
        </div>
      </div>

      <div style={{ background: 'white', border: '2px solid var(--orange)', borderRadius: '8px', padding: '20px', marginBottom: '20px' }}>
        <div style={{ display: 'flex', alignItems: 'center', gap: '12px', marginBottom: '16px', justifyContent: 'space-between', flexWrap: 'wrap' }}>
          <div style={{ display: 'flex', alignItems: 'center', gap: '12px' }}>
            <div style={{ background: 'var(--orange)', color: 'white', borderRadius: '50%', width: '28px', height: '28px', display: 'flex', alignItems: 'center', justifyContent: 'center', fontWeight: 'bold', fontSize: '14px' }}>3</div>
            <h3 style={{ margin: 0, color: '#A04500' }}>Ģenerētais prompts</h3>
            {!allFilled && <span style={{ fontSize: '12px', color: 'var(--orange)', fontStyle: 'italic' }}>(aizpildi visus laukus, lai prompts būtu pilnīgs)</span>}
          </div>
          <CopyButton text={generatedPrompt} label="Kopēt promptu" />
        </div>
        <pre style={{
          background: '#FFF8E1',
          border: '1px solid var(--orange)',
          borderRadius: '6px',
          padding: '14px',
          margin: 0,
          whiteSpace: 'pre-wrap',
          fontFamily: '"Consolas", monospace',
          fontSize: '12.5px',
          lineHeight: 1.6,
        }}>{generatedPrompt}</pre>
      </div>

      <div style={{ background: 'var(--blue-light)', border: '1px solid var(--blue)', borderRadius: '8px', padding: '16px' }}>
        <strong style={{ color: '#0277A0' }}>Pēc MI atbildes saņemšanas:</strong> Pirms iekļauj atbildi audita ziņojumā, izvērtē to ar kontrolsarakstu cilnē <strong>"MI izvērtēšana"</strong>. MI dod struktūru — pašvaldības auditors saglabā spriedumu un atbildību.
      </div>
    </div>
  );
}

function Izvertesana() {
  const [statuss, setStatuss] = useState({});
  const [piezimes, setPiezimes] = useState({});
  const [galaLemums, setGalaLemums] = useState("");
  const [datums, setDatums] = useState("");

  const handleReset = () => {
    if (confirm('Vai dzēst visus ievadītos datus?')) {
      setStatuss({});
      setPiezimes({});
      setGalaLemums("");
      setDatums("");
    }
  };

  const stats = useMemo(() => {
    const s = { ok: 0, parbaudit: 0, kluda: 0, neattiecas: 0, tukss: 0 };
    CHECKLIST.forEach((_, i) => {
      const st = statuss[i] || "";
      if (st === "OK") s.ok++;
      else if (st === "Pārbaudīt") s.parbaudit++;
      else if (st === "Kļūda") s.kluda++;
      else if (st === "Neattiecas") s.neattiecas++;
      else s.tukss++;
    });
    return s;
  }, [statuss]);

  return (
    <div style={{ maxWidth: '1100px', margin: '0 auto', padding: '24px' }}>
      <div style={{ marginBottom: '24px', display: 'flex', justifyContent: 'space-between', alignItems: 'flex-start', flexWrap: 'wrap', gap: '16px' }}>
        <div>
          <h2 style={{ color: 'var(--purple-dark)', margin: '0 0 8px 0' }}>MI atbildes izvērtēšana</h2>
          <p style={{ margin: 0, color: 'var(--grey)', fontSize: '14px' }}>
            MI rīki var izgudrot informāciju, kas izklausās ticami. Pārbaudi ar šo kontrolsarakstu pirms iekļaušanas audita ziņojumā.
          </p>
        </div>
        <button onClick={handleReset} className="no-print" style={{ background: 'var(--grey-light)', color: 'var(--dark)', border: '1px solid var(--grey-border)', padding: '8px 16px', borderRadius: '6px', fontSize: '13px' }}>
          Dzēst visu
        </button>
      </div>

      <div style={{ display: 'flex', gap: '8px', flexWrap: 'wrap', marginBottom: '20px' }}>
        <StatBadge label="OK" value={stats.ok} bg="var(--teal-light)" color="var(--green)" />
        <StatBadge label="Pārbaudīt" value={stats.parbaudit} bg="var(--yellow)" color="#A07000" />
        <StatBadge label="Kļūda" value={stats.kluda} bg="var(--red-light)" color="var(--red)" />
        <StatBadge label="Neattiecas" value={stats.neattiecas} bg="var(--grey-light)" color="var(--grey)" />
        <StatBadge label="Tukšs" value={stats.tukss} bg="white" color="var(--grey)" border />
      </div>

      <div style={{ background: 'white', border: '1px solid var(--grey-border)', borderRadius: '8px', overflow: 'hidden', marginBottom: '20px' }}>
        <div style={{ display: 'grid', gridTemplateColumns: '140px 1fr 140px 1fr', background: 'var(--red)', color: 'white' }}>
          <div style={{ padding: '12px 14px', fontWeight: 'bold', fontSize: '12px' }}>KATEGORIJA</div>
          <div style={{ padding: '12px 14px', fontWeight: 'bold', fontSize: '12px' }}>JAUTĀJUMS</div>
          <div style={{ padding: '12px 14px', fontWeight: 'bold', fontSize: '12px' }}>STATUSS</div>
          <div style={{ padding: '12px 14px', fontWeight: 'bold', fontSize: '12px' }}>MANAS PIEZĪMES</div>
        </div>
        {CHECKLIST.map((c, i) => (
          <div key={i} style={{
            display: 'grid',
            gridTemplateColumns: '140px 1fr 140px 1fr',
            borderBottom: i < CHECKLIST.length - 1 ? '1px solid var(--grey-border)' : 'none',
            background: i % 2 === 0 ? 'white' : '#FAFAFB',
          }}>
            <div style={{ padding: '12px 14px', fontWeight: 'bold', color: 'var(--red)', background: 'var(--red-light)', fontSize: '12px' }}>{c.kat}</div>
            <div style={{ padding: '12px 14px', fontSize: '13px', lineHeight: 1.5 }}>{c.jaut}</div>
            <div style={{ padding: '8px 10px' }}>
              <select
                value={statuss[i] || ""}
                onChange={e => setStatuss({ ...statuss, [i]: e.target.value })}
                style={{
                  width: '100%', padding: '6px',
                  background: statuss[i] === 'OK' ? 'var(--teal-light)' :
                              statuss[i] === 'Pārbaudīt' ? 'var(--yellow)' :
                              statuss[i] === 'Kļūda' ? 'var(--red-light)' :
                              statuss[i] === 'Neattiecas' ? 'var(--grey-light)' : 'white',
                  border: '1px solid var(--grey-border)', borderRadius: '4px', fontSize: '12px', fontWeight: 'bold',
                }}
              >
                <option value="">— izvēlies —</option>
                <option value="OK">OK</option>
                <option value="Pārbaudīt">Pārbaudīt</option>
                <option value="Kļūda">Kļūda</option>
                <option value="Neattiecas">Neattiecas</option>
              </select>
            </div>
            <div style={{ padding: '8px 10px' }}>
              <textarea
                value={piezimes[i] || ""}
                onChange={e => setPiezimes({ ...piezimes, [i]: e.target.value })}
                placeholder="Tavas piezīmes..."
                rows={2}
                style={{ width: '100%', padding: '6px', border: '1px solid var(--grey-border)', borderRadius: '4px', fontSize: '12px', resize: 'vertical', fontFamily: 'Arial, sans-serif' }}
              />
            </div>
          </div>
        ))}
      </div>

      <div style={{ background: 'var(--purple-light)', border: '2px solid var(--purple)', borderRadius: '8px', padding: '20px' }}>
        <h3 style={{ margin: '0 0 16px 0', color: 'var(--purple-dark)' }}>Gala lēmums</h3>
        <div style={{ display: 'grid', gridTemplateColumns: '1fr 200px', gap: '16px' }}>
          <div>
            <label style={{ display: 'block', fontWeight: 'bold', fontSize: '13px', marginBottom: '6px' }}>Vai MI atbilde ir gatava izmantošanai?</label>
            <select value={galaLemums} onChange={e => setGalaLemums(e.target.value)} style={{ width: '100%', padding: '10px', border: '2px solid var(--purple)', borderRadius: '6px', fontSize: '13px', background: 'var(--yellow)', fontWeight: 'bold' }}>
              <option value="">— izvēlies —</option>
              <option value="ja">Jā — lietoju kā ir</option>
              <option value="ja-redakc">Jā — ar redakcionāliem labojumiem</option>
              <option value="dalji">Daļēji — jāpārformulē fragmentus</option>
              <option value="ne-prompts">Nē — jāpārstrādā prompts un jāmēģina vēlreiz</option>
              <option value="ne-vispar">Nē — neder MI atbildei</option>
            </select>
          </div>
          <div>
            <label style={{ display: 'block', fontWeight: 'bold', fontSize: '13px', marginBottom: '6px' }}>Datums</label>
            <input type="date" value={datums} onChange={e => setDatums(e.target.value)} style={{ width: '100%', padding: '10px', border: '2px solid var(--purple)', borderRadius: '6px', fontSize: '13px', background: 'var(--yellow)' }} />
          </div>
        </div>
      </div>
    </div>
  );
}

function StatBadge({ label, value, bg, color, border }) {
  return (
    <div style={{
      background: bg, color: color,
      padding: '10px 16px', borderRadius: '8px',
      border: border ? '1px solid var(--grey-border)' : 'none',
      display: 'flex', alignItems: 'baseline', gap: '8px',
      minWidth: '100px',
    }}>
      <span style={{ fontSize: '20px', fontWeight: 'bold' }}>{value}</span>
      <span style={{ fontSize: '12px' }}>{label}</span>
    </div>
  );
}

function Kvalitate() {
  return (
    <div style={{ maxWidth: '1000px', margin: '0 auto', padding: '24px' }}>
      <div style={{ marginBottom: '24px' }}>
        <h2 style={{ color: 'var(--purple-dark)', margin: '0 0 8px 0' }}>Promptu kvalitāte</h2>
        <p style={{ margin: 0, color: 'var(--grey)', fontSize: '14px' }}>
          Ja MI atbilde nav apmierinoša — bieži problēma ir promptā, ne MI rīkā. Šeit 6 principi labākam promptam.
        </p>
      </div>

      <div style={{ background: 'white', border: '1px solid var(--grey-border)', borderRadius: '8px', overflow: 'hidden', marginBottom: '24px' }}>
        <div style={{ display: 'grid', gridTemplateColumns: '160px 1fr 1fr', background: 'var(--purple-dark)', color: 'white' }}>
          <div style={{ padding: '14px', fontWeight: 'bold', fontSize: '13px' }}>PRINCIPS</div>
          <div style={{ padding: '14px', fontWeight: 'bold', fontSize: '13px' }}>VĀJŠ PROMPTS</div>
          <div style={{ padding: '14px', fontWeight: 'bold', fontSize: '13px' }}>LABĀKAIS PROMPTS</div>
        </div>
        {QUALITY_PRINCIPLES.map((q, i) => (
          <div key={i} style={{
            display: 'grid', gridTemplateColumns: '160px 1fr 1fr',
            borderBottom: i < QUALITY_PRINCIPLES.length - 1 ? '1px solid var(--grey-border)' : 'none',
          }}>
            <div style={{ padding: '14px', fontWeight: 'bold', color: 'var(--purple-dark)', background: 'var(--purple-light)', fontSize: '13px', textAlign: 'center' }}>{q.p}</div>
            <div style={{ padding: '14px', background: 'var(--red-light)', fontStyle: 'italic', fontSize: '13px' }}>{q.v}</div>
            <div style={{ padding: '14px', background: 'var(--teal-light)', fontSize: '13px' }}>{q.l}</div>
          </div>
        ))}
      </div>

      <div style={{ background: 'var(--orange-light)', border: '1px solid var(--orange)', borderRadius: '8px', padding: '20px' }}>
        <h3 style={{ margin: '0 0 14px 0', color: '#A04500' }}>Iteratīvā pieeja</h3>
        <p style={{ margin: '0 0 12px 0', fontSize: '14px' }}>Reti pirmais prompts dod labāko atbildi. Strādā iteratīvi:</p>
        <ol style={{ margin: 0, paddingLeft: '24px', lineHeight: 1.8 }}>
          <li><strong>Sākuma prompts</strong> — pamata jautājums ar kontekstu</li>
          <li><strong>Precizēšana</strong> — "Pārformulē, lai..." vai "Padziļini punktu nr. 2"</li>
          <li><strong>Kritika</strong> — "Kādi ir vājākie punkti šajā atbildē?"</li>
          <li><strong>Alternatīva</strong> — "Piedāvā citu pieeju šim pašam jautājumam"</li>
          <li><strong>Sintēze</strong> — "Apvieno labākos elementus no abām atbildēm"</li>
        </ol>
        <p style={{ margin: '12px 0 0 0', fontSize: '13px', fontStyle: 'italic' }}>Pirmais prompts ir izejas punkts, ne gala produkts.</p>
      </div>
    </div>
  );
}

function App() {
  const [activeTab, setActiveTab] = useState('sakums');

  return (
    <div>
      <Header activeTab={activeTab} setActiveTab={setActiveTab} />
      <main style={{ paddingBottom: '60px' }}>
        {activeTab === 'sakums' && <Sakums setActiveTab={setActiveTab} />}
        {activeTab === 'sabloni' && <Sabloni />}
        {activeTab === 'darba_lapa' && <DarbaLapa />}
        {activeTab === 'izvertesana' && <Izvertesana />}
        {activeTab === 'kvalitate' && <Kvalitate />}
      </main>
      <footer style={{ background: 'white', borderTop: '1px solid var(--grey-border)', padding: '20px', textAlign: 'center', fontSize: '12px', color: 'var(--grey)' }}>
        MI promptu kolekcija · B grupa · Sagatavoja: Ilze Palmbaha · 2026
      </footer>
    </div>
  );
}

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<App />);
</script>
</body>
</html>

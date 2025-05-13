---
marp: true
html: true
footer: ![w:150 brightness](../img/OS2_logo_cmyk.svg)
theme: uncover
transition: reveal
headingDivider: 1
paginate: false
---

#
![bg brightness:0.7 sepia:0.3](https://)
 
> _If you imagine that your project is so different from other projects that you have nothing to learn from them, you will overlook risks that you would catch and mitigate if you instead switched to the outside view._

<!-- _footer: _Prof. Flyvbjerg, IT University of Copenhagen - How Big Things Get Done (2022)_ -->

# 
## Kan du lide at gå hjem kl. 16?
<!-- Hvorfor
_Hvorfor skal OS2 tilbyde fælleskomponenter til vores projekter og produkter?_
-->
#
## Genbrug det der virker!
## 🏅
###### _Som allerede er testet i hundrevis af produktions-instanser_
<!-- Ikke flere all nighters-->

#
## Få vedligehold foræret!
## 🎁
Fælles vedligehold - Som at få 1000 nye kolleger

#
## Fokuser på forretningen!
## 🎯
###### _Frigør ressourcer til at fokusere på forretningsbehov og levere værdi - istedet for at skulle genopfinde og vedligeholde infrastruktur kode_ 

#

#

##### Kvalitetssikring: Mange flere øjne og flere faglige vinkler på videreudvikling og vedligehold.
- Strategisk: Os2 skal bidrage til at sikre vore kritiske fælles infrastruktur, ved at skære ned på antallet og gøre de restende mere robuste og transparente.

### Fordele og ulemper ved fælles komponenter:
- Udviklere skal lære at kende PR processen at kende med alle dens konsekvenser. (Andre læser din kode, du skal kommunikere med andre udviklere)
- Integrationer og moduler skal leveres som generiske, konfigurerbare elementer, der kan anvendes andre steder end i en enkelt applikation. (initielt overhead, enorme gevinster senere)
- Man skal dokumentere sin kode, så det er nemt og forståeligt for andre at integrere og anvende
- Man skal hjælpe andre med at kunne få koden op og køre, så man skal tænke i udrulningskode (deployment manifester) og genanvendelig pakketering (containere)

### Hvad er kravene til en fælleskomponent
Den skal dokumenteres, udvikles og leveres så andre kan tage den i brug


### Hvordan rammesætter vi dette og hvad skal der til

- Os2 introducerer alle produkter og projekter til den gratis rådgivning og sparring de kan få fra sekretariatet på arkitektur og forandringsprocesser
- Vi følger internationale anbefalinger og standarder
- Os2 og leverandørerne investerer tid og penge i hackathons omkring 12-factor app metode
- Vi tager udgangspunkt i Graduated komponenter og projekter fra CNCF (der allerede er modne og kørende andre steder i verden, ingen dybe tallerkner her)
- Os2 faciliterer samarbejde og uddannelse omkring Cloud Native, der hele tiden er i bevægelse.
- Os2 investerer i "forandringsagenter" der kan være ambassadører og evangelister for forandringerne


### Hvordan udvikles og udbredes fælleskomponenter

- Vi vælger eksisterende komponenter, f.eks fra CNCF kataloget.
- Vi tilpasser komponenterne hvis nødvendigt og leverer tilpasningerne upstream til fælles vedligghold
- Produkterne investerer i at forbedre infratrukturkomponenterne ved kilden (upstream)
- Der integreres til de fælles komponenter fra national specifikke behov og hvis upstream projektet vil tage imod, leveres bidragene derop.

### Forvaltning og funding af fælleskomponenter

- Vil upstream projekterne ikke tage imod dem, afstættes der midler til at oprette en organisation til vedligeholde af disse integrationer(ligesom et projekt, det kan gøres med øgede bidrag, crowdfunding eller andre finansieringmetoder)
- Før min tid er der oprettet et lidt blegt underfinansieret forsøg på dette kaldet "os2services" der har sin egen organisation, men INGEN økonomi og INGEN maintainere.

### Hvordan arbejder vi videre herfra
- Identificer leverandører, dygtige maintainere og uddan evangelister/ambassadrører
- Afhold og faciliter Hackathons med helt klare mål for hver sceance. (altså kode der ender i et os2ejet org./repo) Kæl for nørderne og deres behov...
- Find modeller til at hæve niveauet blandt ALLE stakeholders. Koordgrupper, sekretariat, ildsjæle. Lav et uddannelses katalog der henviser... tilbyd os2/oss uddannelser, i samarbejde med uddannelses organisationer? 
- Tag ud på steder som f.eks VIA og hverv unge mennesker og fortæl dem om os2 og fælleskomponenterne.

Evt eller spørgsmål

#
## Samarbejde og læring


#### Samtale
Muliggører effektivt samarbejde imellem myndigheder gennem fokuserede diskussioner.
#### Video
Alternativ til videomøde delen af Microsoft Teams - baseret på upstream Jitsi


#### Dokument
Opbevaring og styring - Baseret på upstream NextCloud

#### os2learn
Open Source LMS portal baseret på f.eks upstream Moodle

#
## Arbejdsgange og Databehandling

#### Connector
Fælles integrationskomponent baseret på upstream Dapr framework

#### Flow 
Orkestrering af automatiserede arbejdgange & løskoblede workloads baseret på upstream Dapr

#
## Sikkerhed og compliance

#### OS2Monitor 
Baseret på upstream f.eks OpenTelemetry og Grafana eller custom frontends

#### Os2Sign
Løskoblet dokument signerings løsning baseret på upstream OpenSign og OS2ID MitID integration.

#### os2ID
Moderne løskoblet identitets styring baseret på upstream open source. Baseret på upstream Authentik


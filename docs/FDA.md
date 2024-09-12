---
marp: true
footer: ![w:200 invert](../img/OS2_logo_cmyk.svg)
theme: uncover
transition: reveal

headingDivider: 1
paginate: false
---
#
![bg left:33% h:650](https://images.unsplash.com/photo-1627008767693-20498ff18ab7?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

### [JAN MAACK KJERBYE]()
*Enterprise Architect*

> Jeg brænder for en mere fair og robust offentlig sektor


<!--
Bred erfaring med værdiskabelse fra både private og offentlige orgs.

Jeg brænder for en mere fair og robust offentlig sektor

-->





# Hvorfor er genbrug så svært?
*Lad os kigge på forudsætningerne*
<!-- class: invert -->

#

###### 🔍 Man skal kunne finde og få adgang til softwaren

###### 🔌 Det er overkommeligt at få en test instans kørende

###### 🎯 Løsningen skal matche de aktuelle forretningsbehov

###### ⚙️ Løsningen kan køres i produktion i myndighedens foretrukne it-miljø


#### Ingen fælles definition af "Genbrug"

Der er ingen enighed om, hvad begrebet "genbrug af software"" præcist indbefatter

#### Manglende akkumuleret viden om OSS

Forsøg med genbrug identificeres ikke nødvendigvis med Open Source, da der er meget lidt akkumuleret viden om OSS i danske myndigheder.

#### Fragmenteret viden om initiativer

Der er meget begrænset opsamlet statistik eller succeshistorier om initiativer i den danske offentlige sektor. Mange kilder peger på op til 10 år gamle kilder.

[Interactive Resource Map | Joinup](https://joinup.ec.europa.eu/collection/open-source-observatory-osor/interactive-resource-map)

# Mine erfaringer med forsøg på genbrug

Baseret på min erfaring falder forsøg med forskellige fortolkninger af genbrug, lidt groft sagt, indenfor fire kategorier. 

### :handshake: Den indidviduelle og manuelle

   Ildsjæle i de mellemste organisatoriske lag af myndighederne,  benytter netværksmøder, personlige kontakter, email anmodninger, og uensartede fremgangsmådet til at fremskaffe programmer og dokumentation på software der håbes genbrugt. Det indebærer mange personafhængige flaskehalse og processen kan være meget langsom og uforudsigelig. I nogle tilfælde dukker disse ildsjæle op igen i anden kontekst involveret i Open Source projekter.

   Risiko: *Bestilleren kan ikke vente og mister tålmodigheden, projektet falder til jorden or et med til at underbygge generelle misforståelser og myter om genbrug af software*.

### :money_with_wings: Den vedligeholdelsestunge

   Der investeres mange timer og penge i at etablere officielle offentlige portaler, med custom søgemaskiner og applikationsdatabaser baseret på indmeldinger og manuel opmærkning. Det viser sig at været så tungt i både teknisk og administrativt vedligehold at det bliver voldsomt dyrt at vedligeholde og meget svært at finde financiering til.

  Risiko:  *Den økonomiansvarlige tvivler på værdiskabelsen, holdt op imod investeringerne og stopper funding.* 

### 🙈 Den udliciterende

    Alle myndigheder placerer deres æg i samme kurv og køber væg-til-væg løsninger f.esk ved en af de store amerikanske tech giganter. Der skal opmandes på juridiske kompetencer til leverandør og licensstyring og myndighederne må tilpasse sig til løsningerne. Selvom man teknisk set "gen"bruger de samme løsninger, må man acceptere et tab af ejerskab og indflydelse.

    Risiko: *Leverandøren kan ved hjælpe af de-facto leverandør lock-in prissætte sine ydelser udelukkende efter deres kommercielle forretningsmodeller og regninger til licenser eskalerer ud af kontrol*

### :people_holding_hands: Det samarbejdskrævende alternativ

    Der genbruges eksisterende åbne delingsportaler til Open Source og investeres i åbne vidensfællskaber, der aktiverer det private SMV lag og arbejder inkrementelt med tilpasninger af eksisterende løsninger.

    Risiko: *Vanetænkning og frygt forhindrer at den nødvendige tillid til OSS kan nåes, og projekterne strander dybt nede i it-adfelingerne*

## 

# Så hvad så?

## Den stoiske tilgang:

I OS2 arbejder vi med det vi har mulighed for at ændre på 

- Udfordre vanetænkningen ved at vise vejen med gode eksempler.

- Uddannelse og rådgivning til når projekterne rammer barrierer

- Formidling og dialog med SMV leverandører så myndighederne kan fokusere på kerneopgaven.

- Bidrag til infrastrukturkomponenter og skabeloner, så barrierer sænkes og det bliver nemmere og hurtigere at komme i gang.

# Lavpraktiske eksempler fra OS2

- Automatiserede processer der bygger og deler genbrugelige komponenter
  
  - Containerbuilds, GitHub hosting, projekt og dokumentations skabeloner

- Evaluering af og bidrag til robuste, genbrugelige infrastruktur komponenter.
  
  - Bidrag til upstream IDP med SAML krypterings funktioner der sikrer interoperabilitet med den danske digitale infratruktur. Implementering og anvendelse internt som "Customer-0" og udbredelse til andre OS2 produkter

- Bidrag til ensartet, søgbare tekniske dokumentationsportaler via "docs-as code" principper og automatisering

# Takeaways

1. Stil krav om at løsninger består af kode der udvikles åbent og versionsstyres i git og at alle kode-bidrag gøres offentligt tilgængeligt via GitHub, GitLab eller lign.

2. Invester i et Open Source program-kontor der kan hjælpe med at styre processer og portefølje. OS2 har tilbudt disse ydelser siden 2012 og byder alle offentlige myndigeheder velkommen.

3. Gør op med vanetænkningen der gør at Open Source evalueres kortsigtet alene på indkøbspris. 

4. Invester i åbne, robuste løsninger og øremærk mindst 15% af vedligeholdelses budgetterne til konsolidering af "usynlige" infrastrukturkomponenter. 

![bg blur:1px brightness:0.7](https://images.unsplash.com/photo-1515856251934-766e064d7b09?q=80&w=1335&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
<!-- Hvordan adskiller vi os fra et "almindeligt" software produkt -->

### OS2 er en missionsdreven organisation
##
Mindre glamour - stærkere leverancer
<!-- Vi inkluderer alt det som er svært at sælge up front.
Mindre glamour, mere leverance
Ingen investorer, intet krav om kommercielt afkast-->
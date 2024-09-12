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
<sub>jan@os2.eu</sub>

> Jeg brænder for en mere **åben** og **robust** offentlig sektor


<!--
Bred erfaring med værdiskabelse fra både private og offentlige orgs.

Jeg brænder for en mere åben og robust offentlig sektor

-->



#
<!-- class: invert -->
<!-- _footer: "jan@os2.eu" -->


<style scoped>
  img {
  width:300px;
  border-radius: 50%;
    }
</style>
![bg brightness:0.2 sepia:0.6](https://s.studiobinder.com/wp-content/uploads/2019/08/What-is-Deep-Depth-of-Field-Deep-Focus-Shot-in-Photography-Feature-StudioBinder.jpg)

![44% opacity:80% sepia:0.1](../docs/image/EARoles/jmk_colour.jpg )
Enterprise Architect OS²

> Jeg brænder for en mere **åben** og **robust** offentlig sektor


#

![bg blur:1px brightness:0.7](https://images.unsplash.com/photo-1515856251934-766e064d7b09?q=80&w=1335&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

> _The architecture function is often seen as inseparable from essential governance and compliance requirements. However, reducing the role of architecture to a compliance function or separating it from day-to-day operations confines its value to a policing entity or an abstract function in an ivory tower."_
> 
> ###### [:arrow_right: McKinsey Digital Insights](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/tech-forward/quantum-technology-use-cases-as-fuel-for-value-in-finance)


# **Hvorfor er genbrug så svært?**

# Historik

Ildsjæle, webportaler & udlicitation
<!--


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

-->
#
> *"Many organizations invest lots of time and effort in adopting technologies, but fail to achieve critical software delivery outcomes, due to limitations imposed by architecture."*

###### [➡️ DevOps Research & Assesment program](https://dora.dev/)
![bg opacity:0.6](https://images.unsplash.com/photo-1539598978120-7d2f5251837c?q=80&w=1287&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

#

<p style="font-size: 84px; color: white; position: relative; display: inline-block;">
  0 - Fejls kultur
  <span style="position: absolute; left: 200px; right: 200px; top: 52%; height: 12px; background-color: #8B0000;"></span>
</p>

#

Hvis du afventer indtil alting er perfekt og feature complete.. så misser du bussen

Expect errors, failures, breakdowns.. but we do them in test, not on prod

# 

## **I OS2 arbejder vi**
 med det
   
vi har mulighed for at ændre på 
<!--

###### - Udfordre vanetænkningen ved at vise vejen med gode eksempler.

###### - Uddannelse og rådgivning til når projekterne rammer barrierer

###### - Formidling og dialog med SMV leverandører så myndighederne kan fokusere på kerneopgaven.

###### - Bidrag til infrastrukturkomponenter og skabeloner, så barrierer sænkes og det bliver nemmere og hurtigere at komme i gang.
-->

#
## Open Source
🔽
<div style="display: flex;">
<div style="flex: 1; padding: 10px;">

### **Transparency**
by
default
</div>

<div style="flex: 1; padding: 10px;">
 
### **ReUse**
by
default

</div>

</div>
<!-- Genbrug og transparens er indbyggede factorer-->

# **OS2 Indsatser 2024**


Standarder & CI som løftestang for Genbrug

Modernisering via upstream infrastruktur bidrag

Transparens via docs-as-code

<!--

- Containerbuilds, GitHub hosting, projekt og dokumentations skabeloner
- Bidrag til upstream IDP med SAML krypterings funktioner der sikrer interoperabilitet med den danske digitale infratruktur. Implementering og anvendelse internt som "Customer-0" og udbredelse til andre OS2 produkter
- Bidrag til ensartet, søgbare tekniske dokumentationsportaler via "docs-as code" principper og automatisering

-->

# **TAKE AWAYs**

# **INSISTER**
 <sub> på at løsninger **skal** bestå af kode der udvikles åbent og versionsstyres i git og at alle kode-bidrag gøres offentligt tilgængeligt via GitHub, GitLab eller lign. 
 </sub>

# **INVESTER**
<sub> i et Open Source program-kontor der kan hjælpe med at styre processer og portefølje efter moderne åbne principper.
</sub>

# **BUDGETTER**
<sub> med konsolidering og vedligehold af "usynlige" infrastrukturkomponenter. </sub>

# **GØR OP**
<sub> med vanetænkningen der gør at Open Source evalueres kortsigtet alene på indkøbspris. Kig på de langsigtede omkostninger</sub> 
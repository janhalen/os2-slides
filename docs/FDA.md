---
marp: true
html: true
footer: ![w:200 invert brightness:10 opacity:0.4](../img/OS2_logo_cmyk.svg)
theme: uncover
transition: swipe
headingDivider: 1
paginate: false

---
#
![bg left:40% h:650 opacity:0.85](https://images.pexels.com/photos/6168066/pexels-photo-6168066.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

<style scoped>
  img {
  width:200px;
  border-radius: 50%;
    }
</style>
![opacity:92% sepia:0.1](../docs/image/EARoles/jmk_colour.jpg )
### [JAN MAACK KJERBYE]()
*Enterprise Architect OS²*
<!-- _footer: "jan@os2.eu" -->



<!--
Bred erfaring med værdiskabelse fra både private og offentlige orgs.

Jeg brænder for en mere åben og robust offentlig sektor

-->



#
<!-- class: invert -->

![bg blur:1px opacity:0.8 brightness:0.8](https://images.unsplash.com/photo-1515856251934-766e064d7b09?q=80&w=1335&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

> _The architecture function is often seen as inseparable from essential governance and compliance requirements. However, reducing the role of architecture to a compliance function or separating it from day-to-day operations confines its value to a policing entity or an abstract function in an ivory tower."_
> 
> ###### [:arrow_right: McKinsey Digital Insights](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/tech-forward/quantum-technology-use-cases-as-fuel-for-value-in-finance)


#
## **GENBRUG**
## 🔃
individuel aktivitet *eller* fælles strategi

![bg brightness:0.4 blur:2px](https://images.pexels.com/photos/716661/pexels-photo-716661.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

<!--
Der mangler en forankring - Er der noget man gør eller er det en strategisk ramme?

Der mangler en fælles forståelse af, 
hvad begrebet **genbrug** præcist indbefatter eller hvilken værdi man forventer

Properitært? En Kopi? Indkøb af samme teknologi?

Hvis folks selv må definere det kommer vi ingen vegne.

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
## **Forudsætninger**
for GENBRUG
## 🔃
###### Anbefalet af andre, nemt at tilgå, gennemskueligt, ukompliceret at dele

![bg brightness:0.5 opacity:0.6 sepia:0.2 blur:1px](./image/FDA/photocopy-1588176329173.webp)


# **OPEN SOURCE**
leverer rammerne
![bg blur:2px brightness:0.7 opacity:0.7](https://images.unsplash.com/photo-1634745646763-1f1183bb91c1?q=80&w=2080&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
###
###### **Transparency** | **Availability** | **Uniformity**

##### ReUse

<!-- Genbrug og transparens er indbyggede faktorer-->

# **METODER**

![bg blur:1px brightness:0.5 opacity:80%](https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?q=80&w=2072&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

###### :cloud: **Design** - 15 factor app &ensp;**|**&ensp; 📦 **Packaging** - OCI containers
###### :arrows_counterclockwise: **Documentation** - Docs-as-Code &ensp;**|**&ensp; ⚙️ **Deployment** - GitOps
###### :arrow_double_up: **Maintenance** - Upstream first

<!--

- Containerbuilds, GitHub hosting, projekt og dokumentations skabeloner
- Bidrag til upstream IDP med SAML krypterings funktioner der sikrer interoperabilitet med den danske digitale infratruktur. Implementering og anvendelse internt som "Customer-0" og udbredelse til andre OS2 produkter
- Bidrag til ensartet, søgbare tekniske dokumentationsportaler via "docs-as code" principper og automatisering

-->
#
## **BIDRAG**
```python
    
     def get_encryption_key_descriptor(self) -> Optional[Element]:  
        """Get Encryption KeyDescriptor, if enabled for the source"""
        if self.source.encryption_kp:
            key_descriptor = Element(f"{{{NS_SAML_METADATA}}}KeyDescriptor")
            key_descriptor.attrib["use"] = "encryption"
            key_info = SubElement(key_descriptor, f"{{{NS_SIGNATURE}}}KeyInfo")
            x509_data = SubElement(key_info, f"{{{NS_SIGNATURE}}}X509Data")
            x509_certificate = SubElement(x509_data, f"{{{NS_SIGNATURE}}}X509Certificate")
            x509_certificate.text = strip_pem_header(
                self.source.encryption_kp.certificate_data.replace("\r", "")
            ).replace("\n", "")
            return key_descriptor
        return None


    def _decrypt_response(self):
        """Decrypt SAMLResponse EncryptedAssertion Element"""
        manager = xmlsec.KeysManager()
        key = xmlsec.Key.from_memory(
            self._source.encryption_kp.key_data,
            xmlsec.constants.KeyDataFormatPem,
        )



```
<!-- _footer : "[contributor](https://github.com/nicolas-semaphor?tab=overview&from=2023-04-01&to=2023-04-30) - [issue](https://github.com/goauthentik/authentik/issues/7999) - [contribution](https://github.com/goauthentik/authentik/pull/10099) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![w:150 invert brightness:10 opacity:0.4](../img/OS2_logo_cmyk.svg) " -->

<!--
En helt github grøn udvikler
Et spørgsmål til et eksisterende projekt
Et bidrag til et fælles vedligeholdt projekt
-->

#
### &nbsp;&nbsp;**IDENTIFICER** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **INVESTER** &nbsp; &nbsp;&nbsp;&nbsp;
&nbsp;Generelle fælles behov&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Distribueret vedligehold &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Eksisterende teknologi &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Standardisering&nbsp;&nbsp;&nbsp;
### **INSISTER**
Open Source
Transparens
Neutralt ejerskab
![bg brightness:0.7 sepia:0.3 blur:1.5px opacity:90%](https://images.pexels.com/photos/157879/gift-jeans-fashion-pack-157879.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

<!-- _footer: "" -->
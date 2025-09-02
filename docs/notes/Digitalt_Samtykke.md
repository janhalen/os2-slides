Noter https://api-pp-digitaltsamtykke.ssl.digst.dk/swagger/index.html

Digitalt Samtykke API - Digitaliseringsstyrelsen
 v1 
OAS 3.0
/swagger/v1/swagger.json
API understøttelse for ekstern integration til Digitalt Samtykke under Digitaliseringsstyrelsen.
# Adgang til API via Fælleskommunal Adgangsstyring
> Brug følgende tilgang for at få adgang til API'et:

## Step 0. Forarbejde:

Registrer et IT-system som anvendersystem med et OCES certifikat med offentlig nøgle i Fælleskommunal Administration:
PreProd: https://saml.admin-test.serviceplatformen.dk/
Produktion: https://saml.admin.serviceplatformen.dk/
Vælg "Serviceaftaler" og klik "Anmod om serviceaftale"
Vælg:
Vælg: "Uden videregivelse af data", skriv et navn og en begrundelse
Vælg det IT-system (Anvender system), der skal forbindes
Vælg ansvarlig myndighed. Her skal vælges den myndighed som man ønsker at agere på vegne af, bemærk venligst at myndigheden skal godkende serviceaftalen før man kan få angang til servicen.
Vælg "Digitalt Samtykke API".
Tilføj rolle: "Digitalt Samtykke API Adgang"
Accepter vilkår og betingelser
Send anmodning

## Step 1. Fremskaf adgangsbillet:

Udform en POST til:
Eksterntest: https://n2adgangsstyring.eksterntest-stoettesystemerne.dk/runtime/api/rest/oauth/v1/issue
Produktion: https://n2adgangsstyring.stoettesystemerne.dk/runtime/api/rest/oauth/v1/issue
Request (POST) skal indeholde:

Certifikatet som ovenfor uden privat nøgle - koblet på http-kaldet som Client Certificate
En form bestående af:
client_id = {entityId}
grant_type = client_credentials
scope = entity_id:{entityId},anvenderkontekst:{cvrnummer}
Dette vil returnere en token.

## Step 2. Konvertér til token, der kan anvendes af Digitalt Samtykke API

Kald af det eksterne API's Authorize endpoint (/v1/api/authorize/jwt) med brug af samme certifikat som Client Certificate sammen med den genererede access token som Bearer token. Her returneres en ny access token til brug mod API'et.
Step 3. Kald Digitalt Samtykke API

Kald af API'ets endpoints (f.eks. /v1/api/myndighed/xxx/samtykker) med brug af samme certifikat som Client Certificate sammen med den genererede access token som Bearer token. XXX står her for cvr-nummer for myndigheden.


# Adgang til API via NemLog-In
Brug følgende tilgang for at få adgang til API'et:

## Step 0. Forarbejde:

Opret en system user (systembruger) i nemlog-in administration med et OCES certifikat med offentlig nøgle.
Send systembrugerens entityId (https://wsc.xxx) til serviceudbyderen (Digst)
## Step 1. Fremskaf adgangsbillet:

Udform en POST til:
Preproduktion: https://SecureTokenService.test-nemlog-in.dk/SecurityTokenService.svc
Produktion: https://SecureTokenService.nemlog-in.dk/SecurityTokenService.svc

Certifikatet som ovenfor uden privat nøgle - koblet på http-kaldet som Client Certificate
Et WS-trust kald (se Digitaliseringsstyrelsens dokumentation med tilhørende referenceimplementationer på OIO Identity Based Web Services 1.2)
Dette vil returnere en token.

## Step 2. Konvertér til token, der kan anvendes af Digitalt Samtykke API

Kald af det eksterne API's Authorize endpoint (/v1/api/authorize/saml) med brug af samme certifikat som Client Certificate sammen med den genererede access token som Bearer token. Her returneres en ny access token til brug mod API'et.

## Step 3. Kald Digitalt Samtykke API

Kald af API'ets endpoints (f.eks. /v1/api/myndighed/[cvrnummer]/samtykker) med brug af samme certifikat som Client Certificate sammen med den genererede access token som Bearer token.
Skemaer til XML validering
Følgende XML-skemaer bliver brugt til validering af modtaget og afsendt XML:

XSD til validering af skabeloner
XSD til validering af samtykkeerklæringer
XSD til validering af samtykkegrupper
XSD til validering af samtykker
XSD til validering af samtykke satatyper
XSD til validering af HTML tags
Dokumentationen af de udstillede endpoints fremgår listen af nedenfor
Digitaliseringsstyrelsen - Website
Send email to Digitaliseringsstyrelsen

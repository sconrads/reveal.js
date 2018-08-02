### Felles standardisering

* Økosystem
* Utviklingsmiljø
* BOB
* Kontainere
* AppShell



notes:
###### Anders:



###### Opprinnelige notater:
* Hva gjorde vi riktig sist?
  * Templating - først og fremst gjenkjennelseseffekt og struktur på hvor ting ligger
    * Feil teknologi men riktig løsning
    * Utløsende for at verktøystøtten vår som Bob fungerer godt i teamene
    * Gitt oss mulighet til å rulle ut endringer på tvers av alle applikasjonene enkelt
  * Build.sh - scripting og løs kobling fra byggserver og byggverktøy
  * Registrerer at SpringBoot har gjort mye av det samme som vi gjorde med Bill-of-Materials for avhengighetshåndtering
    * Ser fordeler her ved at vi ikke trenger å vedlikeholde dette i like stor grad selv, versjonshåndtering av avhengigheter er krevende
  * Vi har en basis som vi kan bygge ut etterhvert som behovene endrer seg
  * Beholdt muligheten for at teamene kan eksperimentere
  * Vi har klart å rulle på mange nye utviklere uten at dette har bremset produktiviteten til eksisterende utviklere
  * Fått et felles stammespråk fordi vi har standardisert, har arkitekturmøter hvor de litt mer omfattende eksperimentene og endringene diskuteres ukentlig, og fokuserer på pull requester med representanter fra andre team
* Hva kan vi gjøre bedre nå?
  * Modning av tredjepartsløsninger gjør at vi kan dra nytte av disse, mye som vi tidligere laget selv er i dag standardløsninger i en hver applikasjon (SpringBoot, Hystrix, templating, SSL, sikkerhet, tofaktor)
  * Fordeler ifht. tilgjengelighet på kompetanse
  * Kontainerteknologien gjør at det er naturlig å droppe flere av de gamle teknologiene som RPM og Apache
  * Vi tror at å levere en kontaineruavhengig applikasjon er riktig for oss
    * Fordi kjøretidsplattformen kan endre seg, det skjer mye på dette området om dagen
    * Vi trenger forutsigbarhet når vi lager verktøystøtten internt
    * Vi liker å stå fritt
  * Bruke nødvendig tid på å strukturere felleskoden godt, det kan vi ta oss tid til å prioritere nå
  * Unngå rendring av frontend fra serverside i størst mulig grad

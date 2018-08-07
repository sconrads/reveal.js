### Felles standardisering

* Økosystem
* Utviklingsmiljø
* BOB
* Kontainere
* AppShell



notes:
###### Anders:

En av de tingene vi føler har fungert for oss er å **standardisere**, spesielt struktur på applikasjonene men også 
utviklingsmiljøet. Det gir oss en **gjenkjennelseseffekt** som vi tror har vært viktig, og ikke minst så har det gjort at 
automatiseringen vi har gjort i ettertid har vært enklere. Når det er sagt så står teamene ganske fritt til å 
eksperimentere, og det blir gjort.

Vi har helt siden starten hatt en **templatingmekanisme** for å lage og oppdatere applikasjonene våre, og vi har tilsvarende for selve **utviklingsmiljøet**.
I tillegg nevnte vi vår venn **Bob** i 2015, og han lever i beste velgående i dag også. 

Disse tingene ligger som **git-prosjekt** og vi har vært heldige å fått et miljø hvor mange av **utviklerne aktivt foreslår endringer** som er testet av enkeltpersoner eller team.
Det er ingen team eller personer som eier disse fellesløsningene, men de er fordelt ut slik at noen har et **overordnet ansvar** for 
at de fungerer og at det finnes en viss basiskompetanse på løsningen.

Ofte diskuteres større forslag til forbedringer eller erfaringer som er gjort i **"Arkitektmøtet for ikke-arkitekter"**, som 
er et åpent forum hvor man kan møtes en gang i uka. 

Vi tror at noen av suksessen her har vært at vi jobber i **inkrementelle steg, konsensusbasert og utviklerdrevet**. Vi har i 
noen år nå hatt et uttalt mål om **24 timer fra ide til produksjon, og 30 minutter fra ferdig kode til produksjon**, og 
at vi har det så tydelig har nok gjort det lettere å **stake ut retningen for bidrag, og få aksept for de større 
endringsbehovene** også hos andre deler av organisasjonen.

Dagens løsning var jo **rigget for å fase ut monolitten** vår, og det medførte jo et visst fokus. Vi er nå godt i gang med 
å prøve å løfte blikket litt og se fremover. Det vi ser er jo at verden rundt oss har tatt oss igjen på mange områder, 
og at for eksempel SpringBoot dekker veldig mye av det vi har forsøkt å løse selv. Det har vært en solid modning av 
åpen kildekode tredjepartsløsninger som vi nå kan dra nytte av i stedet for å bruke utviklingsressurser på å lage mye selv.

I utvikling har vi kjørt diverse varianter av **containere** i mange år, og det siste året har dette endelig begynt å boble 
opp til **testmiljøene** også. Vi har nå endelig de første containerne i produksjon, og forventer at vi får en rask økning 
der det neste året. Kontainerne gjør oss mer frikoblet fra kjøretidsplattform, og ikke minst er det **gunstig når vi 
lager verktøystøtte**.

Det vi ser vi bør legge ned mer tid på fremover er på strukturering av den felleskoden som vi skal beholde i gode bibliotek, 
og api-først tankegangen.


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

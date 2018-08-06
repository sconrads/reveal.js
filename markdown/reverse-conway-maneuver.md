### Reverse Conway maneuver

* Presentasjon til Kristoffer og Jostein
* Tvergående team som Mobilbank og Optimus
* Fellesarena
  * Arkitektmøtet
  * Workshops


notes:
###### Stian:

Som tidligere nevnt, var en veldig viktig driver i 2015, å kunne skalere horisontalt. Med det mener jeg at vi kan etablere flere team rundt mindre applikasjoner. Noe som igjen gjør at vi kan få inn flere utviklere. 
Vi snakket i 2015 om reverse conway manuever. Conways lov sier at applikasjonene man lager vil gjenspeile hvordan man er organisert. Ved at vi splitter monoliltten så vil vi kunne legge til rette for en organisasjonsendring. Man vil ikke få mye utbytte av de nye applikasjonene om man ikke organiserer seg anderledes. Sånn sett vil man presse frem en reorganiserer og man vil legge grunnlaget for å kunne bygge team rundt applikasjonene. 

Dette har skjedd hos oss, og vi har i dag 15 team. Og disse teamene er alle på et eller annet sted på reisen mot autonomi. 

Vi er i dag organisert i domeneteam. Vi har f.eks et team som jobber med betaling og et annet som jobber med finansiering. Hvert team har sin forretningseier og prioriterer selv hvilken funksjonalitet som skal utvikles. Etterhvert har også flere av teamene startet å jobbe hypotesedrevet. Ledelsen gir teamene mål, så finner teamene selv ut hvordan de kan svare på disse målene. Vi vet ikke nødvendigvis hvilken funksjonalitet vi skal lage, men vi har noen hypoteser. Disse tester vi ut, og utfra det vi lærer i disse testene, former vi den nye funksjonaliteten. 

Selv om vi etterhvert har ganske så autonome team og vi ønsker å utnytte Conways lov slik at vi ikke får tette koblinger mellom applikasjonen, har vi noen fellesarenaer:
* Arkitektmøtet for ikke arkitekter
* Workshop-basert arkitektur

Vi har også noen team som ikke er koblet til et fagdomene. Dette er det vi kaller horisontale team. 
De fleste kundene våre bruker helst mobilbanken. De forventer å kunne gjøre det alt også på mobil. Da blir det tullete å lage funksjonalitet som kun virker på stor flate på en PC. Vi så samtidig at vi ikke kunne ha ett team som skulle implementere all ny funksjonalitet på mobil. Den jobben måtte distribueres ut i teamene. 
Det er jo egentlig opplagt, men det er likefullt veldig skummelt når man sitter med en av verdens beste mobilbanker. Ja, det er ikke bare skryt, dere kan sjekke App Store :)
Vi valgte derfor å etablere et nytt team som fikk i oppgave å gjøre de andre teamene supre på mobilbankutvikling. Det har fungert over all forventing. Mobilbanken har faktisk blitt ratet enda bedre på App Store nå. Og vi kan nå utvikle alt med fokus på mobil først. 

På samme måte har vi også etablert et team som har som visjon å gjøre de andre teamene gode. Dette er et devops team som lager løsninger som alle andre team vil ha nytte av. Hovedfokus nå er en ny Kubernetes plattform. En veldig viktig sak for dette teamet er at man roterer inn utviklere. Dette er viktig for å sikre at dette teamet alltid er tett på virkeligheten og lager det utviklerne trenger.  

Det tredje horisontale teamet vi har er API teamet. På samme måte som for de andre horisontale teamene skal dette teamet gjøre de andre gode. Vi jobber nå med at alle teamene skal utvikle med en API først tankegang. Vi tror at vi ved å lage APIene først, og så bruke de på våre klienter først, får de beste APIene. 


Sett i forhold til hvordan vi jobbet frem arkitekturen i 2015, så har vi lært at det er ekstremt viktig å involvere alle underveis. Vi var alt for introverte i 2012. Det at vi nå har en workshopdrevet arkitektur tror vi gjør løsningene bedre og vi sikrer at vi jobber i samme retning, og ikke minst er enige om retningen. 

### Modning


notes:
###### Stian:
Dagens løsning var jo **rigget for å fase ut monolitten** vår, og det medførte jo et visst fokus. Vi er nå godt i gang med å prøve å **løfte blikket** litt og se fremover. Det vi ser er jo at **verden rundt oss** har tatt oss igjen på mange områder, og at for eksempel SpringBoot dekker veldig mye av det vi har forsøkt å løse selv. Det har vært en **solid modning** av åpen kildekode tredjepartsløsninger som vi nå kan dra nytte av i stedet for å bruke utviklingsressurser på å lage mye selv.

###### Anders:
I utvikling har vi kjørt diverse varianter av **containere** i mange år, og det siste året har dette endelig begynt å boble opp til **testmiljøene** også. Vi har nå endelig de første containerne i produksjon, og forventer at vi får en rask økning der det neste året. Kontainerne gjør oss mer frikoblet fra kjøretidsplattform, og ikke minst er det **gunstig når vi lager verktøystøtte**.

Det vi ser vi bør legge ned mer tid på fremover er på strukturering av den felleskoden som vi skal beholde i gode bibliotek, og api-først tankegangen.


###### Opprinnelige notater:
* Hva kan vi gjøre bedre nå?
  * Modning av tredjepartsløsninger gjør at vi kan dra nytte av disse, mye som vi tidligere laget selv er i dag standardløsninger i en hver applikasjon (SpringBoot, Hystrix, templating, SSL, sikkerhet, tofaktor)
  * Fordeler ifht. tilgjengelighet på kompetanse
  * Kontainerteknologien gjør at det er naturlig å droppe flere av de gamle teknologiene som RPM og Apache
  * Vi tror at å levere en kontaineruavhengig applikasjon er riktig for oss
    * Fordi kjøretidsplattformen kan endre seg, det skjer mye på dette området om dagen
    * Vi trenger forutsigbarhet når vi lager verktøystøtten internt
    * Vi liker å stå fritt
  * Bruke nødvendig tid på å strukturere felleskoden godt, det kan vi ta oss tid til å prioritere nå

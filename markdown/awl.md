### Ny generasjon applikasjoner

#### Erfaring:
- Dagens applikasjoner er mikro-monolitter

#### Tiltak:
- Lag skyklare applikasjoner som kun støtter ønskede teknologier


notes:
###### Stian:
Da vi etablerte applikasjonsarkitekturen som overtok for monolitten, så valgte vi å støtte **alle teknologiene** monolitten også støttet. Også de teknologier vi ikke ønsket. 
Grunnen til det var at det skulle være **enkelt å migrere** eksisterende funksjonalitet. Det skulle ikke være nødvendig å skrive om alt. 
Best beskrivende navn for denne applikasjonsarkitekturen er nok **mikro-monolitt**. 

###### Anders:
Når vi nå lager en **ny applikasjonsarkitektur** kutter vi båndet til alle **teknologier vi ikke ønsker** å ta med oss videre. 
For å slippe å lage og vedlikeholde en masse rammeverkskode, så har vi, som de fleste andre, valgt å basere oss på **Spring Boot**. Så kan man diskutere til man blir blå i ansiktet om det er lurt, men for oss ser det ut til å gjøre susen. Vi slipper å finne opp hjulet på nytt og **utviklerne hos oss kjenner Boot**. 

###### Stian:
Vi jobbet frem denne arkitekturen gjennom en del **innledende workshops**. Videre drar vi ut noen applikasjoner i produksjon for å **validere arkitekturen**. På sikt lager vi nok en **templating** mekanisme for å spy ut flere applikasjoner. 

For å sikre at applikasjonene våre er klare for skyen, så har vi sett på **12 factor apps** sine krav. Applikasjonene er **tilstandsløse**, logging skjer til **standard out** og **konfigurasjonen** er en del av **kildekoden**.

###### Anders:
Da vi laget **mikro-monolitt** arkitekturen var dette et stort stykke arbeid med mange involverte. Også kalt **prosjekt**. Denne gang er det Anders og meg som koder frem en applikasjon på ny arkitektur som en del av **vanlig forvaltning**. 
Det er **ikke så mye vi lager** selv denne gang. Mye av jobben er å trekke ut det som er  av felleskode i **biblioteker**, samtidig som vi har høyt **fokus på avhengigheter** mellom disse. 
Personlig tror jeg dette er siste gang vi lager en felles applikasjonsarkitektur. Neste gang kan det være godt nok å si at appen skal følge kravene i 12 factor app. 


###### Opprinnelige notater:

* workshops ønsker
* boot
* templatebasert til api
* industristandarder

* Jobbet frem en ny arkitektur
  * Workshops
  * Arkitekturmøtet
  * Spring Boot og lage alt selv (ail)
    * drodle litt på pros and cons
    * kunnskap og kjennskap til Boot
    * stack overflow
    * standardisering av det alle uansett må gjøre
      * ikke lage ting som ikke gir oss verdi / finne opp hjulet på nytt
    * Spring igjen...
    * Boot gjør mye av det vi tidligere har gjort selv
      * Det meste er laget tidligere
  * 12 factor apps
    * Hystrix / Resilijence4j
  * Slipper å lage dette selv nå
  * Få opp en app kjapt for å validere i produksjon
  * Etter andre applikasjon, lage en template
  * Gjøres som vanlig forvaltning, ikke som et stort prosjekt

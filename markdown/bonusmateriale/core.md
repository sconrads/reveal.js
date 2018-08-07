### Underpunkt: Core - En ny monolitt?

Mye delt kode har skapt en monolitisk kjerne.
Vi ser nå behovet for å i større grad lage biblioteker med løsere koblinger. 
* Prioriteringer
* Kostnad


notes:
###### Anders:



###### Opprinnelige notater:

* 2015 - core ble presentert som teknisk gjeld
* Ble ikke prioritert 
* Fokus var å dele opp monolitten for å kunne skalere
* Eks. logging (logback)
* Git utvikling av core
* Stabilisering
* Ny arkitektur skaper større endringer
  * Nye bibliotek
* Større fokus på rydding nå
  * Ikke ta med ting vi ikke vil ha
* Core støtter alt mulig
* Ville trolig konvert skjermbilder fortsatt om vi ikke tok denne veien
* Vi kunne brukt tid på skjermbilder som uansett skal kastes, og de ville blitt levert på Backbone ark.
* Hvordan lager vi bibiloteker
  * Avhengigheter
  * Git repo
  * Open Source tankegang med frikobling
  * Kan brukes av andre plattformer
  * Ny templating kan effektivisere vedlikeholdet og opprettelse
* Vi er flinke til å deprecere
  * Må bruke tvang eller lage en oppgave på å slette
* Kostnad med å dra med oss ting vi ikke egntlig trenger
  * Forvaltningskost
  * Billgere å rydde først

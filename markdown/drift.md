### Drift

#### Erfaring:
- Mange nye applikasjoner skape mye arbeid for Drift

#### Tiltak:
- Drift måtte fristilles fra repetitive standardoppgaver


notes:
###### Stian:

Hva skjer så når man får en haug med applikasjoner som skal i produksjon hele tiden?
Jo, Drift blir lei av å kjøre yum install. 

Ganske raskt etter at de første appene var på lufta, så vi at Drift måtte fristilles fra repetive standardoppgaver. 
Vi satt da igang med å automatisere produksjonssettingen. Vi satt sammen utviklere og testere og lagte en løsning på toppen av RunDeck. Teamene fikk da mulighet til å selvbetjene installasjon i alle miljøer inkludert produkjson. I dag så installeres de aller aller fleste leveransene av teamene selv. 

Drift og utvikling måles forskjellig. Litt svart på hvitt, så vil utviklere lage ny funksjonalitet, mens Drift er opptatt av stabile tjenester. Som nevnt tidligere etablerte vi teamet Optimus. I dette teamet kan drift og utviking lage løsninger sammen, og på den måten fungere som en brobygger mellom disse to kulturene. Gjennom å jobbe sammen bygger vi også tillit og gjennom tillit kan utviklerene få mer tilganger. 

Alt er midlertidig, og det gjelder nok også for Optimus. Jeg tror det viktig at et slikt team prøver å gjøre seg selv arbeidsledige. Løsnigene som produseres av dette teamet bør forvaltes som intern open source eller som en del av driftplattformen. Det er fare for at slike team lager verktøy som bare kan forvaltes av teamet selv og som ikke har bred forankring blant utviklerene eller drifterene. Så får vi se om tre år, når vi står her igjen, hva som ble fasit.



###### Opprinnelige notater:
Drift måtte fristilles fra repetitive standardoppgaver.
Vi fikk begrensninger fra Drift knyttet til antall applikasjoner vi kunne ha og når disse kunne produksjonssettes.

#### Tiltak:
* Automatiserte produksjonssettingen og ga teamene ansvar for å utføre produkjonssetting selv 
  * OpenShift
  * Rundeck
  * Avstand, organisering


* OpenShift
* Tilganger
* Kultur
* Logger (tilganger, løsning)
* Presset frem endring i Drift
  * Ikke den beste inngangen
* Fokus er stabile tjenester
* Utviklere kommer tettere på 
* Jobber på feil og problemer, ikke med å lage nye løsninger
* Utfordre Drift i forhold til tilganger og endrede behov
* Vi må bygge inn kvalitet
* Optimus
  * Brobygger
  * Lage løsninger sammen
  * Midlertidig?
* Å hjelpe teamene til å levere godt
* Lite ofte vs mye sjelden

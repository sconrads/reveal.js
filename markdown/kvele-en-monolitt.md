### Kvelningen av monolitten

Det tar tid å kvele en monolitt, men verden rundt går raskt fremover.
Det har tatt lengre tid å fase ut monolitten enn vi hadde forutsett.
Samtidig som vi dro med oss teknisk gjeld som Struts og JSF, innførte vi nye teknologier som React og Kotlin.
Vi støtter nå fire frontendteknologier. Det er krevende.

#### Tiltak:
* Behold høyt fokus på å kode bort monolitten.
* Gjør det mulig for de enkelte teamene å teste ut ny teknologi uten å påvirke andre team. 
* Ikke ta med uønsket teknologi videre


notes:
###### Anders:

* **Strategi for å gradvis kvele monolitten har fungert**.
  * Det har gitt veldig stor **frihet og fleksibilitet** til de enkelte teamene.
  * Man har kunnet migrere funksjonalitet i det tempo og rekkefølge teamet mener seg best tjent med.
    * Men det betyr også at utfasing og migrering kan komme i **konkurranse med utvikling av ny funksjonalitet**.
* Det vi ser nå er at vi fortsatt ikke har kunnet skru av monolitten: **Annen funksjonalitet er blitt prioritert høyere**.

##### Lærdom:
* Større **angrepsflate** krever mer kostbar patching og overvåkning
* Færre avhengigheter til **lukket tredjepart**
* **Tungt å forvalte** gammel plattform
  * **Utviklertilgang** og kompetanse
* I denne fasen ønsker vi å **ikke tilrettelegge for uønsket teknologi** - vi ønsker at løsningen skal **selge seg selv**!


###### Opprinnelige notater:

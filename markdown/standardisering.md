### Felles standardisering


notes:
###### Anders:

En av de tingene vi føler har fungert for oss er å **standardisere**, spesielt struktur på applikasjonene men også utviklingsmiljøet. Det gir oss en **gjenkjennelseseffekt** som vi tror har vært viktig, og ikke minst så har det gjort at automatiseringen vi har gjort i ettertid har vært enklere. Når det er sagt så står teamene ganske fritt til å eksperimentere, og det blir gjort.

###### Stian:
Vi har helt siden starten hatt en **templatingmekanisme** for å lage og oppdatere applikasjonene våre, og vi har tilsvarende for selve **utviklingsmiljøet**. I tillegg nevnte vi vår venn verktøykassa-**Bob** i 2015, og han lever i beste velgående i dag også, og er en samling script.

Disse tingene ligger som **git-prosjekt** og vi har vært heldige å fått et miljø hvor mange av **utviklerne aktivt foreslår endringer** som er testet av enkeltpersoner eller team. Det er ingen team eller personer som eier disse fellesløsningene, men de er fordelt ut slik at noen har et **overordnet ansvar** for at de fungerer og at det finnes en viss basiskompetanse på løsningen.


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

Ofte diskuteres større forslag til forbedringer eller erfaringer som er gjort i **"Arkitektmøtet for ikke-arkitekter"**. 

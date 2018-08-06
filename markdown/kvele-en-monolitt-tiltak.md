### Kvelningen av monolitten

#### Tiltak:
* Behold høyt fokus på å kode bort monolitten
* Vurder nøye hvilke teknologier man beholder


notes:
###### Anders:

For å ikke ende opp med å drifte gamle løsninger evig, så kan det nok være lurt at noen faktisk følger opp fremgangen 
og holder trykket på utfasingen oppe. Det har vært **tungt å forvalgte** en gammel plattform i kombinasjon med en ny,
og hvem vil egentlig sitte igjen på noe gammelt? Som i de fleste andre bransjer så er det de **færreste som liker å 
jobbe med utdatert teknologi**. Med andre ord; skal vi greie å beholde utviklerne våre, og finne flere, så må vi **tilpasse 
oss det som finnes av kompetanse** der ute.

Som et eksempel på gammel teknologi så beholdt vi for eksempel **Struts** alt for lenge, noe som har medført ekstra 
patching og overvåkning av sårbarheter. Flere teknolgoier gir en større **angrepsflate**! 
For oss som et relativt stort utviklingsmiljø ser vi det som en fordel å ha få avhengigheter, 
spesielt til **lukket tredjepartskode**.

Sett tilbake, så tilrettela vi kanskje litt for godt for den gamle teknologien vår. Det gjorde migreringen raskere,
men forutsetter at man har fokus på det man driver med og gjør et bevisst valg. Nå har vi sett hvordan det gikk, og når 
vi nå jobber med neste fase så er en av lærdommene at vi forsøker å **tilrettelegge minst mulig for uønsket teknologi**,
men heller forsøker å lage en løsning som skal **selge seg selv** slik at utviklerne ønsker å migrere.


###### Opprinnelige notater:
* Gjør det mulig for de enkelte teamene å teste ut ny teknologi uten å påvirke andre team. 

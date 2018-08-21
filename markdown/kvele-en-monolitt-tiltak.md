#### Tiltak:
* Behold høyt fokus på å kode bort monolitten
* Vurder nøye hvilke teknologier man beholder


notes:
###### Anders:
For å ikke ende opp med å drifte gamle løsninger evig, så kan det nok være lurt at noen faktisk følger opp fremgangen og holder trykket på utfasingen oppe. Det har vært **tungt å forvalte** en gammel plattform i kombinasjon med en ny, og hvem vil egentlig sitte igjen på noe gammelt? Som i de fleste andre bransjer så er det de **færreste som liker å jobbe med utdatert teknologi**. Med andre ord; skal vi greie å beholde utviklerne våre, og finne flere, så må vi **tilpasse oss det som finnes av kompetanse** der ute.

###### Stian:
Som et eksempel på gammel teknologi så beholdt vi for eksempel **Struts** alt for lenge, noe som har medført ekstra patching og overvåkning av sårbarheter. Vi har måtte lage vår egen Struts versjon. Flere teknologier gir en større **sårbarhetsflate**! Vi er veldig tjent med å ha så få avhengigheter som mulig til den type biliotek som mulig, og spesielt til **lukket tredjepartskode**.

###### Anders:
Sett tilbake, så tilrettela vi kanskje litt for godt for den gamle teknologien vår. Det gjorde migreringen raskere, men forutsetter at man har fokus på det man driver med og gjør et bevisst valg. Nå har vi sett hvordan det gikk, og når vi nå jobber med neste fase så er en av lærdommene at vi forsøker å **tilrettelegge minst mulig for uønsket teknologi**, men heller forsøker å lage en løsning som skal **selge seg selv** slik at utviklerne ønsker å migrere.

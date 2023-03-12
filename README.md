# Kösimulering i Skruttemålas postkontor

Nyckelord: Simulering, kontrollstruktur, slumpgenerator

## Uppgiften

### Lydelse

På det lilla postkontoret i Skruttemåla behöver kösituationer simuleras. De öppnar varje dag kl 9 och stänger kl 18. Kunder anlädning i genomsnitt var femte minuter, dvs sannolikheten för att en ny kund ska komma under en viss minut är 20%. För postexpiditen, Fru Franco, tar det exakt två minuter att betjäna ett postärende. Hälften av alla kunder har ett enda ärende, en fjärdedel har två ärenden, en åttondel tre ärenden osv.

Vi stängningsdags låser Fru Franco dörren men betjänar plikttroget de kunder som står i kön redan. DÄrefter för hon dagens kundstatistik (totala antalet kunder, alla kunders sammanlagda väntetid och genomsnittliga väntetid per kund). Allt detta ska simuleras av ditt program enligt följande exempel:

![image](https://user-images.githubusercontent.com/101513815/224565365-1359e5ba-e8ce-4d86-ac2e-d5b6125ef4d9.png)

Alla kunder förutsätts anlända vid hela minuttider, ingen får komma indrällande några sekunder för tidigt eller för sent.

- Vid ankomsten slumpas kundens antal ärenden fram enligt sannolikheten som gavs ovan. Tricket ligger i att köra en loop som bryts med 50% sannolikhet. Varje nytt ärende betyder ökad betjäningstid. Utträdestiden beräknas dock inte förrän kunden ska betjänas.
- Är kön tom när en ny kund anländer, betjänas denna direkt (utträdestiden beräknas).
- Är kön inte tom, ställs kunden i kön.

### Krav för olika betyg

Uppgiften i sin grundform är nog för att uppnå bedömningen A gällande uppgiftens svårighet. Om du vill utmana dig själv kan du införa möjligheten att förändra problemets parametrar, exempelvis öppettider, ankomstsannolikhet m.m., genom inmatning. Inför även felkontroll så att användaren inte försöker mata in något som inte är tal.

## Dokumentation & Planering

### Loggbok

Under arbetet förväntas du föra loggbok. Varje inlägg bör innehålla vad du gjort under passet och hur det gått. Skriv även gärna om du uppnått någon av milstolparna i projektplaneringen, använd gärna då ID:n för referens. Få gärna med eventuella problem du stött på och hur du löst dem (ifall du gjort det).

### Projektplan

Du påbörjar ditt projekt med att planera. Detta görs genom en projektplan med milstolpar och grindhål som ska uppnås under arbetets gång. Din projektplan bör revideras minst tre gånger under arbetet för att nå högsta bedömning. Projektplanen ska vara utförlig med detaljerade mål och uppgifter samt när deadline för dessa sker och vad som ska göras.

Projektplanen är det Google Sheet-arket som finns på classroom.

### Flödesschema

I första stadiet av projektet bör du även skissa upp ett flödesschema i förslagsvis draw.io som ska tillhöra ditt program. Tänk på vad de olika symbolerna betyder, samt att du inte har överflödiga punkter i schemat, eller att det är oläsbart.

## Författare

Niclas Lund

## Disclaimer

Uppgiften (eller inspiration till den) är ärligt stulen från EECS-skolan (gamla CSC) och kursen DD1314.

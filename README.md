# socket-chat

Uppgift  
• Du ska göra en applikation som använder socket.io på klient-sidan (frontend) och server-sidan (backend). Man ska kunna kommunicera mellan klient-sidan och server-sidan och kunna vara uppkopplade som flera användare samtidigt och kommunicera i realtid.  
• Du ska göra ett enkelt tärningsspel på klientsidan som skickar varje kast till server-sidan och skriver ut summan så att alla andra anslutna ser det tillsammans med ditt namn.  
• Varje uppkopplad användare ska kunna skriva kommentarer som visas för alla andra anslutna.  
• Du ska filma en kort demo som visar att det fungerar som det är tänkt som lämnas in tillsammans med labben.  
• Inlämningsuppgiften ska göras individuellt.  

Följande ska finnas med när du lämnar in labben:  
• Källkoden till applikationen som en zip-fil alternativt en textfil med en länk till Github.
Om ni laddar upp applikationen som en zil-fil ta bort node modules mappen så att zip-filen inte blir för stor.  
• En kort film (ca 5 minuter) där du gör en demo där det framgår att allting fungerar genom att du har uppe minst två flikar i en webbläsare (som fungerar som två uppkopplade användare som använder applikationen). Använd t ex programmet OBS för att göra filmen.
Har du gjort VG-delen behöver du visa i Insomnia eller Postman att databasen fungerar som det är tänkt.

Betygskriterier  
Krav för G  
• Du ska göra en applikation med node.js som använder socket.io på server-sidan och klient-sidan.  
• Du ska göra ett enkelt tärningsspel på klientsidan som skickar varje kast till server-sidan och skriver ut summan så att alla andra anslutna ser det tillsammans med ditt namn. Använd slump för att generera ett tärningskast (ett tal mellan 1 och 6).  
T ex: let randDice = Math.floor(Math.random()*6+1);  
Man ska också kunna se den totala summan hittills tillsammans med varje kast.  
Man ska kunna mata in sitt namn i ett formulär med ett textfält som sedan skickas med i varje kast. För att göra ett kast trycker man på en knapp som då skickar till server-sidan och visar för alla andra anslutna. (Om man vill kan man bygga ut funktionalitet i tärningsspelet med t ex antal tärningar för varje kast, först till en vissa summa vinner. Det går också bra att göra om till ett kortspel t.ex Blackjack. Men tanken är att hålla själva spelet enkelt och fokusera på upplägget med kommunikation mellan klient och server och de uppkopplade användarna i realtid.)  
• Varje uppkopplad användare ska också kunna skriva en kommentar som visas för alla andra anslutna.

Krav för VG  
Utöver kraven för G:  
• Du ska spara alla ”tärningskast” i en MongoDB-databas genom Mongoose. Du ska spara namnet på spelaren, tärningskastet samt den totala summan hittills för spelaren. Du ska ha en endpoint (genom att använda Express) som visar alla tärningskast som är sparade i databasen enligt ovan. Du behöver inte göra frontend-kod med Fetch för att visa tärningskasten som är sparade utan räcker att du kan visa i Insomnia eller Postman.

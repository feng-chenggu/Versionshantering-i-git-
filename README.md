Versionshantering-i-Git:
## En kort introduktion till hur versionshantering går till i Git
<html>
<head>
  <title>Vad är Git?</title>
</head>

  <body> 
    
  <p>
    Git är ett verisionshanteringsprogram som bland annat möjliggör: 
    <ul>
      <li>Att återgå till tidigare verisioner och byta ut till den om så önskas</li>
      <li>Att en fils färdiga tillstånd kan sparas</li>
      <li>Enklare samarbete med andra samt bättre och tydligare förståelse av de olika verisionerna</li>
    </ul>
  </p>

  <h1>Stage</h1>
  <p>
    Ni har tidigare lärt er att skapa en mapp samt en fil som ni har redigerat genom Git. 
    Nästa steg är nu stage där ändringar läggs till. Skriv in följade i git under din fil "index.html":
    <ol>
<li>1.<code style="color : red">git add index.html</code></li>
<li>2.<code style="color : red">git status</code> Använd detta kommando för att visa vad som har ändrats</li>
    </ol> 
  </p>

   <h1>Commit fil</h1>
  <p>
    I detta steg sparar ni ändringarna som en verision genom kommandot "commit" och namnger det genom "--message "Lämplig text"", sedan skapar ni nya ändringer och sparar det som en verision. Lämpligt att ni använder er av "git status" efter varje kommando för att se vad som ändrats.
    <ol>
<li>3.<code style="color : red">git commit --message "Skapat index.html"</code></li>
<li>4.Redigera din index.html fil genom att exempelvis lägga till en head: <code style="color : red"><head></head></code></li> 
<li>5.Skriv: <code style="color : red">git add index.html</code></li>
<li>6.<code style="color : red">git commit --message "Lagt till HEAD"</code></li>
    </ol> 
  </p>
  
  </body>
</html>

<h1>Verisionshantering i Git</h1>
En kort introduktion till hur versionshantering går till i Git
<html>
<h2>Vad är Git?</h2>

  <body> 
    
  <p>
    Git är ett verisionshanteringsprogram som bland annat möjliggör: 
    <ul>
      <li>Att återgå till tidigare verisioner och byta ut till den om så önskas</li>
      <li>Att en fils färdiga tillstånd kan sparas</li>
      <li>Enklare samarbete med andra samt bättre och tydligare förståelse av de olika verisionerna</li>
    </ul>
  </p>

  <h2>Stage</h2>
  <p>
    Ni har tidigare lärt er att skapa en mapp samt en fil som ni har redigerat genom Git. 
    Nästa steg är nu stage där ändringar läggs till. Skriv in följade i git under din fil "index.html":
    <ol>
<li><code style="color : red">git add index.html</code></li>
<li><code style="color : red">git status</code> Använd detta kommando för att visa vad som har ändrats</li>
    </ol> 
  </p>

   <h2>Commit fil</h2>
  <p>
    I detta steg sparar ni ändringarna som en verision genom kommandot "commit" och namnger det genom "--message "Lämplig text"", sedan skapar ni nya ändringer och sparar det som en verision. Lämpligt att ni använder er av "git status" efter varje kommando för att se vad som ändrats.
    <ol>
<li><code style="color : red">git commit --message "Skapat index.html"</code></li>
<li>Redigera din index.html fil genom att exempelvis lägga till eller ta bort text.
<li>Skriv:<code style="color : red">git add index.html</code></li>
<li><code style="color : red">git commit --message "Lagt till HEAD"</code></li>
    </ol> 
  </p>
  
  <h2>Git log</h2>
  <p>
    I detta stycke visar "git log" hur många commits (tillstånd) som har sparats, ur informationen som framstår kan författaren, commit message och datum utläsas. Notera att genom tilläget --pretty=online visar commit message, HEAD (talar om vilket det nuvarande tillståndet är) och hash som är en unik indentifikation för en commit (exempelvis 42e95e5b41a4d2351ec2850812b34cf7c2112f11).
   <ol>
<li><code style="color : red">git log</code></li>
<li><code style="color : red">git log --pretty=oneline</code></li>
    </ol> 
  </p>
    
  <h2>Visa innehållsförändringar</h2>
  <p>
    Kommandot visar ändringarna i filen och navigeras med pil upp/ned samt q för avslut.
   <ol>
<li><code style="color : red">git log --patch -2</code></li>
    </ol> 
  </p>
    
  <h2>Återgå till tidigare verision</h2>
  <p>
    I stycket används den hash till den verision som önskas återgå till, antingen hela hash eller de fem första tecknen. Git sänder en respons tillbaka och öppnas filen är den som den tidigare verisionen. Kommandot checkout innebär ett byte.
   <ol>
<li><code style="color : red">git checkout "hash" index.html</code></li>
    </ol> 
  </p>
    
  <h2>Återställa senaste verision</h2>
  <p>
    Använd "git log", notera att den senaste hash är den senaste verisionen, följt av checkout och önskad hash. Öppnas filen bör verisionen vara återställd. 
   <ol>
<li><code style="color : red">git checkout "senaste hash" index.html</code></li>
    </ol> 
  </p>
  </body>
</html>

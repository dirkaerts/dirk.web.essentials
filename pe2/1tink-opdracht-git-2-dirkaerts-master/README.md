# Opgave GIT week 6
### Clone de repository
Clone de repository naar jou lokaal toestel. Instructies hoe je dit kan doen kan je terug vinden in de slides op Blackboard onder week 3.

TIP: git clone

### Opgave
Tijdens de GIT oefening krijg je een index.html bestand, een merge.html bestand en een stijl.css bestand. Deze beginbestanden staan in de map "html". De bedoeling is dat je aan de hand van mediaqueries deze website responsivse maakt.

Daarnaast simuleren we een merge-conflict dat je moet oplossen. Volg hierin duidelijk alle instructies!
 
#### Mediaqueries
Tijdens deze oefening maak je een aantal mediaqueries aan in het stijl.css bestand. Deze mediaqueries gebruik je om het bestand index.html responsive te maken. Je doet minstens één commit per mediaquery.

De website bestaat uit een fixed lay-out. Indien het scherm kleiner is dan 960px voorzie je een relatieve lay-out. De linkerkolom heeft een breedte van 25%, de content heeft een breedte van 75%. De gridview in de content verspringt van 4 kolommen(fixed) naar 4 kolommen(relatief).

Indien het scherm kleiner wordt dan 600 pixels zorg je ervoor dat de gridview in de content bestaat uit 2 kolommen (breedte = 50%).

Indien het scherm kleiner is dan 450 pixels zorg je ervoor dat de linkerkolom 100% breed wordt. De navigatielinks moeten onder elkaar staan waarbij de tekst gecentreerd is. Daarnaast bestaat de gridview in de content uit 1 kolom (breedte = 100%). De header mag niet meer zichtbaar zijn. Voorzie ook een paragraaf met de melding "Je bezoekt onze website op een mobiel device. Heb je onze app al gedownload?" die enkel in deze weergave zichtbaar is.

#TODO: screenshots toevoegen

#### Merge conflict
**!! De naamgevingen van de commits in dit gedeelte zijn van essentieel belang voor de evaluatie !!**

Ga naar de repository op http://github.com en bewerk via github het bestand merge.html. Op deze pagina staat een lijst met vakken uit de eerste semester. Hierin staan 2 foute vakken, namelijk "Cisco CCNA1" en "Security Essentials". Verwijder deze 2 vakken via Github. Bij het opslaan geef je als commit message "merge deel 1".

Open vervolgens het bestand merge.html op je lokaal toestel. Vervang hierbij de vakken "Cisco CCNA1" en "Security Essentials" door "OS Essentials" en commit deze wijzigingen met het bericht "merge deel 2".

Probeer vervolgens je wijzigingen te pushen naar github via `git push origin master`. 
Je krijgt hierbij een foutmelding dat de lokale branch achter loopt op de remote branch. (m.a.w. er zijn aanpassingen gedaan op de remote repository die je nog niet op je lokaal toestel hebt)

Doe vervolgens een `git pull origin master` om de laatste wijzigingen op te halen. Vervolgens krijg je een foutmelding dat er een merge conflict is. (m.a.w. je hebt de laatste versie van de remote repository binnengehaald, maar hebt nu twee verschillende wijzigingen in hetzelfde stukje code. Het mergen van dit stuk code kan niet automatisch uitgevoerd worden ==> **merge conflict**)

Los dit merge conflict op. Het is de bedoeling dat in het bestand merge.html "OS essentials" als vak staat. Commit deze wijzigingen met als message "merge conflict opgelost" en push vervolgens opnieuw naar github. Hoe je een merge conflict kan oplossen, kan je terug vinden in de CodeAcademy cursus op Blackboard.

## Evaluatie
Om punten te scoren op deze opdracht is het belangrijk dat we verschillende commits kunnen zien in jouw repository. De commits tonen een duidelijke vooruitgang van je website! De uiteindelijke uitwerking van de HTML en CSS in de oefening is van minder belang en wordt niet geëvalueerd.

Daarnaast moeten we duidelijk zien dat je het merge conflict hebt opgelost in de commit history. Volg hiervoor nauwkeurig de stappen onder het hoofdstuk "merge conflict"

Indien er geen repository aanwezig is, er minder dan 3 commits waarin duidelijke wijzigingen aanwezig zijn of er geen merge conflict opgelost is, resulteert dit in een 0 op deze deeltaak van de PE.

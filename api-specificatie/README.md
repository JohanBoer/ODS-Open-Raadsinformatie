# API specificaties Open Raadsinformatie
Hier vind je de API specificaties in drie verschillende formaten:
* Open API Specificaties 3 [(yaml)](https://github.com/VNG-Realisatie/Open-Raadsinformatie/blob/master/api-specificatie/openapi.yaml) en [swagger](https://petstore.swagger.io/?url=https://raw.githubusercontent.com/VNG-Realisatie/Open-Raadsinformatie/master/api-specificatie/openapi.yaml#/)
* [JSON schema Draft 5](https://github.com/VNG-Realisatie/Open-raadsinformatie/blob/master/api-specificatie/openapi.json)

In deze versie zijn nu handmatig enkele wijzigingen in het .yaml bestand doorgevoerd die niet in de .json bestanden zijn doorgevoerd. 
Op hooflijnen zijn dit :

- Aan iedere bericht body is toegevoegd:

  - Een @context body 

     ofwel een link, met een mapping speciaal voor de klasse / resourcetype van het hoofdobject. Maak deze link beschikbaar in de buurt van de namespace met een download naar een context JSON bestand zoals in de bijlage.

  - Een @type veld       

    met daarin een link naar de klassedefinitie op VNG site

  - Een @id       

    met een link naar het item zelf (_self)

- Aan iedere _links is toegvoegd:

  - @id

- In de @context moet staan:

  - De mapping naar alle losse keys die in de JSON voorkomen

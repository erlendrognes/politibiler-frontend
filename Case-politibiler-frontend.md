
# Case: Politibiler Frontend

I denne oppgaven skal du utvikle et verktøy som administrerer politibiler for operasjonssentralen. Du står fritt til å velge hvilket rammeverk, og byggverktøy (f.eks. React, Angular, Blazor, Svelte), du ønsker å bruke, men vi ønsker helst at du koder i JavaScript eller TypeScript. Løsningen bør inneholde tester.

*Oppgaven har ingen fasit og brukes kun i vår dialog sammen i det tekniske intervjuet. Det er lov å gjøre antagelser, men forklar disse i en readme-fil.*

## Oppgaven
Du skal utvikle en webside som kan tilby følgende funksjonalitet:

- Vise en oversikt over alle politibiler, inkludert merke, modell, år, registreringsnummer og nåværende status (*Tilgjengelig*, *I oppdrag*, *Under vedlikehold*). Oversikten skal vises sortert etter politibilenes ID i numerisk rekkefølge. Du velger selv hvordan dette skal se ut, vær kreativ!

- La brukeren filtrere hvilke biler som vises, f.eks. kun biler som har status *Tilgjengelig*, eller kun biler av merket *Ford*.

- La brukeren endre statusen til en politibil, og sende et kall som lar backend oppdatere dette. Du bestemmer selv hvordan dette fiktive kallet skal se ut.

Løsningen din må være i stand til å hente dummy-data direkte fra følgende API: *** Lenke ***
<!-- https://api.politiet.no/case/politibiler -->

Endepunktet støtter kun GET, og vil returnere dataene i tilfeldig rekkefølge. Hvert objekt i JSON-arrayen beskriver en bil og dens nåværende status, f.eks.:
```json
[
	{
    	"id": "1",
    	"merke": "Ford",
    	"modell": "Focus",
    	"årsmodell": 2018,
    	"regNr": "DR 96669",
    	"status": "På vei til hendelse",
    	"oppdrag": "Trafikkulykke"
    	},
    	...
]
```

## Innlevering:
Oppgaven leverer du som en lenke til et privat repository med en readme-fil som forteller litt om arbeidsprosessen og forklarer hvordan løsningen din kan kjøres. Du leverer løsningen din til avtalte personer ved å legge dem til som «Collaborators» enten på Github eller Gitlab.

# Eksamen PGR301

Følgende oppgaver har blitt besvart i denne innleveringen:
* DevOps prinsipper & Pipeline
* Terraform og IAC i Pipeline (delvis)

## Oppgave - DevOps

Den beste forbedringen teamet kan gjøre i henhold til arbeid med kildekode og versjonskontroll er å innføre branch
protection på GitHub-repositoriet.

![settings](https://imgur.com/HAWkenD)

Når man er på sitt repository, så trykker man på Settings-tabben og deretter Branches under valgene på venstre side.

Neste steg er å trykke på Add rule-knappen som er til høyre for Branch protection rules.

![add rule](https://imgur.com/1O5ZfU7)

Her er det flere valg man kan ta som vil gjøre arbeidsflyten bedre og mer effektiv. Man kan krysse av for Require
status checks to pass before merging, og tilrettelegge for at kode som ikke kompilerer eller tester som failer
blir markert med en Error eller Failure state, som da ikke kan merges til main før dette er rettet opp i.

![rules](https://imgur.com/xiGXi5f)

Man kan krysse av for Require a pull request before merging og Require approvals for å forsikre seg om at minst
én annen person på teamet går gjennom koden og godkjenner det før det blir merget til main.

Dette kan være en god arbeidsflyt hvis man jobber i team og med flere brancher:

* Checkout main branch og pull siste versjon
* Oprett ny branch med feature du skal lage som navn
* Implementer koden og lag tester for det. Stegvis med flere commits
* Push commitsa til GitHub
* Rebase branchen, fjern unødvendige commits og rydd opp i kommentarer
* Push branchen til GitHub
* Lag Pull request på GitHub
* Få en i teamet til å godkjenne Pull requesten (legg til som collaborator hvis personen ikke er det)



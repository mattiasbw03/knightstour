Knight’s Tour
Denne aflevering gik ud på at programmere og analysere Knight’s Tour-problemet, hvor en ridder på et skakbræt skal besøge alle felter én gang ved at bevæge sig efter skakkens riddertræk (2 frem og 1 til siden).
Opgaven handlede både om logik og strukturering af kode i C.
Jeg har implementeret to forskellige tilgange:
Greedy (første mulige træk)
Ridderen vælger altid det første felt, som er lovligt at flytte til.
Denne metode er meget simpel, men ender ofte med at ridderen “låser sig fast”, før alle felter er besøgt.
Resultatet bliver derfor en tabel, hvor hvert felt viser, hvor mange ruder ridderen nåede at besøge ud fra den startposition. Tallene varierer typisk mellem 30–50 på et 8×8-bræt.

Warnsdorff-heuristikken (den smarte metode)
Her vælger ridderen altid det felt, der har færrest videre muligheder.
Det betyder, at ridderen undgår at “spærre sig selv inde”, og på et 8×8-bræt lykkes det næsten altid at besøge alle 64 felter.
Metoden er markant mere effektiv og viser tydeligt forskellen på en simpel og en heuristisk tilgang til et søgeproblem.

Derudover blev programmet udvidet med funktioner til at:
udskrive tabeller over antallet af besøgte felter fra alle startpositioner

vise et eksempel på den fulde tur (nummereret fra 1–64)

kunne ændre brætstørrelsen nemt ved at justere #define boardN

Projektet blev afsluttet med at jeg lærte, hvordan man opdeler et større C-program i flere filer (.h, .c og main.c), samt hvordan man bruger GitHub til versionsstyring og upload af projekter.
Opgaven styrkede min forståelse af algoritmer, datastrukturer og systematisk fejlsøgning i VS Code.

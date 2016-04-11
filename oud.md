###PROCES:
Projectpartners worden verondersteld samen te willen werken middels onderstaande uitgangspunten:

1. Integraal Ontwerpen waarbij alle partijen Modelleren met *Best Of Breed* Software: Alle Informatie en Data delen en Coördineren en Communiceren op basis van IFC disciplinemodellen.
2. Hanteer een vaste week structuur voor de BIM workflow: Disciplinemodel modelleren->IFC/BCF export->IFC  export intern checken->IFC/BCF uploaden->IFC/BCF model check BIM-coördinator-> Issues constateren->Clash  Sessie houden->Issues interpreteren->Acties toekennen->Acties verwerken->Reactie vastleggen->BCF export. NB. Bij een wijziging in een van de disciplinemodellen wordt bovenstaande workflow ‘getriggerd’.
3. BIM disciplinemodellen opbouwen door korte ‘iteraties’ en kleine ‘batches’ te modelleren -> testen -> aanpassen. 
4. Starten met BIM methodiek vanaf start van het definitief ontwerp, op voorwaarde afgerond voorlopig ontwerp. We kennen daarna minimaal 2  deelfasen van een BIM project: ‘ontwerp’ en ‘engineering’.
5. Eerst 2D Principe Detaillering (schetsmatig) ontwerpen. Daarna pas beginnen met modelleren van het BIM.
6. Eerst het BIM model modelleren. Daarna pas starten met 2D extracten.

###PRODUCT:
Projectpartners zijn zelf verantwoordelijk, en worden verondersteld hun eigen IFC Extracten te verifiëren op onderstaande uitgangspunten:

7. Een BIM bestaat uit Objecten. Objecten hebben Geometrie en Eigenschappen. 
8. Alle 2D extracten (tekeningen, details, annotaties) zijn een Directe Afgeleide uit het BIM model. 
9. Nulpunt, Peil en Bouwlagen (*Revit: Levels/hulplevels*) afstemmen tussen alle projectpartners.
10. Benamingen van Bouwlagen conform RVB BIM norm: “-1 kelder”, “00 begane grond”, “01 eerste verdieping”,  etc. (Revit: een IFC export bevat alleen de hoofdbouwlagen (Building Stories) geen hulplevels).
11. Model consequent, en per Bouwlaag opbouwen en objecten een Relatie geven met de Juiste Verdieping.
12. Eigenlijk Gebruik van objecten toepassen voor alle objecten. Dit betekend wanden modelleren met Wall  objecten, ramen met Window objecten, balken met Beam objecten, vloeren met Slab objecten, etc. (Revit:  *GenericModel* objecten altijd exporteren middels IfcExportAs: *Ifc_Objecttype*).
13. Alle objecten Consequent als losse objecten (*Revit: ‘Disallow Join’*) modelleren met een Bruto Geometrie.
14. Alle objecten modelleren met een correct Materiaal.
15. Alle objecten in het BIM voorzien van een NLsfb codering, minimaal 4 cijfers.
16. Alle objecten in het BIM voorzien van Structural (*LoadBearing*) true/false.
17. Alle objecten in het BIM voorzien van IsExternal true/false.
18. Een BIM altijd modelleren zoals men het fysiek gebouw gaat bouwen, maar met een Praktisch Geometrisch  Detailniveau (b.v. met name bij Profile geometrie zoals b.v. daktrims). 
19. Sparingen altijd modelleren met een ‘sparingmaker’; dit is een GenericModel (*Family in Revit*) die middels  parametrische waarden wordt ingeregeld. Dit maakt het aanpassen en tellen van sparingen makkelijker. (*Revit:  GenericModel Sparingen altijd exporteren middels IfcExportAs: Ifc_Opening*).
20. Staal objecten altijd modelleren vanuit Standaard Profielen (b.v. HEA 120).
21. Benaming van Objecten consequent en conform Dutch Revit Standards:  -NL-SfB_IDbedrijf_omschrijving+dimensie. 

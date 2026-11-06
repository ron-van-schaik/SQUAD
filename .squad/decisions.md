# Squad Decisions

## Active Decisions

### Samenstelling DIT-team en werkgrenzen — 2026-11-02

- **Goedgekeurde samenstelling:** exact zeven DIT-specialisten: Lead & Intake Coordinator; Cloud Process Analyst; Service Delivery Analyst; Evidence & Audit Specialist; Technical Operations Challenger; Data & Automation Engineer; Quality Reviewer & Scribe.
- **Onderscheid supportrollen:** Scribe, Ralph, Rai en Fact Checker blijven de vier standaard Squad-supportidentiteiten. Dit zijn geen extra DIT-rollen en geen gewone specialistische routingbestemmingen. De DIT-specialist Quality Reviewer & Scribe is onderscheiden van de ingebouwde Scribe.
- **Routing:** elk werkitem heeft één accountable specialist, gekozen op basis van het primaire gevraagde resultaat. Extra bijdragen blijven afgebakend en zijn niet speculatief.
- **Scopegrens:** deze inrichtingsfase omvat alleen teamsamenstelling, verantwoordelijkheden, samenwerking en routing. Er wordt geen inventarisatie van kennisbronnen of tools gedaan en er worden geen bedrijfssystemen gewijzigd.
- **Feitelijke basis:** er is geen organisatiespecifieke DIT-uitbreiding, provider, bedrijfssysteem, toolset of compliance-eis opgegeven; agents mogen die niet invullen.
- **Persistentie:** rolgrenzen en scope staan ook in de zeven specialistische `history.md`-bestanden. `memory.*`-tools en de Squad CLI waren niet beschikbaar; daarom is geen afzonderlijke governed memory-entry aangemaakt.

## Governance

- All meaningful changes require team consensus
- Document architectural decisions here
- Keep history focused on work, decisions focused on direction

### VOORSTEL — Capability backlog DIT-team (pending/unapproved) — 2026-11-02

**Status:** voorstel ter beoordeling; niet goedgekeurd, geen teamconsensus vastgesteld. Dit is een backlog, geen besluit, opdracht tot gegevensverzameling, toegangverlening of systeemwijziging.

#### Feiten, grenzen en onbekenden

- De bestaande teamcontext bevestigt zeven DIT-specialisten en hun rolgrenzen. De charters bevestigen geen specifieke organisatie, DIT-uitbreiding, platform, bron, live systeem, tool, account, autorisatie, compliancekader of auditnorm.
- De gevraagde lijst met DNB-bronnen en systemen staat niet in de aangeleverde context. Er worden daarom geen bronnen, systemen of goedkeuringen als bestaand verondersteld. De generieke categorieën hieronder zijn kandidaten, geen bevestigde inventaris.
- In de geverifieerde context staat geen toegangsroute of autorisatie geregistreerd. Dit zegt niets over feitelijke rechten in de organisatie.
- Deze aanvraag is alleen voor een voorstel/backlog. Geen toegang tot DNB- of bedrijfssystemen, verbinding, gegevensverzameling, toestemmingverlening of systeemwijziging is onderdeel van dit voorstel.
- **Write/update is uitgeschakeld.** Geen item in deze backlog vraagt om write/update. Ook later zijn write/update en iedere andere handeling die een systeem wijzigt alleen mogelijk na afzonderlijke, expliciete en afgebakende toestemming van een bevoegde eigenaar; dit voorstel geeft die toestemming niet. `Create-draft` wordt evenmin gevraagd of geactiveerd.

#### Gezamenlijk minimumprotocol voor bewijs en herkomst

Voor toekomstig, afzonderlijk geautoriseerd werk: leg alleen taak-ID en scope vast; de broncategorie en een minimale verwijzing naar het artefact (geen onnodige inhoud); eigenaar/bronhouder en vastgelegde autorisatiebasis; raadpleegmethode en afbakening; datum/tijd en relevante versie of vindplaats; gebruikte criteria; beperkingen, ontbrekende informatie en eventuele tegenstrijdigheden; en wie de bevinding heeft opgesteld en gecontroleerd. Verbind elke materiële conclusie aan die verwijzing en onderscheid feit, interpretatie, conclusie en aanbeveling. Vermeld niet-geraadpleegde onderdelen expliciet. Minimaliseer of redigeer vertrouwelijke en persoonsgegevens; verzamel of registreer geen inloggegevens, tokens of andere credentials. Dit protocol registreert herkomstmetadata, verzamelt zelf geen brondata en verleent geen toegang.

#### Per specialist

Alle bron- en systeemcategorieën zijn kandidaten die eerst door de bevoegde bronhouder moeten worden geïdentificeerd en goedgekeurd. De minimale rechten hieronder gelden alleen voor een later, afzonderlijk geautoriseerde taak; bestaand bezit van die rechten wordt niet verondersteld. Standaard werken de specialisten met context en artefacten die voor de taak zijn aangeleverd.

##### Lead & Intake Coordinator

- **Kennis:** duurzaam: intake, scope, prioritering, één accountable eigenaar, handoffs en escalatie volgens charter/routing/besluiten. Per taak ophalen: doel, acceptatiecriteria, uitsluitingen, eigenaar en expliciete autorisatie.
- **Documentbronnen:** verzoek, aangeleverde artefacten en toepasselijke teamafspraken. **Live systemen:** alleen een eventueel later door de organisatie aangewezen intake-/werkregistratiesysteem. **Best passende mogelijkheden:** lokale intake- en checklisttemplates; eventueel zoeken in expliciet goedgekeurde taakregistraties.
- **Minimumautorisatie:** geen voor aangeleverde informatie; voor later goedgekeurde zoekactie hoogstens search/read-only.
- **Capability request — Must.** **Waarom:** intake en autorisatiegrenzen consequent vastleggen. **Werk:** Ron verzoekt een bevoegde eigenaar een intake-/autorisatiechecklist en bronhouders/verantwoordelijkheden te identificeren en te beoordelen; geen bronnen raadplegen. **Minimumrechten:** geen. **Output:** goedgekeurde of als onbevestigd gemarkeerde checklist, eigenaar en open vragen. **Frequentie:** per nieuwe taak en bij scopewijziging. **Read-only mogelijk:** ja; deze stap vereist geen systeemtoegang. **Handwerk weg:** herhaald handmatig uitvragen van scope, eigenaar en grenzen. **Bewijs/audit:** taakverwijzing, checklistversie, datum en open punten. **Prioriteit:** Must.

##### Cloud Process Analyst

- **Kennis:** duurzaam: processtappen, rollen, overdrachten, afhankelijkheden en aannames onderscheiden; geen provider of proces veronderstellen. Per taak ophalen: aangeleverde procesbeschrijving, varianten en relevante criteria.
- **Documentbronnen:** kandidaatcategorieën zijn procesbeschrijvingen, procedures en architectuur-/procesdiagrammen. **Live systemen:** alleen een later bevestigde procesrepository of cloudprocesomgeving. **Best passende mogelijkheden:** document search en read-only weergave; eventueel gestructureerde query als de informatie daadwerkelijk gestructureerd is.
- **Minimumautorisatie:** geen voor aangeleverde artefacten; voor een goedgekeurde brontaak hoogstens search/read-only.
- **Capability request — Should.** **Waarom:** procesvarianten en overdrachten minder handmatig reconstrueren. **Werk:** na bronhouderbevestiging relevante procesartefacten zoeken en lezen. **Minimumrechten:** search/read-only, beperkt tot goedgekeurde scope. **Output:** procesoverzicht met verwijzingen, aannames en open vragen. **Frequentie:** per toegewezen procesanalyse. **Read-only mogelijk:** ja. **Handwerk weg:** handmatig zoeken en processtappen overtypen. **Bewijs/audit:** bronverwijzing, versie/vindplaats, raadpleegdatum en scope. **Prioriteit:** Should.

##### Service Delivery Analyst

- **Kennis:** duurzaam: deliveryflow, uitkomsten, handoffs, meetbehoeften en geen verzonnen prestatiecijfers. Per taak ophalen: expliciet beoogde uitkomst, servicegrens en toegestane meetdefinities.
- **Documentbronnen:** kandidaatcategorieën zijn servicebeschrijvingen, meetdefinities en deliveryrapportages. **Live systemen:** alleen een later bevestigde catalogus of meet-/rapportageomgeving. **Best passende mogelijkheden:** search voor documentatie en query voor goedgekeurde, afgebakende meetgegevens.
- **Minimumautorisatie:** geen voor aangeleverde informatie; voor goedgekeurde documentatie search/read-only, voor noodzakelijke gestructureerde meetgegevens hoogstens query met minimale scope.
- **Capability request — Should.** **Waarom:** expliciet gedefinieerde delivery-uitkomsten en meetwaarden efficiënt beoordelen. **Werk:** na bevestiging van bronhouder en meetdefinitie relevante informatie zoeken of een beperkte query uitvoeren. **Minimumrechten:** search/read-only; query alleen als de taak dit vereist en afzonderlijk is goedgekeurd. **Output:** deliveryanalyse, meetvragen, bronverwijzingen en beperkingen. **Frequentie:** per toegewezen deliveryanalyse. **Read-only mogelijk:** ja; query is uitsluitend voor lezen. **Handwerk weg:** handmatig verzamelen en vergelijken van toegestane metingen. **Bewijs/audit:** definities, queryscope, datum, bronverwijzingen en ontbrekende waarden. **Prioriteit:** Should.

##### Evidence & Audit Specialist

- **Kennis:** duurzaam: herkomst, relevantie, volledigheid, traceerbaarheid en scheiding tussen feit en interpretatie; geen audit- of complianceclaim zonder criteria en bewijs. Per taak ophalen: expliciete beoordelingscriteria en toegestane artefacten.
- **Documentbronnen:** kandidaatcategorieën zijn aangeleverde bewijsstukken, criteria en metadata van documenten/records. **Live systemen:** alleen een later bevestigde bewijs- of registratieruimte. **Best passende mogelijkheden:** read-only documentinspectie en search; metadata-query uitsluitend als nodig en toegestaan.
- **Minimumautorisatie:** geen voor aangeleverde artefacten; voor een later goedgekeurde bron hoogstens read-only/search, eventueel metadata-query. Geen wijziging van bewijsregistraties.
- **Capability request — Must.** **Waarom:** een gemeenschappelijke, controleerbare bewijs- en herkomststandaard vastleggen vóór toekomstig werk. **Werk:** Ron verzoekt de bevoegde governance-/broneigenaar dit voorstel voor het gezamenlijke minimumprotocol te beoordelen en bronverwijzingen/toegestane metadata te definiëren; geen bewijs verzamelen. **Minimumrechten:** geen. **Output:** beoordeeld protocol en lijst van open criteria/goedkeuringen. **Frequentie:** eenmalig voor de basis; herzien bij formele scope- of beleidswijziging. **Read-only mogelijk:** ja; geen bronraadpleging vereist. **Handwerk weg:** ad-hoc herhaald bepalen hoe bevindingen worden onderbouwd. **Bewijs/audit:** versie, beoordelaar, datum en expliciete open punten; geen broninhoud of credentials. **Prioriteit:** Must.

##### Technical Operations Challenger

- **Kennis:** duurzaam: aannames, afhankelijkheden, foutscenario’s, herstelbaarheid en verificatievragen; hypotheses blijven onderscheiden van feiten. Per taak ophalen: concreet voorstel en geverifieerde operationele randvoorwaarden.
- **Documentbronnen:** kandidaatcategorieën zijn aangeleverde architectuurinformatie, runbooks en herstel-/afhankelijkheidsbeschrijvingen. **Live systemen:** alleen een later bevestigde operationele of configuratie-informatiebron. **Best passende mogelijkheden:** search en read-only documentatie; geen configuratiewijziging of uitvoering.
- **Minimumautorisatie:** geen voor aangeleverde informatie; voor een goedgekeurde beoordeling hoogstens search/read-only.
- **Capability request — Should.** **Waarom:** operationele aannames toetsen aan gecontroleerde documentatie in plaats van onbevestigde aannames. **Werk:** na bevestiging van bronhouder relevante, goedgekeurde runbook-/architectuurartefacten lezen en scenario’s toetsen. **Minimumrechten:** search/read-only. **Output:** compacte challenge met aanname, scenario, verwijzing en verificatievraag. **Frequentie:** alleen wanneer een toegewezen taak operationele risico’s omvat. **Read-only mogelijk:** ja. **Handwerk weg:** handmatig opvragen en doorzoeken van toegestane operationele documentatie. **Bewijs/audit:** artefactversie/vindplaats, datum, scope en onderscheid feit/hypothese. **Prioriteit:** Should.

##### Data & Automation Engineer

- **Kennis:** duurzaam: eisen, data-inputs/transformaties/outputs, foutafhandeling, privacy en herhaalbaarheid; geen taal, platform of databron veronderstellen. Per taak ophalen: data-eigenaarschap, doelomgeving, acceptatiecriteria, toegestane inputs en terugdraairandvoorwaarden.
- **Documentbronnen:** kandidaatcategorieën zijn aangeleverde schema’s, datadefinities en automatiseringseisen. **Live systemen:** alleen een later expliciet bevestigde, toegestane data- of testomgeving. **Best passende mogelijkheden:** read-only schema-/metadata-inspectie en begrensde query; testen met lokaal aangeleverde of expliciet goedgekeurde niet-productie-invoer.
- **Minimumautorisatie:** geen voor ontwerp op basis van aangeleverde informatie; voor later goedgekeurde schema-inspectie hoogstens read-only/search; query alleen bij aantoonbare noodzaak en afzonderlijke autorisatie. Geen productie- of systeemwijzigingen.
- **Capability request — Could.** **Waarom:** data- en automatiseringsontwerpen op echte, goedgekeurde schema’s toetsen zonder onnodige dataverzameling. **Werk:** pas na afzonderlijke taakgoedkeuring beperkte schema-/metadata-inspectie of een minimale query in een bevestigde testcontext. **Minimumrechten:** read-only; query uitsluitend indien noodzakelijk en expliciet goedgekeurd. **Output:** ontwerp-/validatienotitie, beperkingen en testresultaat zonder onnodige data. **Frequentie:** per expliciet toegewezen data-/automatiseringstaak. **Read-only mogelijk:** voor ontwerp en schema-inspectie ja; voor query is afzonderlijke leesautorisatie vereist. **Handwerk weg:** handmatig schema’s opvragen en compatibiliteit nalopen. **Bewijs/audit:** scope, autorisatiebasis, schema-/versieverwijzing en testcriteria; geen credentials of onnodige persoonsgegevens. **Prioriteit:** Could.

##### Quality Reviewer & Scribe

- **Kennis:** duurzaam: onafhankelijke toetsing aan opdracht, criteria, volledigheid, bewijs en overdracht; onderscheid met de ingebouwde Squad Scribe. Per taak ophalen: versie van deliverable, acceptatiecriteria en beoordelingsscope.
- **Documentbronnen:** taakbeschrijving, aangeleverde deliverable, expliciete criteria en relevante toegestane besluiten. **Live systemen:** geen nodig voor de basisreview; eventueel alleen een later aangewezen taakregistratie voor verwijzingen. **Best passende mogelijkheden:** lokale checklist en versie-/documentvergelijking; search alleen bij expliciete goedkeuring.
- **Minimumautorisatie:** geen voor aangeleverde deliverable en criteria; eventueel read-only/search bij afzonderlijk goedgekeurde verwijzingen.
- **Capability request — Must.** **Waarom:** reviewbeperkingen, criteria en herstelvoorwaarden consequent zichtbaar maken. **Werk:** Ron verzoekt de verantwoordelijke teamgovernance de checklistvorm te beoordelen; reviews worden alleen uitgevoerd op aangeleverde stukken en criteria. **Minimumrechten:** geen. **Output:** compacte review met verdict, bevindingen, onderbouwing en niet-beoordeelde onderdelen. **Frequentie:** per expliciet gevraagde review; niet automatisch. **Read-only mogelijk:** ja. **Handwerk weg:** terugkerend handmatig opstellen van reviewstructuur en overdrachtsnotities. **Bewijs/audit:** deliverable-/criteriaversie, reviewdatum, reviewer en afgebakende bevindingen. **Prioriteit:** Must.

#### Gedeelde backlog en volgorde

**Must — eerst uitsluitend organiseren/beoordelen**
1. Laat Ron bevoegde eigenaren vragen de intake-/autorisatiechecklist en de vereiste autorisatiegrenzen te beoordelen en bronhouders/verantwoordelijkheden te identificeren.
2. Laat Ron bevoegde governance-/broneigenaren het gezamenlijke minimumprotocol voor bewijs en herkomst beoordelen.
3. Laat Ron de beperkte Quality Review-checklistvorm laten beoordelen.

Deze Must-items zijn procedurele beoordeling en inventarisatie van eigenaarschap; ze autoriseren geen broninventarisatie door het DIT-team, bronraadpleging, dataverzameling, verbinding of wijziging. Ron wordt gevraagd **eerst alleen deze Must-items te organiseren/beoordelen**. Geen uitvoering van Should- of Could-items in deze eerste stap.

**Should — pas na aparte scope- en bronhouderbevestiging:** begrensde document search/read-only voor procesartefacten en operationele documentatie; service-informatie alleen met vastgelegde meetdefinities en, indien nodig, afzonderlijk goedgekeurde query.

**Could — pas na aparte taakgoedkeuring en toetsing van noodzaak:** begrensde schema-inspectie of query voor een expliciete data-/automatiseringstaak, bij voorkeur in een bevestigde testcontext.

Alle rechten zijn voorstelmatige minima, geen toekenning. Voor elke toekomstige taak zijn afzonderlijke scope, bevoegde goedkeuring en bronhouderbevestiging nodig. Write/update blijft uitgeschakeld, ook voor toekomstige taken, tenzij daarvoor later afzonderlijke, expliciete en afgebakende toestemming is verleend.

## Agreement Register — AGR

Dit register is de centrale index van DIT-teamafspraken. Alle Squad-members lezen dit register via de gedeelde beslissingen bij taakstart en verwijzen waar relevant naar het AGR-nummer. De registerbeheerder kent nummers toe; een nummer is permanent en wordt nooit hergebruikt. Een aanscherping die de kern behoudt, houdt hetzelfde nummer en krijgt een append-only wijzigingsnotitie. Een fundamenteel nieuwe afspraak krijgt een nieuw nummer; de oude afspraak blijft staan met status `Superseded by AGR-xxx`. Gebruik alleen de statussen `Proposed`, `Active`, `Superseded`, `Deprecated` of `Exception`. Wijzig of verwijder historische registraties niet; correcties en statusovergangen worden als nieuwe, gedateerde notities toegevoegd. Capability-items zijn geen AGR-afspraken, tenzij zij expliciet als voorstel voor teambeleid zijn geregistreerd.

De volgende DIT-teamafspraken zijn retrospectief geregistreerd op 2026-11-03. De datum per afspraak is de oorspronkelijke datum van de afspraak; de bronteksten zelf zijn niet gewijzigd. De inventaris omvat de DIT-teamafspraken uit de goedgekeurde teaminrichting, routing, charters en Prompt 1. Squad-frameworkregels blijven onder hun bestaande hogere governance vallen. Het Prompt 2-capabilityvoorstel is afzonderlijk als `Proposed` opgenomen, niet als goedgekeurd beleid.

### AGR-001 — Zeven DIT-specialisten
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Het DIT-team bestaat uit exact zeven goedgekeurde specialistrollen: Lead & Intake Coordinator, Cloud Process Analyst, Service Delivery Analyst, Evidence & Audit Specialist, Technical Operations Challenger, Data & Automation Engineer en Quality Reviewer & Scribe.
- **Reden/achtergrond:** De afgesproken dekking van DIT Operations.
- **Bron:** Goedgekeurde teaminrichting in `.squad/decisions.md`; `.squad/team.md`.
- **Relaties:** AGR-002, AGR-016–AGR-022.

### AGR-002 — Squad-supportrollen zijn geen DIT-specialisten
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Scribe, Ralph, Rai en Fact Checker zijn framework-supportidentiteiten, geen extra DIT-rollen of gewone domein-routingsbestemmingen. De DIT-rol Quality Reviewer & Scribe blijft onderscheiden van de ingebouwde Scribe.
- **Reden/achtergrond:** Voorkom rolverwarring en behoud de afgesproken teamomvang.
- **Bron:** Goedgekeurde teaminrichting in `.squad/decisions.md`; `.squad/team.md`; `.squad/routing.md`.
- **Relaties:** AGR-001, AGR-022.

### AGR-003 — Eén accountable eigenaar en begrensde samenwerking
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Wijs per werkitem precies één accountable specialist aan op basis van het primaire gevraagde resultaat. Andere bijdragen zijn concreet begrensd; geen speculatieve fan-out of stille scope-uitbreiding.
- **Reden/achtergrond:** Heldere verantwoordelijkheid, handoffs en kwaliteitsbewaking.
- **Bron:** Goedgekeurde teaminrichting in `.squad/decisions.md`; `.squad/routing.md`.
- **Relaties:** AGR-004, AGR-014, AGR-015.

### AGR-004 — Specialistische routing
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Route intake en coördinatie naar Lead; procesanalyse naar Cloud Process Analyst; servic delivery-analyse naar Service Delivery Analyst; evidencevragen naar Evidence & Audit Specialist; operationele challenge naar Technical Operations Challenger; expliciet goedgekeurde data-/automatiseringstaken naar Data & Automation Engineer; onafhankelijke review naar Quality Reviewer & Scribe.
- **Reden/achtergrond:** Opdrachten naar de afgesproken expertise en grenzen routeren.
- **Bron:** `.squad/routing.md`.
- **Relaties:** AGR-001–AGR-003, AGR-016–AGR-022.

### AGR-005 — Scope van de eerste inrichtingsfase
- **Status:** Deprecated
- **Datum:** 2026-11-02
- **Afspraak:** De eerste fase betrof alleen teamsamenstelling, verantwoordelijkheden, samenwerking en routing; toen werden geen kennisbronnen of tools geïnventariseerd en geen bedrijfssystemen gewijzigd.
- **Reden/achtergrond:** Dit was een tijdelijke scopegrens voor de teaminrichting en die fase is afgerond.
- **Bron:** Goedgekeurde teaminrichting in `.squad/decisions.md`; oorspronkelijke teamopdracht.
- **Relaties:** AGR-023–AGR-025. Deze historische scopegrens wordt niet als actuele beperking op een later expliciet goedgekeurde fase toegepast.

### AGR-006 — Geen verzonnen feiten; onzekerheid expliciet maken
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Verzin geen ontbrekende informatie. Maak waar relevant onderscheid tussen feit, interpretatie, aanname, risico en aanbeveling en benoem ontbrekende, verouderde of tegenstrijdige informatie.
- **Reden/achtergrond:** Betrouwbare, toetsbare analyses zonder onbewezen claims.
- **Bron:** Oorspronkelijke teamopdracht; specialistcharters; feiten- en scopegrenzen in `.squad/decisions.md`.
- **Relaties:** AGR-007, AGR-012, AGR-025.

### AGR-007 — Betrouwbare en herleidbare bronnen
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Gebruik waar beschikbaar betrouwbare, gezaghebbende en actuele bronnen; vermeld bronnen bij belangrijke conclusies en benoem bronbeperkingen.
- **Reden/achtergrond:** Onafhankelijke controle en onderbouwde conclusies.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/evidence-audit-specialist/charter.md`.
- **Relaties:** AGR-006, AGR-012, AGR-025.

### AGR-008 — Operationele werkelijkheid en reproduceerbare analyse
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Vergelijk managementinformatie waar mogelijk met relevante operationele brondata en geef de voorkeur aan reproduceerbare queries/automatisering boven herhaald handwerk, binnen de goedgekeurde scope en rechten.
- **Reden/achtergrond:** KPI's en conclusies toetsen aan de onderliggende werkelijkheid en handwerk verminderen.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/technical-operations-challenger/charter.md`; `.squad/agents/data-automation-engineer/charter.md`.
- **Relaties:** AGR-007, AGR-010–AGR-012, AGR-025.

### AGR-009 — Taal, stijl en vertrouwelijkheid
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Werk standaard in het Nederlands, behoud gangbare Engelse vaktermen en communiceer kort en zakelijk. Behandel DNB-informatie als vertrouwelijk.
- **Reden/achtergrond:** Aansluiting op de gebruiker en passende omgang met bedrijfsinformatie.
- **Bron:** Oorspronkelijke teamopdracht.
- **Relaties:** AGR-006, AGR-010–AGR-012.

### AGR-010 — Capability-gaps expliciet maken
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Wanneer een taak niet zelfstandig kan worden uitgevoerd door ontbrekende kennis, toegang, tooling of koppeling, benoem concreet wat nodig is, waarom, met welke minimale rechten en welke werkzaamheden daardoor mogelijk worden. Behandel herhaald menselijk zoek-, kopieer-, combineer- of controlewerk als kandidaat voor verbetering.
- **Reden/achtergrond:** Het team stapsgewijs zelfstandiger en minder afhankelijk van handmatige aanlevering maken.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/data-automation-engineer/charter.md`.
- **Relaties:** AGR-008, AGR-011, AGR-023.

### AGR-011 — Least privilege en geen ongemachtigde mutaties
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Least privilege geldt; read-only is de standaard. Geen Squad-member voert zelfstandig mutaties uit in productie of bedrijfssystemen. Write/update vereist afzonderlijke expliciete toestemming van een bevoegde eigenaar, met afgebakende scope.
- **Reden/achtergrond:** Onbedoelde wijzigingen voorkomen en toegangsrisico beperken.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/decisions.md` (capabilityvoorstel, als aanvullende expliciete begrenzing).
- **Relaties:** AGR-008–AGR-010, AGR-023–AGR-025.

### AGR-012 — Evidence moet controleerbaar zijn
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Materiële evidence is volledig, actueel, reproduceerbaar en herleidbaar naar de oorspronkelijke bron, geschikt voor onafhankelijke beoordeling en ondersteunt de conclusie die erop steunt.
- **Reden/achtergrond:** Controleerbaarheid en auditability van conclusies.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/evidence-audit-specialist/charter.md`.
- **Relaties:** AGR-006–AGR-008, AGR-025.

### AGR-013 — Standaard samenwerkingsworkflow
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Lead analyseert de opdracht en criteria, decomponeert en routeert werk; specialisten leveren begrensde bijdragen; ontbrekende capabilities worden gemeld; Quality Reviewer controleert waar passend; Lead levert een geïntegreerd resultaat; structurele leerpunten worden vastgelegd.
- **Reden/achtergrond:** Een samenhangend resultaat met expliciet eigenaarschap en kwaliteitscontrole.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/routing.md`; specialistcharters.
- **Relaties:** AGR-003, AGR-004, AGR-010, AGR-014.

### AGR-014 — Standaard rapportagevelden waar relevant
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Rapporteer waar relevant doel, scope, bronnen, feiten, analyse, ontbrekende informatie, risico's, afhankelijkheden, acties/eigenaar/prioriteit/gewenste datum, evidence, reviewstatus en ontbrekende capabilities.
- **Reden/achtergrond:** Compleet en bruikbaar resultaat met zichtbare open punten en opvolging.
- **Bron:** Oorspronkelijke teamopdracht.
- **Relaties:** AGR-003, AGR-007, AGR-012–AGR-013.

### AGR-015 — Rolcharter: Lead & Intake Coordinator
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Lead beheert intake, triage, decompositie, prioritering, routing, voortgang en integrale samenhang; maakt doel, criteria en scope expliciet en wijzigt die niet stilzwijgend.
- **Reden/achtergrond:** Eén heldere intake- en coördinatiefunctie.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/lead-intake-coordinator/charter.md`.
- **Relaties:** AGR-003, AGR-004, AGR-013–AGR-014.

### AGR-016 — Rolcharter: Cloud Process Analyst
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Cloud Process Analyst analyseert cloud governance- en toetsingsprocessen, waaronder processtappen, rollen, afhankelijkheden, status, KPI's en verbetering binnen verstrekte context; veronderstelt geen provider, proces of norm.
- **Reden/achtergrond:** Procesanalyse voor Cloudtoetsing en Eindtoetsing zonder onbevestigde context in te vullen.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/cloud-process-analyst/charter.md`.
- **Relaties:** AGR-004, AGR-006–AGR-007.

### AGR-017 — Rolcharter: Service Delivery Analyst
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Service Delivery Analyst analyseert service delivery, service-uitkomsten, overdrachten, meetbehoeften en verbeterkansen binnen verstrekte context; verzint geen KPI's of actuele operationele waarden.
- **Reden/achtergrond:** Servicemanagementanalyse zonder ongefundeerde prestatieclaims.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/service-delivery-analyst/charter.md`.
- **Relaties:** AGR-004, AGR-006–AGR-008.

### AGR-018 — Rolcharter: Evidence & Audit Specialist
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Evidence & Audit Specialist beoordeelt evidencekwaliteit, volledigheid, herkomst en traceerbaarheid; onderscheidt feiten en conclusies en claimt geen auditresultaat, certificering of compliance zonder criteria en voldoende bewijs.
- **Reden/achtergrond:** Controleerbare conclusies zonder onbewezen assuranceclaims.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/evidence-audit-specialist/charter.md`.
- **Relaties:** AGR-006–AGR-007, AGR-012.

### AGR-019 — Rolcharter: Technical Operations Challenger
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Technical Operations Challenger toetst operationele aannames, afhankelijkheden, foutscenario's, uitvoerbaarheid en risico's; adviseert en daagt uit maar wijzigt geen bedrijfssystemen.
- **Reden/achtergrond:** Technische onderbouwing van managementinformatie en operationele risico's.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/technical-operations-challenger/charter.md`.
- **Relaties:** AGR-008, AGR-011–AGR-012.

### AGR-020 — Rolcharter: Data & Automation Engineer
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** De Data & Automation Engineer ontwerpt of implementeert data- en automatiseringsoplossingen alleen binnen expliciet goedgekeurde grenzen; technologie, data en systemen worden niet verondersteld en toegang wordt geminimaliseerd.
- **Reden/achtergrond:** Reproduceerbare automatisering binnen geautoriseerde scope.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/data-automation-engineer/charter.md`.
- **Relaties:** AGR-008, AGR-010–AGR-011.

### AGR-021 — Rolcharter: Quality Reviewer & Scribe
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Quality Reviewer & Scribe voert onafhankelijke, afgebakende kwaliteitsreview uit tegen de opdracht en criteria; implementeert eigen bevindingen niet en neemt geen besluitbeheer over van de ingebouwde Scribe.
- **Reden/achtergrond:** Onafhankelijke controle en duidelijke scheiding van DIT-review en framework-besluitcuratie.
- **Bron:** Oorspronkelijke teamopdracht; `.squad/agents/quality-reviewer-scribe/charter.md`; `.squad/agents/scribe/charter.md`.
- **Relaties:** AGR-002, AGR-003, AGR-013–AGR-014.

### AGR-022 — Besluit- en leerbeheer
- **Status:** Active
- **Datum:** 2026-11-02
- **Afspraak:** Team-brede architectuur- en procesafspraken worden centraal in het beslissingenregister vastgelegd; geschiedenis blijft gericht op werk en leerpunten. In de bestaande governance is consensus vereist voor betekenisvolle teamwijzigingen.
- **Reden/achtergrond:** Eén navolgbare bron voor teamrichting en een bruikbaar leergeheugen.
- **Bron:** `Governance` in `.squad/decisions.md`; coordinator-workflow in `.github/agents/squad.agent.md`.
- **Relaties:** AGR-001, AGR-023–AGR-026.

### AGR-023 — Capability backlog DIT-team (voorstel)
- **Status:** Proposed
- **Datum:** 2026-11-02
- **Afspraak:** Beoordeel per specialist de benodigde kennis, documentbronnen, live systemen, tools, minimale autorisatie en autonomie-gaps; prioriteer Must/Should/Could en behandel onbekende systemen/toegang als onbevestigd. Dit blijft een voorstel/backlog en verleent geen toegang of toestemming.
- **Reden/achtergrond:** De zelfstandigheid van het team gecontroleerd vergroten.
- **Bron:** Voorstel “Capability backlog DIT-team (pending/unapproved)” in `.squad/decisions.md`; Prompt 2.
- **Relaties:** AGR-005, AGR-010–AGR-011, AGR-024–AGR-025.

### AGR-024 — Evidence- en provenanceprotocol (voorstel)
- **Status:** Proposed
- **Datum:** 2026-11-02
- **Afspraak:** Het voorgestelde protocol vraagt later, bij afzonderlijk geautoriseerd werk, om minimale herkomstmetadata, verwijzing naar bronartefact, methode/scope, datum/versie, criteria, beperkingen en opsteller/reviewer; minimaliseer gevoelige gegevens en leg geen credentials vast. Niet actief totdat het voorstel is goedgekeurd.
- **Reden/achtergrond:** Een conclusie achteraf reproduceerbaar en controleerbaar maken.
- **Bron:** “Gezamenlijk minimumprotocol voor bewijs en herkomst” in het capabilityvoorstel in `.squad/decisions.md`; Prompt 2.
- **Relaties:** AGR-007, AGR-011–AGR-012, AGR-023.

### AGR-025 — Onveranderlijke AGR-nummering en wijzigingsbeheer
- **Status:** Active
- **Datum:** 2026-11-03
- **Afspraak:** Ken elke nieuwe teamafspraak één uniek `AGR-001`, `AGR-002`, … nummer toe; hergebruik of wijzig een nummer nooit. Registreer minimaal nummer, titel, status, datum, afspraak, reden/achtergrond, bron en relaties. Een verduidelijking behoudt het nummer en krijgt een wijzigingsnotitie. Een fundamenteel nieuwe vervangende afspraak krijgt een nieuw nummer; markeer de oude `Superseded by AGR-xxx`. Houd registraties append-only bij en verwijs waar nuttig expliciet naar AGR-nummers.
- **Reden/achtergrond:** Teamafspraken blijvend vindbaar, eenduidig en herleidbaar houden.
- **Bron:** Expliciete gebruikersopdracht, 2026-11-03.
- **Relaties:** Van toepassing op alle AGR-registraties; sluit aan op AGR-022.
- **Wijzigingshistorie:** 2026-11-03 — initiële systematiek vastgesteld en bestaande DIT-teamafspraken retrospectief genummerd.

### AGR-026 — Capability-voorstellen verlenen geen toegang
- **Status:** Proposed
- **Datum:** 2026-11-02
- **Afspraak:** Een capability-backlogitem, bronvermelding of toolvoorstel verleent op zichzelf geen toegang, autorisatie, verbinding, toestemming tot gegevensverzameling of toestemming tot systeemwijziging. Vereis eerst bevestiging van bronhouder, taakscope en bevoegde toestemming.
- **Reden/achtergrond:** Voorkom dat een voorstel of technische mogelijkheid wordt opgevat als autorisatie.
- **Bron:** Prompt 2 en het pending/unapproved capabilityvoorstel in `.squad/decisions.md`.
- **Relaties:** AGR-011, AGR-023–AGR-025.

### Registercorrectie — 2026-11-03
- In AGR-004 staat een typefout: “servic delivery-analyse” moet worden gelezen als “service delivery-analyse”. De bestaande brontekst is niet aangepast; deze notitie corrigeert uitsluitend de lezing van die term en verandert de afspraak niet.

### AGR-027 — Microsoft Search en Microsoft Graph als centrale Enterprise Knowledge capability
- **Status:** Active
- **Datum:** 2026-11-03
- **Afspraak:** Microsoft Search en Microsoft Graph vormen de centrale Enterprise Knowledge capability. Alle Squad-members mogen deze gebruiken wanneer relevant voor hun werkzaamheden, via delegated access onder de identiteit van Ron en uitsluitend binnen de feitelijke rechten van Ron. Voor Microsoft 365 en andere enterprise-bronnen geldt strikt read-only: zoeken, documenten en metadata lezen, bronlocaties identificeren, bronnen vergelijken en informatie analyseren zijn toegestaan; documenten, lijsten, wiki's of permissions wijzigen, uploaden, verwijderen of anderszins muteren is niet toegestaan. Agents mogen nieuwe Markdown-output schrijven binnen de lokale Squad-workspace; dit staat los van enterprise-bronmutaties.
- **Bronselectie en retrieval:** Search en Retrieval zijn afzonderlijke stappen. Zoek eerst, selecteer relevante bronnen en haal daarna alleen de benodigde inhoud op. Weeg gevonden informatie volgens de Source Registry en canonical source hierarchy; verzin geen authority level als de registry of hiërarchie niet beschikbaar is.
- **Evidence/provenance:** Registreer voor research-, analyse- en evidence-output waar mogelijk Source ID, bronsysteem, titel, canonical URL, retrieval-datum/-tijd, last-modified-informatie indien beschikbaar, relevant object-ID, oorspronkelijke zoekvraag/query, versie of commit indien van toepassing, en authority level uit de Source Registry.
- **Capability gap:** Als technische toegang tot een benodigde bron ontbreekt, meldt de agent dit expliciet aan Ron en registreert de ontbrekende capability als gap. Deze afspraak verleent geen technische toegang of rechten die Ron zelf niet heeft en staat geen enterprise-write toe.
- **Reden/achtergrond:** Enterprise-kennis gecontroleerd, breed en traceerbaar beschikbaar maken voor Squad, met least privilege en zonder mutaties in bedrijfssystemen.
- **Bron:** Expliciete gebruikersopdracht, 2026-11-03.
- **Relaties:** AGR-007, AGR-010–AGR-012, AGR-023–AGR-026.
- **Wijzigingshistorie:** 2026-11-03 — initiële afspraak geregistreerd als AGR-027.

### AGR-028 — Verplichte registratie van capability gaps
- **Status:** Active
- **Datum:** 2026-11-03
- **Afspraak:** Wanneer een Squad-member tijdens een opdracht vaststelt dat noodzakelijke kennis, een bron, systeemtoegang, autorisatie, API, MCP-server, tool, skill of andere capability ontbreekt, registreert de coordinator automatisch een nieuw, uniek en nooit hergebruikt `GAP-001`, `GAP-002`, … record in de centrale capability-gap administratie. Vermeld minimaal GAP-nummer, titel, datum, ontdekkend Squad-member, getroffen taak, ontbrekende capability, impact, gewenste oplossing, minimale rechten, prioriteit (`Must`/`Should`/`Could`), status (`Open`/`In Progress`/`Blocked`/`Resolved`), concrete actie voor Ron en relevante AGR-, CAP- en SRC-relaties. Meld expliciet aan Ron: “Ik heb GAP-xxx geregistreerd. Om dit op te lossen heb ik van jou nodig: …”. Een gap blijft open totdat de benodigde capability functioneel is getest; alleen daarna mag deze `Resolved` worden. Houd de administratie append-only; statuswijzigingen en correcties worden als gedateerde notities toegevoegd, niet door historische gegevens te overschrijven.
- **Reden/achtergrond:** Voorkomen dat terugkerende blokkades of ontbrekende capabilities alleen in een eenmalige uitvoer worden genoemd en vervolgens niet worden opgevolgd.
- **Bron:** Expliciete gebruikersopdracht, 2026-11-03.
- **Relaties:** AGR-010, AGR-025, AGR-027.
- **Wijzigingshistorie:** 2026-11-03 — initiële regel voor automatische GAP-registratie vastgesteld.

## Capability Gap Register — GAP

### GAP-001 — Microsoft Search / Microsoft Graph-toegang voor Enterprise Knowledge ontbreekt
- **Datum:** 2026-11-03
- **Ontdekkend Squad-member:** Lead & Intake Coordinator (coordinator voor de Cloud-toetsingsproces-researchopdracht)
- **Getroffen taak:** Vaststellen welke procesexperts betrokken zijn bij het Cloud-toetsingsproces, met aantoonbare naam, afdeling, expertise/rol, bronnen en tegenstrijdigheden.
- **Ontbrekende capability:** Functioneel beschikbare Microsoft Search- en Microsoft Graph delegated read-only toegang in de Squad/Copilot-sessie, inclusief de mogelijkheid om relevante bronmetadata te vinden en op te halen. Beschikbaarheid van de Source Registry/canonical source hierarchy is eveneens niet bevestigd.
- **Impact:** De zoekfase en retrieval konden niet worden uitgevoerd. Daardoor konden geen betrokken personen, afdelingen of rollen met enterprise-evidence worden vastgesteld; bronvergelijking en provenancecontrole waren niet mogelijk.
- **Gewenste oplossing:** Configureer en verifieer de goedgekeurde Enterprise Knowledge-integratie volgens AGR-027, zodat Search afzonderlijk kan worden uitgevoerd, relevante resultaten kunnen worden geselecteerd en alleen daarna benodigde inhoud en metadata read-only kunnen worden opgehaald. Maak de Source Registry/canonical source hierarchy alleen read-only beschikbaar indien die bestaat en binnen Ron's rechten valt.
- **Minimaal benodigde rechten:** Delegated access onder Ron's identiteit, beperkt tot Ron's bestaande feitelijke autorisaties; read-only search/query, documentinhoud en metadata lezen. Geen enterprise write/update, upload, delete, permission change of andere mutatie.
- **Prioriteit:** Must
- **Status:** Open
- **Wat Ron concreet moet regelen:** Laat de bevoegde beheerder de Microsoft Search/Graph-integratie voor de Squad/Copilot-sessie beschikbaar en bereikbaar maken met uitsluitend Ron's gedelegeerde read-only rechten voor relevante Cloud-toetsingsbronnen. Bevestig ook of de Source Registry/canonical source hierarchy bestaat en read-only beschikbaar is; geen aanvullende rechten boven Ron's eigen autorisatie.
- **Functionele resolutiecheck:** Voer pas na beschikbaarstelling een read-only test uit: (1) zoek de afgesproken Cloud-toetsingsvraag; (2) selecteer een relevante bron; (3) haal alleen de benodigde inhoud en metadata op; (4) registreer provenancevelden conform AGR-027; (5) verifieer dat geen mutatiepad wordt gebruikt. Markeer pas daarna als `Resolved`.
- **Relaties:** AGR-010, AGR-011, AGR-025, AGR-027, AGR-028. CAP- en SRC-nummers: geen toegekend of bevestigd.
- **Bron/evidence:** `output/2026_11_03/cloud-toetsingsproces-procesexperts.md` — vermeldt dat Microsoft Search/Graph niet beschikbaar was in die sessie en dat daarom geen enterprise-bronnen zijn geraadpleegd.

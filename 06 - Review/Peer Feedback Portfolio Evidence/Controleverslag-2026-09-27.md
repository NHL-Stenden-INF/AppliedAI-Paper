# Controle van de aangeleverde paper en reviewverwerking

De feedback is grotendeels zichtbaar verwerkt, maar de aangeleverde paper is nog niet vrij van inhoudelijke en opmaakproblemen. De eerdere GitHub-status dat de eindcontrole volledig geslaagd was, geldt voor een ander bestand en mag niet voor deze versie worden gebruikt. Dit verslag bevat een controle van de huidige inhoud, geen docentbeoordeling.

## Gecontroleerde versie en werkwijze

Controle op 27 september 2026 van `Deepfake paper - Dave & Lucas - Review verwerkt.docx`, SHA-256 `cd00d692921bdee9fd95afe44893f9e4ffbbd21030afe0269cfc87b48f0f3c6b`. Het ongewijzigde bestand staat in [Evidence/paper-review-verwerkt.docx](Evidence/paper-review-verwerkt.docx). De twee ontvangen reviews zijn volledig gelezen, inclusief de afbeeldingen met handschrift en tekst in Marts PDF. De paper is tekstueel, technisch en via een render van 21 pagina’s gecontroleerd. De paginaverwijzingen hieronder verwijzen naar die render; hoofdstukken en tekstankers blijven bruikbaar bij andere paginering.

De controle omvat spelling, grammatica, logica, aansluiting op beide reviews, formele rubricvoorwaarden en de portfolioverplichting. Een gerichte broncontrole is uitgevoerd voor AUC, de recente multimodale overzichtsstudie, praktijkbenchmarks, watermerken, AASIST en juridische context. Er is geen nieuw detectoronderzoek uitgevoerd en niet elke bron, DOI of oorspronkelijke numerieke tabel is integraal opnieuw geverifieerd. Zoekresultaataantallen zijn niet opnieuw uitgevoerd of bevestigd.

Repository bij aanvang: `main` op `bc99dbd66a9cfb9acb3a363290951878b5a3c864`; feedbackbranch op `7d0c283cce2fbf5592d21f4371ba93702124cd87`. PR #2 bevatte al een reviewregistratie. Deze registratie is geactualiseerd in dezelfde branch. PR #1 bevat een afzonderlijke historische conceptversie en is niet als identieke voorversie behandeld. Tijdens de controle verschenen zes verdere commits tot `8d66fd270a1726bef7a50f62432a015e28d5ff69`, met aanvullende zoeknotities en een andere DOCX-hash (`41a1d336…`). Die wijzigingen zijn gelezen en behouden; de huidige audit bouwt op die nieuwere commit voort. Het daarin genoemde bestand is niet aangeleverd.

## Wat goed is verwerkt

De paper bevat nu korte oriëntaties bij hoofdstuk 2 en 4, een expliciet onderzoeksdoel in de tweede alinea van de inleiding, samenvattingen onder 3.1.4, 3.2.6 en 3.3.7 en een letterlijk herhaalde hoofdvraag in 4.2. De keuze voor literatuuronderzoek wordt onderbouwd vanuit de drie deelvragen en de beperkte waarde van één eigen detectorexperiment voor een brede generalisatievraag. AUC, ROC, accuracy en EER worden in hoofdstuk 2 afzonderlijk uitgelegd. Alle niet-lege tekstruns in de vier tabellen hebben expliciet een tekstgrootte van 9 pt; het door Mart genoemde verschil in tekstgrootte is in deze versie niet aangetroffen.

De sterke punten uit de reviews blijven herkenbaar: een logische volgorde langs de deelvragen, cijfers met testcontext, eigen vergelijking van literatuur, aanbevelingen en ondersteunende tabellen en figuren. De paper vermeldt expliciet dat geen eigen detector is gebouwd of getest. Verschillende meetmaten worden niet als dezelfde maat gepresenteerd.

## Belangrijke correctie op de eerdere registratie

Mart Velema’s PDF bevat op p. 6 een afbeelding met algemene opmerkingen, drie sterke punten, twee verbeterpunten en een positieve conclusie. De eerdere omschrijving dat het formulier geen schriftelijke motivatie bevatte, was onjuist. De twee expliciete verbeterpunten zijn AUC/ROC uitleg en inconsistente tekstgrootte in tabellen. De relatief minder sterke rubricmarkering bij B3 methodologische onderbouwing is een afzonderlijke interpretatie van p. 5, geen letterlijk geschreven derde verbeterpunt.

Het formulier van Mart heet *Working Paper*. Het aangeleverde Appendix 9 heet *Research Paper* en is voor de formele controle gebruikt. Marts formulier blijft geldig bewijs van ontvangen feedback; zijn positieve oordeel is geen formele voldoende van de docent.

## Openstaande verbeterpunten

De onderstaande correcties zijn voorstellen en bevindingen. Ze zijn niet stilzwijgend in de aangeleverde DOCX doorgevoerd. Sluiten kan pas na een nieuwe versie met controlebewijs.

| ID | Prioriteit | Vindplaats | Bevinding en vereiste vervolgstap |
| --- | --- | --- | --- |
| QA01 | Hoog | H2 Dataverzameling, tabel 1, p. 6–7; 4.4, p. 19 | Zes zoekopdrachten, databases en aantallen zijn aanwezig, maar zoekdatums, exports/screenshots, ontdubbeling en aantallen met uitsluitredenen ontbreken. De oude registratie zei juist dat historische aantallen niet beschikbaar waren. Leg vast of dit oorspronkelijke zoekacties of latere herhaalzoekacties zijn, met uitvoerder, datum, filters en bewijs. Maak een nieuwe zoekactie nooit met terugwerkende kracht onderdeel van de oorspronkelijke selectie. Als het bewijs ontbreekt, benoem de beperking in H2 én 4.4. |
| QA02 | Hoog | Samenvatting p. 2 en H2 Meetmaten p. 7 | AUC wordt onjuist begrensd op 0,5–1,0. Het bereik is 0–1; 0,5 duidt op willekeurige rangschikking en waarden onder 0,5 zijn mogelijk. Corrigeer beide plaatsen. De ROC-uitleg is wel aanwezig en beschrijft terecht TPR tegenover FPR voor verschillende drempels (Google, 2026). |
| QA03 | Hoog | 3.3, 3.3.7, samenvatting en antwoord deelvraag 3 | Watermerkverwijdering wordt samen met compressie en aanvallen als rechtstreekse verslechtering van passieve detectie beschreven. Watermerken zijn actieve herkomstsignalen. Beschrijf primair verlies van dat signaal; claim alleen een effect op een passieve detector als dat afzonderlijk is gemeten. Zhao et al. (2024) onderzoeken watermerkdetectie. |
| QA04 | Hoog | 4.2, p. 18 | De formulering dat gepubliceerde nauwkeurigheid de praktijk systematisch overschat, gaat verder dan het besproken bewijs en botst met de eigen nuancering van generalisatiemethoden. Beperk dit tot de onderzochte benchmarks en overdrachtssituaties. De formulering dat interpreteerbaarheid de zwakste dimensie is, verwart beperkt bewijs met bewezen zwakte. Benoem dat deze dimensie in de gebruikte literatuur het minst uitgebreid is onderbouwd. Beide punten waren in oudere GitHub-notities al als gecorrigeerd beschreven, maar staan nog in dit bestand. |
| QA05 | Middel | H2 Vastlegging en 4.4 Betrouwbaarheid | De tekst zegt dat de referentielijst per bron mediatype, type onderzoek en deelvraag bevat en dat alle prestatiecijfers in een extractietabel staan. De zichtbare referentielijst is een APA-lijst zonder die velden. Voeg de werkelijk gebruikte bron- en extractiematrix toe of verwijs naar het juiste bestaande bewijsbestand. De oudere repositorymatrices mogen niet zonder vergelijking als bewijs voor deze 14-bronnenversie worden aangemerkt. |
| QA06 | Middel | 3.3.4, p. 15; tabel 4 | PSNR boven 30 dB is geen universele garantie dat verschillen voor het oog nauwelijks zichtbaar zijn. Beschrijf de gemeten beeldkwaliteit binnen het betreffende experiment. Zhao et al. (2024) wijzen zelf op beperkingen van PSNR/SSIM bij vervaging. Noem bij de verwijderingsclaim ook systeem, dataset en detectiedrempel uit de brontabel. |
| QA07 | Middel | Kop 3.2 onderaan p. 10; kop 3.3.6 onderaan p. 15 | Beide koppen staan los van de eerste tekst op de volgende pagina. Stel koppen in op samenhouden met de volgende alinea en render opnieuw. Tabellen 1 en 3 lopen door over twee pagina’s en hebben herhaalde koprijen; dat is op zichzelf geen fout. |
| QA08 | Middel | Tabellen en figuren; referenties p. 20–21 | Er zijn bronvermeldingen en 14 alfabetisch geordende referenties. Alle 14 zijn teruggevonden als citaat in de tekst. Dit is geen volledige APA-goedkeuring: nummers en titels staan als gecombineerde onderschriften onder de tabellen/figuren. Pas de APA-volgorde toe met nummer en titel erboven en toelichtende bronnoot eronder. Controleer daarna ook elke bibliografische beschrijving en DOI tegen de gebruikte publicatie. |
| QA09 | Middel | Portfolio per student | De aangeleverde stukken bewijzen ontvangen feedback, maar bevatten geen eigen verstrekte review, individuele taakverdeling of persoonlijke reflectie van Dave en Lucas. Voeg die echte stukken per persoon toe; vul ontbrekende data of werkzaamheden niet namens hen in. |
| QA10 | Middel | Versiehistorie en bronselectie | De eerdere registratie had 15 bronnen, inclusief Ramanaharan; de aangeleverde paper heeft 14 en bevat die bron niet. De verwijderingsreden en het effect op de analyse zijn niet aangetoond. Noteer de auteursbeslissing en koppel zo mogelijk de echte voorversie. Het ontbreken van die bron is op zichzelf geen kwaliteitsfout. |

## Tekstvoorstellen voor vastgestelde inhoudelijke problemen

**QA02:** “AUC is de oppervlakte onder de ROC-curve en heeft een waarde tussen 0 en 1. Een waarde van 0,5 duidt op willekeurige rangschikking en 1,0 op perfecte scheiding. Waarden onder 0,5 zijn mogelijk wanneer de rangschikking slechter is dan willekeurig.”

**QA03:** “Compressie, onbekende generatiemethoden en doelgerichte aanvallen kunnen de prestaties van passieve detectoren verminderen. Het verwijderen van watermerken tast een afzonderlijk actief herkomstsignaal aan; de aangehaalde watermerkstudie toont daarmee niet automatisch een daling van de prestaties van passieve detectoren aan.”

**QA04:** “De onderzochte vergelijkingen laten zien dat hoge scores op gecontroleerde benchmarks een te optimistisch beeld kunnen geven van prestaties op afwijkend praktijkmateriaal. De omvang van die kloof hangt af van de detector, trainingsdata en testomstandigheden.” En: “Interpreteerbaarheid is in de gebruikte literatuur het minst uitgebreid onderbouwd.”

**QA06:** “In de onderzochte aanval bleef de PSNR boven 30 dB. Dit beschrijft de gemeten pixelafwijking binnen het experiment en garandeert niet dat alle visuele veranderingen voor een waarnemer onzichtbaar zijn.”

## Formele controle

| Onderdeel | Uitkomst voor deze versie |
| --- | --- |
| Vereiste onderdelen | Samenvatting p. 2; inleiding p. 4–5; methode p. 6–7; resultaten p. 8–16; conclusies en discussie p. 17–19; referenties p. 20–21 aanwezig |
| Omvang | 21 pagina’s totaal; resultatenbody p. 8–16 = 9 pagina’s. Voldoet aan de letterlijke bodyregel van 8–10 pagina’s in Appendix 9, p. 4 |
| Figuren en tabellen | 2 figuren en 4 tabellen; in de tekst benoemd en inhoudelijk relevant |
| Tabeltekst | Alle 172 niet-lege tekstruns expliciet 9 pt; visueel geen verschil in grootte tussen gewone tabelrijen geconstateerd |
| Opmaak | Leesbare render; geen evidente overlap of afgekapt tabelmateriaal in de inspectie; twee losse koppen moeten worden hersteld |
| Documenttechniek | Geen ingesloten reviewcommentaren of bijgehouden invoegingen/verwijderingen aangetroffen |
| Taal en logica | Overwegend helder Nederlands; onder meer “Een deepfake is media” kan duidelijker als “Een deepfake is een mediabestand”. De inhoudelijke punten QA02–QA06 wegen zwaarder dan deze taalredactie |
| Beoordelingsstatus | Interne controle met open punten; geen bewijs van formele docentgoedkeuring of succesvolle inzending vastgesteld |

## Eisen voor het portfolio

NHL Stenden University of Applied Sciences (z.d.-a, Appendix 1, sectie 2, gedrukte p. 33 / PDF p. 39) vraagt om de paper, inhoudelijke ontvangen feedback, inhoudelijke verstrekte feedback en waar relevant bewijs van verwerking. Appendix 3 (gedrukte pp. 41–42 / PDF pp. 47–48) vraagt om serieuze overweging en passende verwerking. Dat betekent niet dat elk advies letterlijk moet worden uitgevoerd. Een beargumenteerde andere oplossing is mogelijk, mits die aantoonbaar is.

Het portfolio is individueel en wordt als één gestructureerde PDF ingeleverd. Deze repository levert bewijs en verwijzingen voor die PDF; deze registratie is op zichzelf geen ingeleverd portfolio. De [werkwijze](Reviewverwerking-werkwijze.md), [beslismatrix](Feedback%20Decision%20Matrix.md), [activiteitenregistratie](Activiteitenlog.md) en [individuele invulvelden](Portfolio%20Use%20Note.md) leggen samen de benodigde verbinding.

## Referenties

Google. (2026, 11 mei). *Classification: ROC and AUC*. Google for Developers. https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc

Lübbers, L. (z.d.). *De betrouwbaarheid van AI-gebaseerde deepfakedetectie: Peerreview voor Lucas Wanink en Dave van den Berg* [Ongepubliceerde peerreview]. [Bewijsbestand](Evidence/review-lucas-lubbers.pdf).

NHL Stenden University of Applied Sciences. (z.d.-a). *Applied AI module book V1* [Moduleboek]. Aangeleverd projectdocument, SHA-256 `4bf4961d2c78503623a2004c07840fceffd9e3509d8ca35f7bd0e4dce8cf851a`.

NHL Stenden University of Applied Sciences. (z.d.-b). *Assessment form Applied AI research paper* (versie 2026–2027–1.0) [Beoordelingsformulier, Appendix 9]. Aangeleverd projectdocument, SHA-256 `59ff6c6431d2555c6f5eaf7894d4eec1975b6f0523e6624efefa5f1357faa23c`.

Velema, M. (2026, 25 september). *Assessment form Applied AI working paper: Feedback voor Lucas Wanink en Dave van den Berg* [Ingevuld peerreviewformulier]. [Bewijsbestand](Evidence/review-mart-velema.pdf).

Wanink, L., & Van den Berg, D. (2026, 27 september). *De betrouwbaarheid van AI-gebaseerde deepfakedetectie* [Aangeleverde paper met verwerkte reviews]. [Bewijsbestand](Evidence/paper-review-verwerkt.docx).

Zhao, X., Zhang, K., Su, Z., Vasan, S., Grishchenko, I., Kruegel, C., Vigna, G., Wang, Y.-X., & Li, L. (2024). Invisible image watermarks are provably removable using generative AI. *Advances in Neural Information Processing Systems, 37*, 8643–8672. https://papers.nips.cc/paper/2024/file/10272bfd0371ef960ec557ed6c866058-Paper-Conference.pdf

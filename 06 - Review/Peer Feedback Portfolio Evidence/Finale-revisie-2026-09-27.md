# Finale revisie na reviewcontrole – 27 september 2026

## Doel

Deze revisie verwerkt de resterende inhoudelijke en opmaakpunten die na de controle van de reviewverwerking nog zichtbaar waren. De oorspronkelijke bewijsbestanden en het eerdere controleverslag blijven ongewijzigd bewaard, zodat de ontwikkeling van de paper traceerbaar blijft voor het individuele portfolio.

De definitieve, lokaal opgeleverde versie heet `Deepfake paper - Dave & Lucas FINAL.docx` en heeft SHA-256:

`5a409201c5fc5adb85eda5851ee534de9394fcccd40ec4bcf4e1a51f970669f2`

## Uitgevoerde correcties

| Onderdeel | Wijziging | Controle |
| --- | --- | --- |
| AUC-bereik | AUC is consequent begrensd op 0–1; 0,5 is toevalsniveau en 1,0 perfecte scheiding | Tekst en Figuur 2 gecontroleerd |
| Figuur 2 | X-as eindigt nu op 1,0 in plaats van 1,1 | Nieuwe render visueel gecontroleerd |
| Samenvatting | Ingekort tot 267 woorden en conclusies begrensd geformuleerd | Beknoptheid en inhoud gecontroleerd |
| Conclusies | Formuleringen als “zeer betrouwbaar”, “redelijk betrouwbaar”, “slecht” en “systematisch overschat” vervangen door uitspraken die rechtstreeks bij de geselecteerde studies en testomstandigheden aansluiten | H4 opnieuw gelezen |
| Trainingsdata versus architectuur | Niet meer gesteld dat trainingsdata generaliseerbaarheid “beter voorspelt”; nu begrensd tot de bevinding dat samenstelling zwaar kan wegen en in de geselecteerde studie minstens zo belangrijk kan zijn | H3.1.4 en H4.1 gelijkgetrokken |
| Interpreteerbaarheid | Niet meer aangeduid als bewezen “zwakste” dimensie; nu beschreven als het minst uitgebreid onderbouwd in de gebruikte literatuur | H4.2 gecontroleerd |
| Watermerken | Duidelijk onderscheiden van passieve deepfakedetectie: verwijdering tast een actief herkomstsignaal aan en is niet automatisch bewijs voor lagere prestaties van passieve detectoren | Samenvatting, H3.3 en H4 aangepast |
| PSNR | De claim dat >30 dB visueel onzichtbaar zou zijn is vervangen door een experimentgebonden, voorzichtige interpretatie | H3.3.4 gecontroleerd |
| Bronregistratie | “Referentielijst” vervangen door “bronregistratietabel” waar de interne selectie-/extractieregistratie wordt bedoeld | H2 en H4.4 gecontroleerd |
| Tabel 3 | Rijen kunnen niet meer over pagina’s worden gesplitst; de generaliseerbaarheidsrij staat intact | Render gecontroleerd |
| Koppen | Koppen zijn ingesteld om bij de eerstvolgende alinea te blijven; losse koppen onderaan pagina’s zijn verwijderd | Render gecontroleerd |
| APA-referentielijst | Dubbele regelafstand, geen extra witruimte tussen referenties en 1,27 cm hanging indent | Alle 14 referenties technisch gecontroleerd |
| Inhoudsopgave | Paginanummers aangepast aan de definitieve render | Paginaverwijzingen visueel gecontroleerd |
| Taal | Onder meer “Een deepfake is media” gewijzigd naar “Een deepfake is een mediabestand” | Taalcontrole uitgevoerd |

## Eindcontrole

De definitieve versie is opnieuw naar PDF/PNG gerenderd en alle 23 pagina’s zijn visueel gecontroleerd op clipping, overlap, tabelbreuken, figuren, paginanummers en koppen. De resultaten lopen van p. 8 t/m p. 17 en beslaan daarmee 10 pagina’s. Dat valt binnen de 8–10-paginaregel uit Appendix 9 voor de body, waarbij inleiding, methode, conclusie/discussie en bronnenlijst niet meetellen.

De paper bevat 14 referenties, 4 tabellen en 2 figuren. Alle 36 tabelrijen zijn technisch ingesteld om niet over pagina’s te breken. De samenvatting telt 267 woorden.

## Relatie met de peerreview

De expliciete feedback over AUC/ROC en tabelopmaak is in de definitieve versie zichtbaar verwerkt. De eerder al verwerkte punten over hoofdstukoriëntatie, het onderzoeksdoel, samenvattingen van resultaten en het letterlijk herhalen van de hoofdvraag blijven behouden. De finale controle heeft daarnaast regressies en te stellige formuleringen gecorrigeerd die na eerdere reviewverwerking nog aanwezig waren.

## Portfolio

Het moduleboek vraagt in periode 1 om de voltooide research paper, ontvangen inhoudelijke peerfeedback, verstrekte inhoudelijke peerfeedback en waar relevant bewijs van hoe ontvangen feedback is verwerkt. Deze repository bewaart daarom de oorspronkelijke reviews, de eerdere gecontroleerde versie, de beslismatrix, het activiteitenlog, de vaste reviewwerkwijze en deze finale revisieregistratie.

Voor het individuele portfolio blijven persoonsgebonden bewijsstukken afzonderlijk nodig: welke wijzigingen Dave respectievelijk Lucas zelf uitvoerden, hun eigen reflectie en de feedback die ieder daadwerkelijk aan een andere student heeft verstrekt. Die informatie mag niet uit Git-commits of deze technische controles worden afgeleid als zij niet met echt bewijs is vastgelegd.

## Status

De inhoudelijke en opmaakcorrecties uit de finale controle zijn uitgevoerd en technisch geverifieerd. Het eerdere [controleverslag](Controleverslag-2026-09-27.md) blijft als historische momentopname bewaard. Open punten over zoekdatums/exports en individuele portfolio-evidence zijn bewijs- en procespunten; zij zijn niet stilzwijgend als historische feiten ingevuld.

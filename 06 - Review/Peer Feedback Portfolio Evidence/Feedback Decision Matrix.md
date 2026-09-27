# Beslismatrix van ontvangen feedback

Deze matrix beoordeelt uitsluitend de aangeleverde versie met SHA-256 `cd00d692921bdee9fd95afe44893f9e4ffbbd21030afe0269cfc87b48f0f3c6b`. Controle: 27 september 2026. De oorspronkelijke reviewteksten staan in [Evidence](Evidence). Voor exacte bestandsidentiteit zie het [manifest](Evidence/manifest.json).

“Verwerkt” betekent dat de gevraagde uitkomst zichtbaar is. Het bewijst zonder de oorspronkelijke DOCX geen exacte historische wijziging, datum, uitvoerder of motivering. Beslisredenen hieronder zijn de beoordeling van deze controle; persoonlijke auteurskeuzes moeten waar nodig worden bevestigd. Alle uitvoerders van eerdere paperwijzigingen: **nog vast te leggen door Dave en Lucas**.

| ID | Bron en feedback | Zichtbare verwerking en vindplaats | Oordeel en reden | Nog nodig |
| --- | --- | --- | --- | --- |
| LL01 | Lübbers, p. 1: korte introducties bij H2 en H4 | H2 start met beschrijving van aanpak, bronnen, vastlegging, meetmaten en analyse; H4 licht de volgorde van antwoorden, aanbevelingen en evaluatie toe; p. 6 en 17 | Verwerkt; de lezer krijgt vooraf oriëntatie | Persoonlijke bijdrage en echte voorversie koppelen |
| LL02 | Lübbers, p. 1: compacter inleiden en doel eerder tonen | Context en kenniskloof in eerste alinea; doel in tweede alinea, p. 4 | Verwerkt qua vroege plaatsing; de inleiding blijft twee pagina’s. Een afname van de lengte is zonder voorversie niet bewezen | Auteursmotivering voor verdere inkorting of behoud |
| LL03 | Lübbers, p. 1: technische AUC-uitleg eventueel verplaatsen | Inleiding geeft korte uitleg en verwijst naar H2; uitgebreide uitleg staat onder Meetmaten, p. 7 | Alternatieve oplossing zichtbaar: methode in plaats van apart theoretisch kader. Dit is passend omdat een afzonderlijk kader niet verplicht is. Inhoudelijk resteert QA02 | AUC-bereik op beide plaatsen corrigeren |
| LL04 | Lübbers, p. 2: hoofdvraag letterlijk herhalen | De volledige vraag in H1 en 4.2 is na weglaten van het inleidende label identiek; p. 4 en 18 | Verwerkt; conclusie kan zelfstandiger worden gelezen | Persoonlijke bijdrage vastleggen |
| LL05 | Lübbers, p. 2: belangrijkste resultaten samenvatten | Afsluitende alinea’s met “Samengevat” in 3.1.4, 3.2.6 en 3.3.7; p. 10, 14 en 16 | Verwerkt qua zichtbaarheid; inhoudelijke watermerkafbakening blijft QA03 | QA03 oplossen |
| LL06 | Lübbers, p. 2: zoek- en selectieprocedure reproduceerbaar maken, gevonden en uitgesloten bronnen tonen | H2 noemt arXiv, IEEE Xplore, SpringerLink, periode, zoekvelden, criteria, zes queries en aantallen in tabel 1; 14 opgenomen bronnen | Gedeeltelijk verwerkt; gevonden aantallen zijn vermeld, maar hun herkomst en de selectie tot 14 bronnen zijn niet controleerbaar | QA01: zoekdatums, bewijs, dubbelen, uitsluitredenen, oorspronkelijke versus aanvullende zoekactie |
| MV01 | Velema, p. 6: betekenis en toepassing van AUC/ROC uitleggen of ROC weglaten | H2 Meetmaten legt ROC via TPR/FPR uit, legt de relatie met AUC uit en zegt dat de auteurs bronwaarden overnemen en zelf geen ROC-curves berekenen; p. 7 | Gedeeltelijk verwerkt; functie en gebruik zijn duidelijker, maar het AUC-bereik is fout en een methodologische bron ontbreekt bij de uitleg | QA02 corrigeren en passende verwijzing bij de definitie plaatsen; ROC hoeft niet te worden weggelaten |
| MV02 | Velema, p. 6: inconsistente tekstgrootte in tabellen | Vier tabellen; alle 172 niet-lege tekstruns expliciet 9 pt; gewone rijen ogen consistent | Verwerkt; de gemelde grootteverschillen zijn niet aangetroffen | Bij volgende wijziging opnieuw controleren |

## Afzonderlijke interpretatie van rubricmarkeringen

Marts p. 4 kruist de ontbrekend/niet-voldaan-opties door. Op p. 5 is de methodologische argumentatie relatief het zwakst gemarkeerd. H2 Aanpak en onderbouwing bevat een duidelijke afweging tussen literatuurstudie en één eigen experiment en legt uit waarom geen meta-analyse is gedaan. Dat sluit aan op B3. Deze interpretatie is geen letterlijke extra reviewopdracht en geen numeriek eindcijfer. Reproduceerbaarheid blijft een afzonderlijk open punt.

## Sterke punten uit beide reviews

Lübbers benoemt structuur, kwantitatieve onderbouwing, eigen synthese, beantwoording met aanbevelingen en ondersteunende tabellen/figuren. Mart noemt duidelijke scope en doel, bruikbare grafieken/tabellen met passende bijschriften en het onderscheid tussen wat AUC wel en niet betekent. Deze kwaliteiten zijn nog herkenbaar in de huidige paper; de inhoudelijke grenzen uit het [controleverslag](Controleverslag-2026-09-27.md) blijven van toepassing.

## Bronverwijzingen

Lübbers, L. (z.d.). *Peerreview voor Lucas Wanink en Dave van den Berg* [Ongepubliceerde feedback], pp. 1–2. [PDF](Evidence/review-lucas-lubbers.pdf).

Velema, M. (2026, 25 september). *Assessment form Applied AI working paper* [Ingevuld peerreviewformulier], pp. 4–6. [PDF](Evidence/review-mart-velema.pdf).

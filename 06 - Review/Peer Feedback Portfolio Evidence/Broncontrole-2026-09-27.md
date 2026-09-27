# Afgebakende broncontrole bij de reviewaudit

Op 27 september 2026 zijn onderstaande primaire publicaties en officiële pagina’s gericht gecontroleerd. Dit is een aanvullende controle na het schrijven van de paper, geen reconstructie van de oorspronkelijke literatuurzoekactie en geen nieuwe bronselectie voor de paper. De aangeleverde DOCX is niet gewijzigd.

| Onderwerp | Gecontroleerd bewijs | Uitkomst en grens |
| --- | --- | --- |
| AUC en ROC | Google, uitleg en voorbeelden onder 0,5 | De paper moet het bereik aanpassen van 0,5–1 naar 0–1; willekeurig rangschikken geeft 0,5. QA02 |
| Praktijkbenchmark | Chandra et al., officiële CVF-publicatievermelding en auteursabstract | De gemelde gemiddelde dalingen van 50% video, 48% audio en 45% beeld staan in het abstract. Dit valideert niet automatisch iedere afgeleide grafiekwaarde of iedere individuele detectorvergelijking |
| Multimodale overzichtsstudie | Nguyen-Le et al., uitgeversartikel | Artikel 203 in volume 59 (2026), publicatiegegevens en tekst over 10–15% degradatie en meer dan 80% white-box-aanvalssucces aangetroffen. De laatste claim betreft onverdedigde modellen; die beperking moet ook in samenvattingen blijven staan |
| Watermerken en beeldkwaliteit | Zhao et al., NeurIPS-publicatie, evaluatie en discussie | Studie gaat over watermerkherkenning. De tekst benoemt dat PSNR/SSIM vervaging onvoldoende kunnen weergeven. Geen algemene garantie van visuele onzichtbaarheid afleiden; QA03 en QA06 |
| Audioresultaat AASIST | Officiële auteursrepository | EER 0,83% voor AASIST op ASVspoof 2019 LA bevestigd. AASIST-L heeft een andere score; dit is geen praktijkprestatiegarantie |
| WildDeepfake | Officiële auteursrepository | 7.314 gezichtssequenties uit 707 internetvideo’s vermeld; de 707-videovermelding in de paper sluit daarop aan |
| Statistische ontwijkingsaanval | Hou et al., officiële CVF-publicatievermelding | Titel, auteurs, CVPR 2023 en pp. 12271–12280 bevestigd; abstract ondersteunt het principe van verkleinen van statistische verschillen. Niet elke aanvalconditie opnieuw gereproduceerd |
| Artikel 50 | Europese Commissie, officiële FAQ | Ingang 2 augustus 2026 en beperkte overgang voor al eerder op de markt gebrachte systemen bij de markeer-/detectieplicht bevestigd. Geen zelfstandige juridische analyse uitgevoerd |
| Generalisatie over benchmarks | Yermakov et al., officiële CVF PDF-zoekvermelding | Publicatie en tabelvermelding aangetroffen, maar de volledige PDF kon bij deze controle niet worden geopend. De precieze 0,916-claim is daarom niet volledig opnieuw gevalideerd |

De resterende bronnen en alle volledige auteurreeksen, DOI’s en paginabereiken zijn in deze audit niet integraal opnieuw gecontroleerd. De paperversie bevat 14 referenties; alle 14 zijn als citaat in de tekst teruggevonden. Het eerdere [15-bronnenoverzicht](../../02%20-%20Sources/Current%20Source%20Reliability%20Audit.md) beschrijft een andere versie. De oorspronkelijke zoekdatums, database-uitvoer en uitsluitingen blijven open onder QA01.

## Referenties en primaire controlelocaties

Chandra, N. A., Lee, H., Murtfeldt, R., Qiu, L., Karmakar, A., Tanumihardja, E., Farhat, K., Caffee, B., Lee, C., Choi, J., Paik, S., Kim, A., & Etzioni, O. (2026). Deepfake-Eval-2024: A multi-modal in-the-wild benchmark of deepfakes circulated in 2024. In *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops* (pp. 10668–10678). https://openaccess.thecvf.com/content/CVPR2026W/APAI/html/Chandra_Deepfake-Eval-2024_A_Multi-Modal_In-the-Wild_Benchmark_of_Deepfakes_Circulated_in_2024_CVPRW_2026_paper.html

Clova AI. (z.d.). *AASIST* [Officiële broncoderepository]. GitHub. Geraadpleegd op 27 september 2026, van https://github.com/clovaai/aasist

European Commission. (2026, 24 juli). *Transparency obligations under Article 50 of the AI Act*. https://digital-strategy.ec.europa.eu/en/faqs/transparency-obligations-under-article-50-ai-act

Google. (2026, 11 mei). *Classification: ROC and AUC*. Google for Developers. https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc

Hou, Y., Guo, Q., Huang, Y., Xie, X., Ma, L., & Zhao, J. (2023). Evading DeepFake detectors via adversarial statistical consistency. In *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* (pp. 12271–12280). https://openaccess.thecvf.com/content/CVPR2023/html/Hou_Evading_DeepFake_Detectors_via_Adversarial_Statistical_Consistency_CVPR_2023_paper.html

Nguyen-Le, H.-H., Tran, V.-T., Nguyen, D.-T., & Le-Khac, N.-A. (2026). Deepfake detection across image, video, and audio: A comprehensive survey with empirical evaluation of generalization and robustness. *Artificial Intelligence Review, 59*, Article 203. https://doi.org/10.1007/s10462-026-11608-4

Yermakov, A., Cech, J., Matas, J., & Fritz, M. (2026). *Deepfake detection that generalizes across benchmarks* [Conferentiepublicatie; volledige hercontrole niet afgerond]. IEEE/CVF WACV. https://openaccess.thecvf.com/content/WACV2026/papers/Yermakov_Deepfake_Detection_that_Generalizes_Across_Benchmarks_WACV_2026_paper.pdf

Zhao, X., Zhang, K., Su, Z., Vasan, S., Grishchenko, I., Kruegel, C., Vigna, G., Wang, Y.-X., & Li, L. (2024). Invisible image watermarks are provably removable using generative AI. *Advances in Neural Information Processing Systems, 37*, 8643–8672. https://papers.nips.cc/paper/2024/file/10272bfd0371ef960ec557ed6c866058-Paper-Conference.pdf

Zi, B., Chang, M., Chen, J., Ma, X., & Jiang, Y.-G. (2020). *WildDeepfake* [Officiële datasetrepository]. GitHub. https://github.com/xingjunm/wild-deepfake

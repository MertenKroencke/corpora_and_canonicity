# corpora_and_canonicity
Repository for Contribution Comparing Corpus Canonicity, submitted to for DH 2027.

## Structure

```
code/
  gnd_pipeline.ipynb      GND IDs and canonicity scores for all corpora -> resources/final/
  analysis.ipynb          exploratory analysis
  figures_poster.ipynb    figures for the poster -> figures/
resources/
  raw/                    raw corpus metadata (not included, see info.md)
  cache/                  cached API answers (lobid, Wikidata, GND redirects)
  final/                  pipeline output: one file per corpus, data_all.csv (one row per work),
                          work_authors.csv (one row per work and author), correction and review lists
  canonicity_scores.xlsx  canonicity score and rank per author (GND ID)
  gnd_*.csv               GND name list used for matching
figures/                  poster figures (PNG)
```

## Corpora

Corpora used in the analysis (the folder `resources/final/` also contains translated fiction,
de-Corp non-fiction and DisKo classics, which are not used).

- **Corpus of German Language Fiction** (`01_german-fiction`): Fischer, Frank, and Jannik Strötgen. 2017. *Corpus of German-Language Fiction (txt)*. figshare. https://doi.org/10.6084/m9.figshare.4524680.v1
- **de-Corp** (`03_de-corp`): Rohrbacher, Katrin. 2025. "de-Corp: A Corpus of German-language Fiction and Non-Fiction (1780–1930)." *Journal of Open Humanities Data* 11. https://doi.org/10.5334/johd.350
- **d-prose** (`04_d-prose`): Gius, Evelyn, Svenja Guhr, and Inna Uglanova. 2021. "'d-Prose 1870–1920' a Collection of German Prose Texts from 1870 to 1920." *Journal of Open Humanities Data* 7. https://doi.org/10.5334/johd.30
- **ELTeC-deu** (`05_ELTeC-deu`): Konle, Leonard, Fotis Jannidis, Carolin Odebrecht, and Lou Burnard. 2021. *German Novel Corpus (ELTeC-deu): April 2021 release*. Zenodo, v1.0.0. https://doi.org/10.5281/zenodo.4662482; Schöch, Christof, Roxana Patras, Tomaž Erjavec, and Diana Santos. 2021. "Creating the European Literary Text Collection (ELTeC): Challenges and Perspectives." *Modern Languages Open* 1: 25. https://doi.org/10.3828/mlo.v0i0.364
- **d-RoRo** (`06_romane-der-romantik`): Schumacher, Mareike, Inna Uglanova, and Evelyn Gius. 2022. *d-Romane-Romantik (d-RoRo)*. Zenodo, v1.0. https://doi.org/10.5281/zenodo.7223515
- **Bildungsromankorpus** (`07_bildungsromane`): Boucher, Marie-Christine, J. Berenike Herrmann, Alexander Hummel, and James Wiebe. 2024. *Bildungsromankorpus*. Zenodo. https://doi.org/10.5281/zenodo.14289198
- **glance** (`08_glance`): Hilger, Agnes. 2026. *glance*. Zenodo, v1.0. https://doi.org/10.5281/zenodo.23539457
- **EcoCor-DE** (`09_ecocor`): Schumacher, Mareike, Peer Trilcke, Sören Barkey, Daniil Skorinkin, and Carsten Milling (eds.). 2026. *EcoCor-DE*. Zenodo, v1.0.0. https://doi.org/10.5281/zenodo.19630113
- **19CproseCorpus** (`10_19C-prose`): Schröter, Julian, Johannes Leitgeb, and Theresa Valta. 2023. "Ein digitales Korpus der Novellen und Journalprosa des 19. Jahrhunderts: Herausforderungen der Metadatenerschließung." *DARIAH-DE Working Papers* 46. https://doi.org/10.47952/gro-publ-131
- **DTA core corpus, fiction** (`11_dta-belletristik`): Geyken, Alexander, Matthias Boenig, Susanne Haaf, Bryan Jurish, Christian Thomas, and Frank Wiegand. 2018. "Das Deutsche Textarchiv als Forschungsplattform für historische Daten in CLARIN." In *Digitale Infrastrukturen für die germanistische Forschung*, edited by Henning Lobin, Roman Schneider, and Andreas Witt, 219–248. Berlin/Boston: de Gruyter.
- **Deutscher Novellenschatz** (`13_deutscher-novellenschatz`): Weitin, Thomas (ed.). 2016. *Volldigitalisiertes Korpus. Der Deutsche Novellenschatz*. Ed. by Paul Heyse and Hermann Kurz. Deutsches Textarchiv. http://www.deutschestextarchiv.de/doku/textquellen#novellenschatz
- **Neuer Deutscher Novellenschatz** (`14_neuer-deutscher-novellenschatz`): Weitin, Thomas, and Katharina Herget. 2022. *Neuer Deutscher Novellenschatz (1884–1887)*. Zenodo, v1.0. https://doi.org/10.5281/zenodo.6783577

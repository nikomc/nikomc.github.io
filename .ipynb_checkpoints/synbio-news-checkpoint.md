---
layout: page
title: This Week in Synthetic Biology
---

**_This Week in Synthetic Biology_** is emailed to subscribers every Friday, and covers the latest research, preprints, and news in synthetic biology research.

This is the newsletter for October 23, 2020 (Issue 13). View the full archive on [Substack](https://synbio.substack.com/).

<iframe src="https://synbio.substack.com/embed" width="480" height="320" style="border:1px solid #EEE; background:white;" frameborder="0" scrolling="no"></iframe>

## 🌄Good morning.

##### [Tell me](https://twitter.com/NikoMcCarty) about your research on Twitter. Or just say ‘hello’.

## Let There Be Sight!

The retina, in the back of our eyes, is a delicate and complicated piece of biological machinery. In the retina is a molecule called *11-cis-retinal*; when light hits the photosensitive part of the retina, this molecule converts to a different chemical form (called all-trans retinal), which then triggers a cascade of chemical alterations that, eventually, lets our brain perceive images.

But all-trans-retinal needs to *go back* to its original form—the *cis* version—and prepare to receive a new blast of light. A protein called *RPE65* helps with that, but mutations in that protein can, unfortunately, cause inherited blindness.

In a new study, published in the journal *Nature Biomedical Engineering* on Oct. 19, researchers used a base editor protein, which can change specific nucleic acids in the genome without cutting the DNA, to restore vision to *near-normal* levels. The base editor—and a guide RNA to direct its genomic edits—was packaged inside of a virus, injected into the eyes of adult mice, and corrected the desired mutation in the *Rpe65* gene “with up to 29% efficiency and with minimal formation of indel and off-target mutations”. [Link](https://www.nature.com/articles/s41551-020-00632-6)

## “Honey, I Shrunk the Cas9”

Cas9, a common protein that molecular biologists use to cut and edit DNA, is large: 2.5x bigger than hemoglobin, and more than 27x bigger than an insulin protein. That’s a problem, in part, because it means that Cas9 can’t always be packaged in teeny tiny viruses, and delivered to different parts of the body for CRISPR therapies.

Now, researchers at UC-Berkeley have reported a technique that enables them to test various deletions in the Cas9 protein and then assess whether its function remains, or is lost. The method, called MISER (Minimization by Iterative Size-Exclusion and Recombination), was used to systematically explore the effect of different Cas9 deletions. The result? The authors managed to remove large chunks in several protein domains, and Cas9 *still* retained its function for genome editing. The new, “minified” CRISPR proteins are less than 1000 amino acids in length, and the smallest variant that they created is just 874 amino acids in size, which is about 60% of the mass of the original Cas9. This work was published on *bioRxiv*, is open access, and is the first preprint that I have featured in this newsletter. [Link](https://www.biorxiv.org/content/10.1101/2020.10.19.344077v1)

## E. Coli Were Fed a Diet of Air (Poor Things)

Plants and algae—including cyanobacteria, which are probably the most important bacteria on earth—fix carbon, from atmospheric carbon dioxide, using the *Calvin cycle*. But atmospheric carbon dioxide is present in really low concentrations (about 412 parts per million, and rising), so bacteria and plants first need to concentrate it. To store and concentrate carbon dioxide, some bacteria use a protein capsule called a *carboxysome*. Unfortunately, despite the critical importance that “carbon dioxide concentrating mechanisms” play in photosynthesis, researchers don’t fully understand which genes and proteins are involved.

Now, research led by groups at UC-Berkeley and the Weizmann Institute of Science have figured out a way to get \*E. coli—\*which are definitely not photosynthetic—to concentrate atmospheric carbon dioxide. To do that, they expressed *twenty genes* involved in concentrating carbon dioxide in *E. coli*. The engineered microbes were then able to “grow by fixing \[carbon dioxide\] from ambient air into biomass”. That’s a beautiful result, and one that also led to some important advancements in our understanding of how these carboxysomes work at a fundamental level. This work was published in the journal *eLife* on Oct. 21 and is open access. [Link](https://elifesciences.org/articles/59882)

## Reverse Engineering S. pneumoniae Infections

You have probably, at some point in your life, fallen ill with pneumonia. It’s a terrible feeling—lying on the couch with a glass of OJ, binge watching Jeopardy, is my preferred cure.

Most cases of pneumonia are caused by *Streptococcus pneumoniae*, which are little microbes that look like squat noodles. *S. pneumoniae* naturally resides in the sinuses, nose, throat, and lungs, but sometimes, it causes serious disease (and about 1 million deaths every year). Before *S. pneumoniae* starts to wreak havoc in the body, though, an array of genes come sweeping on, and its infection machinery boots up.

Unfortunately, researchers don’t really understand how *S. pneumoniae* switches from “benign microbe, comfortably residing in your nose” to “terrifying pathogen that induces Jeopardy binge watching”.

Now, synthetic biologists at the University of Groningen have developed methods to control genetic programs in this important microbe. In a new, open access study, published in *PNAS*, the researchers report that they successfully “rewired gene expression of the operon responsible for the main pneumococcal virulence factor, the exopolysaccharide capsule”—referring to the actual surface of the bacteria, which shields the microbe from the human immune system. Further, the authors show that they can build synthetic, gene-regulatory networks, in *S. pneumoniae*, and tweak them to better understand how pneumococcal pathogenicity occurs. The tools developed here could go a long way in bolstering our understanding of *S. pneumoniae* infections. [Link](https://www.pnas.org/content/early/2020/10/20/1920015117)

## DNA Stores Mozart’s Music

In 2012 and 2013, scientists could store about 1MB of digital information in DNA (or about one 52,000 word book). By 2017, the data storage density of DNA was equivalent to roughly 256 petabytes per gram. In recent years, improved technologies, especially parallelized DNA synthesis and high-throughput DNA sequencing, have brought DNA data storage ever closer to a practical reality.

Now, a new study has used a parallelized version of DNA synthesis to store about 100 kB of digital information—“52 pages of digitalized sheet music” from Mozart’s string quartet, called ‘The Hunt’—in 16,383 DNA sequences. The DNA synthesis method used by the authors is extremely error prone, but is cheaper and faster than other options. Despite the higher number of errors in the DNA sequences, the authors were able to retrieve all of the stored information, thanks to some algorithms that “reconstruct” the data. This study was published in *Nature Communications* and is open access. [Link](https://www.nature.com/articles/s41467-020-19148-3)

***

## 🧫 Rapid-Fire Highlights

## More research & reviews worth your time

* A mouse model of Angelman syndrome, a neurodevelopmental disorder caused by a mutation or deletion in a gene called *UBE3A*, was rescued with Cas9. Researchers packaged a modified version of Cas9 and guide RNA in a virus, and injected mice during the embryonic and early postnatal stages of development. The CRISPR/Cas injections effectively unsilenced *UBE3A* expression and “rescued anatomical and behavioural phenotypes” in the animals. *Nature*. [Link](https://www.nature.com/articles/s41586-020-2835-2)
* In a paper related to “DNA Stores Mozart’s Music”, researchers in George Church’s group reported a multiplexed, enzymatic method to synthesize DNA that uses *light* to specify and control the assembly reactions. They use it to store video game music in DNA, but its potential is far, far greater. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18681-5)
* [Prime editors](https://en.wikipedia.org/wiki/Prime_editing) work *really* well in monocot plants, like rice, but are apparently not as good in dicots (like tomatoes). A new study has adapted a mammalian prime editor, and used it in tomato plants. They were able to swap out nucleic acids, delete them, or cause targeted frame shifts in the tomato DNA. *Plant Biotechnology Journal* (*Open Access*). [Link](https://onlinelibrary.wiley.com/doi/10.1111/pbi.13497)
* Cas9 and Cas12a, two commonly-used CRISPR proteins, are limited in that they can’t really make large deletions to genomes. A new study used the Cas3 enzyme, together with accessory proteins, to perform large genomic deletions in several bacterial species (between 7,000-424,000 base pairs, with 100% efficiency). The tool may help genome engineers swap out large chunks of DNA as they redesign or refactor genomes. Read the [press release](https://phys.org/news/2020-10-crispr-pac-man-dna-cut-and-paste-tool.html). *Nature Methods*. [Link](https://www.nature.com/articles/s41592-020-00980-w)
* A new review discusses base editors, and how they can be used in various therapies. A nice, recent demonstration of that is the featured research article this week, in which vision was restored in mice with a genetic mutation in the *Rpe56* gene. *Nature Reviews Drug Discovery*. [Link](https://www.nature.com/articles/s41573-020-0084-6)
* Synthetic biology researchers have exploited only a tiny fraction of the sum diversity of genetic material found on earth. Most labs confine their research to model organisms, like *E. coli* and Baker’s yeas*t*, and tools to efficiently engineer other types of organisms are…lagging behind. A new *Perspective* paper explores how *bacteriophages* (little viruses that infect bacteria) can be used to engineer these understudied organisms. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-19124-x)
* *E. coli* cells with reduced genomes (in some cases, with more than 35% of their genome missing) were engineered with a biosynthetic pathway that produces a pigment called protodeoxyviolacein to study how miniaturized genomes affect resource allocation inside of cells. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.10.19.346155v1.abstract?%3Fcollection=)
* “Designer proteins” that can bind to, and inhibit, the spike receptor binding domain of SARS-CoV-2 were created. The proteins successfully blocked SARS-CoV-2 infection in a cell culture model (I previously covered this study as a pre-print in this newsletter). *Science* (*Open Access*). [Link](https://science.sciencemag.org/content/370/6515/426)
* Another inhibitor of the SARS-CoV-2 receptor binding domain—engineered using a mixture of bioengineering methods—was also effective at preventing infections in a cell culture model. *PNAS* (*Open Access*). [Link](https://www.pnas.org/content/early/2020/10/21/2016093117)
* dCas12a (a type of Cas enzyme) has, for the first time, been used to increase and decrease the expression of multiple genes at once in bacteria. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.08.05.232744v2.full.pdf)
* A new database for CRISPR-Cas9 *off-target* assays has aggregated data from 17 studies, encompassing more than 25,600 genetic targets. *Nucleic Acids Research* (*Open Access*). [Database](http://www.crisprsql.com/) & [Link](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkaa885/5934413)
* Glycopeptide antibiotics are used to treat severe infections by gram-positive bacteria. Unfortunately, this type of antibiotic is difficult to manufacture with existing technologies. A new study engineered a strain of bacteria, called *S. coelicolor* M1154/pAMX4, to produce a whole slew of glycopeptide antibiotic compounds. This could prove useful in finding and producing new antibiotics for hard-to-treat infections. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-19138-5)
* Researchers created synthetic cells with lipids, and then coaxed those cells into aggregating with one another via DNA that was modified to act as a signaling molecule. This study raises new possibilities for the programming of “designer cells”, built from scratch. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.10.18.344432v1)
* A light-inducible BMP signaling pathway has been created and tested in mammalian cells, which could prove useful for studying how this evolutionarily conserved pathway behaves over space and time. *ACS Synthetic Biology*. [Link](https://pubs.acs.org/doi/10.1021/acssynbio.0c00315)
* There are only two biosynthetic pathways that cells use to create NAD+; but now, scientists have engineered a third. The new pathway uses chorismate as a starting molecule and, when introduced in *E. coli* cells, “yielded extremely high cellular concentrations of NAD(H)”. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.10.18.342451v1)
* A method to create many distinct species—which are very nearly genetically identical, but not able to reproduce with one another—has been reported for fruit flies. Scientists used the method to create eight “reproductively isolated” strains of fruit fly, but it could theoretically be used on any insect disease vector, including malaria-causing mosquitoes. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.08.09.242982v2.full.pdf)

*** 

## 📰 #SynBio in the News

## Story of the week:

* A wonderful story in *Undark* tells the story of Indian and Sri Lankan adoptees that are turning to genetic tests to understand their past. *Undark*. [Link](https://undark.org/2020/10/19/south-asian-adoptees-dna-tests/)
* The *New York Times* published a 40-minute audio interview with Jennifer Doudna. The promises and pitfalls of CRISPR are discussed. *New York Times*. [Link](https://www.nytimes.com/2020/10/22/opinion/sway-kara-swisher-jennifer-doudna.html)
* *Quanta*, last week, ran a feature on [Jeff Gore](http://www.gorelab.org/) and his work on biological physics, synthetic biology, and microbial communities. Some of my work at Caltech was deeply inspired by Gore’s findings, particularly his group’s studies related to how *quickly* a functional gene can arise from mutations in totally random DNA sequences. This article is worth your time. *Quanta Magazine*. [Link](https://www.quantamagazine.org/a-physicists-approach-to-biology-brings-ecological-insights-20201013/)
* Bioeconomy.xyz published a story about the history of bacteriophages, and how a company is using them in clinical applications. *Bioeconomy.xyz*. [Link](https://medium.com/bioeconomy-xyz/bacteriophages-harnessing-viruses-to-save-lives-9f47e25dba55)
* Biotechnology companies are being targeted in an onslaught of cyber attacks. *Labiotech.eu*. [Link](https://www.labiotech.eu/regulatory/cyberattack-biotech-startups-covid/)
* The Department of Defense awarded $87M to BioMADE “for a new Manufacturing Innovation Institute”. The goal of the new institute is to research and develop sustainable technologies for biological manufacturing. *DoD*. [Link](https://www.defense.gov/Newsroom/Releases/Release/Article/2388087/dod-approves-87-million-for-newest-bioindustrial-manufacturing-innovation-insti/)
* [Fifty Years](https://fiftyyears.com/), a VC firm in San Francisco, launched a new podcast called Translation, featuring interviews with the first authors of breakthrough papers in synthetic biology. [Link](https://fiftyyears.substack.com/p/introducing-the-translation-podcast)
* Audrey Teh, at St. George’s Hospital in London, is growing antibodies to fight cancer and COVID-19 in plants, in a greenhouse called “Skylab”. *Nature*. [Link](https://www.nature.com/articles/d41586-020-02938-6)
* Some biotechnology companies are going through multiple funding rounds in a single year; some have even gone public within 18 months from launch, setting a record pace (paywall). *STAT*. [Link](https://www.statnews.com/2020/10/19/multiple-fundraising-rounds-biotech/)
* Off-the-shelf CAR-T cell therapies may soon be available for patients with advanced B-cell lymphoma, according to preliminary clinical trial results reported by *STAT* on Oct. 21. *STAT*. [Link](https://www.statnews.com/2020/10/21/crispr-therapeutics-car-t-treatment-shows-encouraging-results-but-one-death-is-tied-to-therapy/)
* (Not synthetic biology) Nokia and NASA are building a cell network on the moon (in 2022). But it will be 4G—your internet connection on the moon will probably be slower than your grandmother’s Wi-Fi. *Forbes*. [Link](https://www.forbes.com/sites/roberthart/2020/10/19/nokia-to-build-cell-network-on-moon/#dfa68d3904d8)

***

Thanks for reading *This Week in Synthetic Biology*, which is supported by [Bioeconomy.XYZ](https://medium.com/bioeconomy-xyz).

Reach me with tips and feedback via Twitter [@NikoMcCarty](https://twitter.com/NikoMcCarty). I can handle your criticism.
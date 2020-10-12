---
layout: page
title: This Week in Synthetic Biology
---

**_This Week in Synthetic Biology_** is emailed to subscribers every Friday, and covers the latest research, preprints, and news in synthetic biology research.

This is the newsletter for October 9, 2020 (Issue 11). View the full archive on [Substack](https://synbio.substack.com/).

<iframe src="https://synbio.substack.com/embed" width="480" height="320" style="border:1px solid #EEE; background:white;" frameborder="0" scrolling="no"></iframe>

### [Data, Stored in DNA, Gets Destroyed](https://www.nature.com/articles/s41467-020-18842-6) (But In A Good Way)

DNA is promising for data storage, mainly because a single gram of DNA can store [256 petabytes](https://www.sciencemag.org/news/2017/03/dna-could-store-all-worlds-data-one-room#:~:text=Capable%20of%20storing%20215%20petabytes,may%20depend%20on%20its%20cost.) of information. But there’s a problem: DNA is, in some cases, *too* stable. To remove a user’s data from DNA on “nucleic acid hard drives” of the future, scientists first need to develop better ways to selectively target, and destroy, DNA. 

A new method, published in *Nature Communications*, could be a contender for wiping DNA hard drives in the year 2087 (assuming the human race survives that long). DNA sequences, each containing a “True” barcode and one, or several, “False” barcodes, are first mixed together. Then, "truth markers”—DNA sequences that selectively bind to the “True” sequences—are added to the mixture. If the mixture is then heated to 95 degrees Celsius, the “truth markers” fall off and information from the “True” bits is lost. It’s a simple technique, with promising results. 

The researchers showed that “8 separate bitmap images can be stably encoded and read after storage at 25 °C for 65 days with an average of over 99% correct information recall, which extrapolates to a half-life of over 15 years at 25 °C. Heating to 95 °C for 5 minutes, however, permanently erases the message.” 

### [Enzymatic Pathway ](https://pubs.acs.org/doi/abs/10.1021/acs.bioconjchem.0c00476)[Literally ](https://pubs.acs.org/doi/abs/10.1021/acs.bioconjchem.0c00476)[Built On A Virus](https://pubs.acs.org/doi/abs/10.1021/acs.bioconjchem.0c00476)

An enzymatic pathway has been assembled on top of a *Tobacco mosaic virus*. Using peptide “linkers”, the scientists, based in Hong Kong, tethered “three terpene biosynthetic enzymes” to the outer particles of the virus, and grew them inside of *E. coli* cells. The goal was to explore how the proximity of enzymes impacts the bioproduction of a molecule (in this case, amorpha-4,11-diene). 

Since the *Tobacco mosaic virus* is 300nm long, metabolic engineers could presumably use it as a foundation to assemble any number of complex enzymatic pathways. This study was published in *Bioconjugate Chemistry*.

### Deep Learning to Design RNA “Switches”

Two studies, published in *Nature Communications*, used deep learning to guide the engineering of RNA “toehold switches”. These RNA switches are, basically, synthetic RNA sequences that can be turned ON and OFF. In their OFF state, the toehold switches form a hairpin loop and cannot be read by the ribosomes—they do not produce a protein. The addition of an RNA “trigger”, however, can be used to turn a toehold switch ON; translation can proceed.

Toehold switches are especially useful because a *lot* of them can be present in a cell at the same time, and triggers can be designed for each of them. This means that many genes can be *precisely* controlled for synthetic biology applications. Unfortunately, toehold switches are really difficult to design, and even a slight tweak to a sequence can impact their utility. 

In the [first study](https://www.nature.com/articles/s41467-020-18677-1), led by Nicolaas M. Angenent-Mari, over 90,000 toehold switches were synthesized and tested using clever experiments that enabled the activity of each toehold switch to be individually assessed. After testing each of the RNAs, data was fed into a deep learning model (which I won’t even pretend to understand). The output from that model looks promising: “\[Deep Neural Networks\] trained on nucleotide sequences outperform (R2 = 0.43–0.70) previous state-of-the-art thermodynamic and kinetic models (R2 = 0.04–0.15).”

In the [second study](https://www.nature.com/articles/s41467-020-18676-2), led by Jacqueline Valeri, *two “*deep learning architectures” were introduced—called STORM and NuSpeak—to improve the performance of RNA toehold switches. Both studies are open access, and represent a paradigm shift in how quickly synthetic biologists will be able to design and engineer biological molecules that behave as expected.

### [Rice Engineered With C4 Photosynthetic Pathway](https://onlinelibrary.wiley.com/doi/10.1111/pbi.13487)

The *vast* majority of plants on earth are C3 plants; when it’s hot or dry, C3 plants close their stomas, oxygen builds up, and the efficiency of photosynthesis goes *down*. C4 plants, on the other hand, have figured out a way to avoid that pesky oxygen buildup. In C4 plants, fixation of entering carbon dioxide occurs in mesophyll cells, while the Calvin cycle instead occurs inside of bundle-sheath cells. This separation means that C4 cells can avoid oxygen buildup, and typically have a higher photosynthesis efficiency.

A new study in *Plant Biotechnology Journal* has introduced *five* genes into a specific strain of rice, boosting its photosynthetic flux by…well, only about 2%. But these early results look promising. If scientists can get the balance of gene expression right, it may one day prove useful for boosting rice yields, a staple food for more than half of the planet’s population.

### [Taking Measure of a Genetic Circuit](https://www.nature.com/articles/s41467-020-18630-2)

Biological circuits, operating inside of cells, can be built from dozens of individual genetic parts. Even a tiny tweak to one of those parts—a promoter, ribosome binding site, or terminator—can impact the performance of the genetic circuit. A new study exhaustively characterized all 54 parts in a circuit, parametrized them, and then used the data to build a mathematical model that could “predict circuit performance, dynamics, and robustness.” They even used the computed parameters to calculate “the cellular power (RNAP and ribosome usage) required to maintain a circuit state.” This study, published in *Nature Communications*, is open access.

***

### 🧫 Rapid-Fire Highlights

#### More research & reviews worth your time

* Gut microbes—packed into the convoluted *yuckiness* of our stomachs and intestines—can be selectively targeted with phages carrying dCas9. A single oral dose of a dCas9-carrying phage was able to selectively target, and repress, a single gene, inside of a bacterium, inside of a mouse’s gut. That’s, like, three layers deep. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18614-2)
* Organisms with an expanded genome (added X and Y base pairs, for example, in addition to A, T, G, and C), must also possess a DNA polymerase to *copy* those unnatural letters. But what “unnatural” polymerases are out there, and how are they engineered? That’s the topic of this excellent review. *The Journal of Biological Chemistry* (*Open Access*). [Link](https://www.jbc.org/content/early/2020/10/01/jbc.REV120.013745.full.pdf)
* A really elegant preprint from the [Leonard lab](https://www.leonard.northwestern.edu/) at Northwestern describes a “model-driven process” to construct and test genetic circuits in mammalian cells, without requiring trial-and-error. I was most impressed by the agreement they observed between their model and experiments, especially when testing logic operations (Figure 2). Though not mentioned in the main text, the authors used HEK293FT cells. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.09.30.320853v1.full.pdf)
* After screening 57 different protein domains, fused to dCas9, scientists have found the “most potent inhibitor” for repressing a gene: the ZIM3 KRAB domain. *Nature Methods.* [Link](https://www.nature.com/articles/s41592-020-0966-x)
* By using CRISPR to remove *one* allele of the *CCR2* gene, poplar plants had 10% less lignin. That’s a good thing, it turns out, because lignin makes it harder to extract sugar from crops. The “CRISPRed” plants did not grow any differently than normal plants, but their sugar could be extracted far more easily. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18822-w)
* While *Mycoplasma genitalium* might be the closest thing we have to a “minimal cell”, it could be even smaller. A new preprint has “simulated eight minimal gene sets from the literature” on *M. genitalium*, to see if any would grow and divide on the computer. The verdict? They didn’t. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.03.26.010363v4)
* Remember JCVI-syn3.0, the cell created by the J. Craig Venter Institute that lives, grows, and divides with just 473 genes? Well, I didn’t know this, but I guess it looks pretty sick. A new study has found that, by adding back just 19 genes to this “minimal genome”, the “striking morphological variation in JCVI-syn3.0 cells” can be removed. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.10.07.326892v1)
* Researchers in India reported the discovery of “iron-sensing bacterial riboswitches”, which are RNAs that bind to reduced iron, change their shape, and then mediate a genetic response. They are called “Sensei RNAs”. *Nature Chemical Biology*. [Link](https://www.nature.com/articles/s41589-020-00665-7)
* A new study used proteases—proteins which can cut other proteins—to construct genetic circuits, including an analog to digital converter. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18840-8)
* A new review discusses genome editing systems in various yeast species, including Baker’s yeast, *Pichia pastoris*, and *Yarrow lipolytica*. *Current Opinion in Biotechnology* (*Open Access*). [Link](https://www.sciencedirect.com/science/article/pii/S0958166920301191)
* Massively parallel reporter assays, or MPRAs, use clever DNA sequencing tricks to analyze how sequences near genes, like promoters, impact a gene’s expression. A new preprint from the Shendure lab offers a means to also analyze *trans*\-acting factors, like transcription factors, in these experiments. *bioRxiv* (*Open Access*). [Link](https://www.biorxiv.org/content/10.1101/2020.09.30.321323v1)
* A database for CRISPR/Cas9 and RNAi screens was published this week. Called CRISP-view, it curates datasets from 167 papers that used CRISPR or RNAi to probe the links between genetics and an organism’s phenotype. *Nucleic Acids Research* (*Open Access*). [Link](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkaa809/5917659)
* The Rios lab, in Edinburgh, wrote a nice review on multiplexed CRISPR (editing or controlling multiple genes at once) methods for yeast. *Frontiers in Bioengineering and Biotechnology*. [Link](https://www.frontiersin.org/articles/10.3389/fbioe.2020.589468/abstract)
* A clever study uses fluoride-responsive riboswitches, “hooked up” to a genetic circuit, to make engineered cells that perform biochemical reactions *only* when fluoride anions are present. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18813-x)
* CRISPRoff is a new, light-inducible method to degrade sgRNAs in living cells; if you shine a light, the engineered sgRNA fragments into pieces, and the CRISPR machinery winds down. *Nature Communications* (*Open Access*). [Link](https://www.nature.com/articles/s41467-020-18853-3#author-information)

***

### A Correction

In last week’s newsletter, I mentioned a research article describing engineered *E. coli* that can grow solely on carbon dioxide and formate. While writing about that study, I neglected some important, prior work. In February of this year, the group of Arren Bar-Even [engineered *E. coli*](https://www.nature.com/articles/s41589-020-0473-5) that could *also* grow on carbon dioxide and formate. That work was published in *Nature Chemical Biology*. I apologize for not including this information. 

***

### 📰 #SynBio in the News

* Doudna and Charpentier shared the Nobel Prize in Chemistry this week. Many outlets covered the story—[*The New York Times*](https://www.nytimes.com/2020/10/07/science/nobel-prize-chemistry-crispr.html) and [*Nature*](https://www.nature.com/articles/d41586-020-02765-9) had some nice coverage—but I am fond of *Quanta’s* news story. [Link](https://www.quantamagazine.org/2020-nobel-prize-in-chemistry-awarded-for-crispr-to-charpentier-and-doudna-20201007) 
* Scientists at UC-Berkeley (including Doudna, the Nobel Laureate) unveiled [Scribe Therapeutics](https://www.scribetx.com/), which plans to develop “an entirely new CRISPR platform that does not rely on molecules found in nature.” The company, which raised $20M in their Series A, hopes to use CRISPR to treat genetic diseases, including ALS. [Link](https://www.fiercebiotech.com/biotech/scribe-therapeutics-emerges-20m-biogen-pact-to-clear-crispr-hurdles)
* Do we need to change how life scientists track their progress, or assess their careers? A nice op-ed in bioeconomy.xyz takes a closer look. [Link](https://medium.com/bioeconomy-xyz/measuring-cultures-of-responsibility-in-the-life-sciences-390ad7ae3182)
* Medieval cesspits are a treasure trove of ancient microbiomes. A cool story from *Ars Technica*. [Link](https://arstechnica.com/science/2020/10/archaeologists-delved-into-medieval-cesspits-to-study-old-gut-microbiomes/)
* Enzymatic DNA synthesis companies, including [DNA Script](https://www.dnascript.com/) & [Ansa Biotechnologies](https://ansabio.com/), were covered in a *Nature Biotechnology* news story. [Link](https://www.nature.com/articles/s41587-020-0695-9)
* Kevin Davies wrote a new book, called “Editing Humanity: The CRISPR Revolution and the New Era of Genome Editing”. I haven’t read it, but I hear it’s pretty good. GenEng News interviewed the author. [Link](https://www.genengnews.com/insights/the-chronicles-of-crispr/)
* [Motif Foodworks](http://madewithmotif.com/), a spin-off from Ginkgo Bioworks, is preparing to launch their first commercial food product made with synthetic biology. [Link](https://techcrunch.com/2020/10/01/motif-foodworks-preps-commercial-production-for-its-first-ingredient-improving-the-flavor-of-beef-substitutes/)
* COVID-19 vaccines grown…in plants? Leslie Nemo reports for *Future Human*. [Link](https://futurehuman.medium.com/the-bold-attempt-to-grow-a-covid-19-vaccine-in-plants-53bc6b3cb77e)
* The [Howard Hughes Medical Institute](https://www.hhmi.org/) announced that they would require all of their scientists to make their papers free-to-read online. The policy won’t take effect until 2022. Reported in *Science*. [Link](https://www.sciencemag.org/news/2020/10/hhmi-one-largest-research-philanthropies-will-require-immediate-open-access)
* Phosphine on Venus may point to the existence of life, but…probably not. There are a lot of caveats, as Caleb Scharf explains in this piece for *Scientific American*. [Link](https://www.scientificamerican.com/article/lifes-small-molecule-problem/)

***

Thanks for reading *This Week in Synthetic Biology*, which is supported by [Bioeconomy.XYZ](https://medium.com/bioeconomy-xyz).

Reach me with tips and feedback via Twitter [@NikoMcCarty](https://twitter.com/NikoMcCarty). I can handle your criticism.
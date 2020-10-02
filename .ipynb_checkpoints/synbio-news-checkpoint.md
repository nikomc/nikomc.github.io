---
layout: page
title: This Week in Synthetic Biology
---

**_This Week in Synthetic Biology_** is emailed to subscribers every Friday, and covers the latest research, preprints, and news in synthetic biology research. [Sign up for the newsletter](https://synbio.substack.com/).

This is the newsletter for October 2, 2020 (Special Issue 10). View the full archive on [Substack](https://synbio.substack.com/).

🌄Good morning.

This week’s issue is focused on the intersection of machine learning and synthetic biology. Two articles were published this week in *Nature Communications* ([read the press release](https://newscenter.lbl.gov/2020/09/25/machine-learning-takes-on-synthetic-biology-algorithms-can-bioengineer-cells-for-you/)) by scientists at the Lawrence Berkeley National Laboratory and the Department of Energy’s Joint BioEnergy Institute, describing a machine learning framework that helps metabolic engineers maximize production of specific molecules (most of the time).

I was seriously impressed by the papers, but I did want to briefly use these studies as an opportunity to espouse the merits of gaining mechanistic understandings as scientists. New machine learning tools may be able to predict an “optimized” metabolic pathway by analyzing datasets from dozens, or hundreds, or thousands of experiments, but they will not provide metabolic engineers with a greater understanding of *why* this combination of proteins, or that batch of promoters, led to a desired outcome. The tool that the authors 

In the two studies, the authors use a machine learning framework (called Automated Recommendation Tool, or ART for short), that can speed up the “Learn” phase of the Design-Build-Test-Cycle. Notably, the tool operates “without the need for a full mechanistic understanding of the biological system.”

One of my *least* favorite articles is a [2008 op-ed in ](https://www.wired.com/2008/06/pb-theory/)[*WIRED*](https://www.wired.com/2008/06/pb-theory/) by Chris Anderson, who was, at the time, editor in chief of that magazine. In that article, he writes that, when “faced with massive data, this approach to science — hypothesize, model, test — is becoming obsolete.” Obviously, that prediction has not come true, and that was *before* machine learning became one of the hottest topics in biology, eager (and, maybe one day, able) to solve all of our experimental problems.

So, while this issue of *This Week in Synthetic Biology* pays homage to machine learning and synthetic biology, and all the wonderful things that they can do together, I hope that synthetic biologists do not lose sight of what it means to be a *biologist*; to be in tune with the wonders and intricacies of life. 

Or, as my undergraduate research mentor used to say, “That’s neat and all, but what’s the mechanism?”

### 🧬Featured Research

#### [Machine Learning Guides Metabolic Engineering; Or, “What Next, Robot?”](https://www.nature.com/articles/s41467-020-18008-4) (Open Access)

The first study by the Berkeley-based researchers describes ART (Automated Recommendation Tool), which is built primarily on Python’s popular [scikit-learn](https://scikit-learn.org/stable/) library. It is a machine learning framework that can help researchers maximize target molecule production, decrease cellular toxicity, or tune the level of a metabolite to a specified concentration. And it works *most* of the time. For example, the researchers used it to engineer *E. coli* and *S. cerevisiae* to produce limonene, to “synthesize metabolites that produce hoppy flavor in beer”, and to manufacture dodecanol from fatty acids. In the last example—dodecanol—it didn’t really provide meaningful predictions, despite being fed data from 50 instances of the engineering cycle. Still, the tool seems useful, and it’s worth checking out. This study was published in *Nature Communications*.

#### [Machine Learning Helps Optimize Tryptophan Biosynthesis in Cells](https://www.nature.com/articles/s41467-020-17910-1) (Open Access)

In the follow-up paper, which was also published in *Nature Communications*, ART was used to improve tryptophan production in engineered *S. cerevisiae*. In this case, it seemed to work really well. Choosing from 7776 combinatorial options (consisting of five different genes, controlled by six promoters, selected from a batch of thirty available promoters), ART successfully identified “designs exhibiting up to 74% higher tryptophan titers than best designs used for training the models.” Still, the researchers had to collect a *lot* of data to train predictive models. They collected more than 120,000 time series data points and generated more than 500 different yeast strains during the study.

#### [Use Your Pasta Maker to Extract DNA. I Know You Want To.](https://www.nature.com/articles/s41596-020-0392-7) (Open Access)

In 30 seconds, you can use “cellulose-based dipsticks” to extract nucleic acids. At least, that’s what a new method, described in *Nature Protocols*, says. Each dipstick (hundreds of which, apparently, can be made in less than 30 minutes) is “dipped” into three buffers: an extract buffer that binds nucleic acids, a wash buffer that removes contaminants, and an amplification buffer “to elute the nucleic acids.” Oh, you’ll also need a pasta maker.

The authors of this study “use a low-cost, unbranded pasta maker purchased through Ebay that is equivalent to an Avanti pasta maker machine (Avanti, cat. no. 26812). However, any brand of pasta maker should work.” Phew, I was worried my Cucina Pro wouldn’t cut it!

#### [Engineered Bacteria Grow Solely on CO2 and Formic Acid](https://www.nature.com/articles/s41564-020-00793-9)

*E. coli,* engineered with synthetic carbon dioxide and formic acid assimilation pathways (and a slew of other tune-ups), can grow solely on carbon dioxide and formic acid. The study, published in *Nature Microbiology*, was conducted by [Sang Yup Lee’s](http://mbel.kaist.ac.kr/lab/family/professor.html) group at the Korea Advanced Institute of Science and Technology. It follows a study from 2019, in which Ron Milo’s group [engineered ](https://www.cell.com/cell/pdf/S0092-8674(19)31230-9.pdf)[*E. coli* ](https://www.cell.com/cell/pdf/S0092-8674(19)31230-9.pdf)[to derive carbon solely from carbon dioxide](https://www.cell.com/cell/pdf/S0092-8674(19)31230-9.pdf) (with formate as a reducing agent). 

#### [A Viral Gene Drive](https://www.nature.com/articles/s41467-020-18678-0) (Open Access)

Viral gene drives have arrived. Using human cytomegalovirus (a form of herpesvirus), Marius Walter & Eric Verdin from the [Buck Institute for Research on Aging](https://www.buckinstitute.org/) developed a gene drive that can propagate through a population of viruses. When two viruses infect a host cell—one with the gene drive, and the other without—the Cas9 on the gene drive cleaves the wildtype sequence. The cut sequence then uses the “gene drive sequence as a repair template”, thus converting the wildtype locus into a new gene drive sequence. It’s a simple, but effective, method to propagate a genetic element in viruses. The study was published in *Nature Communications*.

***

### 🧫 Rapid-Fire Highlights

#### More research & reviews worth your time

* A stiff, functional material made *entirely from living cells* (no biopolymers or biominerals) was created by the Joshi lab. My favorite study this week. *bioRxiv*. [Link](https://www.biorxiv.org/content/10.1101/2020.09.24.311589v1) (*Open Access*)
* DNA nanoswitches were programmed to alter their shape in response to various viral RNAs, including Zika and SARS-CoV-2. The “activated” DNA nanoswitches can be detected by gel electrophoresis. *Science Advances.* [Link](https://advances.sciencemag.org/content/6/39/eabc6246) (*Open Access*)
* A lab-evolved strain of *E. coli* can use “acetate as its sole carbon and energy source”. It was, in turn, engineered to produce mevalonate and n-butanol. *Metabolic Engineering*. [Link](https://www.sciencedirect.com/science/article/abs/pii/S1096717620301464)
* β-xylosidase, an enzyme that hydrolyzes D-[xylose](https://en.wikipedia.org/wiki/Xylose) sugars, was engineered to “form O-, N-, S- and Se- glycosides together with sugar esters and phosphoesters”. The mutant enzyme is called a thioglycoligase. *Nature Communications*. [Link](https://www.nature.com/articles/s41467-020-18667-3) (*Open Access*)
* [A web tool](http://pegfinder.sidichenlab.org/) can design pegRNAs for your next prime-editing experiments. *Nature Biomedical Engineering*. [Link](https://www.nature.com/articles/s41551-020-00622-8)
* Prime-editing was used in adult stem cells to correct “disease-causing mutations in…liver organoids from a patient with Wilson disease”, a rare genetic disorder that causes copper to build-up in the liver, brain, and eyes. *bioRxiv*. [Link](https://www.biorxiv.org/content/10.1101/2020.06.09.139782v2.full.pdf) (*Open Access*)
* A review on how CRISPR–Cas systems can enhance plant yields, help plants fend off disease, and accelerate domestication, was published. *Nature Reviews Molecular Cell Biology*. [Link](https://www.nature.com/articles/s41580-020-00288-9)
* Another review on CRISPR-Cas in plants, but for cotton, specifically. *Trends in Biotechnology*. [Link](https://www.cell.com/trends/biotechnology/fulltext/S0167-7799(20)30235-3)
* Archaea produce some weird lipids, like the mouth-garbling “C25, C25-archaeal diether-type membrane lipids”. Now, engineered *E. coli* can produce them, too. *Synthetic Biology.* [Link](https://academic.oup.com/synbio/advance-article/doi/10.1093/synbio/ysaa018/5913399) (*Open Access*)
* A new Cas9 fusion nuclease, called Cas9-N57, can site-specifically integrate DNA up to 12 kb in length. *Nucleic Acids Research*. [Link](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkaa779/5912567) (*Open Access*)
* An adenine base editor (which can convert A•T to G•C in genomic DNA) was engineered to have enhanced “on-target editing efficiency” and reduced off-target effects. *Nature Communications*. [Link](https://www.nature.com/articles/s41467-020-18715-y) (*Open Access*)
* The Church lab developed a synthetic auxotrophic strain of *E. coli* that was unable to escape from biocontainment, even after 100 days of continuous growth. *bioRxiv*. [Link](https://www.biorxiv.org/content/10.1101/2020.09.27.315804v1.abstract?%3Fcollection=) (*Open Access*)
* Curious about the financial potential of DNA storage? A new review covered that. *Biotechnology Advances*. [Link](https://www.sciencedirect.com/science/article/pii/S0734975020301415) (*Open Access*)
* Synthetic cells are nowhere near as packed as real cells, which have dense interiors crowded with proteins, nucleic acids, and molecules. Now, the “crowded cytoplasm” of cells has been recreated in protocells. Spoiler alert: It changed diffusion rates and, in turn, transcription and translation. *ACS Synthetic Biology*. [Link](https://pubs.acs.org/doi/10.1021/acssynbio.0c00330#)
* Researchers in Bristol engineered a two-heme binding protein, called 4D2, solved its structure, and then further engineered it to create a range of heme binding proteins. *bioRxiv*. [Link](https://www.biorxiv.org/content/10.1101/2020.09.24.311514v1.full) (*Open Access*)
* Every. Single. Residue in the tip domain of T7 bacteriophage was swapped out to help determine the role of each amino acid in mediating bacteriophage:host interactions. Researchers tested 1660 variants in total. *bioRxiv*. [Link](https://www.biorxiv.org/content/10.1101/2020.07.28.225284v2.abstract?%3Fcollection=) (*Open Access*)
* The so-called Z-ring (made primarily of FtsZ and FtsA) initiates bacterial cell division. Now, a new study has reconstituted FtsA-FtsZ “ring-like structures” entirely with cell-free gene expression *inside* of liposome compartments. It’s an important step towards programmable, dividing cells, built from the bottom-up. *Communications Biology*. [Link](https://www.nature.com/articles/s42003-020-01258-9) (*Open Access*)
* An article in *EMBO Reports* details “a policy framework for transitioning towards a sustainable carbon cycle economy.” Synthetic biology can help with that. *EMBO Reports*. [Link](https://www.embopress.org/doi/epdf/10.15252/embr.202051478)
* A variant of ubiquitin was engineered that can conditionally regulate the stability—and expression level—of proteins to which it is fused. *Cell Chemical Biology*. [Link](https://www.cell.com/cell-chemical-biology/fulltext/S2451-9456(20)30376-7)

***

### 📰 #SynBio in the News

***(Not a lot this week)***

* Alden Wicker, a veteran fashion journalist, wrote about “[carbon-neutral, recyclable, biodegradable, and affordable materials](https://neo.life/2020/09/get-up-to-speed-on-the-state-of-eco-fashion/)” for Neo.Life.
* Matthias Berninger, the Head of Public Affairs, Science, and Sustainability at Bayer, [was interviewed for a Bioeconomy.xyz](https://medium.com/bioeconomy-xyz/science-sustainability-business-politics-and-a-hint-of-chocolate-a3b4a95b64a1) article.
* Base editing was used to cure inherited deafness in mice by repairing a mutation in a gene called *TMC1*. Emily Mullin [reported for OneZero](https://onezero.medium.com/a-new-gene-editing-treatment-let-deaf-mice-hear-again-661c4080c83).

***

Thanks for reading *This Week in Synthetic Biology*, which is supported by [Bioeconomy.XYZ](https://medium.com/bioeconomy-xyz).

Reach me with tips and feedback via Twitter [@NikoMcCarty](https://twitter.com/NikoMcCarty). I promise I can handle the criticism.
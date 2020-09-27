---
layout: page
title: This Week in Synthetic Biology
---

**_This Week in Synthetic Biology_** is emailed to subscribers every Friday, and covers the latest research, preprints, and news in synthetic biology research. [Sign up for the newsletter](https://synbio.substack.com/).

This is the newsletter for September 25, 2020 (Issue 9). View all prior issues on [Substack](https://synbio.substack.com/).

### 🧬Featured Research

#### [100+ Promoters Dissected with Base-Pair Resolution (Open Access)](https://elifesciences.org/articles/55308)

During my time at Caltech, I contributed to a study (led by Bill Ireland and Suzy Beeler) that was published in *eLife* this week. In this study, Bill and Suzy created an experimental tool, called Reg-Seq, that combines massively parallel assays with mass spectrometry to determine the nucleotide-by-nucleotide contribution to DNA binding energy for 100+ promoters. With this method, we can determine where transcription factors (activators and repressors) cling to DNA, and then use this information to design new promoters with predictable expression levels. There is also a suite of [online resources](https://github.com/RPGroup-PBoC/RegSeq) that we created, including code, tutorials, and [an interactive figure](https://www.rpgroup.caltech.edu/RegSeq/interactive) so that you can look at the data for 100+ *E. coli* promoters yourself.

#### [Genetic Overhaul Brings Pigs Closer to Viable Organ Donors](https://www.nature.com/articles/s41551-020-00613-9)

Xenotransplantation (taking an organ from one animal to give to another) is an ever-present theme in fiction; it appears in writings by Kazuo Ishiguro and Neal Shusterman, for example. A new study, published in *Nature Biomedical Engineering*, has brought xenotransplantation (from pigs to humans) one tiny step closer to reality. [Luhan Yang](https://www.ted.com/speakers/luhan_yang) (co-founder of a xenotransplantation company) and [George Church](http://arep.med.harvard.edu/)’s group collaborated on the study. The researchers first deactivated all porcine endogenous retroviruses in pigs, which is crucial to prevent cross-species transmission of the virus ([which is infectious to humans](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4997577/#:~:text=preferred%20donor%20animals.-,PERVs%20are%20released%20from%20normal%20pig%20cells%20and%20are%20infectious,pose%20a%20risk%20for%20xenotransplantation.)). Then, they engineered the pigs to express nine human transgenes that “enhance the pigs’ immunological compatibility and blood-coagulation compatibility with humans”. Fiction is one step closer to reality.

#### [CRISPR Detects Malaria, Including Asymptomatic Cases](https://www.pnas.org/content/early/2020/09/15/2010196117) (Open Access)

The [World Health Organization estimates](https://www.who.int/news-room/fact-sheets/detail/malaria) that there were 228 million cases of malaria in 2018. Rapid, easy testing for malaria could go a long way in combatting this global threat (which has [likely killed more people than any disease in human history](https://www.nature.com/articles/news021001-6)). A new CRISPR-based system, developed by the [Collins lab at MIT](https://collinslab.mit.edu/), can be used to diagnose the “four major pathogenic *Plasmodium* species”, and it can do it in 60 minutes with an astounding sensitivity. In the case of *Plasmodium falciparum*, they could detect a single parasite in about three microliters of blood. The study was published in *PNAS*. [Read the Wyss Institute news piece](https://wyss.harvard.edu/news/crispr-based-malaria-testing-on-the-fly/), too.

#### [Artificial Cells “Talk” to Mammalian Neighbors](https://advances.sciencemag.org/content/6/38/eabb4920) (Open Access)

Artificial cells are lipid spheres, usually packed with some protein and DNA, that can be programmed to carry out a simple task, like glow green or produce a protein from a DNA template. From a historical perspective, artificial cells have been quite simple until recently. Now, new research has taken these protean cells one step further, demonstrating the creation of artificial cells that can chemically communicate with mammalian cells under physiological conditions. [Researchers](https://www.simonsfoundation.org/team/sheref-s-mansy/) in Trento, Italy and Alberta, Canada created the cells from POPC (a type of phospholipid) and cholesterol and packaged them with DNA templates to synthesize a neurotrophic factor. When these artificial cells sense a specific small molecule in their environment, they switch on their genetic program, synthesize the neurotrophic factor, and “send it” to a neighboring neuron, triggering neuronal differentiation. This study was published in *Science Advances*.

***

### 🧫 Rapid-Fire Highlights

#### More research & reviews worth your time

* *E. coli* cells were [engineered to produce 2′ fucosyllactose](https://pubs.acs.org/doi/10.1021/acssynbio.0c00304), a sugar in human breast milk, from sucrose (*ACS Synthetic Biology*).
* Protein switches (called Co-LOCKR) have been created that can [bind antigens on a cell’s surface and change their structure](https://science.sciencemag.org/content/369/6511/1637) only when they encounter a “precise combination of antigens.” It’s logic, built into a protein (*Science*).
* [Two new “genetic neutralizing elements”](https://www.sciencedirect.com/science/article/abs/pii/S1097276520306110) could help prevent gene drives from ‘leaking’ into the environment (*Molecular Cell*). [Read the UCSD press release.](https://ucsdnews.ucsd.edu/pressrelease/biologists-create-new-genetic-systems-to-neutralize-gene-drives)
* Providing finer control over resources in a cell, a “dual controller” circuit can [independently control transcription or translation](https://www.sciencedirect.com/science/article/abs/pii/S2405471220303252) (*Cell Systems*).
* Remember the CRISPR babies? A study found that He Jiankui’s work likely [decreased acceptance of genome editing in China](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0238128) (*PLoS One*). *Open Access.*
* Prime editors can make various genetic changes in a cell, without causing double-stranded breaks in DNA. A [new study evaluated “54,836 pairs of prime editing guide RNAs and their target sequences”](https://www.nature.com/articles/s41587-020-0677-y) to determine the factors that govern prime editing efficiencies (*Nature Biotechnology*).
* Short, regulatory RNA molecules regulate gene expression in mammalian cells. [Now, these RNAs can be regulated in space and time](https://www.nature.com/articles/s41467-020-18673-5)—with light (*Nature Communications*). *Open Access*.
* [“History-dependent” genetic circuits](https://www.nature.com/articles/s41467-020-18455-z) can control the expression of different genes in living cells based on the order of input signals (*Nature Communications*). [Read behind-the-paper](https://bioengineeringcommunity.nature.com/posts/rational-programming-of-history-dependent-logic-in-cellular-populations). *Open Access.*
* [DNA nanoswitches were used to detect six biomarkers](https://www.biorxiv.org/content/10.1101/2020.09.22.309104v1) (from six different diseases), in a single test tube, at one time (*bioRxiv*). *Open Access*.
* Can [machine learning models predict the abundance of different proteins](https://www.biorxiv.org/content/10.1101/2020.09.17.302182v1.abstract?%3Fcollection=) in a cell? A new preprint looks like a promising start (*bioRxiv*). *Open Access*.
* A protocol [outlined efficient genetic knockouts in a polyploid fruit fly cell line](https://www.nature.com/articles/s41596-020-0383-8). The method is useful for knocking out genes with a high copy number (*Nature Protocols*).
* Last week, I [featured a study in ](https://www.nejm.org/doi/full/10.1056/NEJMc2026172)[*NEJM*](https://www.nejm.org/doi/full/10.1056/NEJMc2026172) that used CRISPR to detect SARS-CoV-2. Shortly thereafter, a similar [study was published](https://www.nature.com/articles/s41467-020-18575-6) that also used CRISPR-Cas12a to detect SARS-CoV2, and also did not require a separate amplification step (*Nature Communications*). *Open Access.*
* In more COVID-19 diagnostic news, a [study was published](https://www.nature.com/articles/s41551-020-00617-5) that uses fluorescent probes to detect SARS-CoV-2 RNA, with an exceptionally low detection limit (*Nature Biomedical Engineering*). *Open Access.*
* A [specific type of neural network](https://arxiv.org/pdf/1812.08434.pdf#:~:text=Graph%20neural%20networks%20(GNNs)%20are,its%20neighborhood%20with%20arbitrary%20depth.) was [used to generate proteins that, when folded, adopt a specified topology](https://www.cell.com/cell-systems/fulltext/S2405-4712(20)30327-6). It is reportedly 100x faster than alternative methods to predict protein topologies (*Cell Systems*). *Open Access*.
* A preprint from the Church lab used computer-aided designs to create [genetic circuits that can control how human cells ](https://www.biorxiv.org/content/10.1101/807107v2.abstract?%3Fcollection=)grow into three-dimensional shapes (*bioRxiv*). *Open Access.*
* Biosensor system were used to [measure how proteins are created](https://www.biorxiv.org/content/10.1101/2020.09.18.303453v1.abstract?%3Fcollection=), and folded, in living cells (*bioRxiv*). *Open Access.*
* A preprint from David Baker’s lab reported the [creation of two-dimensional materials](https://www.biorxiv.org/content/10.1101/2020.09.19.304253v1), made from co-assembling proteins, that can be tuned and reconfigured by design (*bioRxiv*). *Open Access.*
* A new study (with goat cells!) tested [which method is best for extracting genomic DNA](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0239435) when evaluating CRISPR edits (*PLoS One*). *Open Access*.
* Videos, books, and [entire Netflix documentaries](https://www.youtube.com/watch?v=DMYgjOHgHxc) have been encoded and stored in DNA. But [how should synthetic DNA be stored](https://www.biorxiv.org/content/10.1101/2020.09.19.304014v1) to ensure its data can be retrieved in ten years, or a thousand? A new preprint weighed the options (*bioRxiv*). *Open Access.*
* In more “DNA storage” news, a study has used TNA (α-L-threofuranosyl nucleic acid) to [store a mighty 23 kB of information](https://pubs.acs.org/doi/10.1021/acssynbio.0c00361) and then recover it “with perfect accuracy after exposure to biological nucleases that destroyed equivalent DNA messages” (*ACS Synthetic Biology*).

***

### 📰 #SynBio in the News

* Matthew Hutson wrote a nice [feature on David Baker, designer proteins, and COVID-19](https://www.newyorker.com/tech/annals-of-technology/the-promise-of-designer-protein-in-the-fight-against-covid-19) for *The New Yorker*.
* To curb agricultural damage, Oxitec (the same company that is releasing GM mosquitoes in the Florida Keys) has “created a caterpillar with self-destructing eggs”. [*WIRED* ](https://www.wired.com/story/can-a-genetically-modified-bug-combat-a-global-farm-plague/)[covered this story](https://www.wired.com/story/can-a-genetically-modified-bug-combat-a-global-farm-plague/).
* A Policy Forum, published in *Science*, argues that a [“global citizens' assembly” should inform the governance of genome editing](https://science.sciencemag.org/content/369/6510/1435.summary).
* Sudeep Agarwala, a yeast geneticist at Ginkgo Bioworks, [wrote a great essay](https://www.growbyginkgo.com/2020/09/24/the-food-of-exiles/) for *Grow* on food, memory, and the future (with a subtle touch of yeast).
* A story I missed last week; the *New York Times* [published a piece on mycelium and faux leather](https://www.nytimes.com/2020/09/16/science/fungus-leather.html), featuring [MycoWorks](https://www.mycoworks.com/) and [Bolt Threads](https://boltthreads.com/).
* *Chemical & Engineering News* published a [feature on “gas-to-protein” fermentation](https://cen.acs.org/food/food-ingredients/start-ups-succeed-making-food/98/i36). The goal? To feed “the world with protein made from air or industrial exhaust with minimal use of water and land”.

***

Thanks for reading *This Week in Synthetic Biology*, which is supported by [Bioeconomy.XYZ](https://medium.com/bioeconomy-xyz).

Reach me with tips and feedback via Twitter [@NikoMcCarty](https://twitter.com/NikoMcCarty).
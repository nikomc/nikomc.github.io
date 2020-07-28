---
layout: post
title:  "Early Steps to Create a Synthetic, “Mirrored” Organism"
tags: [ science, synthetic biology]
featured_image_thumbnail:
featured_image: assets/images/posts/2020/ribosome_cartoon.jpg
featured: true
hidden: true
---

George Church, the famous Harvard geneticist, has [famously espoused](https://www.wired.com/2010/11/ff_mirrorlife/) the potential of “mirrored” organisms — living creatures built exclusively with chiral molecules. This idea even featured in his excellent book, [Regenesis](https://www.amazon.com/Regenesis-Synthetic-Biology-Reinvent-Ourselves/dp/0465075703), which was co-authored by [Ed Regis](https://en.wikipedia.org/wiki/Ed_Regis_(author)). Though such organisms are not found in nature, a synthetic “mirrored” organism would be entirely immune from viral infection and could be used to manufacture a new suite of [enantiopure pharmaceuticals](https://en.wikipedia.org/wiki/Enantiopure_drug). All organisms on earth synthesize proteins using exclusively L-amino acids[^1], but perhaps the early steps in creating a “mirrored” organism would best be pursued through the engineering of the ribosome, that great molecular machine underpinning translation.

To date, laboratories have succeeded in creating ribosomes that read orthogonal mRNA messages[^2], stochastically incorporate β-amino acids[^3] or introduce unnatural α-amino acids into proteins within cells by modifying key residues in the ribosome and associated translational machinery[^4]. D-amino acids have been incorporated into polypeptide chains _in vitro_[^5], but efforts to do so _in vivo_ have proven more difficult.

In all organisms, an aminoacyl tRNA synthetase (aaRS) acylates a cognate tRNA with the appropriate L-amino acid[^6]. The D-amino acid-tRNA deacylase (DATD) removes D-amino acids that have been misacylated onto tRNAs[^7]. Elongation Factor Thermo unstable (EF-Tu) transports acylated tRNAs to the A-site of the ribosome, where the anticodon of the incoming tRNA binds to its complementary mRNA codon[^6]. Peptide bond formation occurs when the GTP bound to EF-Tu is hydrolyzed, EF-Tu dissociates, and the amino acid is positioned near the growing polypeptide chain in the ribosome P site[^6], a process shown in the figure below.

{% include image-caption.html imageurl="/assets/images/posts/2020/figure2_ribosome_chiral.png#wide" title="Strategy to engineer ribosome to incorporate D-amino acids." caption="Schematic depicting the general mechanism of prokaryotic translation. The tRNA is acylated by its aminoacyl tRNA synthetase before being transported to the ribosome by EF-Tu. The ribosome adds the amino acid to the growing peptide chain following GTP hydrolysis and EF-Tu release. EF-G signals the ribosome via GTP hydrolysis to move one codon along the mRNA template, with the departure of the E-site tRNA. Images captured in PyMOL. PDB IDs: 4V5L, 3MF2, 2BM0." %}

Early supramolecular crystal structures implicated domain V of the 23S rRNA as the peptidyl-transferase center (PTC) of the ribosome[^8][^9]. The mechanism by which the PTC catalyzes peptide bond formation is via positioning of the translational components by hydrogen bond formation, a feat achieved when an incoming, acylated tRNA induces conformational shifts in the PTC of the ribosome[^10]. To incorporate unnatural amino acids into cells, amber codon suppression is used, wherein the stop codon UAG, which normally recruits release factor 1 (RF1) to signal translation end, is instead decoded by an aminoacylated amber suppressor tRNA to introduce an amino acid[^4]. Ribo-X, an evolved orthogonal ribosome that improved the decoding of amber codons on orthogonal mRNAs and has decreased affinity for RF1, was used to successfully increase site-specific unnatural amino acid incorporation efficiency[^2]. An orthogonal ribosome that efficiently decodes quadruplet codons has also been created[^11]. An orthogonal ribosome in which the ribosomal RNA in the two subunits are covalently linked through an RNA staple has also been engineered[^12]. This RNA staple may enable directed evolution of the large subunit, including the PTC. Further engineering of these orthogonal translation systems could be used to incorporate D-amino acids _in vivo_, drastically expanding the chemical space available to living cells. Importantly, D-amino acids could be used to create partially mirrored organisms without biocontainment hazards[^13] and a cell engineered to incorporate D-amino acids into peptides could be used to produce peptide pharmaceuticals with protease resistance for neurological and infectious diseases[^14].


***

To engineer the ribosome and associated translational machinery in _E. coli_ to facilitate the incorporation of D-amino acids into polypeptides _in vivo_, a few engineering hurdles must first be surmounted. First, the co-translational incorporation of D-amino acids _in vivo_ requires that the aaRS enzymes are able to recognize and utilize the chiral molecules. Additionally, the D-amino acids must be stable in cells, without undergoing racemization, EF-Tu must deliver the D-amino acids to the ribosome, and the ribosome must, finally, faciliate peptide bond formation and translational elongation with the D-amino acids.

_In vitro_ experiments have shown that five different aaRS can charge their cognate tRNA with D-amino acids, including aspartic acid, histidine, lysine, tryptophan and tyrosine[^15]. To begin, it is necessary to develop an orthogonal tRNA/aaRS system which has strong affinity to EF-Tu and stable binding to the A-site of the ribosome. Crystal structures of orthogonal aaRS/tRNA pairs of the two classes (I and II), including tRNA(Tyr)-TyrRS from _M. jannaschii_, tRNA(Amber)-PylRS from _M. barkeri_ and tRNA(Lys)-LysR from _P. horikoshii_ could be simulated via molecular dynamics in Gaussian[^3] with their native L-amino acids and D-isomers to identify residues implicated in substrate binding and proofreading _in silico_. From this information, one could systematically mutate identified residues and screen for aaRS-tRNA pairs that successfully acylate D-amino acids. Aminoacylation rates of the mutant tRNAs with D-amino acids could be measured _in vitro_ using a chemical quench assay and stopped-flow fluorescence to determine the optimal tRNA-aaRS pair to use for the _in vivo_ experiments[^16].

The engineered _E. coli_ must create sufficient quantities of the D-amino acid of interest for peptide incorporation without racemization. To express the D-amino acid, a metabolic engineering approach can be employed, in which DAHP synthase and chorismite mutase-prephenate dehydratase from _E. coli_, together with a D-amino acid aminotransferase from _B. sphaericus_, a deaminase from _P. myxofaciens_ and a racemase, are placed on a single operon and transformed into _E. coli_[^17]. This engineered metabolic pathway would then produce the D-amino acid in vivo, but the expression of each enzyme must be adjusted to optimally express the D-amino acid without causing toxicity. _E. coli_ naturally express racemases which convert L- and D-amino acids; to repress the activity of undesirable racemases, which could decrease the expression of the desired D-amino acid _in vivo_, inducible promoters could be encoded upstream of their coding regions for precise control of racemase expression. Since racemases are necessary to prevent toxic build-up of D-amino acids _in vivo_, their expression should be turned ‘on’ during normal cell growth and temporarily turned ‘off’ for experiments. To prevent deacylation of tRNAs aminoacylated with the D-amino acids, it is also necessary to delete the non-essential DATD gene in the engineered _E. coli_.

EF-Tu enhances the proofreading capabilities of the ribosome, reducing the free-energy barrier during accommodation of the incoming tRNA via its elbow domain[^7]. A ribosome stalled with kirromycin in complex with Phe-tRNA∙EF-Tu∙GDP indicated a hydrophobic gate in EF-Tu as controlling GTPase activation[^18]. EF-Tu has been engineered to carry D-aa-tRNAs (in vitro experiments in which tRNAs were chemically acylated) to the ribosome. Surprisingly, both wild-type EF-Tu and an N273S mutant formed stable tertiary complexes with D-aa-tRNA[^7].

Finally, the ribosome must be engineered to intake the appropriate tRNA∙EF-Tu∙GTP, trigger GTP hydrolysis and shift the incoming tRNA from the A to P site. This engineered ribosome must read orthogonal mRNA sequences containing both Shine Dalgarno sequences not recognized by endogenous ribosomes and the Amber codon (UAG) encoding the D-amino acid. Therefore, the stapled orthogonal ribosome system mentioned previously could be adapted (henceforth called ribo-D). Ribosomal regions which require modification include the PTC and helix 89 of 23S rRNA[^5]. The stapled orthogonal ribosome could be mutated in positions 2447–2450 (PTC) and 2457–2462 (helix 89) to a generate a library of potential D-amino acid incorporating ribosomes in _E. coli_.

To screen for mutant ribosomes that incorporate D-amino acids in the engineered _E. coli_, the selection of an appropriate discriminator is necessary. The UAG Amber codon could be inserted into the chloramphenicol acetyltransferase (Cat) gene, which confers resistance to chloramphenicol in _E. coli_. The Amber codon would then be placed in a site of the mRNA which is distant from the functional domain in the folded protein, so as not to affect its activity. The Cat gene containing the Amber codon and an orthogonal Shine-Dalgarno sequence would then be expressed in the engineered _E. coli_. Ribosomal mutants could be screened at varied concentrations of chloramphenicol, with growth of _E. coli_ at high chloramphenicol concentrations denoting production of functional Cat by the ribo-D[^2]. To confirm, the Cat protein could also be purified and digested with trypsin to yield small fragments. These small peptides would then be analyzed by chiral reverse-phase HPLC and compared to authentic diastereomeric standards made by solid phase peptide synthesis[^1].

***

This technical write-up provides a potential avenue to engineer the ribosome and other relevant, cellular machinery for _in vivo_ chiral peptide production, which would decrease the labor and expense associated with solid phase synthesis, while expanding the precision and diversity of peptides which can be manufactured with D-amino acids. The production of a cell capable of integrating D-amino acids would greatly advance basic biological science by allowing scientists to probe the basis for the evolution of living cells to almost exclusively L-stereoisomers[^7]. Additionally, partially chiral cells are resistant to bacteriophage infection and can be built with strict containment controls, making them ideal for large manufacturing processes prone to phage and for environmental sensing and bioremediation applications[^13]. Finally, this engineered organism, developed with both protein and metabolic engineering methodologies, could be used to produce peptide-based therapies with chiral amino acids inserted into protease recognition sites, which has been shown to significantly expand peptide half-life and minimize the injections necessary for peptide-based therapies[^19]. Peptides are already used as therapies for cancers, infectious and neurological diseases, including polyglutamine and Huntington’s disease, _A. fumigatus_ fungal infection and in G protein-coupled receptor and ion channel disorders[^20][^21][^22].

***

#### Notes:

This is a technical proposal, and was never intended for a general audience. My sincere apologies for the terrible jargon!

This article was also posted on [Medium](https://medium.com/@NikoMcCarty/a-first-step-to-create-synthetic-mirrored-organisms-4f70fbbaf1e).

Featured image from [Flickr user redondoself](https://www.flickr.com/photos/redondoself/3902609089).

***

#### References:

[^1]: Englander M, et al. PNAS 112, 6038–43 (2015).

[^2]: Wang K, et al. Nat. Biotechnol. 25, 770–7 (2007).

[^3]: Czekster C, et al. JACS 138, 5194–7 (2016).

[^4]: Chin JW. Nature 550, 53–60 (2017).

[^5]: Dedkova L, et al. JACS 125, 6616–7 (2003).

[^6]: Schmeing T & Ramakrishnan V. Nature 461, 1234–42 (2009).

[^7]: Achenbach J, et al. Nucleic Acids Res. 43, 5687–98 (2015).

[^8]: Ban N, et al. Science 289, 905–20 (2000).

[^9]: Nissen P, et al. Science 289, 920–30 (2000).

[^10]: Moore P & Steitz T. RNA 9, 155–9 (2003).

[^11]: Neumann H, et al. Nature 464, 441–4 (2010).

[^12]: Fried S, et al. Angew. Chem. 127, 12982–5 (2015).

[^13]: Wang Z, et al. Nat. Chem. 8, 698–704 (2016).

[^14]: Pritsker M, et al. PNAS 95, 7287–92 (1998).

[^15]: Soutourina J, et al. J. Biol. Chem. 275, 32535–42 (2000).

[^16]: Francklyn CS, et al. Methods 44, 100–18 (2008).

[^17]: Taylor P, et al. Applied Biocatalysis in Specialty Chemicals and Pharmaceuticals 776, 65–75 (2001).

[^18]: Fischer N, et al. Nature 520, 567–70 (2015).

[^19]: Fosgerau K, et al. Drug Discov Today 20, 122–8 (2015).

[^20]: Takeuchi T, et al. Curr Med Chem 21, 2575–82 (2014).

[^21]: Matejuk A, et al. Drugs Future 35, 197 (2010).

[^22]: Marelli C & Maschat F. Orphanet J Rare Dis 11, 24 (2016).




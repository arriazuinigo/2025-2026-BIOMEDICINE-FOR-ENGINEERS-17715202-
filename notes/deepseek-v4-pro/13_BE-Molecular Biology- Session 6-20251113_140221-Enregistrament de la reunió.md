# 13_BE-Molecular Biology- Session 6-20251113_140221-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 6 (Thursday, 13 November 2025, 2:02 PM)
- **Video:** [13_BE-Molecular Biology- Session 6-20251113_140221-Enregistrament de la reunió.mp4](../../recordings/13_BE-Molecular%20Biology-%20Session%206-20251113_140221-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%206-20251113_140221-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:27:32 · **Language:** en
- **Transcript:** [13_BE-Molecular Biology- Session 6-20251113_140221-Enregistrament de la reunió.md](../../transcripts/13_BE-Molecular%20Biology-%20Session%206-20251113_140221-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary
This session moved from the NCBI Gene queries done previously to the overall architecture of the human genome and then into hands-on use of the UCSC Genome Browser. The professor reviewed the nuclear genome’s size and composition, the difference between all genes and protein-coding genes, and why the non-coding 99% of the genome is not “junk” but largely regulatory. She covered chromosome structure, euchromatin/heterochromatin, CpG islands, non-coding RNAs, tandem repeats, segmental duplications, retrotransposons, and pseudogenes. The second half was a guided UCSC exercise on chromosome 7: displaying genes, pseudogenes, repeats, sequence conservation across vertebrates, and common SNPs.

- Only about 1.1% of the nuclear genome codes for protein; most of the rest is involved in gene regulation, chromosome architecture, and epigenetic inheritance.
- The genome is packed with repetitive DNA: micro/mini/macrosatellites, segmental duplications, and LINE/SINE retrotransposons.
- Pseudogenes are non-functional copies or remnants of genes and can act as a stored “library” of old genes.
- Exons are highly conserved across vertebrates because changes in coding sequence are more often harmful; introns mutate much more freely.
- UCSC Genome Browser integrates more than 100 annotation databases and is the main tool used to explore genome elements visually.

## Key concepts
- **Nuclear genome**: 23 pairs of chromosomes in the nucleus; 3.1 gigabases (Gb) on the main strand, 6.2 Gb if both strands are counted [00:04:15].
- **Mitochondrial genome**: small, circular, bacterial-like genome; only 13 genes, no introns, little intergenic DNA, no histone packing; mainly metabolism/energy genes [00:09:52].
- **Gene**: a DNA sequence that is transcribed into RNA; not every gene is translated into protein. About 40,000 human genes exist, of which about 20,000 code for protein [00:05:18].
- **Euchromatin / heterochromatin**: white, less-packed chromosome regions with high gene density vs black, highly packed regions with low gene density [00:10:54].
- **Non-coding DNA**: about 99% of the genome; includes intergenic regions, introns, 5′/3′ UTRs, promoters, and non-coding RNA genes [00:08:37].
- **CpG islands**: regions where CpG cytosines are not methylated; often found upstream of genes and can mark promoter regions because methylation would block transcription-factor binding [00:19:33].
- **Non-coding RNAs**: RNA genes not translated into protein; function through their three-dimensional structure; divided into short (<200 nt) and long (>200 nt) classes [00:14:11][00:21:49].
- **Tandem repeats**: adjacent repeated sequences; microsatellites 1–9 nt, minisatellites 10–100 nt, macrosatellites >100 nt; used in parentage testing and linked to disease/phenotypic traits [00:24:59].
- **Segmental duplications**: large duplicated blocks of 10–300 kb with ~95% identity; recent evolutionary events; contribute to copy-number variation and chromosomal rearrangements [00:26:00].
- **Retrotransposons / jumping genes**: mobile DNA elements that move via an RNA intermediate and reverse transcription; LINEs ~7,000 nt and SINEs 100–700 nt; make up roughly 20% + 13% of the genome [00:29:36][00:30:44].
- **Pseudogenes**: duplicated or retrotransposed gene copies that have lost function; processed pseudogenes arise from retrotranscribed mRNA, non-processed pseudogenes arise from gene duplication [00:31:57][00:34:17].
- **Sequence conservation**: degree to which a genomic position/region is unchanged across species; high in coding exons because deleterious mutations are removed by selection [01:10:44].
- **Common SNP**: a single-nucleotide variant with appreciable frequency in the population; not directly disease-causing by itself, but combinations plus environment can predispose to complex disease [01:20:42].

## Detailed notes
### Recap: NCBI Gene work before this session
[00:00:00] The previous session used the NCBI Gene database. With only an organism and a gene name, students located gene information, sequence, chromosome position, transcript and protein sequences, and extracted exons, coding regions, 5′ UTRs, and 3′ UTRs.

### The post-sequencing question: what does the sequence mean?
[00:02:13] Sequencing technology has improved dramatically; a genome is now cheap and fast to sequence. Sequence is always written 5′→3′ on the main strand; the complementary strand runs 3′→5′ and can be computed, so databases store only one strand [00:03:13]. The hard problem after the Human Genome Project was not obtaining sequence, but understanding what those millions of nucleotides mean [00:03:13].

### Nuclear and mitochondrial genomes
[00:04:15] The human genome has two parts:
- **Nuclear genome**: 23 chromosome pairs, 3.1 Gb on the main strand.
- **Mitochondrial genome**: small circular genome in mitochondria.

The mitochondrial genome is bacterial-like: genes are packed one after another, there are no introns and little intergenic DNA, only about 13 genes involved in metabolism/energy, and no histone packaging because it does not need to fit into a nucleus [00:09:52].

### Human genes: number, coding fraction, and independent transcription
[00:05:18] There are about 40,000 human genes, but only about 20,000 are translated into protein. The other 20,000 are transcribed into non-coding RNAs with three-dimensional structures that perform regulatory and other functions [00:14:11].

Human genes are usually transcribed independently, unlike bacteria, where several genes can be carried on one RNA molecule [00:06:22].

### Why the 99% non-coding genome is not “junk”
[00:06:22] Protein-coding sequence is only about 1.1% of the genome. The other ~99% was initially called “junk DNA,” but in the last ~15 years it has become clear that it has essential functions [00:07:36]:
- regulating gene expression;
- chromosome architecture;
- control of epigenetic inheritance.

This non-coding fraction includes intergenic regions, non-coding genes, introns, 5′/3′ UTRs, and promoter regions [00:08:37].

### Chromosome organization and gene density
[00:10:54] Chromosomes vary greatly in size, from about 1 Mb to around 50 Mb. In chromosome banding:
- **black bands = heterochromatin**: tightly packed, genes not accessible, low gene density;
- **white bands = euchromatin**: less packed, high gene density, accessible to transcription machinery.

Different chromosomes have very different proportions of euchromatin and heterochromatin; there is no single fixed percentage [00:10:54].

About 9% of human genes overlap, often with one gene on the main strand and another on the complementary strand; many are small RNA genes [00:14:11].

### Gene architecture, exon/intron diversity, and CpG islands
[00:11:56] Human genes vary enormously:
- mean length roughly 26,000 bases;
- range from about 1,000 bases to about 1 million bases;
- from 1 exon to more than 100 exons.

Genes that must be expressed very frequently often lack introns, to reduce the cost of transcribing extra sequence [00:18:30].

**CpG islands** [00:19:33]:
- Cytosines in CpG dinucleotides are often methylated; this is an epigenetic mark.
- Regions where CpGs are not methylated are called CpG islands.
- CpG islands are usually found upstream of genes and can help identify promoter regions.
- Methylation upstream of a gene would block proteins needed for transcription, so promoter regions tend to remain unmethylated.

### How protein-coding genes were identified
[00:15:14] Protein-coding genes are relatively easy to find because a coding region starts with methionine and continues as a long open reading frame without stop codons. Since genes can be on either strand, there are six reading frames for any genomic sequence: three from the main strand and three from the complementary strand [00:16:16]. Regions that are long, start with methionine, and lack premature stops are candidate coding genes. This approach misses non-coding RNA genes, which are much harder to identify.

A student asked whether every long ORF is a functional protein. The answer: most are, but some long ORFs belong to pseudogenes that no longer produce functional protein [00:17:25].

### Non-coding RNA genes
[00:21:49] The ~20,000 non-coding RNA genes are classified by size:
- **Short non-coding RNAs (<200 nt)**: include RNAs involved in splicing and RNA maturation, small Cajal body RNAs, transfer RNAs, microRNAs, piwi-interacting RNAs, and short interfering RNAs.
- **Long non-coding RNAs (>200 nt)**: regulate target genes and protein translation.

They work mainly as regulators of transcription and translation through their folded 3D structure.

### Tandem repeats
[00:23:54] Tandem repeats are clusters of repeat sequence adjacent to one another. They can occur inside coding regions, but are abundant outside coding regions. Repeats may be identical or similar; similar repeats arose because mutations accumulated after duplication [00:24:59].

Classification [00:24:59]:
- **Microsatellites**: 1–9 nucleotides.
- **Minisatellites**: 10–100 nucleotides.
- **Macrosatellites**: >100 nucleotides.

They are involved in gene expression, gene silencing, alternative splicing, mRNA transport, chromatin organization, and cell-cycle regulation. Changes in microsatellite length are associated with diseases and phenotypic traits. Because repeats are inherited, they are used to establish parentage [00:26:00].

### Segmental duplications and gene duplication
[00:26:00] More than 5% of euchromatin is made of segmental duplications: blocks of 10–300 kb with about 95% sequence identity. High identity means the duplications occurred recently; otherwise they would have accumulated mutations [00:27:02]. They contribute to copy-number variation and chromosomal rearrangements, because duplicated blocks can cause misalignment during chromosome pairing.

Gene duplication follow-up [00:28:00]: an ancestral gene duplicates, the two copies accumulate different mutations, and over time they can become two similar but distinct genes with somewhat different functions. The more mutations, the more functions diverge.

### Retrotransposons: LINEs and SINEs
[00:29:36] Retrotransposons are mobile DNA elements (“jumping genes”) that can move within and between chromosomes. Mechanism:
1. The retrotransposon is transcribed into RNA.
2. Reverse transcriptase converts the RNA into DNA.
3. The DNA inserts into another genomic region.

They are classified as:
- **LINEs**: long interspersed elements, about 7,000 nt.
- **SINEs**: short interspersed elements, about 100–700 nt.

About 20% of the human genome is LINEs and another 13% is SINEs [00:30:44].

### Pseudogenes
[00:31:57] Pseudogenes are gene-like sequences that have lost the ability to be transcribed/translated into a functional product. They may be missing a promoter, start codon, or introns, or contain a premature stop codon. About 16,000 pseudogenes are estimated. They can be viewed as a “library” of old genes; under mutation and evolutionary pressure, a pseudogene can occasionally regain function.

Two origins [00:34:17]:
- **Processed pseudogenes**: messenger RNA is retrotranscribed into DNA and inserted into the genome; the copy lacks introns and regulatory elements.
- **Non-processed pseudogenes**: arise by gene duplication, then one copy loses function. Some are transcribed into RNA but not translated.

### Gene resources and genome browsers
[00:34:17] Key resources:
- **HGNC (HUGO Gene Nomenclature Committee)**: assigns unique gene symbols.
- **RefSeq**: curated database of genome, transcript, and protein sequences.
- **Genome browsers**: UCSC, Ensembl (EBI), and NCBI.

UCSC, from UC Santa Cruz, is the most powerful browser and integrates over 100 annotation databases. It has a genome browser for visualization and a table browser for downloading annotations [00:35:19][00:37:22].

### UCSC Genome Browser practical: exploring chromosome 7
[00:36:21] The exercises are “UCSC Genome Browser Exercises” on the course page. Steps in the guided demo:

#### Browser setup
[00:37:22] Open UCSC Genome Browser. Select the human genome; the professor used the 2013 human assembly because newer assemblies still lack many annotations [00:38:44]. Type `chr7` in the position search to display chromosome 7 [00:39:48].

#### Chromosome 7 bands
[00:42:25] At full view, the top shows black and white chromosome bands: black = heterochromatin, white = euchromatin. The red window indicates the whole chromosome. Use **hide all** to clear default tracks [00:43:54].

#### Available track categories
[00:44:00] UCSC displays many categories:
- **Sequencing**
- **Genes and gene predictions**: NCBI RefSeq and GENCODE
- **Disease**: OMIM maps genes involved in Mendelian diseases
- **Variation**: pathogenic/disease-associated variants vs common population variation
- **RNA/transcriptome**: transcripts, tissue expression, single-cell RNA-seq
- **Regulation**: enhancers, promoters
- **Comparative genomics**: multi-species alignments
- **Repeats**

#### Displaying genes
[00:48:13] Under “Genes and gene predictions,” select **NCBI RefSeq**, choose a display mode such as **pack**, and click **refresh**. Zoom in to see individual genes:
- **Arrows pointing left** = genes on the complementary strand (reverse).
- **Arrows pointing right** = genes on the main strand (forward).
- **Vertical lines inside a gene** = exons.
- Overlapping genes are visible as well [00:51:28].

#### Displaying pseudogenes
[00:53:16] Use the **GENCODE** track, filter to show pseudogenes only, set to **pack**, and submit. Pseudogenes appear in pink; normal genes are blue. The genome contains many pseudogenes [00:54:19]. The dedicated pseudogene track gives essentially the same information.

#### Displaying tandem repeats
[00:56:30] Under **Repeats**, select **Simple Repeats**, choose **pack**, refresh. Chromosome 7 is full of small tandem repeats such as `TTTA` or `AAA` [00:58:37]. These are the micro/mini/macrosatellites.

#### Displaying segmental duplications
[00:59:43] Under **Repeats**, select **Segmental Duplications**, choose **pack**, refresh. This shows large duplicated regions of 10–300 kb. Clicking a position shows other genomic regions with the same sequence. Difference from tandem repeats: segmental duplications are much larger and can contain several genes; tandem repeats are short adjacent repeats [01:02:37].

#### Displaying retrotransposons
[01:03:00] Use the **RepeatMasker** track under repeats, choose **dense** or **full**, refresh. This shows the jumping genes: short and long interspersed repeat elements.

#### Sequence conservation across vertebrates
[01:06:02] Hide everything, display RefSeq genes in pack, then go to **Comparative genomics** and select **UCSC 100 vertebrates**. After selecting all species and using **squish**, the browser produces a conservation plot [01:08:30]. Zoom to a gene:
- Conservation is very high in exons.
- Conservation is low in introns [01:10:44].

Reason: mutations in coding exons can damage protein structure/function, making individuals less likely to survive/reproduce, so those mutations are not retained. Mutations in introns are less harmful and accumulate [01:11:45]. High peaks mean near/at 100% sequence identity. In full mode, the actual amino-acid/nucleotide alignments are visible; exons show conserved amino acids, introns show many differences [01:14:10][01:16:11]. The genetic code is degenerate, so some nucleotide changes still encode the same amino acid and are tolerated; not every amino-acid change causes disease [01:18:24].

#### Common SNPs in the population
[01:20:42] Under **Variation**, select the SNP database track and display with **squish**, **pack**, or **full**. These are single-nucleotide changes common in the population, not directly disease-related. Example: at some position, half the population may have a G and half a C. Individually they are not disease-causing, but combinations of SNPs plus environmental factors can predispose to complex disease [01:22:30].

The professor recommended repeating the “Exploring the human genome,” “Sequence conservation,” and “Variation” exercises [01:24:58].

## What the professor stressed
- The 99% non-coding DNA is not junk; it contains regulatory information that is at least as important as coding sequence [00:07:36].
- The genome is dominated by repeats; repeats are not only structural noise but also used for parentage, gene regulation, and disease association [00:24:59][00:58:37].
- The distinction between tandem repeats and segmental duplications came up in a student question: tandem repeats are short adjacent repeats; segmental duplications are huge blocks that can span multiple genes [01:02:37].
- Pseudogenes are non-functional but may become functional again under environmental/evolutionary pressure—a “library” of old genes [00:31:57].
- The strong conservation of exons across 100 vertebrate species is visible evidence of natural selection on coding sequence. She repeated this several times and tested understanding with questions [01:10:44][01:18:24].
- Common SNPs are not individually disease-causing; complex disease arises from combinations and environmental factors [01:20:42].

## Course logistics mentioned
- Task 2 was opened during the session; deadline for submission is 26 November. The professor recommended starting it early because the partial exam is soon [01:24:58][01:26:24].
- A partial exam covering the concepts worked with all presentations is expected in about two weeks; the professor mentioned 27 November [01:24:58].
- Students can email the professor with questions about the exercises or the task [01:27:25].

## Self-test
1. Why do genome databases store only one strand of sequence, and what convention is used?  
<details><summary>Answer</summary>
Because the complementary strand can be computed by base-pairing rules. The stored strand is the main strand written 5′→3′; the complementary strand runs 3′→5′ and pairs through hydrogen bonds.
</details>

2. Give at least three functions of the non-coding 99% of the human genome.  
<details><summary>Answer</summary>
Regulation of gene expression, chromosome architecture, and control of epigenetic inheritance. Structurally it includes promoters, introns, UTRs, intergenic regions, and non-coding RNA genes.
</details>

3. In the UCSC browser, how can you tell a forward gene from a reverse gene when viewing RefSeq transcripts?  
<details><summary>Answer</summary>
Forward genes lie on the main strand and their arrows point right; reverse genes lie on the complementary strand and their arrows point left. Vertical lines within the gene represent exons.
</details>

4. Why are CpG islands often useful for locating promoter regions?  
<details><summary>Answer</summary>
Most CpGs in the genome are methylated, but promoter regions need transcription factors to bind, and methylation blocks that binding. Therefore, regions upstream of genes are often unmethylated CpG islands, making them useful markers for promoters.
</details>

5. Compare tandem repeats and segmental duplications in terms of size, arrangement, and biological relevance.  
<details><summary>Answer</summary>
Tandem repeats are short adjacent repeated units (microsatellites 1–9 nt, minisatellites 10–100 nt, macrosatellites >100 nt) and are used in parentage and related to gene regulation and disease. Segmental duplications are much larger blocks, 10–300 kb, about 95% identical, recent in evolution, and contribute to copy-number variation and chromosomal rearrangements.
</details>

6. Describe how a retrotransposon moves to a new genomic location, and distinguish LINEs from SINEs.  
<details><summary>Answer</summary>
The element is transcribed into RNA; reverse transcriptase converts the RNA into DNA; the DNA inserts elsewhere in the genome. LINEs are long (~7,000 nt) retrotransposons; SINEs are short (100–700 nt) retrotransposons.
</details>

7. What is the difference between a processed pseudogene and a non-processed pseudogene?  
<details><summary>Answer</summary>
A processed pseudogene arises when an mRNA is retrotranscribed into DNA and inserted into the genome, so it lacks introns and regulatory elements. A non-processed pseudogene arises from gene duplication where one copy loses function through mutations. Both are non-functional.
</details>

8. Why are exons more conserved than introns across vertebrate species? Does any change in an exon necessarily cause disease?  
<details><summary>Answer</summary>
Exons code for protein, so mutations there are more likely to damage protein structure/function and reduce survival or reproduction; such mutations are not fixed. Intron mutations are usually neutral and accumulate. Not all exon changes cause disease: the genetic code is degenerate, so some nucleotide changes give the same amino acid, and not every amino-acid change compromises function.
</details>

9. How can sequence-conservation profiles help identify protein-coding genes?  
<details><summary>Answer</summary>
Because coding exons are under strong purifying selection, they appear as high-conservation peaks in multi-species alignments, whereas intronic and intergenic regions usually show lower conservation.
</details>

10. What is a common SNP, and why is it not directly disease-causing?  
<details><summary>Answer</summary>
A common SNP is a single-nucleotide variant present at meaningful frequency in the population. Individually it is not directly associated with disease, but combinations of many such variants together with environmental factors can predispose to complex disease.
</details>

11. Why is the mitochondrial genome so compact compared to the nuclear genome?  
<details><summary>Answer</summary>
It has a bacterial-like organization: only about 13 genes, no introns, little intergenic DNA, and no histone packaging. Its genes are mainly related to metabolism and energy production.
</details>

12. What did the professor mean by calling pseudogenes a “library of old genes”?  
<details><summary>Answer</summary>
Pseudogenes are non-functional copies or remnants of genes that may be stored in the genome. Under mutation and evolutionary pressure, some could regain function if the environment changes and they become useful again.
</details>

## Related course materials
- [1.5 - The Human Genome](../../materials/06_1.5-The%20Human%20Genome.pdf)
- [1.4 - Sequencing of the human genome](../../materials/05_1.4-%20Sequencing%20of%20the%20human%20genome.pdf)
- [UCSC Genome Browser Exercises](https://campusvirtual.urv.cat/mod/url/view.php?id=4185472)

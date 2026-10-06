# 08_BE-Molecular Biology-Session 3

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology-Session 3 (Thursday, 23 October 2025, 1:22 PM)
- **Video:** [08_BE-Molecular Biology-Session 3.mp4](../../recordings/08_BE-Molecular%20Biology-Session%203.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-Session%203.mp4)
- **Duration:** 01:44:03 · **Language:** en
- **Transcript:** [08_BE-Molecular Biology-Session 3.md](../../transcripts/08_BE-Molecular%20Biology-Session%203.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary
This session covered how the human genome was sequenced and what that sequencing revealed about human genetic variation. It started with a recap of gene structure (exons/introns and alternative splicing in humans vs. bacteria), then moved through the history of DNA sequencing: Sanger sequencing, the public Human Genome Project, the private Celera race, shotgun sequencing strategies, next-generation sequencing, and the collapse in sequencing cost. The second half focused on human genomic variation: SNPs, structural variants, haplotypes, copy-number variants, the HapMap and 1000 Genomes projects, and catalogues such as ExAC/gnomAD. The class ended with a hands-on demonstration of the NCBI Genome database for exploring the human genome and retrieving sequences, plus exercises to practise genome and gene visualisation.

Key takeaways:
- The human reference genome is a representative consensus genome, not the genome of any single individual.
- Sequencing cost fell from ~$3 billion to roughly $500–800 per whole human genome.
- Millions of nucleotide positions differ between humans, but interpreting which variants cause disease is still hard.
- Whole-genome, whole-exome, and targeted sequencing trade off coverage, cost, and speed.
- Haplotypes are blocks of SNPs inherited together, which reduces the number of variants that must be genotyped.
- You must be able to retrieve any sequence, gene, transcript, or protein from public genome databases using tools such as NCBI.

## Key concepts
- **Central dogma of molecular biology** — the flow of genetic information from DNA to RNA to protein. Not all genes are translated; some are only transcribed into RNA [00:04:09].
- **DNA sequencing** — determining the order of nucleotides (A, T, C, G) in a DNA fragment. RNA can also be sequenced by first converting it to complementary DNA with reverse transcriptase [00:06:26].
- **Sanger sequencing** — the first sequencing method, also called chain-terminating inhibition. Developed in 1977; high accuracy but low throughput [00:08:31].
- **Reference genome** — a representative genome built from multiple individuals, using the most frequent nucleotide at each position. It is not the genome of any real individual [00:23:??].
- **Euchromatin** — loosely packed, gene-rich chromatin accessible to transcription machinery [00:17:03].
- **Heterochromatin** — tightly packed chromatin with few genes, less accessible for transcription [00:17:03].
- **Single nucleotide polymorphism (SNP)** — a single-base difference between individuals at a given genomic position [00:25:22].
- **Structural variant** — a larger DNA difference between individuals, such as an inversion, translocation, duplication, or large deletion [00:29:59].
- **Haplotype** — a block of SNPs that are inherited together because recombination tends not to break the region [00:31:22].
- **Copy-number variation (CNV)** — difference between individuals in the number of copies of a large DNA segment [00:34:17].
- **Whole-genome sequencing (WGS)** — sequencing the complete genome, including exons, introns, and intergenic regions [00:38:29].
- **Whole-exome sequencing (WES)** — sequencing only the exon-containing regions of the genome [00:38:29].
- **Targeted sequencing** — sequencing only a specific known region, such as a disease-associated variant [00:39:??].
- **Pseudogene** — a gene remnant in the genome that is no longer transcribed/translated and currently has no function [01:12:15].

## Detailed notes

### 1. Recap: human vs. bacterial gene structure [00:00:00]
The professor recapped the previous session:
- Human genes have exons and introns. Introns are not translated into protein.
- Alternative splicing allows different combinations of exons to generate different RNA molecules from one gene.
- As a result, one human gene can produce multiple mRNA isoforms and multiple protein isoforms of the same protein.
- The isoforms are usually very similar, differing only in some regions (an extra or missing exon). This may affect stability or reaction speed, but the overall three-dimensional structure and function remain essentially the same.
- Bacterial genomes are circular, with mostly coding regions and no large intergenic regions or exon/intron structure.
- In bacteria, one coding gene produces one protein; there is no alternative splicing like in humans.

### 2. DNA sequencing: definitions and early technology [00:06:26]
- DNA sequencing is the process of determining the sequence of nucleotides in any piece of DNA.
- RNA can also be sequenced by first converting RNA to complementary DNA using reverse transcriptase.
- **Sanger sequencing**
  - Method: chain-terminating inhibition.
  - Developed in 1977.
  - Could produce DNA fragments of more than 500 nucleotides.
  - Very low error rate: 99.9% accuracy.
  - Very slow; splitting the 3 × 10⁹-nucleotide human genome into ~500-nucleotide fragments was impractical at scale.
  - First genome sequenced: a bacteriophage genome in 1977.
  - 1986: semi-automatic sequencing machine using the Sanger method.
  - 1987: fully automatic machine able to sequence 1,000 nucleotides per day.
  - Sanger sequencing could not easily achieve high-throughput sequencing [00:08:31].

### 3. The Human Genome Project (public consortium) [00:09:39]
- In 1990, a consortium of 20 public research institutes from the USA, France, Germany, UK, Japan, and others started the Human Genome Project.
- Goal: sequence the entire human genome in 15 years, with completion expected by 2005.
- Budget: $3 billion.
- Aim: make all data openly available to the scientific community, clinicians, and researchers, with no restrictions.
- They used DNA samples from eight individuals from different ethnic backgrounds, assuming they would show some nucleotide sequence differences [00:11:06].

### 4. Celera Genomics and the public–private race [00:12:48]
- Eight years into the public project, the private company Celera Genomics announced it would sequence the human genome in three years.
- Celera’s aims were different:
  - Patent hundreds of genes.
  - Sell gene sequences to pharmaceutical companies.
  - Validate a new sequencing method the company was developing.
- Celera used 150 sequencing machines, 65 technicians, and intensive computing.
- They sequenced five individuals: Chinese, two Caucasian, one African American, and one Hispanic (as transcribed; total five).
- Their data were not open; access was restricted even for researchers.
- The public consortium and Celera entered a race, not sharing information.
- In 2000, both groups published a draft human genome simultaneously in *Nature* and *Science*.
- The draft identified about 26,000 protein-coding genes plus an additional 12,000 genes [00:15:32].

### 5. Shotgun sequencing strategies [00:14:29]
Two strategies were used to sequence the genome:
- **Whole-genome shotgun sequencing (Celera)**
  - The genome is randomly broken into short fragments.
  - These short fragments are easy to sequence.
  - Because the fragments overlap, computational algorithms are needed to reassemble the original sequence.
  - Assembly is harder because many short reads must be put together correctly.
- **Hierarchical shotgun sequencing (public consortium)**
  - The genome is broken into larger fragments, which are harder to sequence.
  - Because the fragments are much longer and their position is better known, reassembly is easier.
- In both cases, computing was essential to reconstruct the original genome from overlapping pieces.

### 6. Quality and content of the first draft [00:17:03]
- Error rate: approximately one error every 100,000 bases.
- The draft covered 99% of the euchromatic genome.
  - Euchromatin is loosely packed and gene-rich, so genes are accessible for transcription.
  - Heterochromatin is tightly packed and usually gene-poor because transcription proteins cannot access it easily.
- The draft included about 94% of the genes in the human genome.
- Data were deposited under the Genome Reference Consortium and made available to the community [00:18:03].

### 7. Next-generation sequencing and the collapse in cost [00:18:03]
- Around 2005, new-generation sequencing methods appeared.
- Costs dropped sharply compared with the HGP era.
- These methods use massively parallel DNA sequencing reactions: thousands to millions of sequences are produced simultaneously.
- Low-cost, high-throughput machines began to be commercialised for individual laboratories.
- The main platforms/methods discussed: Illumina, Roche/454(?), and Thermo Fisher Scientific.
- Important features to compare between sequencing technologies:
  - Read length.
  - Cost per gigabase.
  - Error rate.
- Trade-off: sometimes a slower, more expensive method with fewer errors is preferable depending on the project [00:19:40].

### 8. Genome sequencing growth and model organisms [00:20:44]
- The original HGP budget was $3 billion.
- Now sequencing an individual whole genome costs roughly $500–800.
- As cost fell, the number of sequenced genomes increased greatly across eukaryotes, prokaryotes, and viruses.
- Timeline examples:
  - 2000: *Drosophila melanogaster*, *Arabidopsis thaliana*, *Mus musculus* (mouse) genomes.
  - 2002: mouse draft; genome browsers made genomes and annotations accessible.
  - 2005: *Pan troglodytes* (chimpanzee) and *Oryza sativa* (rice, first crop genome).
- Annotations include gene positions, sequence variations, and other information known about a genome [00:21:49].

### 9. HapMap and the need to study variation [00:22:51]
- The reference genome is a representative genome: at each position it contains the nucleotide with the highest frequency in the studied population.
- It is not the genome of any actual individual.
- The HapMap project started to determine common patterns of DNA sequence variation in the human genome.
- Individuals from Africa, Asia, and Europe were sequenced.
- They obtained genotypes for one million sequence variants, showing that different individuals have extensive sequence variability.
- HapMap results were published in 2003 [00:24:12].

### 10. Types of human genomic variation [00:25:22]
- **Single nucleotide polymorphism (SNP)**
  - Example: individual 1 has A-G-C at a position; individual 2 has A-G-T.
  - One nucleotide is different.
  - SNPs are the most frequent type of variation in the population.
- **Structural variants**
  - Large regions of DNA can differ between individuals.
  - Examples: inversions, translocations, duplications, large deletions, insertions.
- SNPs and structural variants can have different consequences:
  - Some are neutral.
  - Some predispose to complex diseases.
  - Some directly cause monogenic disease.
  - If a variant falls outside a gene, it often has no effect.
  - If it falls inside a coding region, it can change the protein and cause disease [00:28:53].

### 11. De novo mutations and disease [00:28:53]
- Every newborn carries about 60 new nucleotide changes not present in the parents.
- These arise from unrepaired DNA replication errors.
- Most fall outside genes and do nothing.
- Some fall inside genes and can alter proteins.
- Examples:
  - Eye colour is encoded by gene regions, so changes there can affect phenotype.
  - Many epileptic and rare diseases are caused by de novo variants that affect a functionally important region of a protein [00:29:59].

### 12. Haplotypes [00:31:22]
- During recombination, some DNA regions are always kept together.
- A haplotype is a specific combination of SNPs that is inherited together.
- Example: if three positions form a haplotype, seeing an A at the first position implies a T and a C at the other positions.
- This means you do not need to genotype every SNP; identifying a few tag SNPs per haplotype lets you infer the rest.
- This reduces the number of variants that must be tested [00:33:16].

### 13. Copy-number variations (CNVs) [00:34:17]
- Individuals can have different numbers of copies of large DNA regions.
- Example: one individual may have three copies on the maternal chromosome and three on the paternal chromosome; another may have five, one, three, then five copies in a region.
- CNVs are less frequent than SNPs but can also be related to disease.

### 14. 1000 Genomes Project and population variation [00:35:26]
- Goal: sequence 1,000 individuals and catalogue common genetic variants in the population.
- They obtained 88 million variants, mostly SNPs (84.7 million), plus indels and structural variants.
- Because these are common population variants, most are probably not directly disease-causing.
- It was the first project to sequence the genomes of a large number of people and provide a map of human population variation.
- People were sampled from the five continents.
- Different ethnic and isolated populations have different frequencies of variants.
- Examples of isolated groups: Amish and other populations isolated by religion, geography, or history [00:36:30].

### 15. Current sequencing strategies [00:38:29]
- **Whole-genome sequencing (WGS)**
  - Sequences the full genome: exons, introns, genic and intergenic regions, from first to last nucleotide.
- **Whole-exome sequencing (WES)**
  - Sequences only exons, the regions most likely to affect protein function and disease.
  - Much cheaper and faster than WGS because it skips introns and intergenic regions.
- **Targeted sequencing**
  - Sequences only a known region of interest, such as a variant associated with breast cancer or celiac disease.
  - Fastest and cheapest; used to test for a specific mutation or genetic predisposition.

### 16. ExAC and gnomAD catalogues [00:40:07]
- ExAC obtained more than 60,000 exomes and built a catalogue of human genetic variation.
- They observed an average of one variant every eight nucleotides.
- gnomAD is the successor to ExAC.
  - Initially about 125,000 exomes and 15,000 genomes.
  - Version 3: about 70,000 genomes.
  - Version 4: around 300,000 genomes.
- Many worldwide initiatives sequence either disease cohorts or healthy people to understand human variation and disease.

### 17. Why variant interpretation is complex [00:41:08]
- With millions of differences between any individual and the reference genome, identifying which variant causes disease is difficult.
- A patient’s genome will show millions of differences from the reference.
- The challenge is deciding which of these changes is responsible for the disorder.
- Many algorithms and research efforts try to predict variant pathogenicity.
- Some variants are known to be highly penetrant, e.g. BRCA1/BRCA2 in breast cancer and variants linked to colon cancer.
- For complex diseases, many variants contribute small effects; no single variant explains the disease [00:51:41].

### 18. Clinical questions: monogenic vs. complex disease, compatibility testing [00:42:27]
- **Carrier testing / couple compatibility**
  - Private companies analyse genomes to estimate risk of recessive disease in offspring.
  - If both parents carry a harmful mutation in the same gene, the child has about a 50% chance of inheriting both bad copies.
  - Interpretation is still incomplete: for many variants we do not yet know if they destroy protein function or cause disease.
  - These tests are often used in families that already have an affected child, to estimate risk for future children.
- **De novo risk**
  - Even if both parents are negative, the baby can still carry new mutations not present in the parents.
  - Germ-cell mutations can occur at any time during life due to chemicals, radiation, etc.
  - It is impossible to analyse all germ cells; only inherited DNA is tested.
- **Somatic mutations**
  - Mutations after birth in non-germ cells are somatic.
  - These often underlie cancer, rather than inherited disease.
- **Monogenic vs. complex diseases**
  - Monogenic disease: a single mutation is enough to cause disease.
  - Complex disease: genetic variants only predispose; environmental factors and other genes are also involved.
  - Celiac disease example: a person may carry risk variants but not develop disease until an environmental trigger, such as a rotavirus infection, triggers it.
- **Preventive medicine**
  - For known high-risk genes (e.g. BRCA1/BRCA2, colon cancer genes), patients can be monitored more closely.
  - For complex diseases, genetic risk can guide screening frequency but does not guarantee disease [00:48:11].

### 19. NCBI database walkthrough [00:54:01]
Three major centres host genome sequence information:
- NCBI (National Center for Biotechnology Information, USA)
- EBI (European Bioinformatics Institute)
- DDBJ (DNA Data Bank of Japan)

The professor demonstrated the NCBI Genome database:
- Open NCBI, select the **Genome** database, and search.
- The database showed:
  - 2.54 million genome records/assemblies.
  - 38,650 species with a reference sequence.
  - Example counts by group: >18,000 eukaryote genomes, 703 archaea, 19,000 bacteria, 194,000 virus genomes [01:00:08].
- Search for *Homo sapiens*:
  - 1,583 human genome records/releases.
  - Select the reference genome with the green tick.
  - The current reference assembly is from 2022.
  - It is a representative genome, not from any individual [01:02:20].
- On the human genome page:
  - Genome size: 3.1 gigabases (3.1 × 10⁹ nucleotides).
  - About 59,000 genes total.
  - About 20,000 coding genes.
  - Chromosomes 1–22, X, Y, and mitochondrial chromosome are shown with their sizes.
  - NC accessions are from the RefSeq database, a highly curated database with one reference sequence for each gene, genome, and protein; the professor recommended using RefSeq nomenclature [01:04:10].
- Retrieving sequence:
  - Open a chromosome, e.g. chromosome 1.
  - Use the FASTA view to see the nucleotide sequence.
  - Beginning of chromosome 1 contains many Ns, meaning undetermined nucleotides.
  - You can enter a coordinate range (e.g. 100,000–200,000) and update the view to display only that region [01:06:51].

### 20. Gene annotation in NCBI [01:11:12]
- From the genome page, go to the gene annotation list / “Bionnotate Genes” section.
- The human genome annotation showed 68,325 genes.
- Filtering by gene type:
  - Protein-coding genes: about 23,000.
  - Non-protein-coding genes: about 19,000.
  - Pseudogenes: about 19,000; pseudogenes are gene remnants that are no longer transcribed/translated and currently have no function [01:12:15].
- Genes can be on either DNA strand:
  - Genes on the main strand are transcribed to the right.
  - Genes on the complementary strand are transcribed to the left.
  - Transcription always proceeds 5′ to 3′, regardless of strand.
- Filters can be used to list all genes on a specific chromosome, e.g. chromosome 7, or to count protein-coding genes on a chromosome [01:14:57].

### 21. Exercises for practise [01:13:52]
- The professor presented exercises on genome and gene visualisation.
- Objectives: explore different genomes, find genes, and retrieve sequences.
- For next class, students should:
  - Check the solved transcription/translation exercises from the previous week.
  - Start the first section of the genome-database visualisation exercises.
- If questions arise, students can contact the professor by email.

## What the professor stressed
- Understand the structural difference between human and bacterial genomes: exons/introns and alternative splicing explain why one human gene can produce multiple proteins [00:00:00].
- The human reference genome is a consensus, not any individual’s genome [00:23:??].
- Sequencing cost has fallen from $3 billion to roughly $500–800 per genome, which enabled population-scale projects [00:20:44].
- Human genomes are full of variation; the main problem is not finding variants but knowing which variant causes disease [00:41:08].
- Genes can be on either strand, but transcription always goes 5′ to 3′ [01:12:15].
- Use RefSeq accessions and nomenclature when working with sequences [01:06:51].
- By the end of the course, students should be able to extract any sequence, gene, transcript, or protein from public databases [00:53:??].
- Complete the exercises before the next class; database practice is essential for understanding the abstract genome concepts [01:16:??].

## Course logistics mentioned
- The solved exercises on transcription and translation are now available; students should check their answers and contact the professor with questions [00:02:03].
- There is no class next week because the professor is attending a conference. The next class is in two weeks.
- Students should use the gap to ensure they understand the concepts and complete the genome/gene visualisation exercises.
- If content is missed due to the cancelled session, the professor said she may record additional videos at the end of the course if needed [01:16:??].

## Self-test
1. Why can one human gene produce multiple protein isoforms, while a typical bacterial gene produces only one protein?  
<details><summary>Answer</summary>Human genes contain exons and introns. Alternative splicing combines exons in different ways to generate different mRNAs and proteins from the same gene. Bacterial genes generally lack introns, so each coding gene produces one mRNA and one protein.</details>

2. What was the main difference in data-sharing philosophy between the public Human Genome Project and Celera Genomics?  
<details><summary>Answer</summary>The public HGP aimed to release all sequence data openly to the scientific community. Celera aimed to patent genes and sell sequence information, keeping data under restriction.</details>

3. Why was Sanger sequencing alone considered too slow for sequencing the whole human genome?  
<details><summary>Answer</summary>Sanger reads were around 500–1,000 nucleotides, with early automatic machines producing about 1,000 nucleotides per day. The human genome is 3 × 10⁹ nucleotides, so this throughput was far too low without an industrial-scale effort and new methods.</details>

4. Explain the difference between whole-genome shotgun sequencing and hierarchical shotgun sequencing.  
<details><summary>Answer</summary>Whole-genome shotgun randomly breaks the entire genome into short fragments, which are easy to sequence but harder to assemble. Hierarchical shotgun uses larger fragments, which are harder to sequence but easier to reassemble because their positions are better known.</details>

5. Why is the reference genome not the genome of a specific person?  
<details><summary>Answer</summary>It is a representative assembly built from multiple individuals. At each position, it typically uses the most frequent nucleotide, so it is a consensus rather than one person’s actual sequence.</details>

6. What is a haplotype, and why does it reduce the number of SNPs that need to be genotyped?  
<details><summary>Answer</summary>A haplotype is a block of SNPs inherited together because recombination rarely breaks the region. If you genotype a few tag SNPs in the block, you can infer the rest, so not every SNP must be tested.</details>

7. Distinguish a SNP from a copy-number variation.  
<details><summary>Answer</summary>A SNP is a single-base difference between individuals. A copy-number variation is a larger segment of DNA present in different numbers of copies between individuals. SNPs are much more frequent than CNVs.</details>

8. How can a baby have a disease-causing mutation even if both parents are healthy and test negative?  
<details><summary>Answer</summary>The mutation can be de novo, arising during gamete formation or early development. Germ-cell mutations can occur at any time due to replication errors or environmental exposure, so they are not present in the parents’ inherited genomes.</details>

9. Compare whole-genome, whole-exome, and targeted sequencing in cost and use.  
<details><summary>Answer</summary>Whole-genome sequencing covers everything but is most expensive. Whole-exome sequencing covers only exons and is faster/cheaper while capturing most protein-related variants. Targeted sequencing examines only a specific known region and is the cheapest, used for known disease-associated variants.</details>

10. In a genome browser, a gene is shown on the complementary strand. In which direction is it transcribed?  
<details><summary>Answer</summary>Transcription always occurs 5′ to 3′. If the gene is on the complementary strand, it is transcribed in the opposite direction relative to the main strand, i.e. from right to left in the browser view.</details>

11. How would you retrieve only positions 100,000–200,000 of chromosome 1 from NCBI?  
<details><summary>Answer</summary>Open the reference assembly for Homo sapiens, enter chromosome 1, open the FASTA view, enter the coordinate range 100,000–200,000, and update the view.</details>

12. Why are common variants found in the 1000 Genomes Project usually unlikely to directly cause severe monogenic disease?  
<details><summary>Answer</summary>Because they are common in healthy populations, so they are generally compatible with normal development. Severe monogenic diseases are more often caused by rare or de novo variants with strong functional effects.</details>

## Related course materials
- [1.4 - Sequencing of the human genome](../../materials/05_1.4-%20Sequencing%20of%20the%20human%20genome.pdf)
- [1.5 - The Human Genome](../../materials/06_1.5-The%20Human%20Genome.pdf)
- [1.6 - Human Genomic Variations](../../materials/07_1.6-Human%20Genomic%20Variations.pdf)

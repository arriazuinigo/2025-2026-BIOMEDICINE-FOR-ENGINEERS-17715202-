# 18_BE-Molecular Biology- Session 9-20251204_140459-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 9 (Thursday, 4 December 2025, 2:04 PM)
- **Video:** [18_BE-Molecular Biology- Session 9-20251204_140459-Enregistrament de la reunió.mp4](../../recordings/18_BE-Molecular%20Biology-%20Session%209-20251204_140459-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%209-20251204_140459-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:23:25 · **Language:** en
- **Transcript:** [18_BE-Molecular Biology- Session 9-20251204_140459-Enregistrament de la reunió.md](../../transcripts/18_BE-Molecular%20Biology-%20Session%209-20251204_140459-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary

This session covered the biology and classification of human genetic variation: from the basic vocabulary of population genetics (locus, allele, genotype, phenotype, allele frequencies) to the molecular types of DNA change (chromosomal, structural, small-scale and single-nucleotide variants). The professor explained how germline mutations differ from somatic mutations and why only germline variants are transmitted; how common SNPs are organised into haplotypes by linkage disequilibrium; why most variants are neutral but a minority cause disease; and how monogenic and complex diseases differ. She also introduced loss-of-function versus gain-of-function mutations, inheritance patterns, and how causative variants are identified in patients.

Key takeaways:

- A single-nucleotide variant (SNV) is the most common type of human DNA variation; most variation falls outside coding regions.
- Most variants identified in human populations are rare; most variants carried by a single individual are common.
- Only mutations in germ cells are transmitted to children; somatic mutations can contribute to cancer, neurodegeneration and ageing, but are not inherited.
- Every child is born with roughly 60–80 de novo mutations not present in the parents.
- Gain-of-function mutations are usually more disease-causing than loss-of-function mutations.
- The accuracy of computational tools for predicting variant pathogenicity is still low; many variants of uncertain significance require wet-lab validation.

## Key concepts

- **Locus / loci**: a region of DNA with a unique chromosomal location.
- **Allele**: one of the different sequence versions present at a given locus.
- **Genotype**: the combination of alleles at a locus, considering both copies of the genome (e.g. AA, AC, CC).
- **Phenotype**: the observable expression of a genotype as a trait (e.g. epilepsy, blindness).
- **Homozygous / heterozygous**: having identical versus different alleles at a locus on the two homologous chromosomes.
- **Allele frequency**: how frequent a particular allele is in a population.
- **Minor allele frequency (MAF)**: the frequency of the less common allele in a population.
- **Germline mutation**: a DNA change in germ cells that can be transmitted to offspring.
- **Somatic mutation**: a DNA change acquired in non-germ cells during life; not transmitted to offspring.
- **De novo mutation**: a mutation not inherited from the parents, arising in the germline or very early.
- **Chromosomal variant**: change in chromosome number (aneuploidy).
- **Structural variant**: DNA change affecting more than 50 nucleotides, up to hundreds of thousands.
- **Small-scale variant**: DNA change affecting fewer than 50 nucleotides: STRs, short indels, SNVs.
- **SNV (single nucleotide variant) / SNP (single nucleotide polymorphism)**: a one-nucleotide change; SNP usually refers to common variants in populations.
- **Frameshift**: insertion/deletion that changes the triplet reading frame, often producing a truncated protein.
- **Synonymous variant**: nucleotide change that does not alter the amino acid, because the genetic code is degenerate.
- **Non-synonymous variant**: nucleotide change that alters the amino acid; includes missense and nonsense.
- **Haplotype**: a set of SNPs that tend to be inherited together as a block.
- **Linkage disequilibrium (LD)**: non-random association of alleles at nearby loci; they are inherited together more often than expected by chance.
- **Tag SNP**: a SNP used to infer the other common SNPs in the same haplotype block.
- **Heritability**: the proportion of phenotypic variation in a trait attributable to genetic effects.
- **Monogenic disease**: disease caused by mutation(s) in a single gene.
- **Complex disease**: disease caused by many genetic variants plus environmental factors.
- **GWAS**: genome-wide association study; case–control method to find SNPs/environmental factors associated with complex disease.
- **Pleiotropy**: one genetic variant affecting two or more unrelated traits.
- **Loss-of-function / gain-of-function**: mutations that reduce or abolish, versus increase, protein activity.

## Detailed notes

### 1. Basic genetic variation vocabulary

[00:00:00] The professor began with four individuals, each carrying a pair of chromosome 1 homologues. At a given **locus**—a specific position with a unique chromosomal location—the two copies can have identical or different sequences.

- If the two copies at the locus are identical, the individual is **homozygous** for that locus.
- If they differ, the individual is **heterozygous**.
- Example: individuals can be AA, CC, or AC. [00:01:56]

The **allele** is the specific sequence version at the locus, the **genotype** is the combination of both alleles, and the **phenotype** is how that genotype is expressed as a trait (e.g. a clinical phenotype such as epilepsy or blindness). [00:04:04]

### 2. Genotype and allele frequencies in populations

[00:05:07] She gave a population example with three genotypes at one locus:

| Genotype | Number of individuals |
|----------|----------------------|
| AA       | 360                  |
| Aa       | 480                  |
| aa       | 160                  |

From these numbers (total 1,000 individuals), genotype frequencies are 0.36, 0.48 and 0.16. Allele frequencies can be computed from the genotype counts: A = (2×360 + 480) / 2000 = 0.6; a = 0.4. The **minor allele frequency** is the frequency of the less common allele, so here a = 0.4. [00:06:11]

These frequencies can be calculated for specific populations or ethnic groups. [00:07:17]

### 3. Where mutations come from: germline, somatic and de novo changes

[00:07:17] DNA changes occur throughout life. They can occur in:

- **Germ cells**: if the mutation is in the parental germline, all cells of the resulting individual—somatic and germ—may carry it.
- **Somatic cells**: if a mutation arises later in development or post-natally, only the descendants of that cell are affected. The later in development, the fewer cells are affected.
- **De novo mutations**: changes not inherited from parents, arising in the first cells or later. [00:08:20]

Causes of mutation include DNA replication errors, oxidative molecules produced by metabolism, exogenous damage (radiation, X-rays, plant toxins, chemicals, viruses), recombination errors, chromosome segregation errors, and retrotransposition. [00:09:21]

### 4. Three classes of DNA sequence variation

[00:12:26] DNA sequence variation is classified into three broad groups.

**Chromosomal variants** are changes in chromosome number caused by errors in chromosome segregation. They can produce fewer or more chromosomes than normal. Example: trisomy 21 (three copies of chromosome 21) causes Down syndrome. Sex chromosome aneuploidies are generally better tolerated than autosomal ones. The professor was not aware of a viable monosomy syndrome and suspected that having only one copy of an autosome is generally lethal. [00:12:26]

**Structural variants** affect more than 50 nucleotides, sometimes hundreds of thousands. They include:
- Duplications / copy number variants (CNVs)
- Segmental duplications
- Inversions
- Large deletions
- Large insertions
- Translocations
- Retrotransposition events (RNA → DNA inserted back into the genome)

CNVs can duplicate one gene or a whole set of genes (e.g. 15–20 genes) and are related to disease. [00:16:16]

**Small-scale variants** affect fewer than 50 nucleotides. They include:
- Short tandem repeats (STRs)
- Short indels (insertions/deletions of a few nucleotides)
- Single nucleotide variants (SNVs)

SNVs, plus small indels, are the major type of change caused by DNA replication and repair errors. About 99.9% of these replication/repair errors are SNVs or small-scale insertions/deletions, with SNVs being the most common. Because coding regions are only about 1% of the genome, most small-scale variants fall in non-coding or intergenic regions. [00:17:23]

### 5. Single nucleotide variants and their coding consequences

[00:18:57] SNVs can be:
- **Substitutions**: one base replaced, e.g. T → C.
- **Insertions**: an extra nucleotide added.
- **Deletions**: a nucleotide removed.
- **Inversions**: nucleotides changing position.

If an insertion or deletion occurs in a coding region and is not a multiple of three, it shifts the **reading frame**. This changes the translated amino acid sequence from that point onward, often creating a **premature stop codon** and a truncated protein. [00:20:22]

SNVs in coding regions can be:
- **Synonymous**: the nucleotide changes but the amino acid does not, because the genetic code is degenerate. Example: TGT and TGC both code for cysteine. [00:21:25]
- **Non-synonymous**:
  - **Missense**: one amino acid is replaced by another. Example: TGT (cysteine) → TGG (tryptophan). [00:24:17]
  - **Nonsense**: a premature stop codon is introduced, truncating the protein.

The professor noted that synonymous variants can still influence phenotype, for example through effects on regulation or splicing, even though the protein sequence is unchanged. [00:23:14]

Insertions and deletions that cause frameshifts, and nonsense substitutions, usually produce shorter proteins that may lose function. Missense changes may be neutral, damaging, or even beneficial depending on the protein region affected. [00:25:21]

### 6. Haplotypes and linkage disequilibrium

[00:26:53] By analysing many genomes, scientists observed that some SNPs are correlated: if you have an A at one position, you are more likely to have a T at another nearby position. This arises because chromosome recombination occurs at certain positions, so blocks of sequence are inherited together as **haplotypes**.

- **Linkage disequilibrium (LD)** is the occurrence of allele combinations more often or less often than expected by chance.
- Two nearby loci are in LD when they are inherited together more often than expected.
- The human genome can be thought of as made of **blocks of DNA** that are inherited together, each block containing a set of SNPs. [00:29:04]

This is practically useful: by genotyping a **tag SNP**, one can infer the other common SNPs in the same block, without sequencing the whole genome. This applies to common variants. [00:30:14]

### 7. Human population variation and variant frequency distributions

[00:30:14] The human genome has about 3×10⁹ nucleotides, and populations differ at about **4–5 million positions**, most of them single-nucleotide positions. African populations show the highest genetic diversity. Population studies are based on **germ cells**, not somatic mutations. [00:31:27]

Among human DNA variants:
- SNVs account for about **87%**
- Short indels account for about **13%**
- Structural variants are very low in percentage. [00:32:27]

Considering the 4–5 million variant sites identified in populations:
- **10%** are common (frequency > 5%)
- **14%** are low-frequency variants
- **76%** are very rare (frequency < 0.5%)

Most variants within any single individual are common, but most variants identified across human populations are very rare, present in only a few or even one individual. Only an estimated **1.4%** of variants in an individual are rare. [00:33:32] The haplotype/SNP discussion refers to the **common** variants. [00:35:36]

### 8. Somatic mutations in cancer, neurodegeneration and ageing

[00:35:36] The mutation rate in somatic cells is higher than in germ cells. A somatic mutation is passed only to the descendants of the mutated cell, so surrounding cells derived from that original cell are affected. If the mutation hits genes regulating **cell proliferation or apoptosis**, uncontrolled cell growth and cancer can result. Most cancer-causing mutations are somatic, not inherited. Somatic mutations are also linked to neurodegenerative disorders and to ageing: accumulated mutations impair gene function and tissue function over time. [00:36:37]

Only mutations in germ cells are transmitted to children. A somatic mutation cannot be passed on. Inherited germline mutations in cancer-related genes, such as **BRCA2**, usually confer high **predisposition** to cancer, not the disease itself. In a monogenic dominant disease, however, having the mutation means having the disease. [00:38:49]

### 9. Germline mutation rate and de novo mutations

[00:45:13] The germline substitution rate is about **1 × 10⁻⁸ mutations per nucleotide per generation**. This varies between populations and families, and the male germline mutation rate is generally higher than the female germline rate. Many germline mutations arise from unrepaired replication errors.

On average, every child carries about **60–80 de novo mutations** not inherited from the parents. Most fall outside coding regions because most of the genome is non-coding, but both coding and non-coding changes can be disease-causing. [00:46:13]

### 10. Disease-causing variants vs neutral and beneficial variants

[00:48:33] Most sequence variants in human populations are **not disease-causing**. Only a small fraction lead to disease or disease predisposition. Harmful mutations tend to reduce reproductive fitness and survival, so they are often not transmitted to future generations. [00:49:35]

A very small minority of variants can have a **beneficial** effect and may increase reproductive fitness, so positive selection can increase their frequency. Most variants are **neutral**. The functional consequences and mutation rates vary across genomic regions. [00:51:23]

### 11. Molecular pathology: how a variant causes a phenotype

[00:52:24] Molecular pathology seeks to explain why a given genetic change causes a clinical phenotype. This is difficult because each person differs from the reference genome at millions of positions, and many variants are unique to one individual.

Factors influencing whether a SNV causes disease:
- Whether it falls in a coding or non-coding region
- Whether it changes an amino acid
- Whether the changed amino acid is in a functionally critical region (e.g. a binding site)
- Whether the affected gene is essential for the organism

Variants can damage the organism through coding-region changes, but also through non-coding changes affecting **gene expression, RNA stability or RNA splicing**. [00:54:39]

Functional variants can be:
- **Loss-of-function**: the protein loses function (e.g. misfolding, truncation, large amino acid change). Some loss-of-function mutations are not disease-causing if the gene is non-essential or if 50% of normal product remains sufficient.
- **Gain-of-function**: the protein has higher or constitutive activity. Most gain-of-function mutations are disease-causing. It is often worse to increase protein activity than to reduce it. [00:57:48]

Therapeutic logic:
- Loss-of-function → design therapies that **activate** the protein or provide agonists.
- Gain-of-function → design therapies that **reduce or block** protein activity. [00:59:24]

Example: **NMDA receptors** are membrane channels in neurons activated by glutamate. A loss-of-function mutation prevents the channel from opening. A gain-of-function mutation makes the channel open constantly, which is associated with **epilepsy**. Gain-of-function often acts like a switch stuck “on”. [01:00:24]

### 12. How clinicians try to identify a causative mutation

[01:01:19] For a patient with an undiagnosed condition, usually a rare or neurological disorder, clinicians may perform:
- Whole exome sequencing
- Whole genome sequencing
- A gene panel for known disease-related genes

They compare the patient’s variants to the reference genome and filter out variants present in healthy population databases. Often this leaves a few candidate variants in relevant genes. Evidence that a mutation is causative can come from:
- Another patient with the same clinical phenotype and the same/similar mutation
- De novo status (absent in healthy parents)
- Functional experiments in the wet lab

Computational tools such as **SIFT, PolyPhen and AlphaMissense** attempt to predict pathogenicity, but their accuracy is still low; the professor said they cannot be relied upon. Structural studies and molecular simulations are more informative but very time-consuming. [01:05:11]

### 13. Monogenic diseases and inheritance patterns

[01:07:25] **Monogenic diseases** are caused by mutation in a single gene. If you have the necessary mutation (one or two copies depending on dominance), you have the disease. There are about **5,000–8,000 monogenic diseases**, and about **3% of the population** is affected. Examples: **cystic fibrosis and sickle cell anaemia**. Most disease-causing rare variants in monogenic disease are de novo because affected individuals often have reduced reproductive fitness. [01:10:29]

Inheritance patterns:
- **Autosomal dominant**: one mutated copy is enough. An affected heterozygous father with an unaffected mother has a 50% chance of transmitting the condition to each child. [01:14:50]
- **Autosomal recessive**: two mutated copies are needed. Two carrier parents (each with one mutated copy) have a 25% chance of having an affected child. [01:15:54]
- **X-linked recessive**: females need two mutated X copies; males need only one. An affected father cannot pass the X-linked mutation to his sons (they get his Y); his daughters become carriers. A carrier mother has a 50% chance that each son is affected and a 50% chance that each daughter is a carrier. [01:16:56]
- **X-linked dominant**: one mutated X copy is enough. An affected father passes the X to all daughters and none of his sons, so all daughters are affected. An affected mother has a 50% chance of passing it to any child, sons or daughters. [01:18:02]
- **Y-linked**: only males can be affected; an affected father passes it to all sons. [01:18:50]

When an inherited monogenic disease runs in a family, affected and unaffected family members can be compared to identify the variants segregating with the phenotype. [01:12:40]

### 14. Complex diseases, heritability and GWAS

[01:08:27] **Complex diseases** are more common than monogenic diseases. They involve multiple mutations in several genes plus environmental factors; no single mutation is sufficient to cause the disease. **Heritability** is the proportion of total phenotypic variation in a trait that can be attributed to genetic effects. Monogenic disorders have high heritability; complex disorders have lower heritability because environment also matters. [01:09:28]

The main approach for complex diseases is **GWAS (genome-wide association study)**, which compares large groups of patients with healthy controls, looking for SNPs and environmental factors enriched in patients. Because of haplotypes, genotyping tag SNPs lets researchers infer other SNPs in the same blocks. Since 2008, many complex diseases have been studied. [01:19:08]

Despite these efforts:
- Each complex trait is associated with many variants of **small effect**.
- The individual effects are small and, globally, they still do not explain all of the heritability.
- **Pleiotropy** is common: one genetic variant can affect two or more unrelated traits. [01:20:11]

The professor concluded that next week’s session will be practical, using databases of healthy populations and patient databases to examine genetic reports and variants related to disease. [01:22:35]

## What the professor stressed

- The distinction between **germline and somatic mutations**: only germline mutations are transmitted to children; somatic mutations are not. [00:38:49]
- Most cancer is caused by **somatic mutations**, but inherited germline mutations in genes such as BRCA2 confer predisposition. [00:43:14]
- Most sequence variants are **neutral**, many are rare, and only a few are pathogenic or beneficial. [00:49:35]
- **Gain-of-function mutations are usually more disease-causing** than loss-of-function mutations. [00:57:48]
- Current computational pathogenicity predictors have **low accuracy**; wet-lab validation is often needed. [01:05:11]
- Every child carries **60–80 de novo mutations**. [00:46:13]
- Common variants are organised into **haplotype blocks by linkage disequilibrium**, which makes tag-SNP genotyping possible. [00:29:04]
- Most variants fall outside coding regions, but non-coding variants can still cause disease through gene regulation, RNA stability or splicing. [00:56:44]

## Course logistics mentioned

- The next session will be practical exercises on databases of healthy populations and of patients, studying genetic reports and how variants relate to disease. [01:22:35]

## Self-test

1. What is the difference between a locus, an allele, a genotype and a phenotype?
<details><summary>Answer</summary>A locus is a specific position in the genome. An allele is one of the sequence versions present at that locus. The genotype is the combination of the two alleles at the locus in an individual. The phenotype is the observable trait resulting from the genotype, such as epilepsy or blindness.</details>

2. In a population of 360 AA, 480 Aa and 160 aa individuals, what are the allele frequencies and which is the minor allele?
<details><summary>Answer</summary>Total individuals = 1000; total alleles = 2000. A = (2×360 + 480) / 2000 = 0.6. a = (480 + 2×160) / 2000 = 0.4. The minor allele is a.</details>

3. Why do most small-scale variants fall in non-coding regions?
<details><summary>Answer</summary>Because only about 1% of the genome is protein-coding; the rest is non-coding or intergenic, so random mutations are much more likely to fall outside coding regions.</details>

4. Explain how a single-base insertion in a coding region can produce a completely different protein.
<details><summary>Answer</summary>If the insertion is not a multiple of three, it shifts the triplet reading frame. Every downstream codon is changed, often producing a premature stop codon and a truncated, usually non-functional protein.</details>

5. What is linkage disequilibrium, and why is it useful in genetic studies?
<details><summary>Answer</summary>Linkage disequilibrium is the non-random association of alleles at nearby loci, inherited together more often than expected by chance. It means genomes consist of haplotype blocks of correlated SNPs, so genotyping a tag SNP can infer other SNPs in the same block without sequencing the whole genome.</details>

6. A mutation occurs in a patient’s liver cell. Explain whether it can be transmitted to the patient’s children and what diseases it might contribute to.
<details><summary>Answer</summary>It is a somatic mutation and cannot be transmitted to children. It will only affect descendants of that liver cell. If it affects genes controlling proliferation or apoptosis, it can contribute to cancer; accumulated somatic mutations also contribute to ageing and neurodegeneration.</details>

7. Why are gain-of-function mutations often more harmful than loss-of-function mutations?
<details><summary>Answer</summary>Loss-of-function may still leave some residual activity, and in some cases 50% of normal product is enough. Gain-of-function produces excessive or constitutive activity, like a switch stuck “on”, which is usually more disruptive and more often disease-causing.</details>

8. What evidence helps classify a novel variant found in a patient as disease-causing?
<details><summary>Answer</summary>Absence in healthy population databases, presence in another patient with the same phenotype and same/similar mutation, de novo occurrence in healthy parents, location in a disease-relevant gene, and functional wet-lab experiments showing altered protein function.</details>

9. For X-linked recessive inheritance, why are males more frequently affected than females?
<details><summary>Answer</summary>Males have only one X chromosome, so a single mutated copy is sufficient to cause disease. Females have two X chromosomes and require two mutated copies to be affected; with one mutated copy they are usually carriers.</details>

10. What is the purpose of a GWAS, and what has it revealed about complex diseases?
<details><summary>Answer</summary>A GWAS compares large case and control groups to identify SNPs and environmental factors associated with complex disease. It has shown that complex traits are associated with many variants of small effect, that pleiotropy is common, and that these small effects still do not fully explain heritability.</details>

## Related course materials

- [1.6-Human Genomic Variations](../../materials/07_1.6-Human%20Genomic%20Variations.pdf)

# 19_BE-Molecular Biology- Session 10-20251211_140315-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 10 (Thursday, 11 December 2025, 2:03 PM)
- **Video:** [19_BE-Molecular Biology- Session 10-20251211_140315-Enregistrament de la reunió.mp4](../../recordings/19_BE-Molecular%20Biology-%20Session%2010-20251211_140315-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%2010-20251211_140315-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:22:41 · **Language:** en
- **Transcript:** [19_BE-Molecular Biology- Session 10-20251211_140315-Enregistrament de la reunió.md](../../transcripts/19_BE-Molecular%20Biology-%20Session%2010-20251211_140315-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary

This session had two parts. The first half was practical: how to use **ClinVar** to look up disease-causing variants in patients and **gnomAD** to look up neutral/population variation, plus how to download both datasets from the **UCSC Table Browser**. The professor worked through examples with **GLDC** (autosomal recessive) and **GRIN1/GRIN2A** (autosomal dominant severe epilepsy/intellectual disability genes). The second half introduced the **human proteome**: the ~20,000 proteins encoded by the human genome, the 20 amino acids as building blocks, the relationship between sequence, structure and function, the four levels of protein structure, and how proteins evolve by gene duplication and domain shuffling.

Key takeaways:

- **ClinVar** is the reference database for **pathogenic/likely pathogenic variants** found in patients; **gnomAD** is the reference for **healthy population variation**.
- **Missense** variants change one amino acid; **frameshift** and **nonsense** variants usually produce shorter, non-functional proteins.
- A variant found in healthy individuals in gnomAD is strong evidence against it causing a severe **autosomal dominant** disease.
- Both ClinVar and gnomAD contain noise: old incorrect disease associations, healthy carriers of recessive diseases, and sequencing errors.
- **Protein sequence determines 3D structure, and structure determines function**; natural selection acts on protein function, not directly on DNA sequence.
- Most proteins are **multi-domain**; there are **fewer domains than proteins** because domains are reused as building blocks.

## Key concepts

- **ClinVar**: NCBI-hosted database that aggregates genetic variants identified in patients and submitted by diagnostic/research labs, together with the associated disease or phenotype.
- **gnomAD**: database of genome and exome sequences from about one million healthy individuals, used to represent genetic variation not linked to disease.
- **Pathogenic/likely pathogenic**: variants with evidence for causing disease. In ClinVar, these are the classes of interest for monogenic disease.
- **Benign**: neutral variants not associated with disease. The professor said she does not use ClinVar to study benign variants; gnomAD is more appropriate.
- **Missense variant**: a single nucleotide change that changes one codon and therefore one amino acid.
- **Nonsense variant**: a single nucleotide change that creates a premature stop codon, producing a shorter protein.
- **Frameshift variant**: insertion/deletion of nucleotides that is not a multiple of three, shifting the reading frame and usually leading to a premature stop codon.
- **Short variant vs structural variant**: short variants affect fewer than 50 nucleotides; structural variants affect large regions (>50 nucleotides), such as duplications or deletions.
- **Autosomal recessive**: two defective copies of the gene are needed to develop disease; carriers with one copy are healthy.
- **Autosomal dominant**: one defective copy is enough to cause disease; severe dominant disorders are often de novo.
- **De novo variant**: a variant present in the child but not inherited from the parents.
- **SNP/rs code**: a single nucleotide polymorphism common enough in the population to be assigned an “rs” identifier.
- **Domain**: a compact, independently folding structural and functional unit of a protein; many proteins are made of several domains.
- **Primary, secondary, tertiary, quaternary structure**: amino acid sequence; alpha-helices/beta-sheets; 3D folded shape/domain; assembly of multiple polypeptide chains.

## Detailed notes

### 1. Practical work with ClinVar

[00:00:00–00:14:25]

ClinVar is hosted by NCBI. Laboratories around the world that identify a patient with a genetic condition and the causative variant upload that variant together with the clinical phenotype. The result is a database of variants related mostly to **Mendelian/monogenic diseases**.

In ClinVar you query by gene name. The professor used **GLDC** as an example:

- GLDC is associated with an **autosomal recessive** monogenic disease.
- For an autosomal recessive disease, a person needs **two defective copies** of the gene to develop the disease.
- With autosomal dominant disease, one non-working copy is enough.
- *Note: the recording briefly says “autosomal dominant” later in the GLDC discussion, but the surrounding explanation makes clear the professor is describing recessive inheritance: needing two copies.*

In the left-hand filter menu, ClinVar contains pathogenicity classifications. The professor stressed that she **does not use ClinVar to look for benign/neutral variants**, only **likely pathogenic and pathogenic**.

For GLDC, filtering to missense variants classified as pathogenic/likely pathogenic gave **142 missense variants**. For each variant, ClinVar shows:

- The transcript, e.g. the **NM** reference transcript.
- The nucleotide change, e.g. at transcript position **2,983** a **G is changed to A**.
- The resulting amino-acid change, e.g. **aspartic acid (Asp, D) to asparagine (Asn, N)**.

[00:09:19–00:10:20]

This one-nucleotide change falls in the coding sequence (CDS), so it changes one codon and therefore one amino acid in the protein sequence. The professor emphasised that even a single amino-acid change can disrupt protein structure and function.

[00:11:20–00:13:25]

She then used **GRIN2A** as a dominant severe disease example. In ClinVar, filtering to likely pathogenic/pathogenic and then to **frameshift variants** shows deletions such as `DEL`. Deleting nucleotides, unless the number is a multiple of three, changes the reading frame; all downstream codons change and the protein usually ends in a premature stop codon, producing a shorter protein.

GRIN2A-related disease causes **epilepsy and intellectual disability** and is very severe. Because affected individuals often have reduced survival or reproductive fitness, these dominant mutations are usually **de novo** rather than inherited from parents.

[00:13:25–00:14:25]

ClinVar also distinguishes:

- **Structural variants**: large regions of the genome duplicated or removed.
- **Short variants**: variants affecting only a few nucleotides, such as frameshift, missense and nonsense.
- Other classes such as **splice-site**, non-coding RNA, and changes near the gene.
- The professor said she usually focuses on **frameshift, missense and nonsense**, because the effect of splice-site variants is difficult to predict and often unclear.

### 2. Practical work with gnomAD

[00:15:33–00:21:29]

gnomAD collects genomes and exomes from almost **one million healthy individuals** across different ethnic/population groups. It represents variation present in the human population that is **not related to disease**.

Querying the same **GLDC** gene in gnomAD shows many **missense variants** in healthy people. The professor’s point: even in disease-associated genes, there is lots of neutral sequence variation. Many amino-acid changes have no effect because the protein still folds and functions correctly.

For an autosomal recessive gene like GLDC, gnomAD can also contain **healthy carriers** of pathogenic variants: one mutated copy does not cause disease.

On a gnomAD variant page you can see:

- **Allele count**: number of individuals carrying the variant.
- **Population breakdown**, e.g. South Asian, European.
- **Homozygote count**.
- **Allele frequency**.
- **rs code / SNP identifier**, found in external resources.
- Whether the variant was seen in exome or genome sequencing.
- Chromosome and genomic position.

The professor opened a GLDC missense variant found in 159 individuals, mostly European, including one homozygote. She explained that in complex diseases, such common SNPs do not cause disease alone, but combinations of SNPs in different genes plus environmental factors can increase disease probability.

### 3. In-class exercises with gnomAD and ClinVar

[00:30:06–00:40:09]

**Exercise 1 — gnomAD, GRIN1 p.Thr450Ala.**

The professor queried **GRIN1** in gnomAD and filtered to missense variants. The variant of interest was **threonine 450 to alanine (p.Thr450Ala)**.

Inside the variant page:

- One individual carried the variant.
- That individual was from the **Admixed American** population.
- The variant was found in a **healthy** database.

Because GRIN1 is an **autosomal dominant** gene causing a very severe disease with **epilepsy and intellectual disability**, a variant present in a healthy person is interpreted as **not disease-causing**. If a new patient with a rare condition had the same variant, the laboratory would probably look for another causative variant.

The **rs code** for the variant is available in the external resources section of the gnomAD page.

**Exercise 2 — ClinVar, GRIN1.**

For the same gene in ClinVar, filtering to **pathogenic/likely pathogenic** gave:

- **Structural variants**: 28.
- **Short variants**: 114.
- **Frameshift + nonsense variants**: 12.
- **Missense variants**: 89.

The professor used this to illustrate that in gnomAD there are hundreds of GRIN1 missense variants with no effect, while in ClinVar there are 89 missense variants that really change the structure/function and cause disease. Some protein positions are essential; mutations there cause disease. Other positions tolerate change.

### 4. Noise, limitations and clinical use of these databases

[00:24:36–00:29:06]

Both ClinVar and gnomAD contain noise:

- **ClinVar noise**: many entries were uploaded years ago when we lacked large healthy-population databases. A variant might have been incorrectly associated with a disease because it was absent from the reference genome at the time. Later, when many healthy people were sequenced, that variant turned out to be neutral.
- **gnomAD noise**:
  - It includes healthy **carriers** of autosomal recessive pathogenic variants.
  - It includes **sequencing errors**, because sequencing machines make mistakes, roughly at some low rate per nucleotide.
- The solution is **more data**: with hundreds of thousands of individuals, incorrect associations can be cleaned.

The professor described what happens when a child with a rare genetic condition is sequenced:

1. Perform exome or genome sequencing of the child and often the parents.
2. Find variants not present in the reference genome.
3. Remove variants present in gnomAD.
4. Identify variants that are **de novo** or otherwise consistent with the inheritance pattern.
5. Look at genes known to be involved in diseases matching the clinical phenotype.
6. If needed, validate in the lab using cell or animal models.

This validation is expensive and slow, which is why **computational approaches** are important. However, the professor stressed that tools such as **SIFT** and **PolyPhen**, which try to predict whether a mutation is pathogenic, **fail completely** for many variants; accuracy is still low. Currently, associations rely mostly on sequence data and observations in other patients with the same condition.

[00:30:28–00:32:21]

When asked why sequencing data are free in public databases, the professor explained:

- Most large sequencing projects are paid with **public funds**, so data must be made available to the scientific community.
- ClinVar is also a collaborative effort: hospitals and diagnostic labs upload variants so that all laboratories can see whether other patients with the same condition share the same mutation.

### 5. Downloading variants with the UCSC Table Browser

[00:22:32–00:23:36 and 00:43:32–00:46:38]

To download variants:

- Go to UCSC Genome Browser → **Tools → Table Browser**.
- First locate the gene coordinates, e.g. by typing `GRIN1` in the **lookup** field, which gives the genomic region of the gene.
- For healthy population variants:
  - Group: **Variation**.
  - Track: **gnomAD**.
  - Select the latest version, **gnomAD v4**.
- For disease-associated variants:
  - Group: **Phenotypes, variants and literature**.
  - Track: **ClinVar variants**.
- Then choose output fields such as genomic position, reference/alternate nucleotide, allele frequency, allele count, and variant type.
- The downloaded file can be filtered with tools like `grep` to keep only missense, frameshift, upstream, etc.

### 6. Introduction to the human proteome

[00:47:38–00:50:25]

The **human proteome** is the collection of proteins encoded by the human genome: about **20,000 proteins**, corresponding to about **20,000 coding genes**.

Proteins are the **building blocks and workers of the cell**. Cells differ from tissue to tissue because they express different proteins. DNA transmits information; proteins carry out the functions.

When a student asked whether alternative splicing creates more proteins than coding genes, the professor answered that the additional products are **isoforms** of the same protein: slightly different versions, often expressed more in one tissue than another, but performing essentially the same function. She described them as “different flavours of the same protein.”

Different tissues express different protein sets:

- The brain expresses many proteins.
- Kidney or pancreas express fewer.
- Protein expression depends on cell type, disease state, environment and developmental stage.

### 7. Main functions of proteins

[00:51:27–00:53:54]

Major protein functions:

- **Enzymes**: speed up reactions. Reactions could happen in the cell, but without enzymes they are so slow that practically they do not occur on biological timescales. Expressing an enzyme allows a reaction to happen when and where the cell needs it.
- **Mechanical support** for cells and tissues.
- **Transport**: carrying molecules or ions across membranes or within the cell.
- **Storage** of amino acids, ions, or molecules.
- **Signalling switches**: receiving a signal outside the cell and transmitting it inside.
- **Receptors**: detecting signals and transmitting them.
- **DNA binding**: many proteins participate in transcription and gene expression.
- **Messengers**: carrying messages between cells or between parts of the cell.
- **Motors**: moving organelles or components within the cytoplasm.
- **Defence and other roles**: antibodies, toxins, hormones.

### 8. Sequence → structure → function

[00:53:54–00:57:00]

Protein function depends on the **three-dimensional shape** of the protein. If the shape is altered, function changes.

The 3D structure depends completely on the **amino-acid sequence**:

- Identical sequence → identical structure → identical function.
- Sequence comes from translating the CDS using the genetic code.
- DNA sequence → RNA sequence → amino-acid sequence → folded 3D structure → function.

The professor mentioned **AlphaFold** as an algorithm trying to predict structure from sequence, but noted that it still fails in many regions and for many proteins, so accuracy remains limited.

[00:56:00–00:57:00]

A student asked whether **post-translational modifications** influence structure. The professor said they occur once the protein is already folded and usually do not change global structure. They act mainly as **switches**: activating/deactivating the protein or changing whether it binds another protein. They involve small additions such as a methyl or phosphate group and only slightly change conformation.

[00:58:23]

Although mutations occur at the DNA level, **natural selection acts on protein function**. Only nucleotide changes that preserve or improve protein function tend to persist in future generations. Changes that destroy essential protein function reduce survival or reproductive fitness and are removed.

### 9. Amino acids as building blocks

[00:59:26–01:01:29]

Proteins are made of **20 different amino acids**. Each amino acid has:

- An amino group.
- A carboxylic acid group.
- A side chain that gives it specific physicochemical properties.

The 20 amino acids vary:

- Some are **hydrophobic**.
- Some are **negatively charged**.
- Some are **positively charged**.
- Some can form **hydrogen bonds**.
- Some are small; some are big.

The final protein incorporates the collective properties of all its amino acids.

This matters for variant interpretation: a change from a small amino acid such as glycine to a large one such as arginine is a much bigger chemical change than glycine to alanine, so it is more likely to affect structure and function.

### 10. Four levels of protein structure

[01:01:29–01:04:38 and 01:16:31]

1. **Primary structure**: the amino-acid sequence.
2. **Secondary structure**: local folding into **alpha-helices** and **beta-sheets**. This occurs because the polypeptide is surrounded by water and the amino acids arrange themselves to maximise hydrogen bonding. There are only two main ways to satisfy the hydrogen-bond potential completely: alpha-helix or beta-sheet. **Loops** are stretches of about 8–20 amino acids connecting helices/sheets.
3. **Tertiary structure**: the fully folded 3D shape of a protein, or of a **domain**.
4. **Quaternary structure**: some proteins must associate with other polypeptide chains to function. Example: **haemoglobin** requires **four copies** of the globin protein to carry out its function.

### 11. Domains and the evolution of multi-domain proteins

[01:05:46–01:13:12]

A **domain** is a compact, independently folded unit of tertiary structure. Many proteins contain several domains.

The professor showed a large neuronal protein and explained it has **three domains**:

- One domain binds a molecule.
- Another domain binds another molecule.
- The third domain is a channel that opens.

In the example, when the domains do their jobs, the channel opens and ions pass through, transmitting a signal between neurons. The channel domain can be found reused in other proteins combined with other domains.

Evolutionary interpretation:

- Domains are thought to be **ancestral proteins**.
- Early proteins may have been single-domain.
- Genome rearrangements, duplications, deletions and **mix-and-match** events combined ancestral single-domain proteins into today’s **multi-domain proteins**.

The professor used the **Lego analogy**: domains are like a box of Lego bricks. Nature chooses different bricks to build different proteins. There are **fewer domains than proteins**, just as there are fewer Lego brick types than possible constructions.

### 12. Evolution of new proteins

[01:19:01–01:21:09]

The professor described two main evolutionary mechanisms:

1. **Gene duplication followed by mutation accumulation**:
   - A gene/protein duplicates.
   - Over time, the two copies accumulate different mutations.
   - Eventually they become two different proteins with similar but distinct structures and functions.

2. **Mixing and matching of domains**:
   - Large genomic rearrangements combine regions encoding different domains.
   - This creates new multi-domain proteins by reusing existing functional units.

Selection acts on the **function** of the resulting protein to shape the gene sequence.

[00:42:31]

The professor also noted that of the ~20,000 coding genes in the human genome, about **6,000 genes** are associated with genetic diseases where a single nucleotide change can cause disease. For the remaining ~14,000 proteins, a single change often does nothing.

## What the professor stressed

- **Use the right database for the right question**: ClinVar for pathogenic/likely pathogenic variants in patients; gnomAD for healthy population variation. Do not use ClinVar to look for benign variants. [00:02:40–00:05:01]
- **Both databases contain noise**, and the main way to reduce it is **more data**. [00:24:36–00:27:52]
- **Frameshift and nonsense variants usually produce shorter, non-functional proteins** because they introduce a premature stop codon. [00:05:01–00:06:07]
- **A variant found in healthy individuals in gnomAD is unlikely to cause a severe autosomal dominant disease.** [00:35:56–00:36:58]
- **Sequence determines structure, and structure determines function.** This central dogma of protein biology was repeated several times. [00:53:54–00:57:00]
- **Selection acts on protein function**, not directly on DNA sequence. [00:58:23]
- **There are fewer domains than proteins.** Domains are reusable building blocks, like Lego. [01:08:00–01:10:09]
- **Pathogenicity predictors such as SIFT and PolyPhen still fail for many variants**; computational prediction from one nucleotide change is unreliable. [00:29:06]

## Course logistics mentioned

- Scores from the last partial exam and corrections for assignments are available on Moodle. If you want to review the exam, contact the professor to arrange a meeting. [00:00:00]
- At the time of this session, there were **two classes left**: one the following week and one after Christmas. The following class would finish the human proteome topic. [01:21:09]
- The session included the in-class exercises on **human genetic variation** available on the course page. [00:29:56–00:30:06]

## Self-test

1. You find a missense variant in a healthy adult in gnomAD. For an autosomal dominant severe paediatric disease, what does this strongly suggest?  
<details><summary>Answer</summary>  
It strongly suggests the variant is not disease-causing for that dominant disease: if one copy were sufficient to cause severe disease, healthy adults would not be expected to carry it. A patient with the same variant would likely need another explanation for their phenotype.
</details>

2. Why is ClinVar not the appropriate database for studying neutral or benign variation?  
<details><summary>Answer</summary>  
ClinVar is built from patient reports of disease-associated variants, so benign/neutral variation is not its purpose and may be under-represented or poorly classified. gnomAD is specifically designed to represent healthy population variation.
</details>

3. A coding-region deletion removes 2 nucleotides. Which molecular consequence class applies and why?  
<details><summary>Answer</summary>  
Frameshift. Deleting 2 nucleotides is not a multiple of 3, so it shifts the reading frame downstream, changes all subsequent codons, and usually creates a premature stop codon and a shorter, non-functional protein.
</details>

4. How do both nonsense and frameshift variants tend to produce shorter proteins?  
<details><summary>Answer</summary>  
A nonsense variant directly changes a codon into a stop codon, truncating the protein. A frameshift changes the reading frame, frequently generating a new stop codon early in the coding sequence, which also truncates the protein.
</details>

5. Why can gnomAD contain healthy carriers of pathogenic variants for an autosomal recessive disease?  
<details><summary>Answer</summary>  
In autosomal recessive disease, one mutated copy is not sufficient to cause disease. Carriers are healthy because they still have one functional copy of the gene.
</details>

6. The class found 89 pathogenic/likely pathogenic missense variants in ClinVar for GRIN1 but hundreds of missense variants in gnomAD for the same gene. Explain the difference.  
<details><summary>Answer</summary>  
Most amino-acid changes are neutral and occur in regions or positions that do not disrupt protein folding or function, so they appear in healthy populations. Only mutations affecting essential positions or making severe chemical changes are pathogenic and appear in ClinVar patients.
</details>

7. Describe the filtering workflow the professor outlined for finding the causative variant in a child with a rare genetic disorder.  
<details><summary>Answer</summary>  
Sequence the child and parents; identify variants absent from the reference genome; remove variants present in gnomAD; prioritise de novo variants or variants fitting the inheritance pattern; check whether affected genes match the clinical phenotype; if possible, validate in the lab or in animal models.
</details>

8. What does “sequence determines structure determines function” mean, and how do post-translational modifications fit into this idea?  
<details><summary>Answer</summary>  
The amino-acid sequence dictates how the protein folds into its 3D structure, and that structure determines what the protein does. Post-translational modifications generally do not determine global structure; they occur after folding and act as small chemical switches that alter activity, localisation, or binding, with only slight conformational changes.
</details>

9. Why are there fewer domains than proteins?  
<details><summary>Answer</summary>  
Domains are conserved structural/functional units that have been reused and combined during evolution. A limited set of domains can be arranged in many different ways, just as a limited set of Lego bricks can build many different structures, so the number of possible proteins exceeds the number of domain types.
</details>

10. How can gene duplication give rise to a new protein function?  
<details><summary>Answer</summary>  
When a gene duplicates, one copy can continue performing the original function while the other copy accumulates mutations. Over evolutionary time, the two copies diverge in sequence, structure and function, producing a new protein.
</details>

11. Why did the professor say computational tools like SIFT and PolyPhen “fail completely” for many variants?  
<details><summary>Answer</summary>  
Their accuracy is still low; we cannot reliably infer from a single nucleotide change alone whether it will disrupt protein structure and function enough to cause disease. Current associations rely more on population databases, patient cohorts and experimental validation.
</details>

12. What is quaternary structure, and what example was given?  
<details><summary>Answer</summary>  
Quaternary structure is the association of multiple polypeptide chains to form a functional protein. The example given was haemoglobin, which requires four protein subunits to carry oxygen.
</details>

## Related course materials

- [1.6-Human Genomic Variations](../../materials/07_1.6-Human%20Genomic%20Variations.pdf)
- [2-The human Proteome](../../materials/08_2-The%20human%20Proteomev2.pdf)

# 22_BE-Molecular Biology- Session 12-20260108_140204-Meeting Recording

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 12 (Thursday, 8 January 2026, 2:02 PM)
- **Video:** [22_BE-Molecular Biology- Session 12-20260108_140204-Meeting Recording.mp4](../../recordings/22_BE-Molecular%20Biology-%20Session%2012-20260108_140204-Meeting%20Recording.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%2012-20260108_140204-Meeting%20Recording.mp4)
- **Duration:** 01:27:45 · **Language:** en
- **Transcript:** [22_BE-Molecular Biology- Session 12-20260108_140204-Meeting Recording.md](../../transcripts/22_BE-Molecular%20Biology-%20Session%2012-20260108_140204-Meeting%20Recording.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary

This final session covered the **regulation of gene expression**, the third major topic of the molecular biology block. The professor explained that all cells contain the same genome, but cells differ because they express different subsets of genes. The class focused on the main mechanisms that control whether a gene is transcribed: **chromatin structure and accessibility**, **histone modifications**, **ATP-dependent nucleosome remodelling**, **DNA methylation at CpG dinucleotides**, and **transcription factors/enhancers**. She also briefly introduced methods for measuring gene expression: **microarrays**, **RNA-seq**, and **single-cell RNA-seq**, before walking through **UCSC Genome Browser exercises** using the gene *RING1* to visualise expression, CpG islands, histone marks, enhancer-associated marks, transcription factor binding sites, and transcription start sites.

Key takeaways:

- Gene expression is the set of mechanisms by which cells increase or decrease production of RNA and protein products.
- Cell identity and tissue identity are determined by **which genes are expressed**, not by differences in the DNA sequence itself.
- **Heterochromatin** is tightly packed and transcriptionally silent; **euchromatin** is open and transcriptionally active.
- **CpG islands in promoters remain unmethylated in active genes and methylated in inactive genes**; methylation blocks transcription factor binding and can silence genes.
- Histone modifications can be temporary (acetylation, phosphorylation) or more permanent (methylation), and they help control DNA accessibility.
- **Enhancers** can be far away in linear DNA but act at a distance because chromatin remodelling brings them close to their target promoter in 3D.
- Modern transcriptomics (RNA-seq and single-cell RNA-seq) allows quantitative measurement of gene expression and is a major source of data in bioinformatics.

## Key concepts

- **Regulation of gene expression** – the group of mechanisms by which cells increase or decrease the production of gene products (RNA and, ultimately, proteins) [00:02:11].
- **Short-term vs long-term regulation** – short-term regulation responds to the environment, e.g. stress; long-term regulation is associated with stable cell/tissue identity [00:03:19].
- **Chromatin** – DNA wrapped around histone proteins; its packing state controls whether DNA is accessible to transcription machinery [00:08:34].
- **Heterochromatin** – highly packed, silent DNA where transcription proteins cannot bind [00:09:42].
- **Euchromatin** – less packed, active DNA with exposed regions where transcription can start [00:09:42].
- **Histone modification / histone code** – post-translational chemical modifications on histone tails that change DNA–histone interaction and chromatin state [00:14:57].
- **Nucleosome remodelling complexes** – ATP-dependent protein complexes that slide, evict, or exchange histones to expose DNA regions [00:17:47].
- **DNA methylation** – addition of methyl groups to cytosine in **CpG dinucleotides**; promoter methylation is associated with gene silencing [00:19:58].
- **CpG islands** – regions rich in CpG dinucleotides; about 70% of promoters contain CpG islands; unmethylated CpG islands allow protein binding and transcription [00:22:06].
- **Transcription factors** – proteins that bind DNA to activate or repress transcription; about 1,400 are encoded in the human genome [00:24:14].
- **Enhancers** – non-coding DNA regions, roughly 200–1,000 nucleotides, where transcription factors bind to regulate a gene; can be close to or far from the target gene [00:30:28].
- **Transcriptome** – the collection of RNA molecules expressed in a sample, including their sequence and quantity [00:38:45].
- **Post-transcriptional regulation** – one of the regulatory layers listed by the professor, together with chromatin remodelling, DNA methylation, and transcription factors; not expanded in detail in this session [00:07:24].

## Detailed notes

### Why gene expression is regulated

Gene expression is the set of mechanisms by which cells increase or decrease the production of gene products. This can happen **short-term**, in response to the environment, or **long-term**, to establish stable cell/tissue identity [00:02:11–00:03:19].

The professor’s central example: all cells in the body have the same DNA and could potentially express around 20,000 proteins and 40,000 RNA molecules, but no cell expresses everything at once. A **nerve cell** and an **epithelial cell** have the same genome, yet the nerve cell may express the “green” and “yellow” genes, while the epithelial cell expresses the “yellow” and “purple” genes. The green gene would never be expressed in the epithelial cell. Therefore, what makes cells different is the set of RNAs and proteins they produce [00:04:19–00:05:20].

A **short-term** example: if one of two identical nerve cells is under stress, signals can cause a “blue” gene to be transcribed and its protein produced in that cell only. This is an environmental response rather than a stable identity difference [00:06:22].

The main regulators are [00:07:24]:
- chromatin remodelling mechanisms, including histone modifications and ATP-dependent chromatin remodelling complexes,
- DNA methylation,
- transcription factors,
- post-transcriptional regulation.

### Chromatin structure and accessibility

DNA is a double strand wrapped around **histone proteins**, allowing the large genome to fit inside the nucleus. The DNA–histone interaction is electrostatic. At the chromosome level, DNA can exist as [00:08:34–00:09:42]:

- **Heterochromatin** – highly packed; DNA is not exposed, so transcription proteins cannot bind; genes are silent.
- **Euchromatin** – less packed; many DNA regions are exposed, allowing transcription to start.

Euchromatin comprises only **2–3% of total DNA** but contains **more than 90% of transcription-factor-bound regions**. There is competition between histones and transcription factors for DNA binding: histones tend to block transcription, while some transcription factors activate it [00:10:48].

Chromatin remodelling is therefore defined as the **dynamic modification of chromatin architecture to allow access of DNA to regulatory proteins**, and this controls gene expression [00:11:51–00:12:53].

### Histone modifications

Histone modifications are **post-translational modifications** on the tails of histone proteins. Adding chemical groups to histone tails changes the interaction between histones and DNA: some modifications pack DNA more tightly, others loosen it, making DNA accessible [00:12:53–00:14:57].

The combination of chemical modifications is known as the **histone code** or **histone marks** [00:15:58].

Common histone modifications include [00:16:01]:
- acetylation,
- methylation,
- phosphorylation,
- deamination,
- ubiquitination.

The professor stressed the difference in stability [00:16:40–00:17:47]:

- **Phosphorylation and acetylation** are usually temporary changes, added or removed in response to the environment.
- **Methylation** is more permanent and is related to stable tissue-specific gene expression.

### ATP-dependent nucleosome remodelling complexes

These protein complexes use energy to change how DNA wraps around histones. If the transcription start site is buried inside a nucleosome, transcription cannot begin. The remodelling complex can [00:17:47–00:18:48]:

- **nucleosome sliding** – slide histones so the transcription start site becomes exposed,
- **nucleosome eviction** – remove histones, exposing the region,
- **histone exchange** – replace old histones with new ones.

These complexes therefore change which DNA regions are exposed and are also involved in **DNA repair** [00:19:58].

### DNA methylation and CpG islands

DNA methylation is different from histone methylation: it adds methyl groups to **cytosine in CpG dinucleotides** [00:19:58].

Facts given in class [00:20:15–00:21:50]:

- The human genome contains about **28 million CpG dinucleotides**; approximately **75% are methylated**.
- CpG methylation increases the frequency of spontaneous mutation, especially **C → T**.
- DNA methylation is essential for normal mammalian development and is associated with:
  - genomic imprinting,
  - X-chromosome inactivation,
  - repression of transposable elements,
  - ageing,
  - carcinogenesis.
- Adenine methylation has also been identified.

**CpG islands** are regions rich in CpG dinucleotides. In the human genome, less than 10% of all CpGs are CpG islands, but **about 70% of promoter regions contain CpG islands** [00:22:06–00:23:09].

The key rule, corrected during class [00:43:58–00:45:14]:

- In **active genes**, CpG islands in promoter regions remain **unmethylated**, allowing transcription factors and transcription machinery to bind.
- In **inactive genes**, these CpG islands are **methylated**, creating a steric clash that prevents protein binding and therefore silences the gene.

Inactive gene promoters can also recruit proteins that bind methylated DNA; these proteins can recruit **histone methyltransferases or deacetylases**, promoting histone deacetylation and methylation. Thus, DNA methylation and histone modification are connected [00:24:14].

Abnormal methylation of CpG islands that should be unmethylated can silence genes and may be related to **cancer** [00:22:06].

### Transcription factors and enhancers

Transcription factors are proteins that bind specific DNA sequences to control gene expression. There are about **1,400 transcription factors** in the human genome. They can act as **activators** or **repressors**, and the same factor may activate some genes while repressing others [00:24:14–00:30:28].

**Enhancers** are non-coding DNA regions, usually **200–1,000 nucleotides**, where transcription factors bind. They are often close to their target gene but can also be **very distal in linear sequence** while still being structurally close in 3D [00:30:28–00:31:58].

The professor gave a detailed example of an enhancer located far from gene B, with another gene in between [00:31:58–00:34:09]:

- In the linear arrangement, a transcription factor bound at the enhancer is too far from gene B to influence it, and it does not regulate gene A.
- Through chromatin remodelling (histone modifications or ATP-dependent remodelling complexes), the enhancer can be repositioned close to gene B.
- Then the enhancer-bound transcription factor can interact with another factor bound at gene B’s promoter, allowing transcription of gene B.

The full activation sequence in response to a signal is [00:26:57–00:29:08]:

1. A signal triggers post-translational modification of a transcription factor.
2. The modified transcription factor moves from the cytosol into the nucleus.
3. The DNA region containing the transcription factor binding site must be exposed: no DNA methylation and no tight wrapping around histones.
4. The transcription factor binds its DNA sequence.
5. RNA polymerase binds to the promoter and starts transcription.
6. RNA and then protein are produced to respond to the environment.

For this to work, both the **enhancer region** and the **promoter region** must be unmethylated and exposed, and transcription factors must be correctly modified and localised [00:34:09].

### Measuring gene expression

Over the last 15 years, it has become possible to measure which genes are expressed in a given tissue or patient. Differential expression between disease and non-disease samples helps understand disease mechanisms and identify biomarkers [00:35:10–00:36:17].

Three techniques were compared:

- **Microarrays** – detect expression of thousands of genes simultaneously, but only **qualitatively** (expressed vs not expressed); they cannot quantify RNA amount [00:36:17–00:37:41].
- **RNA-seq** – RNA is isolated, fragmented, converted into DNA, and sequenced. It determines the **transcriptome**: the collection of expressed RNA molecules, their sequence, and their quantity [00:37:41–00:38:45]. Bulk RNA-seq captures an **average of thousands of cells**. It can identify post-transcriptional modifications, alternative splice transcripts, SNPs, and gene expression changes over time or between groups [00:38:45–00:39:47].
- **Single-cell RNA-seq** – determines gene expression **for individual cells**, rather than an average across thousands of cells. This is a newer technique [00:39:47].

When comparing expression profiles, researchers usually do not work gene by gene; instead they use **Gene Ontology terms**, which are keywords describing the biological processes or molecular functions of genes. For example, genes involved in the cell cycle may be more active in disease, while lipid metabolism genes may be more active in non-disease [00:39:47–00:42:00].

Methods based on **chromatin immunoprecipitation** can also detect **histone modifications** and **transcription factor binding sites**, linking chromatin marks to gene expression [00:42:00–00:42:24].

The professor emphasised that transcriptomics is a very active area in bioinformatics, producing huge datasets. Together with genome, proteome, and metabolome data, these methods give an increasingly complete picture of a patient, although the causal changes in disease are still not fully understood [00:48:22–00:50:25].

### UCSC Genome Browser practical exercises

The practical used the UCSC Genome Browser with the gene **RING1** to visualise regulatory elements [00:52:51].

**Gene display** – Use NCBI RefSeq to show the gene with exons and introns; zoom out several times because regulatory elements often lie outside the gene body [00:53:54–00:55:10].

**Expression across tissues** – Use **GTEx transcripts** in the expression section. RING1 is expressed mainly in the brain and not appreciably in other tissues. Different transcripts show different brain-region expression: one transcript was restricted to two brain regions, including cerebellum, while another was expressed in more regions. The exercise then filtered to brain tissues only [00:55:39–01:04:07].

**Single-cell expression** – Use the UCSC single-cell RNA-seq track for a **cortex** dataset. This shows expression levels of RING1 in individual cortex cells, rather than an average of the whole tissue [01:04:36–01:05:46].

**Histone marks and CpG islands** – In the ENCODE Regulation section:

- Display **H3K4me3** histone marks; these appear especially in the region upstream of the gene, suggesting the promoter [01:08:37–01:09:08].
- Display **CpG islands**; islands are visible upstream and inside the gene. CpG islands in the promoter region indicate unmethylated DNA where proteins can bind [01:09:08–01:10:49].
- Display a histone **acetylation** mark associated with enhancers; these marks appear close to the gene and suggest an enhancer region [01:11:56–01:14:17].

To locate the promoter: if the gene is on the forward strand, the promoter is to the left (5′ side). The professor suggested considering roughly **5,000–10,000 nucleotides upstream** to be safe, though the exact promoter length varies. CpG islands can help localise it [01:10:49–01:12:59].

**Transcription factors** – Display ENCODE transcription factor peak clusters. Transcription factor binding peaks overlap the same regulatory region already identified by histone marks and CpG islands, reinforcing that this region regulates RING1 expression [01:17:15–01:20:24].

**Regulatory elements and transcription start sites** – Use **GeneHancer** in the Regulation section to display regulatory elements and transcription start sites. The transcription start site appears as a red line [01:23:09–01:24:12].

The overall message: you can combine expression data, histone marks, CpG islands, transcription factor binding, and regulatory element tracks to identify the regions likely controlling a gene’s expression.

## What the professor stressed

- **Cell identity comes from the pattern of expressed genes**, not from a different genome [00:05:20].
- **Regulation of gene expression is extremely complex and not fully understood**; we have identified many pieces but not the complete puzzle [00:48:22].
- **Histone methylation is more permanent**, while **acetylation and phosphorylation are more temporary** responses to the environment [00:16:40–00:17:47].
- The key relationship: **CpG islands in promoters are unmethylated in active genes and methylated in inactive genes** [00:43:58–00:45:14]. She explicitly corrected this during the session.
- An enhancer can be far from its target gene in linear sequence but functionally close in 3D because of chromatin remodelling [00:31:58–00:34:09].
- Gene expression measurement, especially **transcriptomics**, is a hot topic in bioinformatics and generates large patient-level datasets [00:49:25].
- For the UCSC exercises, **different histone marks are not all equivalent**: H3K4me3 is associated with promoters, and acetylation marks are associated with enhancers [00:19:22].
- The professor reminded students that genomic databases change constantly: new transcription factors, enhancers, and promoters are still being discovered and added [00:51:46].

## Course logistics mentioned

- This was the **last class** of the biomedicine course [00:00:00].
- **Task 3** is due around the same time as the exam, approximately one or two days before, in about two weeks [00:00:00, 01:25:36].
- The exam will consist of **short questions** and the professor expects **short answers**, similar to the previous exam [01:25:36].
- The exam will include **genome variation**, **regulation of gene expression**, and **proteins**. She said she would send a message with the exact contents [01:25:36].
- Failed exams can be **reassessed** in about three to four weeks; students can retake exams in which they did not obtain at least a 5 [01:25:36].
- Students can contact her by email or request a tutoring session for questions [01:26:39].

## Self-test

1. Two cells in the same body have identical genomes, yet one is a nerve cell and one is an epithelial cell. Explain why their proteins differ.
<details><summary>Answer</summary>
They express different subsets of genes. Both cells have the potential to express all genes, but regulatory mechanisms such as chromatin accessibility, DNA methylation, histone modifications, and transcription factors activate only certain genes in each cell type. Long-term marks, especially histone methylation, help maintain these tissue-specific expression patterns.
</details>

2. Compare heterochromatin and euchromatin in terms of DNA packing and transcription.
<details><summary>Answer</summary>
Heterochromatin is highly packed DNA associated with histones; the DNA is not exposed, so transcription factors and polymerase cannot bind and genes are silent. Euchromatin is less packed, exposes DNA regions, allows transcription factor binding, and is transcriptionally active. Euchromatin is only 2–3% of DNA but contains more than 90% of transcription-factor-bound regions.
</details>

3. Why does the professor describe histone acetylation as a temporary change but histone methylation as more permanent?
<details><summary>Answer</summary>
Acetylation and phosphorylation can be added and removed quickly in response to environmental signals, so they support short-term gene regulation. Methylation tends to remain longer and is associated with stable, long-term cell- or tissue-specific expression patterns.
</details>

4. A promoter contains an unmethylated CpG island. What does this suggest about the gene? What would happen if that island became methylated?
<details><summary>Answer</summary>
An unmethylated CpG island in a promoter suggests the gene is active, because transcription factors and the transcription machinery can bind. If the island becomes methylated, the methyl groups create a steric clash that prevents protein binding, so transcription cannot start and the gene is silenced. Abnormal methylation of CpG islands can be associated with cancer.
</details>

5. An enhancer is located far from its target gene in linear DNA, with another gene between them. How can it still regulate the target gene?
<details><summary>Answer</summary>
Chromatin remodelling can change the 3D conformation of DNA, bringing the enhancer close to the target gene. Then a transcription factor bound at the enhancer can interact with factors bound at the target gene’s promoter, enabling transcription. The linear distance is less important than structural proximity in 3D.
</details>

6. What is the difference between a microarray experiment and an RNA-seq experiment in terms of quantification?
<details><summary>Answer</summary>
Microarrays are qualitative: they can tell you whether genes are expressed or not, and they can compare expression between samples, but they cannot quantify the amount of RNA. RNA-seq is quantitative: it determines the sequence and the amount of expressed RNA molecules, giving a transcriptome.
</details>

7. Why is single-cell RNA-seq informative compared with bulk RNA-seq?
<details><summary>Answer</summary>
Bulk RNA-seq averages expression over thousands of cells, so it can hide differences between individual cells. Single-cell RNA-seq measures gene expression in individual cells, revealing heterogeneity within a tissue and expression profiles of specific cell populations.
</details>

8. After finding thousands of differentially expressed genes, why might a researcher use Gene Ontology terms instead of listing every gene?
<details><summary>Answer</summary>
Gene Ontology terms describe genes with keywords linked to biological processes or molecular functions. Grouping differentially expressed genes into ontology terms helps identify which cellular processes or pathways are activated or inactivated in a disease or tissue, which is more interpretable than a long gene list.
</details>

9. In UCSC Genome Browser, you see H3K4me3 marks, unmethylated CpG islands, and transcription factor peaks immediately upstream of a gene. What do these observations suggest?
<details><summary>Answer</summary>
They suggest a promoter/regulatory region. H3K4me3 marks are associated with promoters; CpG islands in promoters are unmethylated in active genes; and transcription factor binding peaks indicate proteins that regulate transcription. Together these features identify the region likely controlling the gene’s expression.
</details>

10. How are DNA methylation and histone modification connected in gene silencing?
<details><summary>Answer</summary>
Proteins that bind methylated DNA can recruit enzymes such as histone methyltransferases or deacetylases, which add methyl groups to histones or remove acetyl groups. These histone modifications promote a more closed chromatin state, reinforcing silencing. Thus DNA methylation and histone modification cooperate to keep genes inactive.
</details>

11. What is the role of ATP in nucleosome remodelling complexes?
<details><summary>Answer</summary>
ATP provides the energy needed to slide nucleosomes, evict histones, or exchange histones, thereby changing which DNA regions are exposed. Unlike simple histone modifications, these remodelling activities require energy.
</details>

12. Define the term “transcriptome”.
<details><summary>Answer</summary>
The transcriptome is the collection of all RNA molecules expressed in a sample, including both their sequences and their quantities. RNA-seq is used to determine the transcriptome.
</details>

## Related course materials

- [3 - Regulation of Gene Expression](../../materials/09_3-%20Regulation%20of%20Gene%20Expression.pdf)

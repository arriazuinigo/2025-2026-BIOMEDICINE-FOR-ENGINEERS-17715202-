# 05_BE-Molecular Biology- Session 2-20251009_140113-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 2 (Thursday, 9 October 2025, 2:01 PM)
- **Video:** [05_BE-Molecular Biology- Session 2-20251009_140113-Enregistrament de la reunió.mp4](../../recordings/05_BE-Molecular%20Biology-%20Session%202-20251009_140113-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%202-20251009_140113-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:24:43 · **Language:** en
- **Transcript:** [05_BE-Molecular Biology- Session 2-20251009_140113-Enregistrament de la reunió.md](../../transcripts/05_BE-Molecular%20Biology-%20Session%202-20251009_140113-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary
This session completed the introduction to nucleic acid structure (RNA recap, then DNA double helix in detail) and moved into the central dogma: how DNA replicates, is repaired, is transcribed into RNA, and how RNA is translated into protein. The professor explained DNA packaging by histones, the anatomy of a eukaryotic gene (promoter, exons, introns, terminator), alternative splicing, and the genetic code. The second half of the class was a practical, computational exercise on going from a raw gene sequence to the complementary strand, the pre-mRNA, and finally the protein sequence. The session ended with the professor walking through the exercise solutions and stressing that this DNA→RNA→protein flow is fundamental.

Key takeaways:
- DNA is a double-stranded, antiparallel helix held together by specific base pairing (A–T with 2 H-bonds, G–C with 3 H-bonds); each turn is 3.4 nm with 10 base pairs.
- Histones pack DNA into nucleosomes/chromatin via electrostatic interactions, and this packing also regulates gene expression by controlling access for transcription and replication.
- The central dogma is DNA → RNA → protein; only ~1.5% of the human genome is transcribed into mRNA, while >90% is transcribed into other functional RNAs.
- Replication and transcription always proceed 5'→3'; a gene on the reverse strand is transcribed from right to left, and the promoter is always upstream of the gene, not part of the transcribed sequence.
- Eukaryotic genes contain exons and introns; splicing removes introns and alternative splicing produces multiple different mRNAs (and therefore proteins) from one gene.
- Translation reads mRNA in codons (three nucleotides); the genetic code is redundant/degenerate, which buffers some mutations.

## Key concepts
- **DNA double helix**: two antiparallel polynucleotide chains held together by hydrogen bonds between complementary bases (A–T, G–C), wound around each other to form major and minor grooves [00:01:01–00:06:05].
- **Base complementarity**: chemical consequence of H-bonding potential — G–C makes 3 hydrogen bonds, A–T makes 2; other pairings are chemically impossible [00:02:48].
- **Antiparallel strands**: one strand runs 5'→3', the other 3'→5'; named after the free carbon on the terminal sugar [00:03:55].
- **Histones**: positively charged proteins that bind the negatively charged phosphate backbone of DNA to compact it [00:09:17].
- **Nucleosome**: basic repeating unit of chromatin; contains 8 histone proteins and 146 nucleotides of DNA [00:10:26–00:11:26].
- **Chromatosome**: nucleosome plus one additional histone protein, making two full turns of DNA around the octamer [00:11:26].
- **Central dogma**: flow of genetic information: DNA → (transcription) → RNA → (translation) → protein [00:25:45–00:28:56].
- **Gene**: DNA sequence containing the transcribed region (RNA coding sequence + terminator); the promoter is upstream and not transcribed [00:41:00].
- **Promoter**: upstream sequence containing signals (e.g., TATA box) where transcription factors bind to initiate transcription [00:45:11].
- **Transcription factors**: proteins that bind the promoter to activate or repress transcription [00:46:28].
- **Exons/introns**: exons are retained in mature mRNA; introns are removed by splicing [00:52:44].
- **Alternative splicing**: different combinations of exons produce different mRNAs from a single gene [00:53:46].
- **Codon**: group of three nucleotides read during translation; each specifies one amino acid [00:58:36].
- **Genetic code redundancy (degeneracy)**: multiple codons can specify the same amino acid, buffering mutations [00:59:00].
- **CDS (coding sequence)**: portion of mRNA translated into protein; flanked by 5' UTR and 3' UTR [01:00:41].
- **Mutation**: permanent change in DNA sequence caused by replication errors, chemicals, metabolites, thermal collisions, or radiation [00:37:36].

## Detailed notes

### Recap: RNA structure
**[00:00:00]**
RNA is single-stranded. To satisfy its hydrogen-bonding potential, the bases form H-bonds within the same strand, folding the RNA into a three-dimensional structure that allows it to perform a function inside the cell. Contrast with DNA, which uses two strands.

### DNA structure
**[00:01:01]**
DNA (deoxyribonucleic acid) consists of two long polynucleotide chains held together by hydrogen bonds between bases on opposite strands.
- A always pairs with T; G always pairs with C.
- This pairing rule is chemical: G–C can form 3 hydrogen bonds, A–T forms 2. Pairings like T–C or G–A are chemically impossible [00:02:48].
- The two strands are **antiparallel**: one runs 5'→3', the other 3'→5'. The 5' and 3' designations refer to the free carbon atom on the terminal sugar [00:03:55].
- The backbone is alternating phosphate–sugar; bases attach to the sugars and face each other, forming H-bonds [00:05:00].
- Coiling of the two strands creates alternating **major and minor grooves** on the helix [00:05:00–00:06:05].

### DNA dimensions and genome scale
**[00:06:05]**
- Each turn of the double helix comprises about 10 base pairs; one complete helical turn is **3.4 nm** long; helix diameter is about **2 nm**.
- Each base pair is **0.34 nm** long.
- Human genome: ~3.2 × 10^9 nucleotides (per haploid copy).
- Diploid human genome: 3 billion base pairs; with two copies, **6 billion base pairs** per diploid cell [00:08:08].
- Each diploid cell therefore contains about **2 meters of DNA** (~6 × 10^9 bp × 0.34 nm) [00:08:51].
- The human body has an estimated 50 trillion cells, giving about 100 trillion meters of DNA in a body that must all fit inside cell nuclei [00:09:00].

### DNA packing: histones, chromatin, nucleosome
**[00:09:17]**
How does 2 m of DNA fit into a nucleus? Histone proteins solve this.
- Histones have **positive charges** that interact electrostatically with the **negative charges** of DNA phosphate groups.
- These interactions compact the DNA, making the DNA–protein complex smaller.
- **Chromatin** = DNA + histone proteins. Its basic repeating structural unit is the **nucleosome**.
- A nucleosome contains **8 histone proteins** and **146 nucleotides** of DNA [00:10:26–00:11:26].
- Adding one more histone protein and two full turns of DNA around the octamer gives the **chromatosome** [00:11:26].
- Packing hierarchy: DNA → chromatin → nucleosomes → chromatosome → chromosome [00:12:33].
- **Regulatory role**: histones are not just packaging. To transcribe or replicate DNA, the strands must be separated, so histones must first unpack. Other proteins modify histones to expose the required DNA region, making histones key regulators of gene expression [00:12:33–00:13:50].

### PyMOL visualization exercise (RNA vs DNA)
**[00:14:22]**
The professor demonstrated structures in PyMOL:
- RNA structure: fetch `5TPY` (the code was initially said as "5-DPY" but typed as 5TPY). Single-stranded; backbone orange; bases from the **same strand** form H-bonds, giving 3D structure [00:15:22–00:17:35].
- DNA structure: fetch `5DNM`. Double-stranded; shows major and minor grooves clearly; bases from **opposite strands** interact [00:17:35–00:18:42].
- The `5DNM` structure also contains histone proteins. Visualizing the protein as a surface shows it is extremely tightly packed against DNA.
- Extra molecules (sulfate, magnesium ion) in the structure are experimental artifacts used to stabilize the structure, not real parts of chromatin; they can be hidden with the `h` command [00:20:44–00:21:30].
- Selection shortcuts: `s` (show), `h` (hide) [00:21:30].

### Central dogma of molecular biology
**[00:25:45]**
Information flows: **DNA → RNA → protein**.
- DNA contains all information (genes) for cell survival, replication, etc.
- Transcription produces RNA molecules. Some RNAs fold and function directly; others are translated into proteins.
- Approximate numbers given: 60,000 genomic regions/genes can be transcribed into RNAs; ~20,000 are messenger RNAs translated into proteins [00:29:10].
- **What makes one cell type different from another** is the set of proteins it produces (size, shape, and function of proteins differ per tissue). Gene expression — which genes are transcribed — differs by cell type, disease state, and developmental stage; cells only transcribe/translate what is needed [00:30:00–00:33:08].
- Proteins are what "really do the work" inside the cell, although RNA molecules also have regulatory functions [00:33:30].

### DNA replication
**[00:34:10]**
- Replication is semiconservative: the double helix opens and each original strand serves as a template for a new complementary strand. Starting from one double strand, you end with two double strands.
- Histones must unpack first; proteins such as **topoisomerases** and **helicases** participate in opening the helix (names given as context, not required detail) [00:34:34].
- **Key rule: replication always proceeds 5'→3'** [00:35:22].
- For the main strand (5'→3') replication goes left-to-right; for the complementary strand (3'→5'), replication goes right-to-left because synthesis must always be 5'→3'.
- Fragments of DNA are synthesized and later joined to the template strand; a linked video explains the full mechanism [00:35:50].

### DNA repair and mutations
**[00:36:30]**
- DNA is damaged/mutated constantly; repair mechanisms exist.
- A **mutation** is a permanent change in the DNA sequence that remains in the genome across generations [00:37:20].
- Four main causes of DNA mutation: replication errors, chemicals, body metabolites, thermal collisions, and radiation [00:37:36].
- Replication error rate: about **1 mistake per 10^7 nucleotides**. Repair mechanisms reduce this to about **1 permanent mutation per 10^9 nucleotides** per replication [00:38:36–00:39:47].
- The human genome is ~3.2 × 10^9 nucleotides, so every round of replication produces some permanent mutations.
- Consequences: mutations can be neutral, can predispose to disease when combined with other mutations/environment, or can directly cause malfunctioning proteins and diseases (e.g., cancer) [00:39:47–00:40:30].
- Mutations are "good" in the sense that they generate variation; otherwise we would have the same genome as millions of years ago [00:40:30].

### Transcription: anatomy of a gene
**[00:40:52]**
- Transcription copies a DNA sequence into RNA; the resulting RNA may be translated into protein.
- A **gene** consists of (from upstream to downstream): the **promoter**, the **RNA coding sequence**, and the **terminator**. The promoter is **not part of the gene** and is **not transcribed**; it lies upstream of the coding sequence [00:41:00–00:43:21].
- During transcription, histones unpack, the double helix opens, and **one strand acts as a template** to synthesize a single-stranded RNA molecule.
- RNA uses **U (uracil) instead of T**; otherwise sequence is like the DNA strand [00:42:30].
- **Upstream** = toward 5' region; **downstream** = toward 3' [00:43:21].
- Genes can be on the **forward (main) strand** or the **reverse strand**; transcription always goes 5'→3'.
  - Forward gene: transcription goes left-to-right; promoter is on the **left**.
  - Reverse gene: transcription goes right-to-left; promoter is on the **right**.
  - The promoter is always immediately upstream of the gene [00:43:50–00:45:11].
- Most promoters contain specific sequences such as the **TATA box** (transcribed as "TATA-BOC") recognized by proteins [00:45:11].

### Regulation of transcription
**[00:45:11–00:48:30]**
- Proteins that bind the promoter and regulate transcription are **transcription factors**.
- Transcription is a complex network: to produce a protein, other proteins must bind the promoter; an RNA polymerase holoenzyme ("alloenzyme" in the transcript) then binds to initiate transcription.
- Distant DNA sequences can also bind proteins that interact with transcription factors; because of 3D folding, sequences far in linear distance can be close in space and regulate gene expression.
- Regulatory proteins include:
  - **Activators**: bind promoter to start transcription.
  - **Co-activators**: bind activators to speed up transcription.
  - **Repressors**: bind promoter to block transcription.
  - **Co-repressors**: bind repressors to further stop transcription.
- Transcription always proceeds 5'→3'; the RNA molecule contains the coding sequence and terminator, and is released after the terminator signals stop [00:48:30–00:49:36].

### Prokaryotic vs eukaryotic transcription
**[00:49:36]**
- **Prokaryotes (bacteria)**: genes are arranged together with little intergenic space; one RNA molecule can contain sequences for several (5–6) genes, producing several proteins at once (an operon). Usually these proteins have related functions needed simultaneously [00:50:38–00:51:20].
- **Eukaryotes**: more steps are required before translation:
  1. A **pre-mRNA** is made.
  2. It is processed into **mature mRNA** (5' cap addition, poly-A tail addition, splicing).
  3. Then translation occurs [00:51:39–00:52:44].
- Only ~1.5% of the human genome is transcribed into mRNA that will be translated; **>90%** is transcribed into other RNA molecules. RNA molecules live about **7–10 hours** [00:56:20–00:56:52].
- **RNA-seq** is a technique that quantifies RNA molecules and their sequences, enabling comparison of gene expression between cells, tissues, or disease states [00:56:52].

### RNA processing: splicing and alternative splicing
**[00:52:44]**
- Pre-mRNA processing in eukaryotes:
  - Addition of a **5' cap** (a modified nucleotide at the beginning).
  - Addition of a **poly-A tail** (multiple adenine nucleotides at the 3' end).
  - **Splicing**: removes **introns** (green regions in slides) and joins **exons** (orange) to make mature mRNA [00:52:44–00:53:46].
- **Alternative splicing**: different combinations of exons are included/excluded in different transcripts from the same gene.
  - Example given: one gene with exons 1–5 produces three mRNAs: one with all exons, one lacking exon 3, one lacking exon 4 → three different proteins from one gene [00:53:46–00:55:06].
- The information for which exons to include is **encoded in the DNA sequence itself** (splice sites/signals, in introns and exons). Proteins read these signals, but the "language" is still not fully understood [01:05:00–01:07:50].
- After processing, mature mRNA moves from nucleus to cytoplasm for translation.

### Translation and the genetic code
**[00:57:25]**
- Translation occurs at the **ribosome** (a complex of RNA and protein); **transfer RNAs** (tRNAs) also participate [00:59:38].
- mRNA is read in **codons** — groups of three nucleotides. Each codon specifies one amino acid via the **genetic code** table [00:58:00].
- The genetic code is **redundant/degenerate**: several codons code for the same amino acid (e.g., phenylalanine is UUU or UUC; leucine can be UUA or UUG). This redundancy means some DNA mutations do not change the amino acid sequence, so the protein stays identical [00:59:00–01:00:00].

### mRNA anatomy: UTRs, CDS, start and stop codons
**[01:00:41]**
- A mature mRNA has:
  - **5' UTR** (untranslated region at the beginning) — not translated; contains binding sites that control translation initiation and mRNA stability.
  - **CDS (coding sequence)**: the central region actually translated into protein.
  - **3' UTR** — not translated; important for regulation/stability.
- The first codon of the CDS is always **AUG**, coding for **methionine (M)** — the first amino acid of every protein [01:01:46].
- The last codon is a **stop codon**: UAA, UAG, or UGA. The stop codon is not translated into an amino acid; it signals termination [01:02:10].

### Worked example: from gene sequence to protein
**[01:01:46–01:04:50]**
The professor walked through a slide example:
- A genomic DNA sequence contains a promoter (upstream), then exons (green) and introns (red).
- Transcription initiation site and final transcription site mark the gene boundaries.
- Introns are removed; exons are joined; 5' cap and poly-A tail are added.
- 5' and 3' UTRs are not translated; only the CDS is.
- In the CDS, every three nucleotides form a codon; the first codon is AUG (methionine, M); the last is a stop codon (not included in protein).
- Two alternatively spliced mRNAs from the same gene can produce different protein sequences.

### Practical exercise (transcription and translation)
**[01:09:16]**
Exercise given from the course page "Exercises on Transcription and Translation":
- A gene on chromosome 1 with defined start/end coordinates and 7 exons (each with coordinates).
- Using any programming language (the professor used Bash; Python/R also fine), students must:
  1. Build the **complementary strand** (A↔T, G↔C), knowing it runs 3'→5' if the given strand is 5'→3' [01:12:20].
  2. Identify the **initiation transcription site** (first nucleotide) and **final transcription site** (last nucleotide) [01:16:17].
  3. Construct the **pre-mRNA**: replace T with U, join exons using the coordinates, remove introns, add 5' cap and poly-A tail [01:12:37–01:13:57].
  4. Using the CDS coordinates, cut the mRNA into 5' UTR, CDS, and 3' UTR, then apply the **genetic code** to the CDS to obtain the protein sequence [01:21:58–01:22:55].
- Key clarification from Q&A: the **promoter is made of nucleotides but is not part of the gene** because the gene is the portion that is transcribed [01:13:57–01:14:40].
- Alternative splicing means other exon combinations are possible, so the same gene can yield multiple transcript and protein sequences [01:23:00].

## What the professor stressed
- The **base-pairing rules (A–T, G–C)** are dictated by chemistry (2 vs 3 hydrogen bonds); this governs everything about DNA structure and copying [00:02:48].
- **Replication and transcription always go 5'→3'** — repeated several times for both processes [00:35:22, 00:43:50, 00:48:30].
- The **promoter is not part of the gene** and is not transcribed; it lies immediately upstream [00:41:41, 01:14:09].
- Know where the promoter is for a forward vs reverse gene (left vs right) — she quizzed the class on this directly [00:44:10].
- The flow **DNA → RNA → protein** and the structure of a gene (promoter, exons, introns, CDS, UTRs) is "very important to understand" — explicitly flagged as essential [01:23:30].
- She urged students to **do the practical exercise themselves** before looking at the solutions, to consolidate the concepts [01:20:30].
- Histones are not just structural; they **regulate gene expression** by controlling DNA accessibility [00:12:33].
- The genetic code's **redundancy buffers mutations** [00:59:00].

## Course logistics mentioned
- Class meets every Thursday; next session is the following Thursday [01:24:03].
- Students can email the professor with questions [01:24:03].
- The transcription/translation exercise is available on the course page (with solved version); it is for practice, not submitted in class [01:09:16].

## Self-test
1. Why are A–T and G–C the only base pairings in DNA, and which pair is stronger?
<details><summary>Answer</summary>
G–C forms three hydrogen bonds, A–T forms two. Other pairings (e.g., G–A or T–C) cannot form the correct set of hydrogen bonds, so the chemistry of the bases enforces specificity. G–C is the stronger pair because of the extra hydrogen bond.
</details>

2. A diploid human cell contains about 6 billion base pairs. Using 0.34 nm per base pair, estimate the total length of DNA per cell.
<details><summary>Answer</summary>
6 × 10^9 bp × 0.34 nm/bp ≈ 2.04 × 10^9 nm ≈ 2.04 meters. This matches the ~2 m of DNA per diploid cell stated in class.
</details>

3. How do histones allow 2 m of DNA to fit in a small nucleus, and why does this matter for gene expression?
<details><summary>Answer</summary>
Histones are positively charged and bind the negative phosphate backbone electrostatically, compacting DNA into nucleosomes and higher-order chromatin. This packing is dynamic: to transcribe or replicate, histones must unpack to expose DNA. Thus histone packing/unpacking regulates access to genes, making histones key regulators of gene expression.
</details>

4. A gene is on the reverse strand of a chromosome. In which direction does transcription proceed, and where is its promoter?
<details><summary>Answer</summary>
Transcription always goes 5'→3'. For a reverse-strand gene, this means transcription proceeds from right to left along the chromosome. The promoter is upstream of the gene's 5' end, so for a reverse gene it lies on the right side (immediately before the transcribed region). It is not part of the transcribed gene.
</details>

5. During DNA replication, why must one strand be synthesized in fragments rather than continuously?
<details><summary>Answer</summary>
Replication always proceeds 5'→3'. The two template strands are antiparallel, so one strand (the lagging strand template) must be copied in the direction away from the replication fork, which requires synthesizing short fragments that are later joined. The other strand can be copied continuously 5'→3'.
</details>

6. A mutation changes a codon from UUU to UUC. What is the effect on the protein, and what property of the genetic code explains this?
<details><summary>Answer</summary>
No effect: both UUU and UUC code for phenylalanine. This is due to the redundancy (degeneracy) of the genetic code, which means some mutations do not change the amino acid and the protein remains identical.
</details>

7. Compare bacterial and human transcription/translation in terms of gene arrangement and RNA processing.
<details><summary>Answer</summary>
In bacteria, several related genes can be transcribed together into one polycistronic RNA and translated simultaneously to produce multiple proteins (an operon). In eukaryotes, a single gene produces a pre-mRNA that must be processed (5' cap, poly-A tail, splicing of introns) before it leaves the nucleus and is translated. Humans have introns/exons and alternative splicing; bacteria generally do not.
</details>

8. Explain how one human gene can produce more than one distinct protein.
<details><summary>Answer</summary>
Alternative splicing: different combinations of exons from a single pre-mRNA are included or excluded, producing multiple mature mRNA variants, each of which can be translated into a different protein sequence (e.g., one transcript may skip exon 3, another exon 4).
</details>

9. In an mRNA, what are the 5' UTR, CDS, and 3' UTR, and which parts are translated?
<details><summary>Answer</summary>
The 5' UTR and 3' UTR are untranslated regions at the beginning and end of the mRNA; they contain regulatory information (e.g., binding sites, stability control). Only the central CDS is translated into protein, always starting with an AUG (methionine) codon and ending with a stop codon (UAA, UAG, or UGA).
</details>

10. Why is it misleading to say the human genome has 60,000 protein-coding genes, based on the numbers given in class?
<details><summary>Answer</summary>
The professor gave ~60,000 genomic regions that can be transcribed into RNA and ~20,000 that are translated into proteins. This means most transcribed genes do not code for protein; only ~1.5% of the genome is translated into mRNA/protein, while >90% produces other functional RNAs.
</details>

11. Given a DNA sequence 5'-ATGCA-3', write the complementary strand with its orientation.
<details><summary>Answer</summary>
A→T, T→A, G→C, C→G, A→T, and because the strands are antiparallel, the complement runs 3'→5': 3'-TACGT-5'. (Written left-to-right as 5'-TGCAT-3' it would be the same strand in the opposite orientation.)
</details>

12. A protein translation starts at AUG (methionine) and ends with a stop codon. Why is the stop codon not represented as an amino acid in the protein sequence?
<details><summary>Answer</summary>
Stop codons (UAA, UAG, UGA) do not code for any amino acid; they signal the translational machinery to terminate and release the polypeptide. Therefore they are present in the mRNA/CDS but not in the final protein sequence.
</details>

## Related course materials
- [1.2 - Nucleic Acids slides](../../materials/02_1.2-Nucleic%20Acids.pdf) — DNA and RNA structure covered at the start of the session.
- [1.3 - DNA replication, transcription and translation slides](../../materials/03_1.3-%20DNA%20replication%2C%20transcription%20and%20translation.pdf) — main presentation for the central dogma and related processes.
- [DNA and RNA structure visualization exercise](../../materials/../../materials/) — PyMOL exercise document (course page URL item; see Campus Virtual for the actual link titled "DNA and RNA structure visualization").
- [Exercises on Transcription and Translation](../../materials/../../materials/) — the practical coding exercise used at the end of the session (URL on the course page).
- [Exercises on Transcription and Translation (solved)](../../materials/../../materials/) — solutions walked through at the end of the session.
- [Seq gene file](../../materials/04_Seq_gene.txt) — gene sequence data used for the exercise.

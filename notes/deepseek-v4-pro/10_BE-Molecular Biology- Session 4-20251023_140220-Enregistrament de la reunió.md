# 10_BE-Molecular Biology- Session 4-20251023_140220-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 4 (Thursday, 23 October 2025, 2:02 PM)
- **Video:** [10_BE-Molecular Biology- Session 4-20251023_140220-Enregistrament de la reunió.mp4](../../recordings/10_BE-Molecular%20Biology-%20Session%204-20251023_140220-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%204-20251023_140220-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:23:11 · **Language:** en
- **Transcript:** [10_BE-Molecular Biology- Session 4-20251023_140220-Enregistrament de la reunió.md](../../transcripts/10_BE-Molecular%20Biology-%20Session%204-20251023_140220-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary

This session was largely a hands-on walkthrough of the NCBI Genome and Gene databases. The professor showed how to locate reference genomes, count genes in a species or chromosome, distinguish coding from non-coding genes, download genome/transcript/protein sequences, and interpret a gene page (strand, exons, UTRs, CDS, canonical transcript, isoforms). A major theme was the difference between eukaryotic and prokaryotic genomes, and how to move between the different sequence “levels”: genome → transcript → CDS → protein.

- Use the NCBI Genome database with the **green-tick reference genome** and **RefSeq** records, not older GenBank records.
- On a gene page, the **canonical transcript is not necessarily the first one listed**.
- All transcription goes **5′ to 3′**, so arrow direction on the gene graphic tells you whether the gene is on the plus or minus strand.
- When extracting sequences, the right database matters: **genomic sequence for promoter/introns**, **transcript/CDS for coding sequence**, **protein record for amino acid sequence**.
- Counting **proteins** from a gene list should not be confused with counting isoforms from alternative splicing.

## Key concepts

- **Reference genome / RefSeq status** — A curated, reviewed genome represented by a green tick; use the reference genome (one per species) rather than all deposited versions. RefSeq codes include `NC_`, `NM_`, `NP_`.
- **GenBank vs RefSeq** — GenBank is the older sequence database and may contain partial, unreviewed sequences. RefSeq is curated and validated and is the one to work with.
- **Gene database query fields** — Search syntax such as `GRIN2B[Gene] AND Homo sapiens[Organism]` to find the correct gene entry.
- **Gene structure** — A gene consists of exons (coding/UTR parts kept in mature mRNA) and introns (removed by splicing). Untranslated regions: 5′ UTR and 3′ UTR; coding sequence (CDS) is translated into protein.
- **Alternative splicing** — One gene can give several transcripts by joining different exon combinations. These produce protein **isoforms**, still considered the same protein.
- **Canonical transcript** — The most frequently observed/reference transcript used for mutation reporting and standard experiments.
- **Forward vs reverse gene** — Determined by the sense of transcription relative to the reference chromosome. Transcription is always 5′→3′; an arrow pointing left means the gene is on the complementary strand.
- **Promoter** — Upstream (5′) of the gene; for forward genes it lies to the left, for reverse genes to the right.
- **Orthologs** — Genes in different species derived from a common ancestral gene; similar sequence/structure/function.
- **Prokaryotic vs eukaryotic genomes** — Prokaryotic genomes are circular, compact, mostly coding, no introns or large intergenic regions. Eukaryotic genomes have chromosomes, introns/exons, large intergenic regions, many non-coding genes and pseudogenes.

## Detailed notes

### NCBI Genome database: finding and choosing a reference genome [00:01:59]

- Start at the NCBI website, select the **Genome** database.
- Search for an organism, e.g. `Homo sapiens`.
- The result list contains many deposited genomes. Select the one with the **green tick** (curated/reviewed reference genome).
- In the reference genome page, the files listed at the bottom represent the different molecules:
  - For **Homo sapiens**, there is one file per chromosome.
  - To download the whole genome, you would need all chromosome files.

### Counting genes on human chromosome 7 [00:03:37]

- From the *Homo sapiens* reference genome, use **View annotated genes**.
- Filter by genomic location to chromosome 7.
- Results:
  - **Total genes on chromosome 7: 3,475**
  - **Protein-coding genes on chromosome 7: 1,004**
- Total gene count includes coding genes, non-coding genes, and **pseudogenes**.
- Pseudogenes are genes that have lost their function; they remain in the genome but are not transcribed/functional. Mutations can accumulate and eventually erase the information.

### Alternative splicing and counting proteins [00:06:42]

- In humans, one gene can produce multiple proteins through alternative splicing.
- Different exon combinations generate different transcripts and therefore different **isoforms** of the same protein.
- These isoforms have small variations; some may be less stable or more active, and tissues may express one isoform rather than another.
- Therefore, **1,004 protein-coding genes = 1,004 proteins**, but the number of isoforms would be larger and is not how you count proteins.

### RefSeq vs GenBank [00:07:48]

- Question asked: what is the difference between the chromosome views from GenBank and RefSeq?
- RefSeq (`NC_` codes) is highly curated and annotated.
- GenBank includes older, sometimes partial or unreviewed sequences.
- Transcript sequences from RefSeq begin with `NM_`, and corresponding proteins begin with `NP_`.
- `NM`/`NP` are the curated, validated sequences to use.

### Counting mammalian and rodent genomes [00:10:58]

- To count how many mammals have been sequenced:
  - Search `mammalia` in Genome.
  - Total deposited mammalian genomes: **4,448**.
  - But many species have multiple versions, so filter to **reference genomes**: **880 mammals** sequenced.
- Rodents:
  - Filtering to reference genomes gives **156 rodents**.

### Prokaryotic genome: Staphylococcus aureus [00:13:06]

- Prokaryotic genomes are very different from human:
  - Circular genome, no chromosomes.
  - Coding regions close together; almost no intergenic regions.
  - No intron/exon structure.
  - Very high percentage of genes are protein-coding.
- Human genome has about 60,000 genes, of which roughly 20,000 code for protein; the rest are non-coding RNAs, pseudogenes, etc.
- **Staphylococcus aureus** example:
  - Huge number of deposited genomes, e.g. 118,000 versions, because bacterial genomes are small, fast and cheap to sequence.
  - Reference genome size: **2,821,361 nucleotides**.
  - Total genes: **2,872**.
  - Protein-coding genes: **2,767**.
  - In the annotated view, genes are adjacent on plus and minus strands.
- To download the complete bacterial genome, open the reference record and use **FASTA**.

### Escherichia coli exercise [00:22:48]

- Search `Escherichia coli K12`, select the reference genome.
- Genome size: **4,641,000 nucleotides**.
- Total genes: **4,651**.
- Protein-coding genes: **4,290**.
- Again, almost all genes are protein-coding, unlike the human genome.

### NCBI Gene database: searching for a gene [00:26:16]

- The Gene database has one entry per gene per organism.
- You must specify both the gene name and organism, for example:
  - `GRIN2B[Gene] AND Homo sapiens[Organism]`.
- The gene page gives a curated summary: protein-coding status, RefSeq status, organism, orthologs, genomic location, exon count, and coordinates.

### GRIN2B gene example [00:28:53]

- GRIN2B is a protein-coding gene.
- **Location**: chromosome 12, p arm.
- **Exons**: 15.
- **Coordinates**: on the chromosome 12 sequence `NC_000012`, between two defined coordinate positions.
- GRIN2B is a **reverse gene**, meaning it sits on the complementary strand.

### Reading gene orientation from arrows [00:32:15]

- The gene graphic shows neighbouring genes and an arrow indicating transcription direction.
- Transcription is **always from 5′ to 3′**.
- Arrow pointing **right** = forward gene on the plus strand.
- Arrow pointing **left** = reverse gene on the complementary strand.
- For a reverse gene:
  - The 5′ end of the gene is on the **right**.
  - The promoter is **upstream of the gene**, so it is on the **right**.
- For a forward gene:
  - Promoter is on the **left**.

### Transcripts and alternative splicing [00:34:23]

- Below the gene graphic, the page shows several transcript variants.
- For GRIN2B, the professor identified **five transcript variants** produced by alternative splicing.
- Vertical green boxes = exons; intronic sequence is removed in the mRNA.
- Pale green = non-coding regions (UTRs); dark green = coding regions.
- The **canonical transcript** is the most frequent, reference transcript shown at the top of the graphic.
- The transcript contains:
  - **5′ UTR** at the start.
  - **CDS** in the middle.
  - **3′ UTR** at the end.

### Transcript and protein sequence records [00:42:32]

- Scroll down to the **NCBI Reference Sequence (RefSeq)** table.
- `NM_` codes = transcript/mRNA sequences.
- `NP_` codes = protein sequences.
- Example from the GRIN2B canonical transcript:
  - Transcript length: **30,609 nucleotides**.
  - CDS coordinates: **709–5163**.
  - Therefore:
    - 5′ UTR = positions **1–708**
    - 3′ UTR = positions **5164–end**
  - The CDS is translated into the corresponding protein.
- RNA normally contains U, but in these FASTA files sequences are written with **T instead of U** by convention, to allow direct alignment with DNA.

### Extracting specific sequence regions [00:46:00]

- Inside a transcript record, you can see exon coordinates:
  - Example GRIN2B exon 1: nucleotides **1–261**
  - Exon 2: **262–690**
- You can use **Change region shown** / **update view** to display any part:
  - CDS only
  - One exon
  - 5′ UTR
- For **promoter region or introns**, you must use the genomic sequence (`NC_`), not the transcript.
- For **CDS/exons**, use the transcript (`NM_`).
- For **protein sequence**, use the protein record (`NP_`).

### Reverse gene sequence and reverse complement [00:50:41]

- The GRIN2B genomic span in this example is **444,798 bp**.
- When viewing the genomic sequence of a **reverse gene**, using the plus-strand coordinates alone will give the wrong strand.
- Use the option **“show reverse complement”** to obtain the gene sequence in the correct 5′→3′ orientation.

### RXFP2 exercise [00:54:18]

- Search for `RXFP2` in the Gene database.
- RXFP2 is:
  - A **forward** gene (arrow to the right).
  - Located on chromosome 13.
  - Contains **18 exons**.
  - Has three transcript variants.
- Of the three transcripts, only some are curated:
  - Two are `NM_` curated transcripts.
  - One is `XM_`, meaning computationally predicted, not experimentally validated.
- The **canonical transcript is not the first one listed** in the table; in this case it was the second one.
- Canonical RXFP2 transcript example:
  - Transcript length: **3,336 nucleotides**.
  - CDS: positions **88–2352**.
  - Therefore:
    - 5′ UTR = **1–87**
    - 3′ UTR = **2353–3336**

### Extracting promoter and gene segments [01:07:45]

- To extract a promoter region of, e.g., **1,000 nucleotides upstream of the gene**:
  1. Open the genomic sequence (`NC_`).
  2. Determine the first nucleotide of the gene.
  3. Use coordinates from `start − 1000` to `start − 1`.
- Example used in class for a forward gene:
  - If the first nucleotide of the gene is **31,739,526**, the 1,000 bp promoter region is **31,738,526–31,739,525**.
- To extract the **first 500 nucleotides of the gene**:
  - For a forward gene, use `start` to `start + 499`.
- The professor stressed that we do not know exactly how long the promoter is; practical extractions often use 3,000 or 5,000 bp upstream depending on the study.

### Ortholog exercise: LDHC vs DLD [01:15:14]

- Two genes were given for homework:
  - **LDHC** in *Homo sapiens*.
  - **DLD** in *Escherichia coli*.
- They are described as orthologous: derived from a common ancestral gene, similar in sequence/structure/function despite being in very different species.
- Use two browser windows to compare:
  - Genomic sequence structure.
  - Transcript length.
  - Protein length.
  - Number of transcript variants.
  - Coordinates in the genome.
- Use the **zoom tool** to compare the landscape:
  - In *Homo sapiens*, large intergenic regions with no genes.
  - In *E. coli*, genes packed one after another.

## What the professor stressed

- **Use the green-tick reference genome** and RefSeq curated records (`NC`, `NM`, `NP`).
- **Check that you have the canonical transcript**; it is not always first in the RefSeq table.
- **Transcription is always 5′→3′**; never 3′→5′. Arrow direction tells you the strand.
- **Choose the right sequence level**:
  - Genomic sequence → promoter, introns, full gene region.
  - Transcript sequence → exons, CDS, UTRs.
  - Protein sequence → amino acid sequence.
- **Draw the gene model on paper** to understand coordinates, strand, transcription and translation.
- **Do the database exercises carefully**, especially the LDHC/DLD comparison, because they consolidate genome → transcript → protein concepts.
- Next week there is no class; the session continues in two weeks.

## Course logistics mentioned

- The previous week’s recording was recovered and posted as “Molecular Biology session 3.”
- The genome/gene database exercises are for homework; complete them carefully.
- Exercise comparing LDHC and DLD should be done using two browser windows and drawings.
- No class the following week; next class in two weeks.
- Questions can be sent to the professor by email.

## Self-test

1. In the NCBI Genome database, how would you find the number of protein-coding genes on human chromosome 7? What numbers did the professor report?  
<details><summary>Answer</summary>
Select Genome, search Homo sapiens, choose the green-tick reference genome, use View annotated genes, filter to chromosome 7, then filter to protein-coding. The professor reported 3,475 total genes and 1,004 protein-coding genes on chromosome 7.
</details>

2. Why should you not count protein isoforms when asked how many proteins are encoded by a chromosome?  
<details><summary>Answer</summary>
Alternative splicing can produce several isoforms from one gene, but these are variants of the same protein. The number of proteins corresponds to the number of protein-coding genes (in the simple class example, 1,004 proteins for chromosome 7), not the number of isoforms.
</details>

3. What is the difference between an `NM_` transcript and an `XM_` transcript in RefSeq?  
<details><summary>Answer</summary>
`NM_` transcripts are curated, validated reference transcripts. `XM_` transcripts are computationally predicted and lack experimental validation; they may later be upgraded to `NM_`.
</details>

4. A gene is shown with an arrow pointing to the left. Which DNA strand is it on, and where is its promoter?  
<details><summary>Answer</summary>
It is on the complementary (reverse) strand because transcription is always 5′→3′. Therefore the promoter is on the right, which is upstream (5′) for that gene.
</details>

5. For the GRIN2B canonical transcript, the CDS is positions 709–5163. What are the 5′ UTR and 3′ UTR positions?  
<details><summary>Answer</summary>
5′ UTR = positions 1–708. 3′ UTR = positions 5164 to the end of the transcript.
</details>

6. Which NCBI sequence record should you use to extract a promoter region: `NC_` genomic or `NM_` transcript? Why?  
<details><summary>Answer</summary>
Use the `NC_` genomic sequence, because the promoter is upstream of the transcribed region and is not included in the `NM_` transcript.
</details>

7. Which record should you use to download the coding sequence (CDS) of a gene?  
<details><summary>Answer</summary>
Use the `NM_` transcript record and select the CDS coordinates, because the CDS is the joined coding portion of the mature transcript after intron removal.
</details>

8. Why do FASTA files of RNA sequences show T instead of U?  
<details><summary>Answer</summary>
By convention, nucleotide sequences are written with T so they can be easily aligned to DNA sequences. RNA-specific differences are not shown in these files.
</details>

9. Why does a bacterial genome such as *Staphylococcus aureus* have a much higher percentage of protein-coding genes than the human genome?  
<details><summary>Answer</summary>
Bacterial genomes are compact, circular, mostly coding, with no introns and little intergenic DNA. Human genomes have large intergenic regions, introns, many non-coding genes and pseudogenes.
</details>

10. Is the canonical transcript always the first row in the RefSeq transcript table?  
<details><summary>Answer</summary>
No. The professor stressed that the canonical transcript can be listed second or later. In the RXFP2 example, the canonical transcript was the second one; always check the gene graphic/table rather than assuming the first row.
</details>

11. How would you extract the first 500 nucleotides of a forward gene?  
<details><summary>Answer</summary>
Open the genomic `NC_` sequence, identify the first nucleotide of the gene, and select coordinates from the start position to start + 499.
</details>

12. What features would you compare between orthologous genes from human and *E. coli* to see how genome organisation differs?  
<details><summary>Answer</summary>
Compare transcript length, protein length, number of transcript variants, genomic coordinates, surrounding gene density, and intron/exon structure. In humans you see large intergenic regions; in *E. coli* genes are packed one after another.
</details>

## Related course materials

- [1.4- Sequencing of the human genome](../../materials/05_1.4-%20Sequencing%20of%20the%20human%20genome.pdf)
- [1.5-The Human Genome](../../materials/06_1.5-The%20Human%20Genome.pdf)

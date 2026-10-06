# 15_BE-Molecular Biology- Session 7-20251120_140244-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 7 (Thursday, 20 November 2025, 2:02 PM)
- **Video:** [15_BE-Molecular Biology- Session 7-20251120_140244-Enregistrament de la reunió.mp4](../../recordings/15_BE-Molecular%20Biology-%20Session%207-20251120_140244-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%207-20251120_140244-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:20:48 · **Language:** en
- **Transcript:** [15_BE-Molecular Biology- Session 7-20251120_140244-Enregistrament de la reunió.md](../../transcripts/15_BE-Molecular%20Biology-%20Session%207-20251120_140244-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary
This final session before the partial exam focused on practical work with the UCSC Genome Browser. The professor showed how to look up a specific gene (NR4A2) and display its transcript structure, strand, UTRs, CDS, conservation and population variation. The session then covered the Table Browser, a tool for bulk-downloading genome annotations such as transcript sequences, promoter regions, CDS coordinates, repeats and SNPs for whole chromosomes or the whole genome. The professor also explained the exam format, recommended study strategies, and gave guidance on Task 2.

- Next week’s partial exam covers all Unit 1 topics **except human genetic variation**; it combines short theoretical questions with practical database exercises.
- The exam is open-book for slides and databases, but artificial intelligence is not allowed; camera must be on and microphone off.
- UCSC Genome Browser is often faster than NCBI for extracting promoter, transcript, gene and protein sequences.
- In a gene track, thick exon blocks are CDS, thin blocks are UTRs; arrows pointing left mean a reverse gene.
- The Table Browser can download sequence or annotation tables for any track, for one position, a chromosome, or the whole genome.

## Key concepts
- **Reverse vs forward gene** [00:13:34]: Transcription is always 5′→3′. If the UCSC arrows point left, the gene is transcribed from the complementary strand and is called a reverse gene; a minus strand in the coordinates confirms this.
- **Curated vs predicted RefSeq transcripts** [00:09:11]: NM (mRNA) and NP (protein) accessions are curated/reviewed; XM and XP accessions are computationally predicted and should not be fully relied on.
- **CDS and UTRs** [00:15:23]: CDS = coding sequence, shown as thicker blocks; UTRs are thinner non-coding blocks at the 5′ and 3′ ends of the transcript.
- **Promoter region** [00:19:44]: Sequence upstream of the gene, often the ~2,000 nucleotides before the transcription start, involved in regulating expression.
- **Conservation track** [00:29:29]: Alignment of the human region with orthologous sequences from other species; exons are more conserved than introns, and coding regions more than non-coding exons.
- **Common SNPs** [00:31:45]: Single-nucleotide variants common in healthy populations; not individually disease-causing, but combinations may contribute to complex disease.
- **Table Browser** [00:34:07]: UCSC tool that downloads sequence or annotation tables from any displayed track, for the whole genome, a chromosome, or a specific region.
- **Segmental duplications / retrotransposons / simple repeats** [01:04:55]: Different repeat classes available as separate UCSC tracks under the Repeats group.

## Detailed notes

### Exam format and scope
- The next session is the partial exam covering the first unit, the human genome [00:00:00].
- Included topics: introduction, duplication, repair, transcription, translation, human genome sequencing, the human genome and UCSC Genome Browser [00:01:00].
- Excluded: human genetic variation will not be in this exam; it will be covered in a later partial exam together with the human proteome and regulation of gene expression [00:01:00, 01:14:10].
- Exam format: short questions requiring short answers, **not multiple-choice** [00:02:01, 00:03:26].
- There will be theoretical questions and practical exercises using NCBI Gene, NCBI Genome/Genome Data Viewer and the UCSC Genome Browser [00:02:01].
- Slides and class materials may be used; AI is not allowed; camera must be on and microphone off, otherwise the exam is invalidated [00:02:01, 01:15:06].
- Estimated duration: about 1 hour to 1 hour 15 minutes [00:02:01].
- Study recommendation: understand the theoretical slides and repeat all exercises done in class [01:13:09].
- If something is unclear, students can email the professor or ask for a tutoring session [01:15:06].

### Locating a gene and displaying its structure in UCSC
- Work flow: go to UCSC Genome Browser → Genome Browser; type the gene name, e.g. NR4A2, and select it [00:11:23].
- Hide all tracks, then in **Genes and Gene Predictions** display the **NCBI RefSeq** track in full or compact mode and refresh [00:12:33].
- The displayed region contains the genomic coordinates of the gene; these are the same coordinates found in the NCBI RefSeq genomic record [00:13:34].
- The track shows two curated transcripts with NM accessions. The arrows point left, meaning transcription goes to the left; since transcription is always 5′→3′, this is a **reverse gene** on the minus strand [00:13:34, 00:14:23].
- Reading the exon blocks for a reverse gene:
  - The leftmost block is the last exon (e.g. exon 8 of 8 for NR4A2) and contains the **3′ UTR** [00:15:23].
  - The rightmost exons contain the **5′ UTR** [00:15:23].
  - Thick parts of exon blocks are CDS; thin parts are UTR.
- Clicking on a transcript accession, e.g. NM_006186.4, opens its transcript page [00:16:29]:
  - **Transcript size** = exons only, no introns; in the example NR4A2 transcript size was 3,472 nt [00:17:32].
  - **Strand** is shown as minus for reverse genes [00:17:32].
  - Coordinates of the first and last nucleotide of the transcript [00:17:32].
  - Further down: **gene position** and gene size, including introns and exons [00:17:32].
- From the transcript page, links allow jumping to:
  - **Predicted protein** → FASTA protein sequence of that isoform [00:18:32].
  - **Predicted messenger RNA** → exons joined, no introns [00:18:32].
  - **Genomic sequence** → gene sequence including exons and introns [00:18:32].

### Extracting specific sequences for one gene
- The genomic sequence page lets you choose what to display [00:18:32]:
  - **Promoter region**: e.g. 2,000 nucleotides upstream of the gene, something difficult to extract from NCBI manually [00:19:44].
  - **5′ UTR exons, CDS exons, 3′ UTR exons**: together equal the transcript sequence [00:19:44].
  - **Exons plus introns**: the full gene sequence [00:19:44].
- Format options include exons in uppercase and introns in lowercase, or only CDS in uppercase [00:20:49].
- Rule of thumb for where to go [00:27:22]:
  - Only exons / transcript → **messenger RNA**.
  - Protein → **predicted protein**.
  - Regions outside exons, intronic sequence, or promoter → **genomic sequence**.

### Conservation and SNPs for a gene
- Conservation is displayed from the **Comparative Genomics** section, using the **100 vertebrates** track [00:24:50, 00:29:29].
- Select species for the multiple-sequence alignment, then submit; the track shows conservation across the gene window [00:29:29].
- Observed pattern: exonic regions show high conservation, intronic regions show low conservation [00:30:38].
- Explanation: exons are more functionally important; mutations in coding regions are more likely to disrupt protein structure/function. Coding regions are more conserved than non-coding exons, and non-coding exons are more conserved than introns [00:30:38].
- To display SNPs, go to **Variation** and select **dbSNP**; use pack and refresh [00:31:45].
- These are **common SNPs**: variants present in healthy populations, not directly disease-causing. Several SNPs combined, together with environmental factors, can increase disease predisposition [00:31:45].
- In the SNP track, be careful to check that all variant classes are selected if you want everything [00:31:45].

### Table Browser: bulk data download
- Entry: UCSC main menu → **Tools** → **Table Browser** [00:34:07].
- The first settings choose the data source, equivalent to selecting a UCSC browser track:
  - **Genes and Gene Predictions** → e.g. NCBI RefSeq [00:35:11].
  - **Repeats** → Simple Repeats, Segmental Duplications, RepeatMasker [00:59:19].
  - **Variation** → dbSNP [01:09:23].
  - **Comparative Genomics** → conservation tracks [00:24:50].
- For the NCBI RefSeq track you can choose:
  - All transcripts, **curated only** (NM-coded transcripts), or predicted-only transcripts [00:36:14].
- Position options: whole genome, a chromosome, or a specific region [00:37:17].
- Output format can be **sequence** or **selected fields from primary and related tables** [00:37:17, 00:44:32].

#### Bulk sequence downloads
- To download all curated transcript sequences for the whole genome [00:38:17]:
  - Group: Genes and Gene Predictions; track: NCBI RefSeq; select curated only.
  - Position: genome.
  - Output format: sequence.
  - In sequence options, select 5′ UTR, CDS and 3′ UTR exons and **uncheck introns**; this gives transcripts, not genes.
  - To get gene sequences instead, include introns [00:39:33].
- To download all promoter regions for curated genes [00:40:35]:
  - Same settings as above, but in sequence options select only **promoter region**, e.g. 2,000 nucleotides upstream, and uncheck other boxes.
- To download CDS sequences for chromosome 7 [00:54:18]:
  - Position = chr7; sequence output; select only CDS.

#### Bulk annotation tables
- Instead of sequence output, choose **selected fields from primary and related tables** [00:44:32].
- Example: for all curated transcripts in the genome, select the transcript name, chromosome, strand, CDS start, CDS end, exon count and gene name (name2) [00:45:33].
- This produces a table that can be written to a file and then processed with Python, R, or basic Linux commands [00:57:11].
- Example: to get CDS coordinates for all RefSeq genes on chromosome 7 [00:51:57]:
  - Select all RefSeq genes, position chr7.
  - Output format: selected fields.
  - Choose CDS start, CDS end, transcript name.
  - The coordinates are genomic coordinates on chromosome 7, not transcript coordinates [00:54:18].
- Example: all genes in the genome with transcript name, gene name, strand and exon count [00:55:50].
  - The strand column lets you count forward vs reverse genes later [00:57:11].

#### Repeats and variation bulk downloads
- **Simple repeats** [00:59:19]:
  - Group: Repeats; track: Simple Repeats.
  - Fields: chromosome, start, end, repeat name, number of copies, length.
- **Segmental duplications** [01:04:55]:
  - Group: Repeats; track: Segmental Duplications.
  - Fields: chromosome, start, end of the duplication, strand, and the other chromosome/coordinates where the duplicated copy is found.
  - These are very large duplicated regions that can contain several genes [01:06:32].
- **Retrotransposons / jumping genes** [01:07:37]:
  - Group: Repeats; track: RepeatMasker.
  - Fields: position in the chromosome, repeat name, aligned positions elsewhere in the genome, and strand.
  - This shows that a retrotransposon sequence has “jumped” to another genomic region and that the two sequences can be aligned [01:09:23].
- **dbSNP for chromosome 1** [01:09:23]:
  - Group: Variation; track: dbSNP 155, common SNPs.
  - Position: chr1; selected fields.
  - Fields: chromosome, position, SNP name, reference nucleotide, alternate nucleotide, and variation class [01:10:42].

### Task 2 guidance
- Task 2, on the human genome, is due the following week; doing it is recommended before the exam [01:12:01].
- Students can use NCBI and cross-check with UCSC Genome Browser [01:12:01].
- If asked for the first 20 nucleotides of the **gene**, use the **NC accession** (genomic RefSeq), not the NM transcript accession, because the question concerns the gene sequence [01:16:09].
- For reverse genes, manual coordinate extraction can be confusing; the UCSC Genome Browser can extract a 100-nucleotide promoter region directly, avoiding manual coordinate arithmetic [01:16:09].
- If using NCBI for a reverse gene promoter, take the highest coordinate of the gene and add 1–99 nucleotides downstream, but the professor recommended validating with UCSC [01:16:09].
- Tasks about exon positions or transcript sequences should be based on the gene sequence (NC) and the exon positions annotated within it; a small script can cut the exonic regions from the gene sequence if needed [01:20:12].

## What the professor stressed
- The exam will mix theory with practical database exercises; simply memorizing slides is not enough, students must be able to operate NCBI and UCSC [00:02:01, 01:13:09].
- Always remember: NM/NP = curated; XM/XP = predicted and less reliable [00:09:11].
- Transcription is always 5′→3′; use this to decide whether a gene is forward or reverse [00:14:23, 00:22:45].
- Exons are more conserved than introns; coding sequence is more conserved than non-coding exons [00:30:38].
- UCSC is quicker and easier than NCBI for extracting promoter, gene, transcript and protein sequences [00:06:15, 00:19:44].
- The Table Browser is “very powerful” and useful for downloading any type of annotation for the whole genome [00:07:17, 00:34:07].
- Camera on and microphone off are mandatory for the exam; failing to have the camera on invalidates the exam [00:02:01, 01:15:06].
- Complete Task 2 and repeat all exercises before the exam [00:12:01, 01:13:09].

## Course logistics mentioned
- **Partial exam**: next week; covers all Unit 1 topics except human genetic variation; short-answer only; allowed materials are slides, notes and databases; AI is not allowed; camera on, microphone off [00:00:00–00:03:26, 01:14:10].
- **Task 2**: due Wednesday after the session (26 November 2025); instructions in a Google Doc linked on the course page; uses NCBI and/or UCSC [01:12:01].
- **Later partial exam**: will include human genetic variation, the human proteome and regulation of gene expression [01:14:10].
- **Support**: professor available by email or tutoring session for questions on the concepts [01:15:06].

## Self-test
1. In a UCSC gene track, the arrows point left. Is the gene forward or reverse, and how do you know?  
<details><summary>Answer</summary> It is a reverse gene. Transcription is always 5′→3′, so if the direction of transcription points left, the gene must be transcribed from the complementary strand, which UCSC shows as the minus strand.</details>

2. For the reverse gene NR4A2, which end of the displayed gene contains the 5′ UTR and which contains the 3′ UTR?  
<details><summary>Answer</summary> In the UCSC display, the rightmost exons contain the 5′ UTR and the leftmost exon contains the 3′ UTR, because transcription runs from right to left for a reverse gene.</details>

3. What is the practical difference between NM/NP accessions and XM/XP accessions?  
<details><summary>Answer</summary> NM (transcript) and NP (protein) accessions are curated/reviewed in RefSeq and can be trusted. XM and XP accessions are computationally predicted and not yet curated, so they are less reliable.</details>

4. In UCSC’s 100-vertebrate conservation track, where would you expect the highest conservation in a gene, and why?  
<details><summary>Answer</summary> The highest conservation is in exons, especially coding regions, because mutations there are more likely to disrupt protein structure and function. Introns and intergenic regions are less conserved.</details>

5. You want to download the transcript sequence of one specific gene from UCSC. Which link should you use: predicted mRNA, predicted protein, or genomic sequence?  
<details><summary>Answer</summary> Predicted mRNA, because it gives the exons joined together without introns, which is the transcript sequence.</details>

6. In the Table Browser, how would you download all curated RefSeq transcript sequences for the whole human genome?  
<details><summary>Answer</summary> Go to Tools → Table Browser; choose group Genes and Gene Predictions, track NCBI RefSeq, curated-only transcripts; set position to genome; set output format to sequence; then select 5′ UTR, CDS and 3′ UTR exons and uncheck introns before getting the sequence.</details>

7. If a task asks for 2,000 nucleotides upstream of every curated RefSeq gene, which UCSC sequence option should you select in the Table Browser?  
<details><summary>Answer</summary> Use the gene/gene-predictions NCBI RefSeq curated track, position genome, output format sequence, then select only the promoter region and set the number of nucleotides to 2,000, unchecking the exon/intron options.</details>

8. You need a table with CDS start, CDS end and transcript name for all RefSeq genes on chromosome 7. Which output format and fields should you choose?  
<details><summary>Answer</summary> Use NCBI RefSeq all genes, position chr7, output format “selected fields from primary and related tables”. Then select CDS start, CDS end, and transcript name; the coordinates will be genomic coordinates on chromosome 7.</details>

9. What is the difference between the Simple Repeats, Segmental Duplications and RepeatMasker tracks in the context of the UCSC Repeats group?  
<details><summary>Answer</summary> Simple Repeats are tandem repeats; Segmental Duplications are large duplicated genomic regions that may contain genes; RepeatMasker can be used to display retrotransposons/jumping elements and where their sequences align elsewhere in the genome.</details>

10. A student is asked for the first 20 nucleotides of a gene. Should they use the NC or NM accession, and why?  
<details><summary>Answer</summary> The NC accession, because it represents the genomic sequence of the gene, including introns and flanking regions. NM is the mRNA/transcript sequence, which lacks introns and is not the full gene sequence.</details>

11. Why are common dbSNP variants not considered directly disease-causing, even though they may be relevant to disease?  
<details><summary>Answer</summary> They are present in healthy populations and individually do not cause disease. However, combinations of several common SNPs, together with environmental factors, can increase predisposition to complex diseases.</details>

12. How can you quickly extract a 100-nucleotide promoter region for a reverse gene without manually calculating coordinates?  
<details><summary>Answer</summary> Use the UCSC Genome Browser genomic sequence page for the gene, select promoter region, set 100 nucleotides upstream, and download the sequence. This avoids having to work out forward/reverse coordinate arithmetic manually.</details>

## Related course materials
- [1.5-The Human Genome](../../materials/06_1.5-The%20Human%20Genome.pdf)
- [UCSC Genome Browser Exercises](https://campusvirtual.urv.cat/mod/url/view.php?id=4185472)
- [Exercises on Genome and Gene visualization](https://campusvirtual.urv.cat/mod/url/view.php?id=4185469)
- [Exercises on Genome and Gene visualization (solved)](https://campusvirtual.urv.cat/mod/url/view.php?id=4185470)

# 21_BE-Molecular Biology- Session 11-20251218_140227-Enregistrament de la reunió

- **Subject:** 2025-2026 BIOMEDICINE FOR ENGINEERS (17715202)
- **Recording:** BE-Molecular Biology- Session 11 (Thursday, 18 December 2025, 2:02 PM)
- **Video:** [21_BE-Molecular Biology- Session 11-20251218_140227-Enregistrament de la reunió.mp4](../../recordings/21_BE-Molecular%20Biology-%20Session%2011-20251218_140227-Enregistrament%20de%20la%20reunió.mp4) · [online](https://rovira.sharepoint.com/sites/A_2025-26_108771/_layouts/15/stream.aspx?id=/sites/A_2025-26_108771/Documentos%20compartidos/General/Recordings/BE-Molecular%20Biology-%20Session%2011-20251218_140227-Enregistrament%20de%20la%20reuni%C3%B3.mp4)
- **Duration:** 01:22:46 · **Language:** en
- **Transcript:** [21_BE-Molecular Biology- Session 11-20251218_140227-Enregistrament de la reunió.md](../../transcripts/21_BE-Molecular%20Biology-%20Session%2011-20251218_140227-Enregistrament%20de%20la%20reuni%C3%B3.md)
- **Notes by:** DeepSeek `deepseek-v4-pro` (effort: high) on 2026-10-05 — check against the slides

## Summary

This session finished the human proteome block. It consolidated the relationship between protein sequence, structure, and function, then explained how homologous proteins arise through gene duplication and speciation, distinguishing orthologues from paralogues. The professor demonstrated the sequence–structure correlation with sequence alignments and introduced the thresholds used to infer homology (70% nucleotide identity for genes; >25% amino acid identity for proteins), while warning that real homologues can exist below these thresholds if structural evidence is available. The class then moved to PyMOL visualisation of representative proteins (hemoglobin, antibodies, histones, sirtuins, lac repressor, a membrane channel) to show how structure determines function. Finally, the professor introduced UniProt as the reference protein database and walked through searching with advanced queries, reading a UniProt entry, and answering biological questions such as how many human proteins are reviewed, involved in synapse, or have experimental 3D structures.

Key takeaways:

- A protein’s sequence determines its structure, and structure determines function; therefore, sequence similarity lets us infer structure and function computationally.
- Homologous proteins arise by gene duplication (paralogues) or speciation (orthologues); sequence identity thresholds are used to propose homology.
- Conserved positions in multiple sequence alignments highlight residues that were not tolerated to mutate because they are essential for structure/function.
- UniProt Swiss-Prot is the curated, low-redundancy reference protein database; use gene name + organism for efficient searching.
- Experimental structures (X-ray, electron microscopy) should be preferred over AlphaFold computational models when available.
- The reviewed human proteome contains 20,420 proteins, but experimental 3D structures exist for only 8,605 of them.

## Key concepts

- **Primary structure**: the linear amino acid sequence of a protein [00:00:40].
- **Secondary structure**: local interactions of residues to satisfy hydrogen-bond potential, mainly alpha helices and beta sheets [00:00:40].
- **Tertiary structure / domain**: a folded, packed region of a protein that can perform a specific function [00:00:40, 00:29:51].
- **Quaternary structure**: a protein made of several polypeptide chains/subunits [00:23:59].
- **Homologous proteins/genes**: two genes or proteins that descend from the same ancestral gene/protein [00:05:38].
- **Orthologous proteins/genes**: homologues created by a speciation event; they belong to different organisms [00:07:02].
- **Paralogous proteins/genes**: homologues created by a gene duplication event; they belong to the same genome [00:07:02].
- **Sequence identity**: the percentage of nucleotides or amino acids that are identical between two aligned sequences [00:09:12].
- **Gene Ontology (GO)**: a controlled vocabulary of keywords describing molecular function and biological process of a protein [00:45:36].
- **Swiss-Prot / reviewed proteins**: UniProt entries manually curated from the literature; low redundancy [00:43:24].
- **TrEMBL / unreviewed proteins**: computationally predicted proteins that are not yet curated; can include redundancy [00:43:24].
- **AlphaFold**: a computational method for predicting protein structure; should be used with caution when no experimental structure exists [00:53:15].

## Detailed notes

### Protein structure recap: sequence → structure → function

The professor reviewed the hierarchy of protein structure [00:00:40]:

- Primary structure: the sequence of amino acids, the building blocks of proteins.
- Secondary structure: residues interacting locally to satisfy hydrogen bond potential.
- Tertiary structure: the folded domain that forms a functional part of a protein.
- Quaternary structure: a protein composed of several folded subunits.

A protein can contain several domains, and a functional protein may need to interact physically with other proteins. The professor referred to this network of interactions as the **interactome**: some interactions are permanent, while others are transient and switch processes on or off [00:00:40].

### Protein evolution and domain mixing

The professor presented evolution using a Lego analogy [00:03:31]:

- An ancestral protein undergoes **gene duplication**, producing two identical proteins.
- Over evolution, each copy accumulates mutations, so they remain similar but not identical.
- They will generally have similar sequence, similar structure, and similar function.
- Domains can be combined and recombined, like Lego blocks, generating diverse protein structures and functions.

### Homology, orthology, and paralogy

Homologous proteins/genes are those that descend from the same ancestral protein/gene [00:05:38]. Two biological events generate homologues [00:07:02]:

- **Gene duplication**: creates paralogues, which are in the same genome.
- **Speciation**: creates orthologues, which are in different organisms.

Examples given [00:08:08]:

- Horse hemoglobin alpha and human hemoglobin alpha are **orthologues**.
- Human hemoglobin alpha and human hemoglobin beta are **paralogues**.

The professor stressed that we can hypothesize homology because very similar sequences are extremely unlikely to arise by chance de novo [00:09:12, 00:19:13].

### Sequence identity thresholds and the limits of the rule

The standard guideline proposed in class [00:09:12]:

- For **genes/RNA**: at least 70% nucleotide identity to propose homology.
- For **proteins**: more than 25% amino acid identity to propose homology.

However, the professor answered a question about low identity explicitly [00:15:15, 00:18:12]:

- If identity is below 25%, you **cannot be sure** two proteins are homologous based purely on sequence.
- There are many real cases with only 13–15% sequence identity whose structures are almost identical and whose functions are similar.
- Below 25%, you need additional evidence, especially structural superposition, to propose homology.
- When doing standard database searches, 25% is the practical minimum accepted to suggest homology.

### Sequence identity correlates with structural similarity

The professor showed pairwise alignments of 9-PAP with 2-ACT and other proteins [00:10:29]:

- High sequence identity → superimposed structures almost identical.
- Lower sequence identity → structures begin to show differences.
- Very low sequence identity (<15%) → some regions differ, but most of the fold can still be quite similar.

The conclusion [00:14:11, 00:19:13]:

- Sequence is completely correlated with structure.
- Therefore, if two proteins have similar sequences, they likely have similar structures.
- Since structure determines function, similar sequences likely perform similar functions.
- This is the basis of computational structure/function prediction without experimental work.

### Multiple sequence alignments and conserved positions

A multiple sequence alignment of a homologous protein family shows positions kept exactly the same during evolution [00:14:11]. The professor’s interpretation:

- All positions have mutated at some point over thousands of years.
- But mutations in **super-conserved positions** were not tolerated: individuals carrying them did not survive, so those mutations never became fixed.
- Conserved positions are therefore essential for maintaining protein structure and function.
- This allows scientists to identify which residues are essential and which regions can be modified while preserving function.

### PyMOL tour: structure and function examples

The professor used PyMOL to visualise representative proteins [00:22:50].

#### Hemoglobin: a transporter

- Hemoglobin is composed of **four proteins/subunits**, each with one domain [00:23:59].
- It is mainly alpha-helical, with loops connecting helices [00:25:55].
- Each subunit contains a **heme group** in its core, which binds oxygen.
- Oxygen binding/release is modulated by changes in affinity, allowing oxygen transport.
- The red dots in the structure are water molecules; the chemical groups are not proteins but help the protein perform its function [00:23:59, 00:27:08].

#### Antibody: multi-domain and multi-chain protein

- An antibody is made of several polypeptide chains [00:28:14].
- The blue chain alone contains **four domains**, which appear as separate packed structures [00:29:51].
- The domains are similar, suggesting they arose by gene duplication.
- Each domain can perform a specific function, such as binding the partner chain or binding other proteins.
- Overall antibody function emerges from combining domain functions across chains.

#### Histones: small single-domain DNA-packaging proteins

- Histones are short proteins that wrap DNA [00:31:38].
- Each histone is a short sequence folded into a single domain.
- Histones are similar in sequence, structure, and function, but small differences are important for the overall nucleosome fold.

#### Sirtuin: an enzyme with a catalytic cavity

- Sirtuins are enzymes that speed up reactions by modifying other proteins through post-translational modifications [00:33:56].
- The protein contains an **NAD** chemical group used to perform a chemical reaction on another protein.
- The surface representation shows a specific shape with a hole; the substrate residue fits into this cavity.
- Without this shape and catalytic activity, the reaction would be too slow.

#### Lac repressor: a gene regulator

- The lac repressor binds DNA to stop transcription of a gene [00:36:00].
- The structure shows DNA at the bottom and the protein composed of several copies/subunits.
- The green and blue chains each have two domains: a small DNA-binding domain and a large protein-interaction domain.
- The small domains bind DNA; the large domains interact between proteins.

#### Membrane channel: beta-sheet structure

- A channel protein is built from **beta sheets**, not alpha helices [00:37:58].
- The beta-sheet fold creates channels that span the membrane and allow passage of molecules.
- This illustrates that structure is completely related to function.

The professor’s closing point: whenever you see a protein name, imagine a three-dimensional fold that determines its function; many proteins need other proteins, and most are composed of more than one domain [00:39:15].

### UniProt: the main protein database

UniProt is the reference database for proteins [00:40:17]. The professor contrasted it with NCBI Reference Sequence:

- NCBI Reference Sequence is useful to relate a protein/isoform to its transcript.
- UniProt is where you find curated information on protein function, structure, variants, and interactions.

UniProt has several sections; the class focused on the **Proteins** database [00:41:18].

### Searching UniProt efficiently

The professor recommended using the **advanced search** with two fields [00:42:21]:

- Gene name (e.g., GRIN1, which the transcript misheard as “green one”)
- Organism (e.g., Homo sapiens)

This returns a list including computationally predicted, unreviewed proteins. To reduce redundancy and get curated entries, filter by **Reviewed (Swiss-Prot)** [00:43:24]. The reviewed GRIN1 entry is **glutamate receptor ionotropic NMDA1**, length **938 amino acids** [00:43:24].

### Anatomy of a UniProt entry

Using GRIN1 as the example, the professor walked through the entry sections [00:44:52]:

- **Function**: summary of what the protein does, curated from published papers.
- **Important positions**: e.g., glycine-binding residues.
- **Gene Ontology (GO) keywords**:
  - **Molecular function**: “zoom in” — e.g., glutamate-binding, calcium-ion binding.
  - **Biological process**: “zoom out” — e.g., brain development, calcium ion homeostasis, synapse [00:46:12, 00:47:27].
- **Subcellular location**: e.g., GRIN1 is located in the membrane, with regions inside and outside the cell.
- **Disease and variants**: lists disease-causing mutations with supporting publications. This is more curated than ClinVar but shorter. Also includes non-disease variants.
- **Links to other databases**: e.g., DrugBank for molecules that can bind the protein.
- **Post-translational modifications**: chemical modifications on specific residues.
- **Expression**: tissues expressing the gene.
- **Interactions**: list of proteins interacting with the protein.
- **Structure**: experimental structures from X-ray diffraction or electron microscopy; choose structures covering the whole protein. AlphaFold is a computational model.
- **Sequence/isoforms**: different isoforms from alternative transcripts; all share the same UniProt entry because they are very similar.
- **Download**: download the full text or the **canonical FASTA sequence** [00:55:36].

### AlphaFold warning

AlphaFold is described as a computational prediction method [00:53:15]. The professor stressed:

- AlphaFold can fail when a protein lacks similar proteins with experimentally determined structures.
- Always prefer experimental structures (X-ray, electron microscopy) when available.
- Use AlphaFold only when no experimental structure exists.

### UniProt queries and counts

The professor demonstrated advanced searches and gave these results [00:56:37, 01:00:41, 01:18:19]:

- Searching Homo sapiens without filters gives around **200,000 entries**, but this includes redundancy and unreviewed proteins.
- Reviewed human proteins: **20,420** — the current human proteome count in UniProt Swiss-Prot.
- Reviewed human proteins involved in **type 1 diabetes**: **4**.
- Reviewed human proteins with an experimental 3D structure: **8,605**.
- Why so few structures? Experimental structure determination is expensive and can take years per protein.
- Reviewed human proteins of length 1–30 amino acids: **50**.
- Reviewed human proteins associated with **synapse** via Gene Ontology: **1,682**.
- Reviewed human proteins involved in **activation of the immune response**: **403**.
- HIV-2 proteome (one selected isolate): **9 proteins**.

### Exercise corrections

The professor corrected part of the UniProt exercises [01:09:44]:

- **FGFR3 (Homo sapiens)**:
  - Found via gene name FGFR3 and organism Homo sapiens.
  - Reviewed entry length: **806 amino acids**.
  - Contains **four domains**, e.g., Ig-like C2-type domains at positions 24–126, 151–244, 253–355.
  - Experimental structures cover all domains.
  - Involved in diseases: **achondroplasia**, **Crouzon syndrome**, and other dysplasias; disease-causing mutations are listed in the variant section.
- **EGFR exercise**: locate the variant (e.g., a mutation such as position 428), find its **rs code** and the corresponding **PDB code** from the structure section [01:16:25].
- **Exercise 3**: download sequences of all reviewed human proteins involved in activation of the immune response → 403 proteins.
- **Exercise 4**: download the HIV-2 proteome → 9 proteins for the selected isolate.

### Recommended follow-up

The professor recommended [01:20:33]:

- Do the PyMOL protein structure/function exercises yourself.
- Do the UniProt exercises to learn how to extract biological answers.
- Use solved versions to check answers.

## What the professor stressed

- **Sequence, structure, and function are tightly linked**: if two proteins are similar in sequence, they likely share structure and function; this underpins computational prediction [00:19:13, 00:20:36].
- **Homology thresholds**: 70% nucleotide identity for genes and >25% amino acid identity for proteins [00:09:12]. Below 25%, do not claim homology from sequence alone; structural evidence is needed [00:18:12].
- **Conserved positions in multiple alignments** mark residues essential for survival and function [00:14:11].
- **Use UniProt Swiss-Prot reviewed entries** to avoid redundancy and uncurated predictions [00:43:24].
- **Prefer experimental protein structures over AlphaFold** whenever possible [00:53:15].
- **Remember the human proteome counts**: 20,420 reviewed proteins but only 8,605 with experimental structures [00:56:37, 00:59:37].

## Course logistics mentioned

- After Christmas, the next session will cover **regulation of gene expression**; this will be the last session before the block ends [01:20:33].
- The exam will cover **regulation of gene expression and the human proteome** [01:20:33].
- There is a **Task 3** covering Unit 2 and Unit 3; it is available/posted and due in January, the day before the exam [01:20:33].
- A student noted the Task 3 submission entry said it would open on 11 January and the instructions were not visible; the professor said she would post the link with all task information after class [01:21:34].

## Self-test

1. Distinguish orthologous and paralogous proteins, using hemoglobin examples.

<details><summary>Answer</summary>
Orthologous proteins arise from a speciation event and belong to different organisms, e.g., horse hemoglobin alpha and human hemoglobin alpha. Paralogous proteins arise from a gene duplication event within the same genome, e.g., human hemoglobin alpha and human hemoglobin beta. Both are homologous because they descend from the same ancestral protein.
</details>

2. Why can an ancestral protein give rise to two similar but non-identical proteins?

<details><summary>Answer</summary>
After gene duplication, the two identical copies independently accumulate mutations during evolution. Most mutations are neutral or tolerated, so after many generations the copies remain similar in sequence and structure but are no longer identical.
</details>

3. What sequence identity thresholds did the professor give for hypothesizing homology, and what is the limitation below the protein threshold?

<details><summary>Answer</summary>
For genes: about 70% nucleotide identity. For proteins: more than 25% amino acid identity. Below 25% amino acid identity, you cannot confidently claim homology from sequence alone. Two proteins may still be homologous at 13–15% identity, but that requires additional evidence, such as structural superposition showing a very similar fold.
</details>

4. Explain the chain of reasoning: similar sequence → similar structure → similar function.

<details><summary>Answer</summary>
Because sequence identity correlates strongly with structural similarity, two proteins with similar sequences are expected to fold into similar three-dimensional structures. Since a protein’s function depends on its shape, similar structures imply similar functions. This allows computational prediction of structure and function from sequence without doing experiments.
</details>

5. In a multiple sequence alignment of a homologous protein family, why are some positions perfectly conserved?

<details><summary>Answer</summary>
These positions are not allowed to mutate because they are essential for maintaining protein structure or function. Mutations in these super-conserved positions were eliminated by natural selection because individuals carrying them did not survive or reproduce.
</details>

6. What is the biological role of the heme group in hemoglobin, according to the PyMOL example?

<details><summary>Answer</summary>
The heme group is a non-protein chemical group located in the core of each hemoglobin subunit. It binds oxygen, allowing hemoglobin to transport oxygen. Changes in the protein’s affinity for oxygen determine whether oxygen is bound or released.
</details>

7. In UniProt, why should you filter for reviewed (Swiss-Prot) entries when counting proteins in the human proteome?

<details><summary>Answer</summary>
Unfiltered UniProt searches include unreviewed (TrEMBL) entries and many redundant or computationally predicted proteins, which can inflate the count. The reviewed Swiss-Prot set is manually curated and low-redundancy; it gives the current high-confidence human proteome of 20,420 proteins.
</details>

8. Why does the professor recommend using experimental structures instead of AlphaFold models?

<details><summary>Answer</summary>
AlphaFold is a computational prediction and can fail when the target protein lacks similar proteins with experimentally determined structures. Experimental structures from X-ray crystallography or electron microscopy directly determine atom positions, so they are more reliable. AlphaFold should be used mainly when no experimental structure exists.
</details>

9. How would you use UniProt advanced search to count reviewed human proteins involved in activation of the immune response, and what is the result?

<details><summary>Answer</summary>
Use advanced search: field “Organism” = Homo sapiens, add Gene Ontology term “activation of immune response”, then filter to reviewed (Swiss-Prot). The result is 403 reviewed human proteins.
</details>

10. How many reviewed human proteins have an experimental 3D structure, and why is this number much lower than the total?

<details><summary>Answer</summary>
8,605 of 20,420 reviewed human proteins have an experimental 3D structure. The gap exists because determining a structure experimentally is expensive and can take years for a single protein.
</details>

11. Describe the difference between Gene Ontology “molecular function” and “biological process” as explained in class.

<details><summary>Answer</summary>
Molecular function is a “zoom in”: what the protein does at the molecular level, e.g., binding glutamate or calcium ions. Biological process is a “zoom out”: the larger process in which the protein participates, e.g., brain development or synapse function.
</details>

12. What information can you obtain from the “Disease and variants” section of a UniProt entry?

<details><summary>Answer</summary>
It lists disease-causing variants linked to specific diseases, with supporting publications, and may also list variants not associated with disease. It is a curated but shorter alternative to ClinVar for associating mutations with disease.
</details>

## Related course materials

- [08_2-The human Proteomev2.pdf](../../materials/08_2-The%20human%20Proteomev2.pdf)
- [Exercises on Protein Structure and Function](https://campusvirtual.urv.cat/mod/url/view.php?id=4185476)
- [Exercises on Uniprot](https://campusvirtual.urv.cat/mod/url/view.php?id=4185478)
- [Exercises on Uniprot (solved)](https://campusvirtual.urv.cat/mod/url/view.php?id=4185479)

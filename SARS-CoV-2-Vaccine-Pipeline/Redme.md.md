\# In-Silico Structural Modeling, Validation \& Epitope Prediction of SARS-CoV-2 Spike Protein



\## 📌 Project Overview

This project implements a complete cross-disciplinary \*\*Computational Biology \& Reverse Vaccinology\*\* pipeline to analyze the SARS-CoV-2 Spike Protein. Using open-source immunoinformatics and structural biology tools, the pipeline retrieves viral sequences, predicts secondary and tertiary structures, validates structural geometry, computes physicochemical properties, and screens for high-score antigenic B-cell epitopes for vaccine candidates.



\---



\## 🧬 Methodology \& Pipeline Stages



\### 1. Sequence Retrieval

\* \*\*Database:\*\* NCBI Protein Database

\* \*\*Target:\*\* SARS-CoV-2 Spike Protein (Wuhan-Hu-1)

\* \*\*Accession Number:\*\* `YP\_009724390.1`

\* \*\*Format/Length:\*\* FASTA Sequence (1273 amino acids)



\### 2. Structural Analysis

\* \*\*Secondary Structure:\*\* Predicted structural topology (Alpha-helices, Beta-sheets, and Coils) using the \*\*PSIPRED\*\* workbench to understand protein folding domains.

\* \*\*Tertiary (3D) Modeling:\*\* Generated a high-accuracy 3D structural model via homology modeling using \*\*SWISS-MODEL\*\*. The final output is preserved in standard `.pdb` format.



\### 3. Structure Validation (Stereochemical Verification)

\* \*\*Tool:\*\* SAVES v6.0 (PROCHECK)

\* \*\*Metric:\*\* Ramachandran Plot analysis

\* \*\*Result:\*\* \*\*83.7%\*\* of residues fell within the core/most-favored regions, and \*\*13.3%\*\* in additionally allowed regions. 

\* \*\*Inference:\*\* With a combined score of \*\*97%\*\* in acceptable geometric regions and only \*\*0.9%\*\* in disallowed regions, the model demonstrates high stereochemical quality, ensuring its reliability for vaccine design.



\### 4. Physicochemical Characterization

\* \*\*Tool:\*\* ExPASy ProtParam

\* \*\*Molecular Weight:\*\* 141178.47 Da (\~141.1 kDa)

\* \*\*Theoretical pI:\*\* 6.24 (Slightly acidic nature)

\* \*\*Instability Index:\*\* \*\*33.01\*\* (Classified as mathematically \*\*STABLE\*\*)

\* \*\*GRAVY Score:\*\* \*\*-0.079\*\* (Hydrophilic/water-soluble, ideal for in-vivo dispersion)



\### 5. Immunoinformatics (Epitope Screening)

\* \*\*Database/Tool:\*\* IEDB (Immune Epitope Database)

\* \*\*Algorithm:\*\* Bepipred Linear Epitope Prediction 2.0

\* \*\*Outcome:\*\* Mapped surface-accessible flexible loop regions matching the verified 3D structure to identify potential antigenic B-cell peptide candidates for vaccine formulation.



\---



\## 🌐 Interactive 3D Visualization

Since this model was built using local high-resolution coordinates, you can reload the entire interactive 3D simulation session in seconds without installing any software:

1\. Download the file \*\*`models/selected\_model/spike\_3d\_interactive\_session.molx`\*\* from this repository.

2\. Open the free open-source viewer in your browser: \[Mol\* Viewer](https://molstar.org/viewer/)

3\. Simply \*\*Drag \& Drop\*\* the downloaded `.molx` file anywhere onto the Mol\* browser window.

4\. \*Result:\* The fully colored, structured, and validated 3D SARS-CoV-2 Spike Protein model will instantly load, allowing you to rotate, zoom, and measure residues interactively.

\*(A direct high-resolution static render is also available at `results/phase3\_3d\_modeling/11\_direct\_3d\_model\_render.png`)\*



\---



\## 📂 Repository Deliverables

\* `/data/`: Raw primary sequences (`.fasta`) and screened immunoinformatics B-Cell prediction data.

\* `/models/`: The validated 3D Tertiary Model (`spike\_3d\_model.pdb`) and the interactive session file (`.molx`).

\* `/results/`: Comprehensive visual proofs, phase-separated verification plots, and execution screenshots of the entire pipeline.



\---



\## 💻 Technical Skills Showcased

\* \*\*Domain Knowledge:\*\* Bioinformatics, Reverse Vaccinology, Immunoinformatics, Structural Biology.

\* \*\*Tools \& Frameworks:\*\* NCBI, PSIPRED, SWISS-MODEL, SAVES (PROCHECK), ExPASy ProtParam, IEDB, Mol\* Viewer.

\* \*\*Data Formats:\*\* FASTA, PDB (Protein Data Bank coordinate files).


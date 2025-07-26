# Computational Practice: Align two protein structures with NCBI VAST+
##  Lab Overview
If two proteins have similar structures, then that is evidence for two hypotheses:
Hypothesis A: If protein A and protein B are similar enough in total structure, then they are descended from a common ancestral gene that had 1+ molecular function(s).
Hypothesis B: High conservation of substructures (e.g. conserved protein domains) between protein A and protein B is where the functional protein fold is located but may not be indicated of homology but may indicate common function.
One can compare structures using programs like the NCBI Vector Alignment and Search Tool (VAST+).  We will do that in this lab.

##  Lab Objectives:
In this lab we will align two protein structures. Specifically, you will:

* BLAST a protein sequence against the PDBdatabaseof sequences with solved structures to find a structural template.
* Use this template to find other similar structures with VAST+

Follow these lab instructions:
###  Task A: 
Find a protein structure template that has high sequence similarity to a target sequence.
Before protein structure prediction, you should look for structure templates with homology to the protein structure you are trying to solve.  Any modelling program will do thedatabasesearch for you, but let’s do it by hand by BLASTing a query sequence for homologous sequences that have a solved structure in a structuredatabase(PDB).  Let’s always start with a gene sequence from the genome browser.  Hold your horses, this is going to be fun!

#### Step A. Find the gene encoded in the genome chr19:10,133,346-10,195,135 (hg38 build).  Save the peptide sequence in a FASTA file on the Linux desktop.   		

#### Step B. At NCBI, BLASTP align the protein encoded in ENST00000340748.8 to the pdb protein structuredatabaseat a stringency of E < 1e-100.  Note the PDB accession number for the first hit in the structure da## ase?  (Note:  PDB accession numbers are four characters long.  An underscore ‘_’ followed by a letter means a sequence chain in a structure, so cut of _X to get the PDB accession number. Structures may contain more than one sequence chain.) Find and paste the protein sequence for this structure template into the FASTA file from Step A.

#### Step C. Search the NCBI structuredatabasefor the accession number from Part B (Just use the first 4 characters – not the subchain letter).  

#### Step D. Using a molecular structure viewer open, view and rotate the structure.  Zoom in and out.  Animate (spin it).  Render the structure as a space-filling model, ball and stick, and wireframe.   

###  Task B: 
View the structural homolog using VAST+
Click the VAST+ button on the MMDB page (right-hand side) for the structure.  Choose the best matching structure and click ‘visualize 3D structure superposition’ iCN3D to view the aligned structures.  Note where the peptide backbone diverges between the two structures.  What does the pairwise sequence alignment look like in this substructure?  Paste the FASTA sequence of this template into the FASTA file.

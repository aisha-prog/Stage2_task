# Stage2_task
# Task Code 2.4:
Biochemistry & Oncology
Proteins structures are known to be strongly connected to their functions. However, at the amino acid level, not all amino acids contribute to structure and function equally. Galardini and colleagues decided to investigate the impact of all possible individual, non synonymous nonsense mutations on the structure and function of protein.
The functional impact was computed as SIFT scores and the structural impact was calculated as FoldX Score (in kCal/mol).
Dataset Here:
SIFT Dataset
FoldX Dataset
Task
Import both sift and foldx datasets; in both datasets, create a column specific_Protein_aa which will be a cantenation of the Protein and Amino_acid columns such that If you have Protein A5A607 and Amino_acid E63D, you have specific_Protein_aa A5A607_E63D
Using the specific_Protein_aa column, merge sift and foldx dataset into one final dataframe.
According to the authors;
A SIFT Score below 0.05 is deleterious
A FoldX score greater than 2 kCal/mol is deleterious
Using the criteria above, Find all mutations that have a SIFT score below 0.05 and FoldX Score above 2 (i.e: Mutations that affect both structure and function)
Study the amino acid substitution nomenclature
Investigate for the amino acid that has the most functional and structural impact
Hint: Using the amino acid column, find a way to select the first amino acid. Solution here
Generate a frequency table for all the amino acids
Using the amino frequency table above, generate a barplot and pie chart to represent the frequency of the amino acids.
Briefly describe the amino acid with the highest impact on protein structure and function
What can you say about the structural property and functional property of amino acids with more than 100 occurences.

# Task Code 2.6:
Transcriptomics
This is a processed RNAseq dataset involving reading in quantitated gene expression data from an RNA-seq experiment, exploring the data using base R functions and then interpretation. The dataset contains an experiment between a diseased cell line and diseased cell lines treated with compound X. The difference in expression change between the two health status is computed as Fold change to log 2 (Log2FC) and the significance of each is computed in p-value.
Access Dataset Here
Task:
Generate a volcano plot. (Hint search for volcano plot online)
Determine the upregulated genes (Genes with Log2FC > 1 and pvalue < 0.01)
Determine the downregulated genes (Genes with Log2FC < -1 and pvalue < 0.01)
What are the functions of the top 5 upregulated genes and top 5 downregulated genes. (Use genecards)

# hackathon-bioinfo4400-F24
Hackathon for Final
# Tay-Sachs Disease
## Introduction
Tay-Sachs is an inherited genetic disorder that is caused by an absence of the enzyme that breaks down gangliosides in the brain. Buildup of these fatty ganglioside substances becomes toxic in the brain and spinal cord and leads to diminished nerve cell function. Tay-Sachs usually shows phenotypic symptoms 3-6 months after birth and can cause muscle weakening, seizures, vision and hearing loss, and paralysis. There is no cure for this disease but supportive care can be administered to lessen symptoms and improve quality of life. Thus, children diagnosed with Tay-Sachs generally live around five years. The diagnostic criteria for this disease is genetic testing for two copies of the HEXA gene, how early symptoms start (infantile, juvenile, and late onset), a cherry red spot in the eye in infants, and family history. The prognostic criteria for infantile form is not good with only 2-4 years to live. The infantile form is the most severe form of the disease The prognostic criteria for juvenile form is a little more variable with life expectancy to mid-teenage years. The prognostic criteria for late-onset form which has the best prognosis of a normal life expectancy. There are two main frontline treatments: supportive care and symptom management. Supportive care consists of improving day-to-day life, while symptom management consists of anticonvulsant medication, respiratory care, nutritional support through feeding tubes, physical therapy, and medications for pain. In order for it to be a successful treatment it must help relieve symptoms, slow disease progression, improve the quality of life, and improve biomarkers. It is important to note that occasionally frontline therapies fail. If they fail, there are other options that are being researched. These options include stem cell transplantation, substrate reduction therapy (GM2 ganglioside), gene therapy, pharmaceutical chaperone therapy, and combination therapy. There are also new clinical trials happening for different medications and treatments. The most notable organ involved in the expression of Tay-Sachs is the brain and spinal cord. This disease causes progressive damage to neurons in the brain and spinal cord. Tay-Sachs is a recessive disorder with mutations in the HEXA gene located on chromosome 15. The HEXA gene encodes the alpha subunit of the beta-hexosaminidase A enzyme, which breaks down GM2 ganglioside. GM2 ganglioside is a fatty substance that is abundant in nerve cells. So, whenever this is mutation, it leads to neurodegeneration. 

## Background: Building a Protein
A PPI is a model that represents the physical interactions between proteins. This can include direct or indirect interactions. This means when proteins are working together. A gene co-expression network, on the other hand, is a network that shows similar expression patterns across different conditions or samples. This has more to do with the expression of the genes than the genes themselves, and does not imply physical interaction between gene products. 
Proteins interacting with a seed protein can be found by searching a database. Using a seed protein’s name, gene symbol or accession number in the search bar can find proteins. IntAct can be accessed via Cytoscape by installing IntAct importing it through Cytoscape, and then searching for the protein as noted above. 
A PPI network can be visualized and analyzed by importing a file, either locally or from a database, and analyzing it by using the tools, network analyzer, network analysis, analyze network and similar tools on a program. An example is doing this exact process through Cytoscape. A network can be determined to be scale-free by running a network analyzer, looking at the “Degree Distribution” plot, and analyzing the goodness of fit of data and the R-squared. 
Pathway and disease enrichment for genes can be found through functional enrichment analysis tools. As an example, on ToppFun, identifiers such as gene symbols, Ensembl IDs, or Entrez Gene IDs can be used to search for genes through the “Input Genes” box. Analysis options such such as Pathway or Disease can be selected, and additional parameters can be adjusted as needed. After these steps, the analysis can be run and interpreted. Important values to analyze are the “Pathway” or “Disease” table, the “P-value,” “Genes from Input,” “Q-value FDR B&H,” etc. 

[Toppfun PPI Network.xlsx](https://github.com/user-attachments/files/18024092/Toppfun.PPI.Network.xlsx)

[hexa-disease-edges.xlsx](https://github.com/user-attachments/files/18024389/hexa-disease-edges.xlsx) (cytoscape table)


## Background: Find tissue-specific eQTL
An eQTL (expression Quantitative Trait Locus) is a genomic region (a locus) containing a DNA variation that influences the expression levels of one or more genes. In simpler terms, an eQTL is a genetic variant that affects how much a particular gene is expressed (how much RNA or protein is produced from that gene).

In the context of the human organism, eQTLs play a critical role in understanding the relationship between genetic variations and biological processes, including the development of diseases and traits. In Tay-Sachs, mutations in the HEXA gene often result in diminished function, such as frameshift mutations, insertions, and deletions. However, eQTLs offer an interesting physiological opportunity to modify the severity of heterozygous Tay-Sachs patients and determine HEXA expression for therapeutic strategies. Identifying these eQTLs could be essential for developing targeted gene therapy and small molecule treatments. 

There are multiple eQTLs that could alter the expression of the HEXA gene. HEXA is primarily expressed and mutated in neuronal tissues within the central nervous system. This is the primary location at which beta-hexosaminidase A breaks down a fatty acid substance known as GM2 Ganglioside. The physical symptoms of Tay-Sachs suggest that the expression of HEXA in the brain and spinal cord is critical for neurological health and development. 

There are numerous single nucleotide polymorphisms associated with aberrant HEXA expression in patients with Tay-Sachs. These mutations can occur throughout the gene and result in a variety of HEXA expression interruptions, particularly in the form of  intron variants. For example, rs10640468 is a low frequency insertion mutation located near the TATA promoter region in the frontal cortex of the brain. This mutation may alter polymerase binding for reduced HEXA expression. Conversely, rs3087652 consists of a higher frequency C to T mutation specifically found in the c-1 region of the spinal cord. This mutation is found in the 3’ untranslated region of the HEXA gene, which may impact silencer or enhancer activity of the gene. rs7174287 is a nucleotide mutation that changes a T to either an A, G, or C in an intron of the HEXA gene. This mutation, primarily occurring in the putamen of the basal ganglia, can lead to dysfunctional HEXA protein variants. Next, rs4777505 consists of a nucleotide switch from T to A or C and results in a non-coding transcript variant or an upstream variant, suggesting that this mutation primarily occurs in the untranslated region and affects regulatory elements of the HEXA gene. Interestingly, some eQTLs, such as rs1800428, can actually result in a synonymous variant of the gene. This mutation (G to an A) may not impact a patient’s phenotype but could be an interesting identifier in developing targeted therapies. 

This is the tissue-specific eQTLs DNA polymorphisms found for the HEXA gene. The highest tissues as shown here, are cultured fibroblasts, brain tissue particularly the cerebral hemisphere, and the coronary artery. 

[GTE eQTL for HEXA.pdf](https://github.com/user-attachments/files/18023941/GTE.eQTL.for.HEXA.pdf)
This is the tissue-specific eQTLs DNA polymorphisms found for the HEXA gene. The highest tissues as shown here, are cultured fibroblasts, brain tissue particularly the cerebral hemisphere, and the coronary artery. 

## Experiment: Hypothesis & Methods
Hypothesis: Alterations in the PPI network involving the HEXA gene product (β-hexosaminidase A) leads to a non-wild- type gene expression pattern in Tay-Sachs disease. 

Methods: 
1. Cell Culture Preparation:

a. Obtain fibroblast cell lines from:
Healthy individuals (wild-type)
Tay-Sachs patients (HEXA mutations)

b. Culture cells under standard conditions.

2. PPI Network Analysis

a. Perform Co-IP assays to identify proteins interacting with β-hexosaminidase A in both wild-type and Tay-Sachs cells.

b. Use mass spectrometry to analyze the co-precipitated proteins.

c. Construct PPI networks for wild-type and Tay-Sachs cells 

3. Gene Expression Profiling:

a. Extract RNA from both wild-type and Tay-Sachs cell lines.

b. Perform RNA sequencing to obtain gene expression profiles.

c. Analyze differential gene expression between wild-type and Tay-Sachs cells

4.) Network Perturbation Experiments 

a. We will be looking at the GM2 Activator Protein (GM2A) since it is necessary for the function of the β-hexosaminidase A, product of the HEXA 

b. gene, which breaks down the GM2 ganglioside. 

c. Use CRISPR-Cas9 to create knockout cell lines for the GM2 activator proteins in wild-type cells

d. Overexpress these proteins in Tay-Sachs cells using lentiviral vectors

5.)  Gene Expression Analysis After Network Perturbation:

a. Perform RNA-seq on the knockout and overexpression cell lines

b. Compare gene expression profiles with the original wild-type and Tay-Sachs cells

6.) Functional Assays:

a.  Measure β-hexosaminidase A enzyme activity in all cell lines.

b.  Assess GM2 ganglioside accumulation using thin-layer chromatography.

c. Evaluate lysosomal function through lysosomal pH measurements and cathepsin activity assays.

7.)  Data Integration and Analysis:

a. Integrate PPI network data with gene expression profiles.

b. Use systems biology approaches to identify key regulatory nodes and potential feedback loops.

c. Perform pathway enrichment analysis to identify affected cellular processes.

## Conclusion
This experimental design investigates the alterations in the PPI network within the HEXA gene product, which lead to non-wild-type gene expression in Tay-Sachs Disease. This experimental approach helps cover all bases to support the hypothesis. The results show that Tay-Sachs disease pathology goes beyond enzyme deficiency, and involves complex protein-protein interactions. Mass spectrometry shows the distinct differences in PPI networks between Tay-Sachs cells and wild-type cells. Co-immunoprecipitation also aids in this. The RNA sequencing data showed significant alterations in gene expression. CRISPR-Cas 9 highlights the complex role of the PPI networks that can affect the phenotype. Overexpression of GM2 activator proteins also showed these dynamic interactions. Using these different systems within show many regulatory pathways with protein-protein interactions, including feedback loops. This experiment is critical in fully understanding Tay-Sachs disease, and potentially other lysosomal storage disorders. Therapeutic approaches should consider altering these PPI networks in order to help symptoms or even cure the disease. 


## How to Make A Github
The github markdown language includes important aspects including headers, emphasis, lists, links, images, blockquotes, code, horizontal rules, tables, task lists, mentioning users and teams, emojis, and strikethrough. ‘#’ symbols can be used to create headers. Italics should be surrounded with a single asterisk or underscore. Bold texts should use double, and bold and italic texts should use triple. Unordered lists can use asterisks, plus signs or hyphens whereas ordered lists should use numbers and periods. Links can be inline or reference links, and should always have some kind of URL reference. Images can be inserted using “![Alt text](image URL).” Blockquotes always start with a ‘>.’ Codes can be inline codes or code clocks. Inline codes use backticks whereas code blocks use triple backticks or indents with four spaces. Horizontal rules say to use three or more hyphens, asterisks, or underscores. Tables are basic tables with headers and cells. Task lists can include completed tasks, which are marked with an ‘X,’ or uncompleted tasks. Users and teams can be mentioned by heading their title with an ‘@.’ Emojis can be inserted by using a colon on both sides of the emoji name. Strikethrough can be inserted by using double tildes on both sides (the squiggly lines).
### Contributions
Contributions:

Rachel: Task G and various prometheus prompts, task g questions

Lily: Task F (Hypothesis and Experimental Design)

Sophia: creator of github repository and searched gene data bases for data files for all tasks

Alyssa: Task C (overview of Tay-Sachs,), putting all into github, conclusion

Morgan: Task E (eQTLs) writing portion, Task D (cytoscape)

Prometheus

![Screenshot 2024-12-05 090730](https://github.com/user-attachments/assets/8c49a871-1e03-4255-b531-4c6ac41f356f)

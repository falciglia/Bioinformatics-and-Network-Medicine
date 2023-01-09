# Putative Disease Genes Identification and Drugs Repurposing for Miller-Dieker syndrome

<p align="center">
  <b>BIOINFORMATICS AND NETWORK MEDICINE a.y 2022-2023<br />
La Sapienza University of Rome<br />
ARTIFICIAL INTELLIGENDE AND ROBOTICS<b>  <br />
Course of Data Science<b>  <br />
Salvatore Falciglia, Gerardo Loffredo, Olga Almudena Martinez<b> <br />
</p>


## ABSTRACT

Classical lissencephaly (smooth brain) or generalized agyria-pachygyria is a severe brain malformation which results from an arrest of neuronal migration at 9-13 weeks gestation. It has been observed in several malformation syndromes including Miller-Dieker syndrome (MDS) and isolated lissencephaly sequence (ILS). The loss of a particular gene on chromosome 17, PAFAH1B1, is responsible for the syndrome’s characteristic sign of lissencephaly. The loss of another gene, YWHAE, in the same region of chromosome 17 increases the severity of the lissencephaly in people with Miller-Dieker Syndrome. Recent results strongly support the hypothesis of MDS as a multi-genes disorder, specifically as a contiguous gene deletion syndrome. Nevertheless, papers in literature about MDS are more focused on the phenotype of the disease, looking just at the two genes YWHAE and PAFAH1B1. 

This study wants to apply heuristic research, within the Human Interactome (HI), looking up putative disease genes – associated to Miller-Dieker syndrome – through techniques of Network Medicine. We applied classical network-based tools – such as the two clustering algorithms DiaBLE and Markov Clustering – developed to predict potential disease genes. We took advantage of the scientific knowledge acquired so far through BioGRID, one of the most informative databases of PPIs, and DisGeNET, database from which we gathered known gene disease associations (GDAs) for MDS. Details about networks and graphs were reproduced using both Cytoscape and NetworkX, on Python, as computational and graphical tools. Here we strongly suggest a biological validation – through research biology laboratories – of a list of 34 putative disease genes we found, for which we provide a GO enrichment analysis. On these genes we also performed Drug Repurposing, via DGIdb – the drug-gene interactions database.

## FOLDER TREE
```bash
├── code_py
│   ├── DIAMOnD.py
│   ├── __init__.py
│   └── backbone.py
├── cytoscape_diffusion_algorithm
│   ├── diffusion_time_0.01
│   │   ├── diff_0.csv
│   │   ├── diff_1.csv
│   │   ├── diff_2.csv
│   │   ├── diff_3.csv
│   │   └── diff_4.csv
│   ├── diffusion_time_0.002
│   │   ├── diff_0.csv
│   │   ├── diff_1.csv
│   │   ├── diff_2.csv
│   │   ├── diff_3.csv
│   │   └── diff_4.csv
│   ├── diffusion_time_0.005
│   │   ├── diff_0.csv
│   │   ├── diff_1.csv
│   │   ├── diff_2.csv
│   │   ├── diff_3.csv
│   │   └── diff_4.csv
│   ├── disease_genes_train_0.txt
│   ├── disease_genes_train_1.txt
│   ├── disease_genes_train_2.txt
│   ├── disease_genes_train_3.txt
│   └── disease_genes_train_4.txt
├── data
│   ├── Biogrid_4.4.216.txt
│   ├── C0265219_disease_genes.txt
│   ├── C0265219_disease_genes_DiaBLE.txt
│   ├── C0265219_predicted_genes_directlyconnectedto_PAFAH1B1_YWHAE.txt
│   ├── C0265219_predicted_genes_MCL.txt
│   ├── C0265219_predicted_genes_MCL.txt
│   ├── diseaseLCC_measures.csv
│   ├── diseaseLCC_with_directlyconnectedtoPandY.txt
│   ├── diseaseLCC_with_directlyconnectedtoPandY_measures.csv
│   ├── diseaseLCCpluspredicted_edgetable.txt
│   ├── diseaseLCCpluspredicted_edgetable.txt
│   └── drugs_associatedto_predicted_genes_directlyconnectedto_PAFAH1B1_YWHAE.txt
├── images    
│   ├── fig1_HI.png
│   ├── fig2_LCC.png
│   ├── fig3_diseaseLCC.png
│   ├── fig4_new_diseaseLCC.png
│   ├── fig5_signalingpathways.jpg
│   ├── degreedistribution_initialdiseaseLCC.png
│   └── degreedistribution_newdiseaseLCC.png
├── outputs    
│   ├── pkl_datasets
│   │   └── C0265219.pkl
│   └── results_table
└── notebook_networkmedicineanalysis.ipynb
```

## References
Brock S, Dobyns WB, Jansen A. PAFAH1B1-Related Lissencephaly/Subcortical Band Heterotopia. 2009 Mar 3 [Updated 2021 Mar 25]. In: Adam MP, Everman DB, Mirzaa GM, et al., editors. GeneReviews® [Internet]. Seattle (WA): University of Washington, Seattle; 1993-2022.

Chong S. et al. A revision of the lissencephaly and Miller-Dieker syndrome critical regions in chromosome 17p13.3. 1996 Oct 4. Human Molecular Genetics, 1997, Vol. 6, No. 2.

Lo Nigro C. et al. Point mutations and an intragenic deletion in LIS1, the lissencephaly causative gene in isolated lissencephaly sequence and Miller-Dieker syndrome. 1996 Nov 18. Human Molecular Genetics, 1997, Vol. 6, No. 2.

Cardoso C. et al. Refinement of a 400-kb Critical Region Allows Genotypic Differentiation between Isolated Lissencephaly, Miller-Dieker Syndrome, and Other Phenotypes Secondary to Deletions of 17p13.3. 2003. The American Journal of Human Genetics.

Petti M. et al. Connectivity Significance for Disease Gene Prioritization in an Expanding Universe. IEEE/ACM Trans Comput Biol Bioinform. 2020 Nov-Dec.

*Code inspired from Alessandro Quattrociocchi and Tansel Simsek GitHub repository, Bioinformatics and Network Medicine a.y. 2021-2022.

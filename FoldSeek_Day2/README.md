# Using the suite of Foldseek

The files found in this folder are results, code, downloads and pictures that were obtained by the use of the [FooldSeek suite](https://search.foldseek.com/search).

Here are the steps that were followed, the main objetive was to get a better undertanding of the **protein domains**.

## Consult to CATH
[CATH](https://www.cathdb.info/) is a web page is focused in hierarchical protein structure classification system that organizes **protein domains** based on their structural and evolutionary relationships.

While in the CATH web page, a protein domain was searched in the [CATH sunburst](https://www.cathdb.info/browse/sunburst) menu, in this case the cluster was ["Protein Do-like 9"](https://www.cathdb.info/version/latest/superfamily/3.20.190.20/classification), once here all the protein domains were saved in [domains_used.txt](./foldseekdotcom_downloads/domains_used.txt).

## Foldseek
In the menu was selected [FoldMason MSA](https://search.foldseek.com/foldmason) were all the domains were loaded, then the program was run, from here we could get each .pdb file and the pictures of the structures and also de MSA aligment shown.
Then the results was send to FoldSearch, were all the tables were downloaded and saved in the file [table_fasta-like.tar.gz](./foldseekdotcom_downloads/table_fasta-like.tar.gz)

## Code
For the final part the code [identity_n_RMSD.py](./code/identity_n_RMSD.py) was a modified a little to allow the calculation of the identity, the method to calculate the RMSD was already applied when the code was clone from [GitHub/prog3.1.py](https://github.com/eead-csic-compbio/bioinformatica_estructural/blob/master/code/prog3.1.py). From the same repository the [SVD.py](https://github.com/eead-csic-compbio/bioinformatica_estructural/blob/master/code/SVD.py) library was cloned.



<br>
<br>
<br>
<br>
<br>


Full course in: https://eead-csic-compbio.github.io/bioinformatica_estructural/
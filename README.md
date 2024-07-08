# poore-58-missed-genomes
This provides a quick way to import the TCGA metadata and data and find 58 genomes that should have been excluded in Kraken-TCGA-Voom-SNM-Most-Stringent-Filtering-Data.csv

You will need to get at least 3 files from 
https://ftp.microbio.me/pub/cancer_microbiome_analysis/TCGA/Kraken/

This is required obviously to see which genomes it included.
Kraken-TCGA-Voom-SNM-Most-Stringent-Filtering-Data.csv

Then you need one of these sets. Both sets produce the same 58 genomes that should have been removed.

Metadata-TCGA-Kraken-17625-Samples.csv
Kraken-TCGA-Raw-Data-17625-Samples.csv

or

Metadata-TCGA-All-18116-Samples.csv
Kraken-TCGA-Raw-Data-All-18116-Samples.csv

I have included the imports you will need for R to run the first part of Poore's normalization code, the part that identifies genomes with no information that need to be removed prior to voom normalization.

Change your working directory from C:\\tcga to where you save the data files.
Please report any errors so I can update this project.

Poore's normalization code project can be found here:
https://github.com/biocore/tcga/blob/master/jupyter_notebooks/TCGA%20Batch%20Correction%20--%20Final%20Analysis.ipynb

References:
Poore GD, Kopylova E, Zhu Q, Carpenter C, Fraraccio S, Wandro S, Kosciolek T, Janssen S, Metcalf J, Song SJ, Kanbar J, Miller-Montgomery S, Heaton R, Mckay R, Patel SP, Swafford AD, Knight R, Microbiome analyses of blood and tissues suggest cancer diagnostic approach. Nature. 579, 567–574 (2020).

Sepich-Poore, GD. 2019. "TCGA Batch Correction -- Final Analysis.ipynb". GitHub repository, https://github.com/biocore/tcga/blob/master/jupyter_notebooks/TCGA%20Batch%20Correction%20--%20Final%20Analysis.ipynb, February 19.


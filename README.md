Identification of Hox-regulated transcription factors in C.elegans

This set of codes tries to find the TFs that contain Hox protein binding sites. 

TF_promoters.Rmd contains codes that extract the 1kb promoter sequences (upstream of the start codon ATG) of 921 TFs (from a list from the Walhout lab); the sequences are stored in TF_promoter_sequences.txt with the gene names in TF_promoters_granges_II.csv

HoxPbxSites_in_TF_promoters.Rmd searches the above TF promoter sequences to find conserved HoxPbx sites ("TGATNNATKR") (K=[G/T], R=[G/A]). The results are located in the folder "HP sites found for TGATNNATKR". 185 TF promoters contain at least one sites (check "HoxPbxSites_in_TF_promoters_counts.csv").

I have also used more liberal sites ("TGATNNATNN"). Results are found in "HP sites found for TGATNNATNN" folder.

modencode.Rmd contains codes that extract the ChIP-seq data for lin-39, mab-5, and egl-5; and overlap the ChIP peak granges with the conservative HoxPbx binding sites found in TF promoters. 35 TF promoters contain good Hox site and are bound by Hox proteins in ChIP-seq experiments. See "TF_ConHPsites_bound_by_HOX.csv" for details 
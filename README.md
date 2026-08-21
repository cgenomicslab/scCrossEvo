# scCrossEvo
Single Cell Cross Species Evolutianary Pipeline

This pipeline compares both the Cell atlases of Hydra Vulgarys and Nematostella Vectensis. Scope of this was to find the 1-1 orthologs and see their evolutionary distance on the same space. In addition in order to find this we used different metrics TAI(Transcption Age Index) and a newly developed index TAI* which computes the expression-weighted mean of evolutionary gene ages (Phylostrata) across the shared 1:1 ortholog subset. With this we can weigth older genes and more newer in order to see in which  cell type an invhas been done. The older the genes are the smaller the index and the more newly the gene is the higehr the vaule.

The value is based on a species ladder (which was made by orthofinder) . Where 1 is the clsoer the closest species to that specif organims and and then the max of value is based on the last and more lest common species on that specid ladder. 

So , the better the speceis we choose to make the ladder the finer resuls we will get . 

This indxing is based on a species ladder which were made by  orhofinder .


This pipeline uses the Python's library Scanpy
Psedobulk
Diffeent approches for ortholog normalization (z-score on centorids as well as cluster each species independently, build pseudobulk centroids, correlate the centroids directly)

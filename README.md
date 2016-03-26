# Extracting gene–disease associations from the GWAS Catalog

The [GWAS Catalog](https://www.ebi.ac.uk/gwas/ "NHGRI-EBI Catalog of published genome-wide association studies") compiles associations from published GWAS [[ref](http://doi.org/10.1093/nar/gkt1229 "Welter et al (2013) The NHGRI GWAS Catalog, a curated resource of SNP-trait associations")]. We're [using the resource](http://doi.org/10.15363/thinklab.d80 "Thinklab discussion: Extracting disease-gene associations from the GWAS Catalog") in rephetio, our network for drug repurposing. This repository extracts associations for the diseases and genes in rephetio.

## Execution

The notebooks are executed as follows:

+ [`windows.ipynb`](windows.ipynb) processes the results of a SNAP proxy search to extract windows (genomic regions) around each lead SNP based on linkage disequilibrium ([`data/snap/windows.tsv`](data/snap/windows.tsv)). See [this discussion](http://doi.org/10.15363/thinklab.d71 "Thinklab discussion: Calculating genomic windows for GWAS lead SNPs") for details.

+ [`loci.ipynb`](loci.ipynb) extracts disease–loci (SNP) associations ([`data/snp-associations.tsv`](data/snp-associations.tsv)) and disease–gene associations ([`data/gene-associations.tsv`](data/gene-associations.tsv)).

## License

GWAS Catalog downloads and derivatives are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) in accordance with the EBI's [terms of use](http://www.ebi.ac.uk/about/terms-of-use "Terms of Use for EMBL-EBI Services"). All original content in this repository is licensed under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/ "CC0 1.0 Universal: Public Domain Dedication").

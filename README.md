# GRCm38-C57-DBA-Variant-Calls

Generate available variant calls for C57BL/6NJ and DBA/2J heterozygosis (GRCh38) from MGP variant calls.

## Objective

The Mouse Genomes Project (MGP) uses next generation sequencing technologies to sequence the genomes of key laboratory mouse strains. Here, we integrated the variant calls (SNPs) from C57BL/6NJ and DBA/2J for the analysis of filial generation.

MGP: https://www.sanger.ac.uk/data/mouse-genomes-project/

## Workflow

Outputs:

1. results/C57BL_6NJ_DBA_2J.mgp.v5.snps.dbSNP142.vcf.gz
2. results/C57BL_6NJ_DBA_2J.mgp.v5.snps.dbSNP142.vcf.gz.tbi

Commands:

    # Download variants from MGP
    mkdir -p data
    cd data
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/C57BL_6NJ.mgp.v5.indels.dbSNP142.normed.vcf.gz
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/C57BL_6NJ.mgp.v5.indels.dbSNP142.normed.vcf.gz.tbi
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/C57BL_6NJ.mgp.v5.snps.dbSNP142.vcf.gz
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/C57BL_6NJ.mgp.v5.snps.dbSNP142.vcf.gz.tbi
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/DBA_2J.mgp.v5.indels.dbSNP142.normed.vcf.gz
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/DBA_2J.mgp.v5.indels.dbSNP142.normed.vcf.gz.tbi
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/DBA_2J.mgp.v5.snps.dbSNP142.vcf.gz
    wget https://ftp.ebi.ac.uk/pub/databases/mousegenomes/REL-1505-SNPs_Indels/strain_specific_vcfs/DBA_2J.mgp.v5.snps.dbSNP142.vcf.gz.tbi
    cd ..

Next, perform the integration at the `jupyter.ipynb`.
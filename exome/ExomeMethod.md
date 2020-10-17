# Whole exome sequencing
Exome sequencing was carried out by the UCLA Neuroscience Genomics Core. DNA was hybridized with probes from the Nimblegen SeqCap EZ Exome v2/3 Kapa/IVTL kit (Roche, Basel, Switzerland) and samples were run on an Illumina Hiseq4000 and an average of 44 million paired reads were acquired for each sample. Exome sequencing data was mapped to HG19 using BWA (Li & Durbin, 2009) and the variant calling analysis was performed by Samtools and Bcftools (Li et al., 2009, Narasimhan et al., 2016). Resulting vcf files were filtered for high quality variant calls (%QUAL<20 || DP>100).The variants (CNVs were evaluated by Phred-scaled likelihood values (PL) and individual high quality reads (with either wt or variants were counted.

## Citations:
 * [Li H, and Durbin R, Fast and accurate short read alignment with Burrows-Wheeler Transform. Bioinformatics, 2009;25:1754-60.](https://pubmed.ncbi.nlm.nih.gov/19451168)

 * [Li H, Handsaker B, Wysoker A, Fennell T, Ruan J, Homer N, Marth G, Abecasis G, Durbin R, The Sequence Alignment/Map format and SAMtools. Bioinformatics 2009;25;16;2078-9](https://pubmed.ncbi.nlm.nih.gov/19505943)

 * [Narasimhan V, Danecek P, Scally A, Xue Y, Tyler-Smith C and Durbin R, BCFtools/RoH: a hidden Markov model approach for detecting autozygosity from next-generation sequencing data. Bioinformatics 2016;32;11;1749-51](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4892413)

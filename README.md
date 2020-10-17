# ISOSeqNeoAntigen-nf
This workflow uses PacBio ISOSeq reads, exome reads, and RNA-sequencing reads to faciliate the selection of neoantigens that are disease and patient specific.   

## Summary PacBio ISOSeq discovery

## Summary RNAseq:

  * Hisat2
  * stringtie
  * Subread::featurecounts
  * limma::voom
  * EdgeR::DGEList

## Summary Exome seq

 * bwa mem
 * bcftools mpileup
 * bcftools filter
 * bcftools annotate
 * annotate_variation.pl
 * table_annovar.pl
 * http://shiva.rockefeller.edu/SeqTailor/index_protein.php
 * Filter for SIFT_prediction: deleterious, Polyphen2_HDIV_prediction: deleterious (PP_D) and probable deleterious (PP_P):

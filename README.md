# bMarkerGenerator

To facilitate fine mapping, the b:MarkerGenerator module generates binary markers that represent genetic variations in HLA.


[Development Log]

(2019. 05. 02.) Independent repository to manage bMarkerGenerator alone.

(2020. 04. 29.) Introduced Phasing with Beagle4.1. Now bMarkerGenerator can generate an reference panel for Beagle4.1 reference panel(*.vcf).



[Example]

```
$ python bMarkerGenerator.py \
    --variants example/HAPMAP_CEU \
    --chped example/HAPMAP_CEU_HLA.imgt3320.4field.chped \
    --hg 19 \
    --out tests/MyRef/HAPMA_CEU.REF \
    --dict-AA data/HLA_DICTIONARY_AA.hg19.imgt3320 \
    --dict-SNPS data/HLA_DICTIONARY_SNPS.hg19.imgt3320 \
    --phasing

```
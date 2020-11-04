---
title: "File Formats in Bioinformatics"
excerpt: "Bioinformatics에서 만날 수 있는 file format들을 확인해보자."

categories: 
    - Bioinformatics
    - Data
last_modified_at: 2020-10-15T08:06:00-05:00
---

BI 분석을 하다 보면 굉장히 많은 file format들을 만나는데, 자주 쓰는 파일들의 형식은 거의 비슷하다.  
여기에서는 여러 file formats 을 정리해보았다!

### fastq file

### bam / sam / cram file

### bed file

### vcf file
https://gatk.broadinstitute.org/hc/en-us/articles/360036725531--Tool-Documentation-Index

info field
AC : 
AF : 
AN : 
DP : 
Excess Het : Phred-scaled p-value for exact test of excess heterozygosity
FS : Strand bias estimated using Fisher's exact test
MLEAC : 
MLEAF : 
MQ : Root mean square of the mapping quality of reads across all samples
QD : Qual By Depth
        Quality score normalized by allele depth (AD) 
        각 read가 quality score에 일부 기여하기 때문에, deep coverage가 있는 위치의 변이는 인위적으로 과장된 quality score를 가질 수 있다.
        그러면 실제 quality 보다 더 높게 평가될 수 있다
SOR : 
BaseQRankSum : Rank sum test of REF versus ALT base quality scores
MQRankSum : 


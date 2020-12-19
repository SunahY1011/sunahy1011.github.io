---
title: "Bioinformatics Terminology"
excerpt: "BI에서 자주 쓰이는 용어 정리"

categories: 
    - Bioinformatics
last_modified_at: 2020-11-17T09:15:00-18:00
---

1. Target size : 나의 custom panel에 사용한 gene들에 해당하는 base의 수
(ex. 내가 2개의 gene을 사용하고 각 gene은 exon들의 해당하는 base가 1000개라면, 총 target size는 2000bp)
1. sequencing throughput over target size :
1. depth coverage : 하나의 nucleotide 위치에 어떤 염기가 sequencing 되어 나타나는 횟수를 의미



1. allele fraction : the number of times a mutated base is observed / the total number of times any base is observed at the locus.
1. allele frequency : the number of times a mutated gene is observed / the total number of times any gene is observed at the site.
=> allele frequency != allele fraction
1. VAF : variant allele frequency (특정 위치에 대립 "유전자"가 나타나는 빈도)
1. MAF : mutant allele fraction (특정 위치에 대립 "염기"가 나타나는 빈도)
1. MAC : mutant allele concentration (단위: copies / ml)



1. SNP : Single Nucleotide Polymorphism, 단일 염기의 변이인데 population 내에서 발생하는 변이
1. SNV : Single Nucleotide Variant, 단일 염기의 변이인데 특정 개인에서 발생하는 변이
6, 7을 비교해보자면, SNP는 빈도수가 1% 이상인 경우, SNV는 전체를 다 커버하는 용어


1. CNV : Copy Number Variation, 특정 유전자가 한 번만 나타나는 것이 아닌 반복해서 나타나는 것.  
정상인에서도 많이 갖고 있는 정상 변이를 포함하고 있어, 정상인에서의 다양한 형질의 차이를 일부 설명하며 유전적 진화와 변이의 축적에서도 중요한 역할을 차지.  
germline cell에서의 copy number 변이 => 개체의 모든 세포에서 동일하게 나타남
1. CNA : Copy Number Alteration
somatic cell에서의 copy number 변이 => 특정 종양에서만 나타나게 된다. 
그렇지만, 종종 CNA를 germline, somatic 상관없이 혼용해서 사용하는 경우가 있어, 더욱 명확히 말하고자 할 때는 somatic copy number alterations (SCNAs) 라고 하기도 함.


1. Mutant : 영구적인 변이
1. Variant : 일시적인 변이


1. germline vs somatic mutation : 생식세포 돌연변이, 체세포 돌연변이
유전질환 검사 -> germline mutation
암 환자 조직 -> somatic mutation
1. Inheritance : 부모로부터 물려받은 변이인지, 사아가면서 새로 발생하고 축적된 돌연변이인지
1. Mosaicism : 개체의 모든 세포들이 공유하는 변이인지, 특정 세포에만 발생된 변이인지


1. in vitro : 시험관 실험
1. in vivo : 생체 내 실험 (동물실험)
1. in silico : 컴퓨터 시뮬레이션을 이용하는 방법
1. de novo : 


1. oncogene : is a gene that has the potential to cause cancer. 

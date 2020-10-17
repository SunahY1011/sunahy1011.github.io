---
title: "What is Microarray?"
excerpt: "Microarray란"

categories: 
    - BI&BMI
    - Microarray
last_modified_at: 2020-10-03T09:00:00-01:00
---

블로그를 만들기 이전에 공부했던 내용으로, 당시 구글 검색을 통해 정보를 얻었습니다.  
이번 포스트를 쓰면서 인용한 사이트를 표시하고 싶었지만 그 당시 참고했던 사이트를 
찾지 못했습니다. 자료를 찾는대로 바로 추가하겠습니다.

#### Microarray란

DNA-chip 또는 Biochip 이라 하여 유리슬라이드와 같은 고체 표면에 수천개에서 수만개의 유전자를 고정시켜, 형광표지를 한 probe DNA를 hybridization 시킨 것을 말한다.  
  
주로 두 그룹 간의 상대적인 유전자 발현 정도를 비교하는데 사용하는데,  
여러 종류의 시료에 대한 유전자 발현 정도를 비교하여 다수의 시료 간에  
유전자 발현 정도를 clustering 함으로써 상대적 유사성을 비교분석 하는 데에도 사용한다.  
   
이렇게 찾은 DEG data는 DAVID, IPA를 이용해 분석한다.

#### Microarray의 종류

1. **one-dye** : 두 샘플에 동일한 형광물질을 입힌 후, 두 개의 서로 다른 Microarray에서 반응시켜 측정하는 방식
1. **two-dye** : target과 reference에 각각 적색과 녹색 형광물질을 입힌 후 한 개의 Microarray에서 반응시켜 측정하는 방식

#### Microarray 순서 
1. array를 만든다.
1. 연구하고자 하는 sample에서 mRNA를 추출한다.
1. mRNA를 RT-PCR을 이용해서 cDNA로 만든다.
1. dsDNA를 ssDNA로 만들어
1. array와 hybridization 한 후
1. fluorescence scan하면
1. Raw data 추출!


#### *tips
RNA의 종류에는 두 가지가 있다.  
**mRNA** : 단백질의 아미노산 서열 정보를 담고있음  
**ncRNA** : 전사, splicing, 번역 등에 관여하는 RNA  
(tRNA, rRNA, snoRNA, miRNA, IncRNA ...)

#### Array 제작 과정
유리 slide에 알고 있는 DNA probe를 고정함 -> printing 기법으로 표면에 붙임  
*DNA probe : 짧은 DNA, RNA 조각 / cDNA / oligonucleotide(합성한 가닥)  
=> array를 만들 때 마다 매번 다른 array가 만들어 져 probe가 혼성화 되는 효율이 다르므로 두 샘플을 비교하려면 한 개의 array에 두 샘플을 혼성화 시켜서 비교해야한다. 

#### Microarray의 장단점
**장점**  
- 대량의 유전자 발현 상황을 총체적으로 탐색할 수 있다.    

**단점**
- chip위에 존재하는 서열만 결합 가능하다.
- 교차혼성화(cross hybridization)로 인한 noise 생성
- 특정 gene과의 혼성화는 알지만, 어느 위치에서인지는 알 수 없어 RNA의 염기서열을 알 수 없음

=> 이를 극복한 방법이 RNA-seq이다.  


---

#### What is Microarray?

Microarray (also known as DNA-chip or Biochip) is a collection of microscopic DNA spots attached to a glass-like surface and hybridization with fluorescence-marked probe DNA.  
  
This is usually used for comparison of relative gene variation between two groups.  
Sometimes, people use this for comparative analysis of relative similarity by clustering gene variation between multiple samples.  

Raw data from microarray is analyzed with DAVID, IPA.  

#### Types of Microarray
1. **one-dye** : It is a measurement using two different Microarrays and each of them is hybridized with each sample marked with one same fluorescent material.
1. **two-dye** : It is a measurement using one Microarray which is hybridized with two samples marked with different fluorescent material.

#### Order of Microarray 
1. Make an array
1. Extract mRNA in a sample that you want to search.
1. Make cDNA with mRNA by usig RT-PCR
1. Change dsDNA to ssDNA
1. Hybridize with an array
1. Fluorescence scan
1. Get raw data


#### *tips
There are two types of RNA.   
**mRNA** : has information of protein.
**ncRNA** : participates in transcription, splicing, and translation.  
(tRNA, rRNA, snoRNA, miRNA, IncRNA ...)




**Quotation**  
[Wikipedia](https://en.wikipedia.org/wiki/DNA_microarray)
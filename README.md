Aligned Bible Corpus Data
=========================

Mapping/aligning different Bible editions, variants, corpora and apparatuses.

`greek.tsv` columns
-------------------

This is the main file for comparing Greek editions.

 - **Ref**: Book/Chapter/Verse reference, using USFM book names
 - **TAGNT:Idx**: Line index of TAGNT (values above 80 are lines added to TAGNT)
 - **Greek**: Greek word from TAGNT (or from other sources if in parentheses)
 - **TAGNT:RefSuffix**: Reference suffix from TAGNT (e.g. different verse number)
 - **TAGNT:Strongs**: Strongs number from TAGNT
 - **TAGNT:RMAC**: RMAC morphology from TAGNT
 - **TAGNT:Lemma**: Lemma from TAGNT
 - **Strongs:Lemma**: Lemma from Strongs Dictionary based on Strongs number from TAGNT
 - **Strongs:Origin**: Origin (Greek or Hebrew) Strongs Number(s) from Strongs Dictionary based on Strongs number from TAGNT
 - **Strongs:Root**: Greek Root Strongs Number(s) from Strongs Dictionary based on Strongs number from TAGNT
 - **Strongs:RootLemma**: Lemma(s) associated with those Strongs Numbers
 - **TAGNT:Editions**: Editions line from TAGNT
 - **TAGNT:SBL-Idx**: Computed index of this word in SBL, according to TAGNT
 - **TAGNT:NA28-Idx**: Computed index of this word in NA28, according to TAGNT
 - **TAGNT:Byz-Idx**: Computed index of this word in Byz, according to TAGNT
 - **SBLGNT:Idx**: Actual index of this word in SBLGNT
 - **SBLGNT:Greek**: Greek word from SBLGNT if different from main Greek word (compared in normalized form)
 - **SBLGNT:Location**: Location reference from SBLGNT
 - **SBLGNT:Markers**: Markers (e.g. for apparatus) from SBLGNT
 - **SBLGNT:SBLText**: Greek text from SBLGNT, including diacritics
 - **MorphGNT:Loc**: Location reference from MorphGNT
 - **MorphGNT:Part of Speech**: Part of speech from MorphGNT
 - **MorphGNT:Parsing Code**: Parsing code from MorphGNT
 - **MorphGNT:Text**: Greek text from MorphGNT
 - **MorphGNT:Word**: Word without punctuation from MorphGNT
 - **MorphGNT:Normalized**: Normalized word from MorphGNT
 - **MorphGNT:Lemma**: Lemma from MorphGNT
 - **MorphGNT:Derived:Strongs**: Strongs number derived from Lemma from MorphGNT according to Strongs dictionary
 - **MorphGNT:Derived:RMAC**: RMAC derived from Parsing code from MorphGNT
 - **RP05:Idx**: Actual index of this word in RP05
 - **RP05:Greek**: Greek word from RP05 if different from main Greek word (compared in normalized form)
 - **SemDic:Reference**: Reference from Semantic Dictionary that refers to this word
 - **SemDic:Lemma**: Lemma(s) from Semantic Dictioanry
 - **SemDic:Strongs**: Strongs number(s) from Semantic Dictionary
 - **SemDic:MeaningID**: Meaning ID(s) from Semantic Dictionary
 - **SemDic:LouwNida**: Louw Nida Number(s) from Semantic Dictionary

`greek_mini.tsv` columns
------------------------

Smaller file containing the bare minimum of columns needed to map between different Bible editions. This file is redundant.

 - **Ref**: Book/Chapter/Verse reference, using USFM book names
 - **TAGNT:Idx**: Line index of TAGNT (values above 80 are lines added to TAGNT)
 - **Greek**: Greek word from TAGNT (or from other sources if in parentheses)
 - **TAGNT:SBL-Idx**: Computed index of this word in SBL, according to TAGNT
 - **TAGNT:NA28-Idx**: Computed index of this word in NA28, according to TAGNT
 - **TAGNT:Byz-Idx**: Computed index of this word in Byz, according to TAGNT
 - **SBLGNT:Idx**: Actual index of this word in SBLGNT
 - **SBLGNT:Greek**: Greek word from SBLGNT if different from main Greek word (compared in normalized form)
 - **RP05:Idx**: Actual index of this word in RP05
 - **RP05:Greek**: Greek word from RP05 if different from main Greek word (compared in normalized form)


`na28+ubs4.tsv` columns
-----------------------

Extracted to a separate file since those editions are not Creative Commons licensed. Lines are only included in this file if words exist in either NA28 or UBS4.

 - **Ref**: Book/Chapter/Verse reference, using USFM book names
 - **TAGNT:Idx**: Line index of TAGNT (values above 80 are lines added to TAGNT)
 - **Greek**: Greek word from TAGNT (or from other sources if in parentheses)
 - **NA28:Idx**: Actual index of this word in NA28
 - **NA28:Greek**: Greek word from NA28 if different from main Greek word (compared in normalized form)
 - **UBS4:Idx**: Actual index of this word in UBS4
 - **UBS4:Greek**: Greek word from UBS4 if different from main Greek word (compared in normalized form)


`greekstrongs.tsv` columns
--------------------------

Data derived from Strongs dictionary, by Strongs number instead of by word reference. A lot smaller that way.

 - **Strongs:Number**: Strongs number
 - **Strongs:Lemma**: Lemma from Strongs dictionary
 - **Strongs:Origin**: Origin (Greek or Hebrew) Strongs number(s)
 - **Strongs:Root**: Greek Root Strongs Number(s)
 - **Strongs:RootLemma**: Lemma(s) associated with those Strongs Numbers


Sources and their licenses
==========================

Both Greek And Hebrew
---------------------

- **[STEPBible Data Repository](https://github.com/STEPBible/STEPBible-Data/tree/4d7137189a602e4789069e13f2a5fc2ec5b7ef0f)**

  Licensed under Creative Commons Attribution 4.0 International License.

- **[UBS Dictionaries](https://github.com/ubsicap/ubs-open-license/tree/1a6d31828b933d19974a76ab6e68e43c184f9f7a)**

  This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.


Greek
-----

- **[Strong's Greek Dictionary in XML with real Greek](https://github.com/morphgnt/strongs-dictionary-xml/tree/dd6758b82f46b620804a8ea677d715844679eea1)**

  Released under the Creative Commons CC0 waiver.

- **[SBL Greek New Testament](https://github.com/LogosBible/SBLGNT/tree/4025c2dafe0b1d12799eb8a3e43e2e6137a9253a)**

  The SBLGNT is licensed under a Creative Commons Attribution 4.0 International License.

- **[MorphGNT SBLGNT](https://github.com/morphgnt/sblgnt/tree/aaed91e57c8e4a8dc9a2383e129ca5e75fe6393d)**

  The SBLGNT text itself is subject to the SBLGNT EULA and the morphological parsing and lemmatization is made available under a CC-BY-SA 3.0 License.

- **[The New Testament in the original Greek: Byzantine textform](https://github.com/byztxt/byzantine-majority-text/tree/b844fff9cac3e5788504652d50802b94808b5905)**

  This is free and unencumbered software released into the public domain.

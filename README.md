Aligned Bible Corpus Data
=========================

Mapping/aligning different Bible editions, variants, corpora and apparatuses.


`hebrew.csv` columns
--------------------

This is the main file for comparing Hebrew editions.

- **Ref**: Book/Chapter/Verse reference, using USFM book names
- **Idx**: Line index (values above 80 are lines added to TAHOT, rest is filled with consecutive values)
- **Hebrew**: Hebrew word from TAHOT
- **TAHOT:Idx**: Line index from TAHOT
- **TAHOT:RefSuffix**: Reference suffix from TAGNT (e.g. different verse number)
- **TAHOT:Type**: Text type from TAHOT
- **TAHOT:dStrongs**: Strongs number from TAHOT
- **TAHOT:Grammar**: Grammar information from TAHOT
- **TAHOT:RootStrongs**: Strongs numbers of root from TAHOT
- **OSHB:Idx**: Index of this word in OSHB
- **OSHB:Hebrew**: Hebrew word from OSHB if different from main Hebrew word (compared in normalized form)
- **OSHB:Strong**: Strongs number from OSHB
- **OSHB:Morph**: Morphology information from OSHB
- **OSHB:FullHebrew**:Hebrew word from OSHB, even when same as main Hebrew word
- **LHB:Idx**:  Index of this word in LEB
- **LHB:Hebrew**: Hebrew word from LEB if different from main Hebrew word (compared in normalized form)
- **UHB:Idx**:  Index of this word in UHB
- **UHB:Hebrew**: Hebrew word from UHB if different from main Hebrew word (compared in normalized form)
- **UHB:Strong**: Strongs number from UHB
- **UHB:Morph**: Morphology information from UHB
- **UHB:Lemma**: Lemma from UHB
- **UXLC:Idx**:  Index of this word in UXLC
- **UXLC:Hebrew**: Hebrew word from UXLC if different from main Hebrew word (compared in normalized form)
- **DocumentaryHypothesis**: Documentary hypothesis tagging of the Pentateuch according to UXLC

`hebrew_mini.csv` columns
-------------------------

Smaller file containing the bare minimum of columns needed to map between different Bible editions. This file is redundant.

- **Ref**: Book/Chapter/Verse reference, using USFM book names
- **Idx**: Line index (values above 80 are lines added to TAHOT, rest is filled with consecutive values)
- **Hebrew**: Hebrew word from TAHOT
- **OSHB:Idx**: Index of this word in OSHB
- **OSHB:Hebrew**: Hebrew word from OSHB if different from main Hebrew word (compared in normalized form)
- **LHB:Idx**:  Index of this word in LEB
- **LHB:Hebrew**: Hebrew word from LEB if different from main Hebrew word (compared in normalized form)
- **UHB:Idx**:  Index of this word in UHB
- **UHB:Hebrew**: Hebrew word from UHB if different from main Hebrew word (compared in normalized form)
- **UXLC:Idx**:  Index of this word in UXLC
- **UXLC:Hebrew**: Hebrew word from UXLC if different from main Hebrew word (compared in normalized form)


`greek.csv` columns
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
 - **RP18:Idx**: Actual index of this word in RP18
 - **RP18:Greek**: Greek word from RP18 if different from main Greek word (compared in normalized form)
 - **RP18:Strongs**: Strongs number from RP18
 - **RP18:Morph**: Morphology from RP18
 - **SBLGNT+App:Idx**: Index of this word in either SBLGNT or its apparatus (starting at 70)
 - **SBLGNT-App:Idx**: Indexes of this word (variation group `:` Greek word) in the SBLGNT apparatus
 - **UGNT:Idx**: Actual index of this word in UGNT
 - **UGNT:Greek**: Greek word from UGNT if different from main Greek word (compared in normalized form)
 - **UGNT:Strongs**: Strongs number from UGNT
 - **UGNT:Morph**: Morphology from UGNT
 - **UGNT:Lemma**: Morphology from UGNT

`greek_mini.csv` columns
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
 - **RP18:Idx**: Actual index of this word in RP18
 - **RP18:Greek**: Greek word from RP18 if different from main Greek word (compared in normalized form)
 - **SBLGNT+App:Idx**: Index of this word in either SBLGNT or its apparatus (starting at 70)
 - **SBLGNT-App:Idx**: Indexes of this word (variation group `:` Greek word) in the SBLGNT apparatus
 - **UGNT:Idx**: Actual index of this word in UGNT
 - **UGNT:Greek**: Greek word from UGNT if different from main Greek word (compared in normalized form)


`na28+ubs4.csv` columns
-----------------------

Extracted to a separate file since those editions are not Creative Commons licensed. Lines are only included in this file if words exist in either NA28 or UBS4.

 - **Ref**: Book/Chapter/Verse reference, using USFM book names
 - **TAGNT:Idx**: Line index of TAGNT (values above 80 are lines added to TAGNT)
 - **Greek**: Greek word from TAGNT (or from other sources if in parentheses)
 - **NA28:Idx**: Actual index of this word in NA28
 - **NA28:Greek**: Greek word from NA28 if different from main Greek word (compared in normalized form)
 - **UBS4:Idx**: Actual index of this word in UBS4
 - **UBS4:Greek**: Greek word from UBS4 if different from main Greek word (compared in normalized form)


`greekstrongs.csv` columns
--------------------------

Data derived from Strongs dictionary, by Strongs number instead of by word reference. A lot smaller that way.

 - **Strongs:Number**: Strongs number
 - **Strongs:Lemma**: Lemma from Strongs dictionary
 - **Strongs:Origin**: Origin (Greek or Hebrew) Strongs number(s)
 - **Strongs:Root**: Greek Root Strongs Number(s)
 - **Strongs:RootLemma**: Lemma(s) associated with those Strongs Numbers


`sblgnt-apparatus.csv` columns
------------------------------

Data derived from SBLGNT's apparatus.

 - **Ref**: Book/Chapter/Verse reference, using USFM book names
 - **Idx**: Number of variation group `:` Number of greek word in variation group.
   Possible additions `(1)` denote parts of that word, or `(+)` joined with next word.
 - **Greek**: Greek word
 - **Editions**: Editions this greek word is included. `+` or `-` are used to record discrepancies from original document.
 - **TAGNT-Idx**: Corresponding line in `greek.csv`, if unambiguous
 - **SBL:Idx**: Index of word in SBLGNT
 - **SBL:TAGNT-Idx**:  Corresponsing line in `greek.csv` for SBLGNT
 - **NA28:Idx**: Index of word in NA28
 - **NA28:TAGNT-Idx**: Corresponsing line in `greek.csv` for NA28
 - **RP05:Idx**: Index of word in RP05
 - **RP05:TAGNT-Idx**: Corresponsing line in `greek.csv` for RP05


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

- **[unfoldingWord® Greek New Testament](https://git.door43.org/unfoldingWord/el-x-koine_ugnt/src/commit/fc95b2b8aad08bb65ab54628ab685413a1139e97)**

  This work is made available under the Creative Commons Attribution-ShareAlike 4.0 International License.

- **[The New Testament in the original Greek: Byzantine textform](https://github.com/byztxt/byzantine-majority-text/tree/b844fff9cac3e5788504652d50802b94808b5905)**

  This is free and unencumbered software released into the public domain.


Hebrew
------

- **[Open Scriptures Hebrew Bible](https://github.com/openscriptures/morphhb/commit/3d15126fb1ef74867fc1434be1942e837932691f)**

  License: Creative Commons Attribution 4.0 International (CC BY 4.0)

- **[unfoldingWord® Hebrew Bible](https://git.door43.org/unfoldingWord/hbo_uhb/src/commit/0231ffdfea1ec5a3061e19fcf5f58943007aeb9d)**

  This work is made available under the Creative Commons Attribution-ShareAlike 4.0 International License.

- **[Unicode/XML Leningrad Codex](https://www.tanach.us/Pages/XMLFiles.html)**

  All biblical Hebrew text, in any format, may be viewed or copied [without restriction](https://www.tanach.us/License.html)

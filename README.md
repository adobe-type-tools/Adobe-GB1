# The Adobe-GB1-6 Character Collection
---
© 1995–1998, 2000, 2005, 2007, 2012, 2017, 2023 Adobe.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file to use, copy, publish, distribute, sublicense, and/or sell copies of the documentation, and to permit others to do the same, provided that:

No modification, editing or other alteration of this document is allowed; and

The above copyright notice and this permission notice shall be included in all copies of the documentation.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file, to create their own derivative works from the content of this document to use, copy, publish, distribute, sublicense, and/or sell the derivative works, and to permit others to do the same, provided that the derived work is not represented as being a copy or version of this document.

Adobe shall not be liable to any party for any loss of revenue or profit or for indirect, incidental, special, consequential, or other similar damages, whether based on tort (including without limitation negligence or strict liability), contract or other legal or equitable grounds even if Adobe has been advised or had reason to know of the possibility of such damages. The Adobe materials are provided on an "AS IS" basis. Adobe specifically disclaims all express, statutory, or implied warranties relating to the Adobe materials, including but not limited to those concerning merchantability or fitness for a particular purpose or non-infringement of any third party rights regarding the Adobe materials.

Adobe holds no patents on the subject matter of this specification.

Last updated 2023-04-21

---
## Introduction
The purpose of this document is to define and describe the *Adobe-GB1-6* character collection, which enumerates 30,572 glyphs, and whose designation is derived from the following three /CIDSystemInfo dictionary entries:

* /Registry (Adobe)
* /Ordering (GB1)
* /Supplement 6

CIDFont resources that reference this character collection must include a /CIDSystemInfo dictionary that matches the /Registry and /Ordering strings shown above.

This document is designed for font developers, for the purpose of developing Simplified Chinese fonts for use with PostScript products, or for developing OpenType Simplified Chinese fonts. It is also useful for application developers and end users who need to know more about the glyphs in this character collection. This document expects that its readers are familiar with the CID-keyed font file format, which is described in [Adobe Technical Note #5014](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5014.CIDFont_Spec.pdf), entitled *Adobe CMap and CIDFont Files Specification*.

A character collection contains the glyphs that are required to develop font products for a specific language, script, or market. Specific encodings are defined through the use of CMap resources that are instantiated as files, and generally reference a subset of the character collection.

The character collection that results from each Supplement includes the glyphs associated with all earlier Supplements. For example, Supplement 6 includes all glyphs defined in Supplements 0 through 5.

The Adobe-GB1-6 character collection enumerates 30,572 glyphs, specifically CIDs 0 through 30571, among seven Supplements, designated 0 through 6. Adobe-GB1-6 supports the GB 2312-80, GB 1988-89, GB/T 12345-90, GB 13000.1-93, and GB 18030-2022 Implementation Level 2 character set standards. The following table summarizes these seven Supplements, and also provides the pages on which their glyphs are shown in the [*Adobe-GB1-6.pdf*](https://github.com/adobe-type-tools/Adobe-GB1/raw/master/Adobe-GB1-6.pdf) file:

**Supplement** | **Additional CIDs** | **CID Range** | **Total CIDs** | **Date of Establishment** | **Pages**
--- | --- | --- | --- | --- | ---
0 | *n/a* | 0–7716 | 7,717 | 1995-06-26 | 1–16
1 | 2,180 | 7717–9896 | 9,897 | 1996-02-06 | 16–20
2 | 12,230 | 9897–22126 | 22,127 | 1997-11-13 | 20–45
3 | 226 | 22127–22352 | 22,353 | 1998-10-08 | 45
4 | 6,711 | 22353–29063 | 29,064 | 2000-11-20 | 45–59
5 | 1,220 | 29064–30283 | 30,284 | 2005-12-04 | 59–61
6 | 288 | 30284-30571 | 30,572 | 2023-04-21 | 61-62

Each CID (*Character ID*) in a character collection is associated with a class of character shapes or glyphs. The specific shape of a glyph from a given glyph class is dependent on the typeface style and possibly other factors. Glyphs for all CIDs are illustrated in this document, providing a specific example or instance of the correspondence between a CID and its glyph shape class. Font developers should design glyphs for each CID of the character collection, and may use this document as a reference when proofing or otherwise validating CIDFont resources.

The following sections detail the history and contents of each of the seven Supplements of the Adobe-GB1-6 character collection.

---
## Supplement 0—Adobe-GB1-0

Supplement 0, which enumerates 7,717 glyphs, specifically CIDs 0 through 7716, support the GB 2312-80 and GB 1988-89 character set standards, to include corrections and additions specified in GB 6345.1-86, along with the Macintosh® versions thereof. Also included are vertical characters specified in GB/T 12345-90.

---
## Supplement 1—Adobe-GB1-1

Supplement 1 provides 2,180 additional glyphs, specifically CIDs 7717 through 9896, that are necessary to support the GB/T 12345-90 character set standard. These 2,180 additional glyphs are traditional forms of hanzi that are included in Supplement 0.

---
## Supplement 2—Adobe-GB1-2

Supplement 2 adds 12,230 glyphs, specifically CIDs 9897 through 22126, and provides support for the GBK character set standard (aka, GB 13000.1-93). These 12,230 additional glyphs include the hanzi necessary to completely support both the GBK character set standard and the complete set of 20,902 Chinese characters in Unicode Version 1.1.

---
## Supplement 3—Adobe-GB1-3

Supplement 3 adds 226 glyphs, specifically CIDs 22127 through 22352, and was designed to add only pre-rotated versions of all non–full-width Latin and Latin-like glyphs found in Supplement 0, for the specific purpose of supporting the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB (*Glyph SUBstitution*) feature.

---
## Supplement 4—Adobe-GB1-4

Supplement 4 adds 6,711 glyphs, specifically CIDs 22353 through 29063, to support the GB 18030-2000 character set standard. CIDs 22353 through 22356 provide glyphs for additional currency symbols with proportional and half-width properties, CID+22357 provides the ideographic half fill space that serves as a visual indicator of a screen space for half an ideograph, CID+22358 provides a full-width glyph for the Euro currency symbol, CIDs 22359 through 22397 provide glyphs for additional hiragana and katakana characters and symbols, some of which are adjusted for vertical use, CIDs 22398 through 22400 provide the so-called “Hangzhou” or “Suzhou” numerals that correspond to ten, twenty, and thirty, and CIDs 22401 through 22427 provide glyphs for extended Bopomofo.

The major portion of Supplement 4, specifically CIDs 22428 through 29058, provide the glyphs necessary to support CJK Unified Ideographs Extension A in its entirety, as defined by Unicode Version 3.0 and ISO 10646-1:2000.

---
## Supplement 5—Adobe-GB1-5

Supplement 5 adds 1,220 glyphs, specifically CIDs 29064 through 30283, and provides support for Yi, which is one of the regional scripts referenced in the GB 18030-2005 character set standard.

---
## Supplement 6—Adobe-GB1-6

Supplement 6 adds 288 glyphs, CIDs 30284 through 30571, to support Implementation Level 2 of the GB 18030-2022 character set standard.

---

## Special Glyphs & Other Notes
The following sections detail special glyphs and other notes that are of interest to font developers. Several glyph classes are complex, and deserve some amount of explanation and clarification.

### Space Glyphs

The following table lists all of the Adobe-GB1-6 glyphs that are classified as a space, or are otherwise rendered as a space, and provides information with regard to their intended usage, along with their recommended set widths:

**CID** | **Set Width** | **Description**
--- | --- | ---
1 | Proportional | Latin space—U+0020
96 | Full-width | Ideographic space—U+3000
7716 | Half-width | Latin space—U+2002
22127 | Full-width | Pre-rotated version of CID+1
22352 | Full-width | Pre-rotated version of CID+7716

The space glyphs that are described as a pre-rotated version of another glyph must be assigned full-width set widths in terms of their horizontal set widths, but when instantiated as an OpenType font, their vertical set widths as specified in the OpenType ‘[vmtx](https://www.microsoft.com/typography/otspec/vmtx.htm)’ (*Vertical Metrics*) table should match those of their unrotated counterparts.

### Hanzi Glyphs

Adobe-GB1-6 includes 27,917 glyphs that are classified as hanzi (aka ideographs), and their CID ranges, separated by Supplement, are shown in the table below:

**Supplement** | **CID Ranges**
--- | ---
0 | 940–7702
1 | 7717–9896
2 | 10072–22126
3 | *none*
4 | 22428–29058
5 | *none*
6 | 30284-30571
### Pre-Rotated Glyphs

In order to support the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB feature, the Adobe-GB1-6 character collection includes pre-rotated forms for all Latin and Latin-like glyphs that are not full-width. The table below details how horizontal CIDs and CID ranges map to their corresponding pre-rotated CID ranges:

**Supplement** | **Horizontal CIDs & CID Ranges** | **Pre-Rotated CID Ranges**
--- | --- | ---
3 | 1–95, 7712–7715, 814–939, 7716 | 22127–22352
4 | 22353–22357 | 29059–29063

### Glyph Set Widths

The following table provides CIDs and CID ranges that explicitly indicate which glyphs are intended to be designed with proportional- or half-width set widths. All other glyphs are expected to be full-width.

**Set Width** | **CIDs & CID Ranges**
--- | ---
Proportional | 1–95, 7712–7715, 22353–22354
Half-width | 814–939, 7716, 22355–22357

The glyph tables that are provided in this document include registration marks that serve to indicate relative set width. Explicitly specifying width classes, such as in the above table, is clearly more accurate and reliable than measuring the distance between registration marks. Please use both resources as your guide.

Note that the registration marks used in the glyph tables are in a separate layer, and if their presence is annoying, that layer can be turned off, thus preventing their display.

---
## CMap Resources

The CMap resources associated with the Adobe-GB1-6 character collection, along with the [*cid2code.txt*](https://raw.githubusercontent.com/adobe-type-tools/cmap-resources/master/Adobe-GB1-6/cid2code.txt) datafile that provides additional details for font developers, are available as part of the [*CMap Resources*](https://github.com/adobe-type-tools/cmap-resources/) open source project.

More complete descriptions of the individual Adobe-GB1-6 CMap resources can be found in [Adobe Technical Note #5094](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5094.CJK_CID.pdf), entitled *Adobe CJKV Character Collections and CMap Files for CID-Keyed Fonts*.

In general, the CMap resources that are based on legacy encodings, such as GBK, are no longer being updated. Rather, the Unicode CMap resources—available for UTF-8, UTF-16 (UTF-16BE), and UTF-32 (UTF-32BE) encodings, and kept perfectly synchronized—are updated on a regular basis, with new mappings being triggered by a new Supplement or a new version of Unicode. Furthermore, the UCS-2 CMap resources are obsolete and deprecated. Developers should use the UTF-16 CMap resources instead, because they are forward compatible with the now-obsolete UCS-2 ones.

---
## Unicode Variation Sequences

The [Standardized Variation Sequences](http://www.unicode.org/Public/UCD/latest/ucd/StandardizedVariants.txt) (SVSes) that are specified in the [*Adobe-GB1_sequences.txt*](https://github.com/adobe-type-tools/Adobe-GB1/raw/master/Adobe-GB1_sequences.txt) datafile correspond to CJK Compatibility Ideographs.

---
## Glyph Tables

Representative glyphs for CIDs 0 through 30571 are provided in the [*Adobe-GB1-6.pdf*](https://github.com/adobe-type-tools/Adobe-GB1/raw/master/Adobe-GB1-6.pdf) file that is included in this repository, with 500 glyphs shown per page. And, for reader convenience, the beginning of each Supplement is clearly marked. The typeface used to exemplify each glyph is *Adobe Song Std L* (aka, AdobeSongStd-Light or Adobe 宋体 Std L), designed by Changzhou SinoType Technology Co., Ltd, owned by Adobe, and certified by the Press and Publication Administration of the People’s Republic of China, the China State Language Commission, and the National Typeface Committee. The specific font instance is Version 6.000, as reflected in its /CIDFontVersion dictionary entry.

---
## Changes Since Earlier Versions

The following sections detail the history of this document, which was originally referred to as Adobe Technical Note #5079.

### Since the 2000-11-30—Supplement 4—Version

The glyphs for Supplement 5, aimed to provide support for the Yi regional script of GB 18030, were added, and AdobeSongStd-Light (*Adobe Song Std L*) with /CIDFontVersion value 5.002 was used for the representative glyphs. Note that previous versions of this Adobe Tech Note used STSongStd-Light (*STSong Std Regular*) for its representative glyphs.

### Since the 2007-02-28—Supplement 5—Version

The entire document was completely re-written.

### Since the 2012-01-24—Supplement 5—Version

The entire specification was ported to GitHub markdown syntax and revised.

### Since the 2019-07-29—Supplement 5—Version

The glyphs for Supplement 6 were added to support Implementation Level 2 of the GB 18030-2022 character set.

That is all.

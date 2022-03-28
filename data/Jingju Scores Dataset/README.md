# Jingju Music Scores Collection
The **Jingju Music Scores Collection** (**JMSC**) is part of the [**Jingju Music Corpus**](http://compmusic.upf.edu/corpora) created in the [**CompMusic** project](http://compmusic.upf.edu/). Created with the purpose of the melodic research of jingju singing lines, it contains **108 MusicXML** scores, covering **1084 melodic lines**. In terms of the jingju musical system, it covers the following elements:
- **role type**: *laosheng*, *dan*, *laodan*
- **_shengqiang_**: *erhuang*, *xipi*, *nanbangzi*, *sipingdiao*
- **_banshi_**: *manban*, *sanyan*, *zhongsanyan*, *kuaisanyan*, *yuanban*, *erliu*, *kuai'erliu*, *liushui*, *kuaiban*

The following table gives details about the content of the **JMSC** in terms of scores:

||*laosheng*|*dan*|*laosheng* + *dan*|*dan* + *laodan*|Total|
|---|---:|---:|---:|---:|
|**_erhuang_**|22|18|1|1|42|
|**_xipi_**|28|31|3|0|62|
|**_nanbangzi_**|0|2|0|0|2|
|**_sipingdiao_**|0|2|0|0|2|
|**Total**|50|53|4|1|**108**|

The following table gives details about the content of the **JMSC** in terms of lines (*ls* stands for *laosheng*, *da* stands for *dan*, *ld* stands for *laodan*, *eh* stands for *erhuang*, *xp* stands for *xipi*):

||*lseh*|*lsxp*|*daeh*|*daxp*|*danbz*|*daspd*|*ldeh*|Total|
|---|---:|---:|---:|---:|---:|---:|
|**_manban_**|69|17|84|50||||220|
|**_sanyan_**|12|17|||||2|31|
|**_zhongsanyan_**|||6|||||6|
|**_kuaisanyan_**|26|6|35|||||67|
|**_yuanban_**|113|61|54|55|10|9||264|
|**_erliu_**||1||22||||23|
|**_kuai'erliu_**||22||||||22|
|**_liushui_**||92||142||||234|
|**_kuaiban_**||85||47||||132|
|**_daoban_**||2||1||||3|
|**_sanban_**|2|4||3||||9|
|**_yaoban_**|1|12|1|1||||15|
|**_kutou_**|4||2|||||6|
|**Total**|227|319|182|321|10|9|2|**1070**|

The scores are sourced from printed editions and created with [MuseScore 2.1.0](https://musescore.org/), including the lyrics. The original [*jianpu* notation](https://en.wikipedia.org/wiki/Numbered_musical_notation) is transnotated into staff notation. All the scores contain a separated staff for the accompaniment (jinghu) line.

## Content of the **JMSC**
The **JMSC** contains the following three folders:
- The `MusicXML` folder contains the MusicXML scores and the `scores_data.csv` and `lines_data.csv` files containing metadata and annotations.
- The `MuseScore` folder contains the scores created with MusicScore in its original format, from which the MusicXML scores were exported.

## Annotations and metadata
The `MusicXML` folder of the **JMSC** contains the following two files with annotations and metadata.
- The `scores_data.csv` file contains metadata and annotations for each score. The included information consists of the following data: title of the aria (in Chinese), role type, *shengqiang*, *banshi*, 'yes' or 'no' the original score contained a separated line for the accompaniment, the reference to the printed source, and the MusicBrainz ID of related recordings.
- The `lines_data.csv` file contains annotations for each line in the **JMSC**. The included information consists of the following data: role type, *shengqiang*, *banshi*, line type, lyrics of the line, starting offset of the line, ending offset of the line, linguistic tones, lyrics of the first line section, starting offset of the first line section, ending offset of the first line section, lyrics of the second line section, starting offset of the second line section, ending offset of the second line section, lyrics of the third line section, starting offset of the third line section, and ending offset of the third line section. Regarding line types, 's' stands for opening line in *xipi*, 's1' for the long opening line type, and 's2' for the short opening line type in *erhuang*, and 'x' for closing line.

## Using the **JMSC**
Since the scores are sourced from copyrighted printed editions, they can be only shared for non commercial research purposes (see below). The metadata and annotations files are released under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/) license.

Different datasets from the **JMSC** have been used in the following publications:

Gong, Rong, Nicolas Obin, Georgi Dzhambazov, and Xavier Serra (2017) "Score-informed syllable segmentation for jingju a cappella singing voice with mel-frequency intensity profiles." In *Proceedings
of the 7th International Workshop on Folk Music Analysis*
(FMA 2017), Málaga, Spain, June 14–16, pp. 107–113. https://doi.org/10.5281/zenodo.556820

Gong, Rong, Jordi Pons and Xavier Serra (2017) "Audio to Score Matching by Combining Phonetic and Duration Information." In *Proceedings of the 18th International Society for Music Information Retrieval Conference* (ISMIR 2017), Suzhou, China, October 23–27, 428–434. https://arxiv.org/abs/1707.03547

Gong, Rong, and Xavier Serra (2018) "Singing voice phoneme segmentation by hierarchically inferring syllable and phoneme onset positions." In *Interspeech 2018*, Hyderabad, India, September 2–6, 716–720. https://arxiv.org/abs/1806.01665

Caro Repetto, Rafael (2018) *The musical dimension of
Chinese traditional theatre: An analysis from computer aided musicology*. PhD thesis, Universitat Pompeu Fabra, Barcelona, Spain. http://hdl.handle.net/10803/665357

## Contact
For any questions or comments about the **JMSC**, please contact  
  Rafael Caro Repetto  
  (rafael.caro@upf.edu)

## Acknowledgements
The creation of the **JMSC** is funded by the European Research Council under the European Union’s Seventh Framework Program (FP7/2007-2013), as part of the CompMusic project (ERC grant agreement 267583).

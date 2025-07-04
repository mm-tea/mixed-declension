# The transfer of former \*_ja_-stems to a mixed declension in Old Czech and Slovak

This repository contains additional data for my BA thesis _Comparative Indo-European Linguistics_ at Universiteit Leiden.

The data is presented here both as an appendix to the thesis itself, but also in case anyone else wants to reuse the data for another use.

## Included files

- [`bibliography.yaml`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml) contains the used bubliography in [Hayagriva](https://github.com/typst/hayagriva/) format.
- [`thesis.pdf`](https://github.com/mm-tea/mixed-declension/blob/main/thesis.pdf) is the text for the thesis itself.
- [`data/`](https://github.com/mm-tea/mixed-declension/tree/main/data) contains comma-separated table files in which the data used in the thesis is stored. Specifically, these are:
	- [`data/declensions.csv`](https://github.com/mm-tea/mixed-declension/blob/main/data/declensions.csv) contains data collected from [`tesitelova1986`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml) and [`mistrik1976`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), described in Section 2.
	- [`data/excluded data.csv`](https://github.com/mm-tea/mixed-declension/blob/main/data/excluded%20data.csv) lists the data excluded, as described in Section 2.2.
	- [`data/attestations.csv`](https://github.com/mm-tea/mixed-declension/blob/main/data/attestations.csv), the file containing the data collected, described, and used in Section 4.
	- [`data/texts.csv`](https://github.com/mm-tea/mixed-declension/blob/main/data/texts.csv) explains the `Citation` column in the above table. If the given entry comes from one of the two sources on Old Czech, this file will point to a more comprehensive description of the original text.
- [`interactive-charts/`](https://github.com/mm-tea/mixed-declension/tree/main/data) contains the charts from Section 4.3.1 in the thesis.
	- [`interactive-charts/time-total.html`](https://github.com/mm-tea/mixed-declension/blob/main/interactive-charts/time-total.html) is Figure 1,
	- [`interactive-charts/time-freq.html`](https://github.com/mm-tea/mixed-declension/blob/main/interactive-charts/time-freq.html) is Figure 2.

## Visualisations

- [Figure 1](https://html-preview.github.io/?url=https://github.com/mm-tea/mixed-declension/blob/main/interactive-charts/time-total.html)
- [Figure 2](https://html-preview.github.io/?url=https://github.com/mm-tea/mixed-declension/blob/main/interactive-charts/time-freq.html)

Hovering over a datapoint will display an infobox listing information about the attestation.

## Table descriptions

### [Declensions](https://github.com/mm-tea/mixed-declension/blob/main/data/declensions.csv)
This table has two groups of columns, one for data from Slovak ([`mistrik1976`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml)), the other from Czech ([`tesitelova1986`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml)).

| ID Sk | Word Sk | Frequency Sk | Type Sk | Page Sk | ID Cz | Word G Cz | Page G Cz | Word N Cz | Frequency Cz | Page Cz | Comment |
| ----- | ------- | ------------ | ------- | ------- | ----- | --------- | --------- | --------- | ------------ | ------- | ------- |
| 133   | inšpirácia | 2         | 6       | 120     | 96    | inspirace | 188       | inspirace | 6            | 23      |         |
|       | inštalácia | 1         | 6       | 118     | 34    | instalace | 187       | instalace | 14           | 23      |         |
|       |         |              |         |         | 104   | instaurace | 188      | instaurace | 1           | 23      |         |
| 159   | intuícia | 2           | 6       | 124     |       | intuice   |           | intuice   | 1            | 26      |         |
| 63    | jašterica | 2          | 6       | 110     |       | ještěřice |           | ještěřice | 1            |         |         |

Each row corresponds to a paired lexeme. If it only appears in one language, the column group for the other is empty, like in _instaurace_ above.

The word has an assigned ID value if it meets the inclusion criteria specified in Section 2.1 (e.g. _instalace_ above); if it is only included as a parallel to a qualifying word in the other language, the ID is missing (e.g. _inštalácia_ above).

In the Slovak section, the lemma form of the word is listed, its frequency and declension type according to [`mistrik1976`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), and the page where this information can be found.

In the Czech section both the lemma form and the "genitival form" (G.sg or NAV.pl) is listed. These have to be collected from two different sections of [`tesitelova1986`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), so two page numbers are listed. The frequency value listed refers to the total frequency of the lexeme, found alongside the lemma value.

If the word is present in [`havranek1989`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml) but not in [`tesitelova1986`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), page information is not listed and the word is assigned a frequency of 1. If the lexeme appears in [`tesitelova1986`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml) but not in a "genitival" form, only one page number is listed (e.g. _intuice_ above).

The `Comment` column may contain any extra notes.

#### [Excluded data](https://github.com/mm-tea/mixed-declension/blob/main/data/excluded%20data.csv)

The structure of this table is identical to that described above. The `Comment` column describes reason for exclusion, also described in Section 2.2.

### [Attestations](https://github.com/mm-tea/mixed-declension/blob/main/data/attestations.csv)

This table lists the various attestations from [`gebauer1960`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), [`porak1979`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), and [`blanar`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml).

| Number | Case | Word  | Item                                       | Ending | Citation           | Source          | Date      |
| ------ | ---- | ----- | ------------------------------------------ | ------ | ------------------ | --------------- | --------- |
| SG     | A    | hráz  | plot neb hrazy dělati                      | -i     | KolB. 67a          | Gebauer, p. 207 | 1497      |
| SG     | G    | chvíl | od tyech panow, kterzyz gſu te chwyle byli | -e/-ě  | PráZem. Chrest. 1a | Porák p. 157    | ~1400     |
| SG     | N    | díž   | deža, w které se wjno tlači                | -a     | LD 18. st          | HSSJ "dieža"    | 1700-1800 |

Each row represents one attestation of a relevant word.

The attestation is written out in column `Item`, and the lexeme found in the attestation is listed under `Word`, in endingless form found in [`gebauer1960`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml).

The `Number` and `Case` columns identify the function of the form used. The `Ending` column categorises it among one of a few categories, specifying whether it ends in a consonant (`-∅`), has a vowel ending (`-a`, `-e/-ě`, `-i`, `-u`), or a longer ending (e.g. _-ách_ cell left blank).

The `Source` column specifies where the attestation was listed. `Citation` is the original text from which the attestation originates. The `Date` column specifies the attestation date. An exact date is simply represented by the year, an approximate date is preceded by `~`, and a date range is specified by a year range.

#### [Texts](https://github.com/mm-tea/mixed-declension/blob/main/data/texts.csv)

If an attestation comes from [`gebauer1960`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml) or [`porak1979`](https://github.com/mm-tea/mixed-declension/blob/main/bibliography.yaml), the attestation date is not usually listed directly in the same place where it is found. The attestation dates were supplemented by descriptions found elsewhere in these sources, so the page numbers where these can be found are listed here.
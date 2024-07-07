<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: bookshort

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`book`](featuresbynodetype.md#book-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `bookshort` feature provides the abbreviation of the book name as it is used in various tools, such as [Paratext](https://paratext.org/). It allows for concise references and is often used in digital and print formats.

## Feature values

This feature: bookshort | feature: [book](book.md#README) | feature: [num](num.md)
--- | --- | ---
MAT | Matthew | 1
MRK | Mark | 2
LUK | Luke | 3
JHN | John | 4
ACT | Acts | 5
ROM | Romans | 6
1CO | I_Corinthians | 7
2CO | II_Corinthians | 8
GAL | Galatians | 9
EPH | Ephesians | 10
PHP | Philippians | 11
COL | Colossians | 12
1TH | I_Thessalonians | 13
2TH | II_Thessalonians | 14
1TI | I_Timothy | 15
2TI | II_Timothy | 16
TIT | Titus | 17
PHM | Philemon | 18
HEB | Hebrews | 19
JAS | James | 20
1PE | I_Peter | 21
2PE | II_Peter | 22
1JN | I_John | 23
2JN | II_John | 24
3JN | III_John | 25
JUD | Jude | 26
REV | Revelation | 27

## Notes

This value of this feature is identical to the first three characters of feature [ref](ref.md#start).

For mapping to OSIS Book abreviations, see [OSIS Book Abbreviations](https://wiki.crosswire.org/OSIS_Book_Abbreviations).

## Source description

This feature is based upon the XML attribute `id` of the tag `book`.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


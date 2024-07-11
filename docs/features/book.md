<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: book

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `book` feature provides the full name of the book as it is used by the [Bible Online Learner (Bible OL)](https://learner.bible/).

## Feature values

For any node type (and view type):

This feature: book | feature: [bookshort](bookshort.md#readme) | feature: [num](num.md#readme)
--- | --- | ---
Matthew | MAT | 1
Mark | MRK | 2
Luke | LUK | 3
John | JHN | 4
Acts | ACT | 5
Romans | ROM | 6
I_Corinthians | 1CO | 7
II_Corinthians | 2CO | 8
Galatians | GAL | 9
Ephesians | EPH | 10
Philippians | PHP | 11
Colossians | COL | 12
I_Thessalonians | 1TH | 13
II_Thessalonians | 2TH | 14
I_Timothy | 1TI | 15
II_Timothy | 2TI | 16
Titus | TIT | 17
Philemon | PHM | 18
Hebrews | HEB | 19
James | JAS | 20
I_Peter | 1PE | 21
II_Peter | 2PE | 22
I_John | 1JN | 23
II_John | 2JN | 24
III_John | 3JN | 25
Jude | JUD | 26
Revelation | REV | 27

## See also

The feature [num](num.md#readme) for the node type 'book' contains the sequence number of the book within the Greek New Testament corpus.

For mapping to OSIS Book abbreviations, see [OSIS Book Abbreviations](https://wiki.crosswire.org/OSIS_Book_Abbreviations).

## Source description

This feature is based upon the XML attribute `id` of the tag `book`.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: strong

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`integer`](featuresbydatatype.md#integer-datatype) |  [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `strong` feature provides the number of the lexeme according to Strong's numbering system. This system assigns a unique number to each root word in the original biblical languages, facilitating easier reference and study.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

Note from [biblicalhumanities/Nestle1904](https://github.com/biblicalhumanities/Nestle1904/tree/master/morph) regarding absent strong information:
> It is well known that Strong's numbering system is inadequate for describing the full range of lemmas necessary for an accurate description of modern editions such as Nestle's 1904 edition. This is because Strong's numbering system is incomplete: It only contains the lemmas that were extant in the Textus Receptus, whereas the full range of lemmas needed for New Testament lexicography in all editions and manuscripts is not covered in its totaliy by the Strong's numbers.

Note from [biblicalhumanities/Nestle1904](https://github.com/biblicalhumanities/Nestle1904/tree/master/morph) regarding double numbers for this feature:
> The Strong's number. This has one of two formats: Either a single Strong's number in base 10, or two numbers separated by an ampersand (ASCII 0x26, i.e., "&"). In the latter case, the first number is the Strong's number, and the second number is a so-called "Tense Voice Mood" number, or "TVM number". The TVM number was popularized by Dr. Robinson's analyses of various texts, and was probably first used in the Online Bible. The TVM numbers are not further described here, and in any case, the morphological tags should always be consulted over and above the TVM number. No effort has been made to keep the TVM numbers in sync with the morphological tags, nor are TVM numbers always provided for a verb.

## Source description

This feature is derived from the XML attribute `strongs` of the tag `w` (word).

---
##### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

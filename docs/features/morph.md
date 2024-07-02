<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: morhp

Feature group | Feature type | Data type | Available for node types | Used in viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `morph` feature provides the morphological tag according to Sandborg-Petersen morphology. This feature helps in understanding the morphological properties of words, such as their part of speech, tense, mood, voice, case, gender, and number.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

For detailed information, see [biblicalhumanities/Nestle1904/morph/parsing.txt](https://github.com/biblicalhumanities/Nestle1904/blob/master/morph/parsing.txt).

## Source description

This feature is derived from the XML attribute `morph` of the tag `w` (word).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


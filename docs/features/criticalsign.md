<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) | [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: criticalsign

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Textcritical`](featuresbygroup.md#textcritical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description 

The `criticalsign` feature includes text-critical marks found before or after a word.

This feature is also populated for `phrase` or `subphrase` nodes, but only if they consist of just one `word` node.

## Feature values 

Value | Description | Unicode codepoint | Frequency<sup>1</sup>
--- |  --- | --- | ---
`—` | Em Dash | [`&#8212`](https://www.codetable.net/decimal/8212) | 25
`(` |	Left parenthesis | [`&#40`](https://www.codetable.net/decimal/40)| 11
`)` |	Right parenthesis | [`&#41`](https://www.codetable.net/decimal/41)| 11
`[[` | Left square bracket (2x) | [`&#91`](https://www.codetable.net/decimal/91) (2x) | 7
`]]` | Right square bracket (2x) | [`&#93`](https://www.codetable.net/decimal/91) (2x) | 7
`[` |	Left square bracket | [`&#91`](https://www.codetable.net/decimal/91) | 1
`]` |	Right square bracket | [`&#93`](https://www.codetable.net/decimal/93) | 1

<sup>1</sup> Frequency figures are listed for word nodes only. 

## Notes

See also the following related features:
   * [after](after.md#start): All material found after a word.
   * [before](before.md#start): All material found before a word.
   * [punctuation](punctuation.md#start): Punctuations found after a word.
   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [translit](translit.md#start): Transliteration of the word surface texts.
   * [unaccent](unaccent.md#start): word without accents and diacritical markers.
   * [unicode](unicode.md#start): Unicode presentation including all material before and after word.


The following image shows the relation between these features.

<img src="images/details_surface_features.png" width="400" >

## Source description

The `criticalsign` feature is calculated from the XML attribute `unicode` of the `w` (word) tag.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

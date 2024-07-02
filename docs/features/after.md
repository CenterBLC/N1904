<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: after

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description 

The `after` feature includes all material found after a word, such as regular space characters, punctuation marks followed by a space, and text-critical markers. This feature is essential for preserving the context and formatting of the text.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values 

All material found after a word. The frequency is provided by the table below.

Value | Description | Unicode codepoint | Frequency<sup>1</sup>
---  |  --- | --- | ---
`&nbsp` | Space | [`&#32`](https://www.codetable.net/decimal/32)  |  119261
`,&nbsp` | Comma | [`&#44`](https://www.codetable.net/decimal/44) & [`&#32`](https://www.codetable.net/decimal/32)   | 9439
`.&nbsp` | Full stop | [`&#46`](https://www.codetable.net/decimal/46) & [`&#32`](https://www.codetable.net/decimal/32)| 5704
`·&nbsp` | Midle dot | [`&#183`](https://www.codetable.net/decimal/183) & [`&#32`](https://www.codetable.net/decimal/32) | 2355
`;&nbsp` | Semicolon | [`&#59`](https://www.codetable.net/decimal/59) & [`&#32`](https://www.codetable.net/decimal/32) | 969
`,—&nbsp` | Comma, em dash & space | [`&#44`](https://www.codetable.net/decimal/44) & [`&#8212`](https://www.codetable.net/decimal/8212)  & [`&#32`](https://www.codetable.net/decimal/32) | 18
`—&nbsp` | Em dash & space | [`&#8212`](https://www.codetable.net/decimal/8212) & [`&#32`](https://www.codetable.net/decimal/32) | 7
`).&nbsp` | Closing round bracket, full stop & space | [`&#41`](https://www.codetable.net/decimal/41) & [`&#46`](https://www.codetable.net/decimal/46) & [`&#32`](https://www.codetable.net/decimal/32) | 6
`.]]&nbsp` | full stop & 2 Right Square Bracket | [`&#46`](https://www.codetable.net/decimal/46) & 2x [`&#93`](https://www.codetable.net/decimal/93)| 4
etc.. | various | various | another 15

<sup>1</sup> Frequency figures are listed for word nodes only. 

## Notes

See also the following related features:
   * [before](before.md#start): All material found before a word.
   * [criticalsign](criticalsign.md#start): Text-critical signs.
   * [punctuation](punctuation.md#start): Punctuations found after a word.
   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [translit](translit.md#start): Transliteration of the word surface texts.
   * [unaccent](unaccent.md#start): word without accents and diacritical markers.
   * [unicode](unicode.md#start): Unicode presentation including all material before and after word.

The following image shows the relation between these features.

<img src="images/details_surface_features.png" width="400" >

The following [text-formating options](../textformats.md#start) are defined in this dataset using this feature:
<pre>
  A.showFormats()
     format              level    template
     lex-orig-plain      word     {lemma}{punctuation}
     lex-translit-plain  word     {lextranslit}{punctuation}
     text-orig-full      word     {before}{text}{after}
     text-orig-plain     word     {text}{punctuation}
     text-translit-plain word     {translit}{punctuation}
     text-unaccent-plain word     {unaccent}{punctuation}
</pre>
  
## Source description

The `after` feature is based on the XML attribute `after` of the `w` (word) tag.


---
##### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


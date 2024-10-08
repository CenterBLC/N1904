<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: unaccent

Feature group | Feature type | Data type | Available for node types | Used by viewtype
---  | --- | --- | --- | ---
[`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

Surface Greek form of the word in Unicode characters without accents and diacritical markers.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

The following set of features describe the full surface text:
   * [after](after.md#start): All material found after a word (including critical signs).
   * [before](before.md#start): All material found before a word.
   * [criticalsign](criticalsign.md#start): Text-critical signs.
   * [normalized](normalized.md#start): Normalized Greek text.
   * [punctuation](punctuation.md#start): Punctuations found after a word.
   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [trailer](trailer.md#start): all material found after a word (excluding critical signs).
   * [translit](translit.md#start): Transliteration of the word surface texts.
   * unaccent (this feature): Word without accents and diacritical markers.
   * [unicode](unicode.md#start): Unicode presentation including all material before and after word.

The following image shows the relation between these features.

<img src="images/details_surface_features.png" width="400">

The following [text-formating options](../textformats.md#start) are defined in this dataset using this feature:
<pre>
  A.showFormats()
     format              level    template
     lex-orig-plain      word     {lemma}{trailer}
     lex-translit-plain  word     {lextranslit}{trailer}
     text-orig-full      word     {before}{text}{after}
     text-orig-plain     word     {text}{trailer}
     text-translit-plain word     {translit}{trailer}
     text-unaccent-plain word     {unaccent}{trailer}
</pre>
## Source description

Taken from the XML attribute `unicode` of tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

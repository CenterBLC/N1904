<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: lemma

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `lemma` feature represents the lexical lemma according to the Bible Dictionary of Ancient Greek (BDAG) and/or ANLEX by Friberg, Friberg, and Miller. This feature helps in identifying the base form of a word as used in dictionaries.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

When using the [Bible Online Learner (BibleOL)](https://learner.bible/) as an aid in exploring text and creating Text-Fabric queries, it is advisable to use the [bol_lemma](../additions/bol_lemma.md#start) feature instead of this one to circumvent potential issues arising from a slightly different handling of Unicode codepoints.

See also features:
 * [lemmatranslit](lemmatranslit.md#start): Transliteration of the lexical lemma.
 * [variant](variant.md#start): Variant of the lexical lemma based upon [Bible Online Learner (BibleOL)](https://learner.bible/).

And the following [add-on features](../additions/README.md#start):

* [bol_lemma](../additions/bol_lemma.md#start): BibleOL based lexeme.
* [bol_lemma_dict](../additions/bol_lemma_dict.md#start): BibleOL based lexeme as it appears in the dictionary.
* [lemma_dict](../additions/lemma_dict.md#start): Lexeme as it appears in the dictionary.

## Source description

This feature is derived from the XML attribute `lemma` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

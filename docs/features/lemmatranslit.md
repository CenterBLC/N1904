<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: lemmatranslit

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) |  [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `lemmatranslit` feature provides a transliteration of the lexical lemma according to the Bible Dictionary of Ancient Greek (BDAG) and/or ANLEX by Friberg, Friberg, and Miller. This transliteration allows for creation of queries using a Latin keyboard.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

When using the [Bible Online Learner](http://www.dadel.org/) as an aid in exploring text and creating Text-Fabric queries, it is advisable to use the [bol_lemma](bol_lemma.md#start) feature instead of this one to circumvent potential issues arising from a slightly different handling of Unicode codepoints.

See also features:
 * [lemma](lemma.md#start): lexical lemma according to BDAG.
 * [variant](variant.md#start): variant of the lexical lemma.

## Source description

This feature is derived from the XML attribute `lemma` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: variant

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 


## Feature description

The `variant` feature matches the variant of the lemma indicating a different sense, as shown in the [Bible Online Learner](https://learner.bible/). This feature helps identify the specific entry when two entries for a lemma are available (like in case of homonyms or polysemes).

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Value | Description | Frequency
---|---|---
1 | First entry/sense | 36
2 | Second entry/sense | 302

## Notes

The indication of the variant was present in our source data as a  parenthesis and in a Roman numeral indicating the number of the variant (I or II). For instance, the lemma δοῦλος was portrayed in the XML source data as δοῦλος (II). A summary of the variants in the lemmas of the words in the Greek New Testament is shown in the following table:

Lemma | Variant | Occurrence
---|---|---
βάτος | 1 | 5 
βάτος | 2 | 1 
δοῦλος | 2 | 126
λοιμός | 2 | 2 
μήν | 1 | 1
μήν | 2 | 18 
σύνειμι | 1| 2
σύνειμι | 2 | 18
χῶρος |2|1
ἄπειμι | 1| 7
ἄπειμι |2 |1
ἦχος |1 | 3
ἦχος |2 | 1

When using the [Bible Online Learner](http://www.dadel.org/) as an aid in exploring text and creating Text-Fabric queries, it is advisable to use the [bol_lemma](bol_lemma.md#start) feature instead of this one to circumvent potential issues arising from a slightly different handling of Unicode codepoints. More information regarding Unicode can be [found here](../characterencoding.md#start).

See also features:
 * [lemma](lemma.md#start): lexical lemma according to BDAG.
 * [lemmatranslit](lemmatranslit.md#start): transliteration of the lexical lemma.

 And the following [add-on features](..additions/README.md#start):

* [bol_lemma](additions/bol_lemma.md#start): Bible Online Learner (BOL) based lexeme.
* [bol_lemma_dict](additions/bol_lemma_dict.md#start): BOL based lexeme as it appears in the dictionary.
* [lemma_dict](additions/lemma_dict.md#start): Lexeme as it appears in the dictionary.

## Source description

This feature is derived from the XML attribute `lemma` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

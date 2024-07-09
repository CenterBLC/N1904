<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: ln 

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `ln` feature represents the Louw-Nida lexical classification of the semantic domain. This classification helps organize New Testament Greek vocabulary into meaningful categories based on context and meaning.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values:

Value | Description | Frequency<sup>1</sup>
--- | --- | ---
xx.yy  | One or more entries for the Louw-Nida references | 126756
&lt;empty&gt; | Data not provided | 11023

<sup>1</sup> Frequency figures are listed for `word` nodes only. 

## Interpreting the data

The Louw-Nida Lexical Classification, developed by Johannes P. Louw and Eugene A. Nida, categorizes New Testament Greek vocabulary into 93 semantic domains based on meaning and context. This system emphasizes the importance of context in understanding word nuances. Lookup of values for the `ln` feature can be performed in the [Louw-Nida Lexicon](https://www.laparola.net/greco/louwnida.php).

## Notes

See also related feature [domain](domain.md#readme) (Lexical Domain).

## Source description

This feature is derived from the XML attribute `domain` of the tag `w` (word). The word sense data for this feature was compiled by the United Bible Societies MARBLE project. See [Macula-Greek Licence](https://github.com/Clear-Bible/macula-greek/blob/main/LICENSE.md).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

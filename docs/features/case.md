<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: case

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `case` feature indicates the grammatical case for word types such as nouns, pronouns, adjectives, articles, or participles.

This feature is also populated for `phrase` or `subphrase` nodes but only if they consist of just one `word` node.

## Feature values

case | explanation | Frequency<sup>1</sup> 
--- | --- | ---
accusative | Generaly indicating the direct object of a verb | 23031
dative | Generaly indicating indirect object of a verb | 12126
genitive | Generaly indicating possesion | 19515
nominative | Generaly indicating the subject | 24197
vocative | Adressee of speech | 649
'' | empty for any other word type | 58261

<sup>1</sup> Frequency figures are listed for `word` nodes only. 

## Source description

This feature is derived from the XML attribute `case` of the tag `w` (word).

---
##### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


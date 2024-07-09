<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: person

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features)  | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `person` feature indicates the grammatical person of a verb (`word` node with the feature [cls](cls.md#start)=verb). This feature helps in identifying whether the verb is in the first, second, or third person.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`p1` | First person (either singular or plural) | 2943
`p2` | Second person (either singular or plural) | 3729
`p3` | Third person (either singular or plural) | 12747
&lt;empty&gt; | Empty for any wordtypes other than verb | 118360

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`p1` | First person (either singular or plural) | 2886
`p2` | Second person (either singular or plural) | 3447
`p3` | Third person (either singular or plural) | 12474
&lt;empty&gt;  | Empty for any wordtypes other than verb | 50200

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`p1` | First person (either singular or plural) | 2943
`p2` | Second person (either singular or plural) | 3729
`p3` | Third person (either singular or plural) | 12747
&lt;empty&gt;  | Empty for any wordtypes other than verb | 115566

## Note

See also related feature [number](number.md).

## Source description

This feature is derived from the XML attribute `person` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


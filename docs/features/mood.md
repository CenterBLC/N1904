<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: mood

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) |  [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `mood` feature indicates the grammatical mood of a verb (`word` node with feature [cls](cls.md#start)=verb). This feature helps in understanding the mode of action expressed by the verb, whether it's a command, a statement of fact, a possibility, etc.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values 

mood | Comment | Frequency<sup>1</sup>
--- | --- | ---
`imperative` | expresses a command | 1877
`indicative` | expresses an action being portrayed as real | 15617
`infinitive` | (pseudo mood) | 2285
`participle` | (pseudo mood) | 6653
`optative` | expresses something is possible | 69
`subjunctive` | expresses a probable or desired action | 1856
` ` | Any other wordtype | 109422

<sup>1</sup> Frequency figures are listed for word nodes only. 

## Source description

This feature is derived from the (optional) XML attribute `mood` of the tag `w` (word).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: rela

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `rela` feature specifies the apposition details of a node, indicating whether the entity forms an apposition. An apposition is a grammatical construction where two elements, typically noun phrases, are placed side by side, with one element serving to define or modify the other.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values 

Value | Description | Frequency
---  | --- | --- 
` ` |  This entity forms no apposition | 
`Appo` | This entity forms an apposition | 1958

## Note

The following image presents a nested apposition demonstrating this feature and the related feature [appositioncontainer](appositioncontainer.md#start).

<img src="images/appositioncontainer.png" width="600">

## Source description

Taken from the optional XML attribute `appositioncontainer` of the tag `wg` (wordgroup).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

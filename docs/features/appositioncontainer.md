<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT -  Feature: appositioncontainer

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`integer`](featuresbydatatype.md#integer-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description 

The `appositioncontainer` feature indicates whether a word group or phrase contains an apposition. An apposition is a grammatical construction where two elements, typically noun phrases, are placed side by side, with one element serving to define or modify the other.

## Feature values 

Frequency for nodetype [`wg`](featuresbynodetype.md#wordgroup-nodes) (used in [`wg-view`](../wg-view.md#start)):
Value | Description | Frequency
---  | --- | --- 
` ` | this word group contains no appositioncontainer | -
`1` | this word group contains an appositioncontainer | 1908


Frequency for nodetype [`phrase`](featuresbynodetype.md#phrase-nodes) (used in [`syntax-view`](../syntactic-view.md#start)):
Value | Description | Frequency
---  | --- | --- 
` ` | this phrase contains no appositioncontainer | -
`1` | this phrase contains an appositioncontainer | 715


Frequency for nodetype [`subphrase`](featuresbynodetype.md#subphrase-nodes) (used in [`syntax-view`](../syntactic-view.md#start)):
Value | Description | Frequency
---  | --- | --- 
` ` | this subphrase contains no appositioncontainer | -
`1` | this subphrase contains an appositioncontainer | 1908

## Note

The following image presents a nested apposition demonstrating this feature and the related feature [rela](rela.md#readme).

<img src="images/appositioncontainer.png" width="600">

## Source description

This feature is derived from the (optional) XML attribute `appositioncontainer` of tag `wg` (wordgroup).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

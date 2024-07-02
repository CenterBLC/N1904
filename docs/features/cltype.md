<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: cltype

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`clause`](featuresbynodetype.md#clause-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

The `cltype` feature provides classification for different types of clauses, specifically focusing on verbless, verb-elided, and minor clauses.

## Feature values

Frequency for [sentence](featurebynodetype.md#sentence-nodes) nodes:
value | description | Frequency
---  | --- | --- 
`Verbless` | Verbless clause type| 77
`VerbElided` |  Verb-elided clause type | 47
`Minor` |  Minor clause type | 1

Frequency for [`clause`](featuresbynodetype.md#clause-nodes) nodes:
value | description | Frequency
---  | --- | --- 
`Verbless` | Verbless clause type| 1003
`VerbElided` |  Verb-elided clause type | 884
`Minor` |  Minor clause type | 831

Frequency for [`wg`](featuresbynodetype.md#wordgroup-nodes) nodes:

value | description | Frequency
---  | --- | --- 
`Verbless` | Verbless clause type| 1050
`VerbElided` |  Verb-elided clause type | 961
`Minor` |  Minor clause type | 832

## Source description

This feature is derived from the XML attribute `cltype` of the tag `wg` (wordgroup).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

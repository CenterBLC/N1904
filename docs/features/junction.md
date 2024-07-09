<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: junction

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `junction` feature indicates details about coordinating and subordinating clauses in the Nestle 1904 Greek New Testament. This feature helps in understanding the syntactic structure of the text.

## Feature values 

For [`sentence`](featuresbynodetype.md#sentence-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
---  | --- | --- 
`coordinate` | Coordinate | 1117
`subordinate` |  Subordinate | 989
&lt;empty&gt;  | Not applicable | 17597

For [`clause`](featuresbynodetype.md#clause-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
---  | --- | --- 
`coordinate` | Coordinate | 8186
`subordinate` |  Subordinate | 7449
&lt;empty&gt;  | Not applicable | 15179

For [`wg`](featuresbynodetype.md#wordgroup-nodes) nodes (used in [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
---  | --- | --- 
`coordinate` | Coordinate | 9367
`subordinate` |  Subordinate | 8554
&lt;empty&gt;  | Not applicable | 88947

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
---  | --- | --- 
`subordinate` |  Subordinate | 57
&lt;empty&gt;  | Not applicable | 68950

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
---  | --- | --- 
`subordinate` |  Subordinate | 116
`coordinate` | Coordinate | 64
&lt;empty&gt;  | Not applicable | 116055

## Note

See also the related feature [crule](crule.md).

## Source description

The `junction` feature is derived from the optional XML attribute `junction` of the `wg` (wordgroup) tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

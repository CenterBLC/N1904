<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: junction

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `junction` feature indicates details about coordinating and subordinating clauses in the Nestle 1904 Greek New Testament. This feature helps in understanding the syntactic structure of the text.

## Feature values 

Frequency for nodetype `sentence`:

value | description | Frequency
---  | --- | --- 
`coordinate` | coordinate | 1117
`subordinate` |  subordinate | 989
`&nbsp`  | empty | 

Frequency for nodetype `clause`:

value | description | Frequency
---  | --- | --- 
`coordinate` | coordinate | 8186
`subordinate` |  subordinate | 7449
`&nbsp`  | empty | 

Frequency for nodetype `wg`:

value | description | Frequency
---  | --- | --- 
`coordinate` | coordinate | 9367
`subordinate` |  subordinate | 8554
`&nbsp`  | empty | 

Frequency for nodetype `phrase`:

value | description | Frequency
---  | --- | --- 
`subordinate` |  subordinate | 57
`&nbsp`  | empty | 

Frequency for nodetype `subphrase`:

value | description | Frequency
---  | --- | --- 
`subordinate` |  subordinate | 116
`coordinate` | coordinate | 64
`&nbsp`  | empty | 


## Note

See also the related feature [crule](crule.md).

## Source description

The `junction` feature is derived from the optional XML attribute `junction` of the `wg` (wordgroup) tag.

---
##### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

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
` `  | empty | 

Frequency for nodetype `clause`:

value | description | Frequency
---  | --- | --- 
`coordinate` | coordinate | 8186
`subordinate` |  subordinate | 7449
` `  | empty | 

Frequency for nodetype `wg`:

value | description | Frequency
---  | --- | --- 
`coordinate` | coordinate | 9367
`subordinate` |  subordinate | 8554
` `  | empty | 

Frequency for nodetype `phrase`:

value | description | Frequency
---  | --- | --- 
`subordinate` |  subordinate | 57
` `  | empty | 

Frequency for nodetype `subphrase`:

value | description | Frequency
---  | --- | --- 
`subordinate` |  subordinate | 116
`coordinate` | coordinate | 64
` `  | empty | 


## Note

See also the related feature [crule](crule.md).

## Source description

The `junction` feature is derived from the optional XML attribute `junction` of the `wg` (wordgroup) tag.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

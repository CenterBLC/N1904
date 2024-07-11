<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: clausetype

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features)  | [`String`](featuresbydatatype.md#string-datatype) | [`clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `clausetype` feature provides information about the type of clauses within the a sentence.

## Feature values

Frequency for [`sentence`](featuresbynodetype.md#sentence-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and [`wg-view`](../wg-view.md#start)): 

Value | description | Occurences
--- | --- | ---
nominalized | | 59
&lt;empty&gt; | | 19644

Frequency for  [`clause`](featuresbynodetype.md#clause-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | description | Occurences
--- | --- | ---
nominalized | | 5237
&lt;empty&gt; | | 25577

Frequency for [`wg`](featurebynodetype.md#wordgroup-nodes) nodes (used in [`wg-view`](../wg-view.md#start)):

Value | description | Occurences
--- | --- | ---
nominalized | | 5296
&lt;empty&gt; | | 101572 

## Notes

To find all sentence which are not nominalized, use the following snippet:

```python
Query = '''
sentence 
   clausetype#nominalized
'''
Results = A.search(Query)
```

## Source description

This feature is derived from the XML attribute `clauseType` of the tag `wg` (wordgroup).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: gender

Feature group |Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

The `gender` feature indicates the grammatical gender for word types such as nouns, adjectives, pronouns, participles, and definite articles. This feature helps in understanding the gender-based grammatical rules applied to these word types.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
--- | --- | --- 
masculine | Grammatical gender is masculine | 41486
feminine | Grammatical gender is feminine | 18736
neuter | Grammatical gender is neuter | 13753
&lt;empty&gt; | Empty for any other wordtype | 63804

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | --- 
masculine | Grammatical gender is masculine | 12430
neuter | Grammatical gender is neuter | 3066
feminine | Grammatical gender is feminine | 2162
&lt;empty&gt; | Empty for any other wordtype | 51349

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | --- 
masculine | Grammatical gender is masculine | 41486
feminine | Grammatical gender is feminine | 18736
neuter | Grammatical gender is neuter | 13753
&lt;empty&gt; | Empty for any other wordtype | 63804

## Source description

This feature is derived from the XML attribute `gender` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

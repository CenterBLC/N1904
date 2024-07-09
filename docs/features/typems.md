<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: typems

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 
[`Syntactical`](featuresbygroup.md#syntactical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`group`](featuresbynodetype.md#group-nodes)  [`clause`](featuresbynodetype.md#clause-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

This feature provides details regarding the type. For word nodes, this information is related to morphology (hence the 'm' in the feature name), indicating the type of noun or pronoun. For other node types, it provides details on the syntactical type (the 's' in the feature name).

## Feature values

Frequency for nodetype `word`:

Value | Description | Frequency
---- | ---- | ---
common | Designating objects (not specific) | 23644
personal | Designating specific person/objects (e.g. εγώ, εσύ, etc.) | 11521
proper | Name of a person, place, thing, etc. | 4639
demonstrative | Indicates a specific object ([examples](https://ugg.readthedocs.io/en/latest/determiner_demonstrative.html)) | 1722
relative | Introduces relative clauses | 1674
interrogative | Introduces a question ([examples](https://ugg.readthedocs.io/en/latest/determiner_interrogative.html)) | 633
indefinite | Refering to nonspecific people or things | 552
possessive | Indicating ownership or possession | 70
adverbial | Adverbs functioning similarly to pronouns | 3
'' | Empty for wordtypes other than noun or pronoun | 93321

Frequency for nodetype `wg` (wordgroup):

Value | Description | Frequency
---- | ---- | ---
modifier-scope | | 29645 
wrapper-clause-scope | | 12166 
wrapper-scope	| | 11264 
conjuncted-wg | | 8075
group | | 4957 
modifier-clause-scope | | 1712
apposition-group | | 891

Frequency for nodetype `sentence`:

Value | Description | Frequency
---- | ---- | ---
wrapper-clause-scope	|| 12039
group	|| 2525
apposition-group ||	1

Frequency for nodetype `group`:

Value | Description | Frequency
---- | ---- | ---
conjuncted-wg ||	8075
apposition-group ||	889

Frequency for nodetype `clause`:

Value | Description | Frequency
---- | ---- | ---
wrapper-clause-scope ||	127
group	|| 43
apposition-group || 1

## Source description

Based upon XML attribute `type` of tag `w` (word) and tag `wg` (wordgroup).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: type

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 
[`Syntactical`](featuresbygroup.md#syntactical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype)  | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`group`](featuresbynodetype.md#group-nodes)  [`clause`](featuresbynodetype.md#clause-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

For `word` nodes: Gramatical type of noun or pronoun. For all other nodes: syntactical type.

## Feature values

Frequency for nodetype `word`:

Value | Description | Frequency
---- | ---- | ---
adverbial |  | 3
common | objects | 23644
demonstrative | Indicate a specific object ([examples](https://ugg.readthedocs.io/en/latest/determiner_demonstrative.html)) | 1722
indefinite | | 552
interrogative |  Introduces a question ([examples](https://ugg.readthedocs.io/en/latest/determiner_interrogative.html)) | 633
personal | Pronoun designating a person (e.g. εγώ, εσύ, etc.) | 11521
possessive | | 70
proper | Name of a person, place, thing, etc. | 4639
relative |  | 1674
'' | Empty for wordtypes other than noun or pronoun | 93321

Frequency for nodetype `wg` (wordgroup):

Value | Description | Frequency
---- | ---- | ---
apposition-group | | 891
conjuncted-wg | | 8075
group | | 4957 
modifier-clause-scope | | 1712
modifier-scope | | 29645x 
wrapper-clause-scope | | 12166 
wrapper-scope	| | 11264 

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
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

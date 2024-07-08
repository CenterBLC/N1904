<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: typ

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactical`](featuresbygroup.md#syntactical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes)  | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

This feature provides provides syntactic labels for textual elements like words and wordgroups based upon their syntactical functions and structures. This includes distinguishing between nominal phrases, prepositional phrases, verbal phrases, adjectival phrases, adverbial phrases, conjuncted phrases, and appositions, which are fundamental to interpreting the [syntaxtrees](syntaxtrees.md#start).

## Feature values

Frequency for nodetype `group`:

Value | Description | Frequency
---- | ---- | ---
conjuncted | |	8075
apposition | |	889

Frequency for nodetype `wg`:

Value | Description | Frequency
---- | ---- | ---
NP	| nominal phrase | 30911
PP	| prepositional phrase | 11169
conjuncted	|| 8075
apposition	|| 889
VP	| verbal phrase | 207
AdjP | adjectival phrase |168
AdvP | adverbial phrase |166

Frequency for nodetype `phrase`:

Value | Description | Frequency
---- | ---- | ---
NP | nominal phrase | 10935
PP | prepositional phrase | 9609
AdvP | adverbial phrase |	154
AdjP | adjectival phrase |	60
VP | verbal phrase | 10

Frequency for nodetype `subphrase`:

Value | Description | Frequency
---- | ---- | ---
NP | nominal phrase | 30911
PP | prepositional phrase| 11169
VP | verbal phrase | 207
AdjP | adjectival phrase | 168
AdvP | adverbial phrase | 166

## Source description

Taken from the XML attribute `typ` of tag `w` (word) and tag `wg` (wordgroup).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


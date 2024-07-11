<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: voice

Feature group |Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 
 
## Feature description

The `voice` feature indicates the grammatical voice of a verb (`word` node with feature [cls](cls.md#start)=verb). This feature helps in identifying whether the subject of the verb is performing the action or receiving it.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Value | Description | Frequency<sup>1</sup>
--- | --- | ---
active | Sentences subject is agent of the verb's action | 20742
middle | Sentences subject is both agent and affected by the verb's action | 2408
middlePassive | | 1714
passive | The subject of the verb is being acted upon | 3493
'' | Empty for wordtypes other than verbs | 109422

<sup>1</sup> Frequency figures are listed for word nodes only. 

## Notes

The Bible Online Learner dataset contians additional details regarding verb types.

The following features provide ready access to eight morphological properties:

 - [person](person.md#start): gramatical person
 - [tense](tense.md#start): gramatical tense of the verb
 - [voice](voice.md#start): Gramatical voice of the verb
 - [mood](mood.md#start): gramatical mood of a verb
 - [case](case.md#start): gramatical case
 - [number](number.md#start): gramatical number
 - [gender](gender.md#start): gramatical gender
 - [degree](degree.md#start): indicates comparative or superlative adjective

The feature [morph](morph.md#start) provides the morphological tag, which condenses various details such as part of speech and the above listed morphological characteristics.

## Source description

This feature is derived from the XML attribute `voice` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: tense

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `tense` feature indicates the grammatical tense of a verb (`word` node with feature [cls](cls.md#start)=verb). This feature helps in identifying the time frame of the action described by the verb, such as past, present, or future.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Value | Explanation | Frequency
--- | --- | ---
aorist | Describing a simple action in the past | 11803
imperfect | Describing an ongoing action in the past | 1689
perfect | Describing a completed action in the present time | 1572
pluperfect | Describing a completed action in the past | 88
present | Describing an ongoing action in the present time | 11579
future | Describing a simple or ongoing action in the future | 1626
&lt;empty&gt; | Empty for any wordtype other than a verb | 109422

## Note

The 'future perfect' tense (describing a completed action in the future) is not found in the text.

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

Based on the optional XML attribute `tense` of tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

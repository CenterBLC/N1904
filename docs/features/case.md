<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: case

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `case` feature indicates the grammatical case for word types such as nouns, pronouns, adjectives, articles, or participles.

This feature is also populated for `phrase` or `subphrase` nodes but only if they consist of just one `word` node.

## Feature values

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`nominative` | Generaly indicating the subject | 24197
`accusative` | Generaly indicating the direct object of a verb | 23031
`genitive` | Generaly indicating possesion | 19515
`dative` | Generaly indicating indirect object of a verb | 12126
`vocative` | Adressee of speech | 649
&lt;empty&gt; | empty for any other word type | 58261

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`nominative` | Generaly indicating the subject | 24197
`accusative` | Generaly indicating the direct object of a verb | 23031
`genitive` | Generaly indicating possesion | 19515
`dative` | Generaly indicating indirect object of a verb | 12126
`vocative` | Adressee of speech | 649
&lt;empty&gt; | empty for any other word type | 57113

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`nominative` | Generaly indicating the subject | 9609
`accusative` | Generaly indicating the direct object of a verb | 6170
`dative` | Generaly indicating indirect object of a verb | 3265
`genitive` | Generaly indicating possesion | 1408
`vocative` | Adressee of speech | 1
&lt;empty&gt; | empty for any other word type | 48554

## Notes

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

This feature is derived from the XML attribute `case` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


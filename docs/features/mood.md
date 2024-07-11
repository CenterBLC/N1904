<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: mood

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `mood` feature indicates the grammatical mood of a verb (`word` node with feature [cls](cls.md#start)=verb). This feature helps in understanding the mode of action expressed by the verb, whether it's a command, a statement of fact, a possibility, etc.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values 

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`indicative` | Indicative (expresses an action being portrayed as real) | 15617
`participle` | Participle (pseudo mood) | 6653
`infinitive` | Infinitive (pseudo mood) | 2285
`imperative` | Imperative (expresses a command) | 1877
`subjunctive` | Subjunctive (expresses a probable or desired action) | 1856
`optative` | Optative (expresses something is possible) | 69
&lt;empty&gt; | Any other wordtype than a verb | 109422

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`indicative` | Indicative (expresses an action being portrayed as real) | 15617
`participle` | Participle (pseudo mood) | 6653
`infinitive` | Infinitive (pseudo mood) | 2285
`imperative` | Imperative (expresses a command) | 1877
`subjunctive` | Subjunctive (expresses a probable or desired action) | 1856
`optative` | Optative (expresses something is possible) | 69
&lt;empty&gt; | Any other wordtype than a verb | 115176

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
`indicative` | Indicative (expresses an action being portrayed as real) | 15245
`participle` | Participle (pseudo mood) | 6320
`infinitive` | Infinitive (pseudo mood) | 2228
`subjunctive` | Subjunctive (expresses a probable or desired action) | 1832
`imperative` | Imperative (expresses a command) | 1663
`optative` | Optative (expresses something is possible) | 67
&lt;empty&gt; | Any other wordtype than a verb | 41652

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

This feature is derived from the (optional) XML attribute `mood` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


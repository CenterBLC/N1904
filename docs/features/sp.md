<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: sp

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)| [`syntax-view`](../syntax-view.md#start)

## Description

The `sp` feature provides the part-of-speech (POS), which classifies words based on their function in a sentence.

This feature mimicks BHSA nomenclature for feature function and is designed to be used in the [`syntax-view`](../syntax-view.md#start).

## Feature Values

Frequency for [phrase](featuresbynodetype.md#phrase-nodes) nodes:

Value | Description | Frequency
--- | --- | ---
`verb`| Verb |27355
`pron`| Pronoun |8751
`advb`| Adverbial |4384
`subs`| Substantive|2822
`adjv`| Adjective |2304
`art`| Article |257
`intj`| Interjection |90
`conj`|Conjunction|85
`num`| Number |25
`prep`| Preposition |4

Frequency for nodetype [subphrase](featuresbynodetype.md#subphrase-nodes):

Value | Description | Frequency
--- | --- | ---
`subs`| Substantive |28455
`verb`| Verb |28357
`art`| Article |19786
`conj`| Conjunction |18227
`pron`| Pronoun |16177
`prep`| Preposition |10914
`adjv`| Adjective |8452
`advb`| Adverbial |6147
`intj`|Interjection |788
`num`| Number |476


Frequency for [word](featuresbynodetype.md#word-nodes) nodes:

Value | Description | Frequency
--- | --- | ---
`subs`| Substantive |28455
`verb`| Verb |28357
`art`| Article |19786
`conj`| Conjunctio |18227
`pron`| Pronoun |16177
`prep`| Preposition |10914
`adjv`| Adjective |8452
`advb`| Adverbial |6147
`intj`| Interjection |788
`num`| Number |476

## See also

The matching feature for use in the [`wg-view`](../wg-view.md#start) is [cls](cls.md#start).
 
## Source description

The `sp` feature is based on the modified XML attribute `cls` of the `wg` tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

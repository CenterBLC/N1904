<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: number

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `number` feature indicates the grammatical number of any `word` node with the feature [cls](cls.md#start) set to a verb, noun, determiner, adjective, or pronoun. This feature helps in identifying whether the word is in singular or plural form.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start)):

Value | Description | Frequency
--- | --- | ---
singular | Singular form (either first, second, or third person) | 69846
plural | Plural form (either first, second, or third person) | 29091
&lt;empty&gt; | Empty for wordtypes without number  | 38842

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
singular | Singular form (either first, second, or third person) | 26293
plural | Plural form (either first, second, or third person) | 12967
&lt;empty&gt; | Empty for wordtypes without number  | 29747

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Frequency
--- | --- | ---
singular | Singular form (either first, second, or third person) | 69846
plural | Plural form (either first, second, or third person) | 29091
&lt;empty&gt; | Empty for wordtypes without number  | 56501

## Note

See also the related feature [person](person.md) available for `word` node where feature [cls](cls.md#start)=verb).

## Source description

This feature is derived from the XML attribute `number` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


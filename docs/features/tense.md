<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: tense

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

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
'' | Empty for any wordtype other than a verb | 109422

## Note

The 'future perfect' tense (describing a completed action in the future) is not found in the text.

## Source description

Based on the optional XML attribute `tense` of tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

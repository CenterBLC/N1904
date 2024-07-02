<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: referent

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features)  | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `referent` feature stores information about the entity (usually a pronoun) to which the current node refers. The value of the referent often crosses sentence and verse boundaries and is, to a certain extent, more of a discourse feature than a syntactic one.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

The [id](id.md#start) of the referent according to the following format:

```
An 'n' followed by a 11-digit unique id in the format
    BBCCCVVVWWW
    BB          => zero-padded book, NT starts at 40
      CCC       => zero-padded chapter
         VVV    => zero-padded verse
            WWW => zero-padded word index (instance within the verse)
```

## Notes

The following image demonstrates how feature `referent` links back to [`id`](id.md#start). In this example the ὑμῖν and ἡμῶν in Philippians 1:2 refers back to the ἁγίοις in verse 1:

<img src="images/referent.png" width="650">

See also the following related features:
   * [framespec](framespec.md#start): Reference to the id of subject, object or idirect object.
   * [frame](frame.md#start): Edge feature that links nodes that are part of the frame; labelled as A0, A1, etc.
   * [id](id.md#start): A uniqe identifier for each individual word in the corpus.
   * [subjrefspec](subjrefspec.md#start): Subject reference to a node id.
 

## Source description

This feature is derived from the optional XML tag `referent` of node `w`. Annotation data originates from [Clear Bible](https://github.com/Clear-Bible/macula-greek/tree/main/sources/Clear/annotations).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

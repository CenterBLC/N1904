<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: id

Feature group | Feature type | Data type | Available for node types | Used by viewtype
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

This feature provides a unique identifier for each individual word in the corpus.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

The `id` is formatted as follows:

```
The letter 'n' (node) followed by a 11-digit unique id in the format

    BBCCCVVVWWW
    BB          => zero-padded book, the first NT book (Matthew) starts at 40
      CCC       => zero-padded chapter
         VVV    => zero-padded verse
            WWW => zero-padded word index (instance within the verse)
```

## Notes

The feature [`ref`](ref.md#start) contains identical information as the feature `id`, albeit in a different format.

A related feature, which references not individual words but word groups, clauses, and sentences, is [`nodeid`](nodeid.md#start).

## Source description

The ID is derived from the XML attribute `xml:id` of the `w` (word) node. When loading the XML source in Python note that the the xml:id attribute is part of an XML namespace, so it should be referenced in the code using [{http://www.w3.org/XML/1998/namespace}id](https://www.w3.org/TR/xml-id/).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

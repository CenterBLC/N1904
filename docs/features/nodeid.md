<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: nodeid 

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `nodeid` feature provides a reference to the range of words inside a word group, clause, or sentence within the text.

## Feature values

A string formated like `400010200010490` which can be decoded as:
```
    400010200010490
    BBCCCVVVWWWSSSL
    BB               => zero-padded book number, the first NT book (Matthew) starts at 40
      CCC            => zero-padded chapter
         VVV         => zero-padded verse
            WWW      => Beginning position (the Nth word) of a node/sub-tree
               SSS   => The SPAN of a node (how many words it covers)
                  L  => (Level) distinguishes nodes which have the same span (in cases of non-branching nodes)
```

## Notes

A related feature, albeit referencing individual word nodes, is [id](id.md#start).

## Source description

The ID is derived from the numeric part of the optional XML attribute `nodeId` of the `wg` (WordGroup) node.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


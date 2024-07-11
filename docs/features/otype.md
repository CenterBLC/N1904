<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: otype

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`clause`](featuresbynodetype.md#clause-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

This feature, known as "object type" (otype), categorizes various types of textual objects within the corpus. In Text-Fabric, all objects are represented by nodes, each assigned an object type label. It associate higher-level objects (like sentences or phrases) with their constituent lower-level objects (like words). When querying or analyzing the text, you can specify the otype to focus on particular node types, corresponding to different levels of the text structure.

## Feature values

Node names (word, wg, sentence, verse, chapter, book, phrase, subphrase, group, clause).

## Notes

The two main usages of this feature are:

Generating a list of nodes of a certain type, e.g. `verse` nodes:

```python
for verse in F.otype.s('verse'):
    "do something with verse nodes"
```
To determine the node type of a node id, for example node=1 (the first word of Matt. 1:1), the following snippet can be used: 
 
```python
F.otype.v(1)   # the node for the first word in Matt. 1:1
'word'         # result is the node type
```

For a more comprehensice list of usages for feature otype, see the [documentation on special node feature otype](https://annotation.github.io/text-fabric/tf/cheatsheet.html#special-node-feature-otype).

The information on which object occupies a specific slot is stored in the edge feature [oslots](oslots.md).

## Source description

The data for this feature is calculated during creation of the Text-Fabric dataset.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: oslots

Feature group | Feature type |  Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Warp`](featuresbygroup.md#warp-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`Sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`Book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`Group`](featuresbynodetype.md#group-nodes) [`Clause`](featuresbynodetype.md#clause-nodes) |  [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `oslots` feature represents the set of slots associated with an object. Every object corresponds to exactly one slot set, which is the set of word occurrences that form the textual representation of that object. Each word fills a slot, and each slot has a unique sequence number. Earlier words have lower numbers than later words. An object does not have to be consecutive; it may be interrupted at any place. Different objects may or may not overlap.

The slot set is given as a comma-separated list of slot ranges. A range has the form *n* - *m*, where *n* is a number smaller than or equal to *m*. The range *n* - *n* may be abbreviated to *n*.

## Note

The value of this feature for word objects is always just one number: the number of the slot the word occupies. All word occurrences are numbered from 1 to 137779 in the order they occur in the Greek New Testament.

A typical useage of this feature is provided by the following snippet showing nodes associated with node #382714 (= verse node for Matt. 1:1):

```python
E.oslots.s(382714)                     # verse Matt. 1:1
array('I', [1, 2, 3, 4, 5, 6, 7, 8])   # result: the word nodes for this verse
```

For a more comprehensice list of usages for feature otype, see the [documentation on special node feature oslots](https://annotation.github.io/text-fabric/tf/cheatsheet.html#special-edge-feature-oslots).

## Source description

The data for this feature is calculated during creation of the Text-Fabric dataset.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


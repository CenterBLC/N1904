<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: oslots

Feature group | Feature type |  Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`string`](featuresbydatatype.md#string-datatype)  | *not applicable* |  [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)


## Feature description 

The `oslots` feature represents the set of slots associated with an object. Every object corresponds to exactly one slot set, which is the set of word occurrences that form the textual representation of that object. Each word fills a slot, and each slot has a unique sequence number. Earlier words have lower numbers than later words. An object does not have to be consecutive; it may be interrupted at any place. Different objects may or may not overlap.

The slot set is given as a comma-separated list of slot ranges. A range has the form *n* `-` *m*, where *n* is a number smaller than or equal to *m*. The range *n* `-` *n* may be abbreviated to *n*.

##### Note
The value of this feature for word objects is always just one number: the number of the slot the word occupies. All word occurrences are numbered from 1 to 137779 in the order they occur in the Greek New Testament.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


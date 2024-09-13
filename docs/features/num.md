<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: num

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | ---  | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype)  | [`book`](featuresbynodetype.md#book-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)    [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

This feature provides the sequential number for the various node type. The context depends on the node type (see next section).

## Feature values

For node type:
  * [`book`](featuresbynodetype.md#book-nodes): Sequence within the Greek New Testament corpus (Matthew=1, Mark=2, ..., Revelation=27)
  * [`sentence`](featuresbynodetype.md#sentence-nodes): Sentence sequence number within a book.
  * [`group`](featuresbynodetype.md#group-nodes): Group sequence number within a book.
  * [`clause`](featuresbynodetype.md#clause-nodes): Clause sequence number within a book.
  * [`phrase`](featuresbynodetype.md#phrase-nodes): Phrase sequence number within a book.
  * [`subphrase`](featuresbynodetype.md#subphrase-nodes): Subphrase sequence number within a book.
  * [`word`](featuresbynodetype.md#word-nodes): Word numbered inside the verse (matching the last part of feature [ref](ref.md)).

## Notes

To determine the sequence number of a word inside a sentence, the following snippet can be used: 

```python
    # the node number of the word is stored in wordNode
    wordNode=32048  # first word of Luke 3:24
    sentenceNode=L.u(wordNode,otype='sentence') # returns a tuple
    E.oslots.s(sentenceNode[0]).index(wordNode)
```
Running this code returns `7`. Since the index starts with zero, this means this word is the eigth one in the verse.

To find the sequence number inside a book, use the following snippet:

```python
    # the node number of the word is stored in wordNode
    wordNode=29588   # first word of Luke 1:2
    sentenceNode=L.u(wordNode,otype='book') # returns a tuple
    E.oslots.s(sentenceNode[0]).index(wordNode)
```
This returns `11` since this is the 12th word in the Gospel of Luke.

## Source description

The num feature is calculated and not present in the source XML data, but derived from the structure of the  corpus and is calculated based on the sequence of elements.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


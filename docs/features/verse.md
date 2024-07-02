<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: verse 

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`integer`](featuresbydatatype.md#integer-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`verse`](featuresbynodetype.md#verse-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

This feature indicates the verse number within a chapter.

## Feature value

The value of this feature is an integer representing the verse number.

## Notes

When using verse numbers inside a script, it is not save to assume verse number within a chapter are sequential without gaps. The folling is a list of 'missing' verses: Matthew 17:21; 18:1;  23:14, Mark 7:16;  9:44&46; 11:26; 15:28, Luke 17:36;  23:17,  Acts 8:37; 15:34;  24:7;  28:29,  Romans 16:24, and a 'gap' after Mark 16:20 until verse 99.

The `sentence` nodes do not have a `verse` feature since sentences can span multiple verses. To map a sentence to the verse it starts in, use the following Python code snippet:

```python
    # node number of the sentence is stored in variable 'sentence'
    firstNode=E.oslots.s(sentence)[0]
    bookName=F.book.v(firstNode)
    chapterNumber=F.chapter.v(firstNode)
    verseNummber=F.verse.v(firstNode)
```

## Source description

This feature is calculated from the XML attribute `ref` of the `w` (word) tag.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

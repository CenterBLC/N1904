<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: chapter

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- |---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`verse`](featuresbynodetype.md#verse-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description  

This feature indicates the chapter number within a book.

## Feature values

An integer.

## Notes

Not all nodetypes provide this feature. To determine the chapter for nodetypes `sentence`, `wg`, `phrase`, `subphrase`, or `group`, the following snippet can be used.

```python
    # the node number of the wordgroup is stored in wgNode
    wgNode=390658   # this is a wg in Matt. 1:1
    chapterNode=L.u(wgNode,otype='chapter')[0]  # returns a tuple
    chapter=F.chapter.v(chapterNode)
    print (chapter) # Output: 1
```

This snippet returns 1 as the value for the chapter feature.

## Source description

The chapter information is calculated from the XML attribute ref of the w (word) tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


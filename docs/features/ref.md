<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: ref

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `ref` feature provides a unique identifier for each individual word in the corpus.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

A compound string indicating book, chapter, verse and sequence number of the word *inside the verse* formatted as follows:

<pre>
  MAT 1:2!11
</pre>

This format consists of:
- **Book**: The first three characters (e.g., `MAT` for Matthew), matching the value of feature [bookshort](bookshort.md#start) for each `book` node.
- **Chapter**: Following the book, the chapter number (e.g., `1`)
- **Verse**: Following the chapter, the verse number (e.g., `2`)
- **Word Sequence Number**: This is the part after the `!` symbol, which is the word sequence number within a verse (in this example `11`), matching the value of feature [num](num.md#start) for each `word` node.

### Example

To extract all components in this feature using Python, the following code snippet can be used:

```python
    ref = "MAT 1:2!11" # example content
    # Regular expression pattern to match the book, chapter, verse, and position of the word in the verse
    pattern = r"(\w+)\s(\d+):(\d+)!(\d+)"
    # Using re.match to extract the parts based on the pattern
    match = re.match(pattern, ref)
    book, chapter, verse, positionInVerse = match.groups()
```

## Notes

This first three characters of this feature value are identical to the feature [bookshort](bookshort.md#start).

The feature [`id`](id.md#start) contains identical information as the feature `ref`, albeit in a different format.

## Source description

The identifier is based on the XML attribute ref of the w (word) tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

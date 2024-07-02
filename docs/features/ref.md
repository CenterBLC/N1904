<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: ref

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `ref` feature provides a unique identifier for each individual word in the corpus.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

A compound string indicating book (following the format of feature [bookshort](bookshort.md#start)), chapter, verse and sequence number of the word *inside the verse* formatted as follows:

<pre>
  MAT 1:2!11
</pre>

This format consists of:
- **Book**: The first three characters (e.g., `MAT` for Matthew)
- **Chapter**: Following the book, the chapter number (e.g., `1`)
- **Verse**: Following the chapter, the verse number (e.g., `2`)
- **Word Sequence Number**: After the `!` symbol, the word sequence number within the verse (e.g., `11`)

### Example

To extract the word sequence number from the identifier `MAT 1:2!11`, use the following Python code:

```python
<pre>
ref = "MAT 1:2!11"
print ('word sequence number: ', ref.split("!")[1])
# Output: Word sequence number:  11
```

## Notes

This first three characters of this feature value are identical to the feature [book_short](book_short.md#start).

See also the related feature [id](id.md#start).

## Source description

The identifier is based on the XML attribute ref of the w (word) tag.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

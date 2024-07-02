<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: subjrefspec

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `subjref` feature indicates a subject reference to one or more nodes. This feature is essential for understanding the syntactic relationships and dependencies within the text. The subject reference points to a node formated as [id](id.md#start).

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Id in the format like `n40006028008`, A uniqe identifier for each individual word in the corpus.

```
The letter 'n' followed by a 11-digit unique id in the format

    BBCCCVVVWWW
    BB          => zero-padded book, the first NT book (Matthew) starts at 40
      CCC       => zero-padded chapter
         VVV    => zero-padded verse
            WWW => zero-padded word index (instance within the verse)
```

## Notes

See also related feature [subjref](subjref.md#start)

## Source description

Based on the optional XML attribute `subjref` of the tag `w` (word).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

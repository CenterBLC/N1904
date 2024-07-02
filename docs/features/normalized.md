<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: normalized

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

This feature provides the normalized Greek form of the surface text in the Nestle 1904 Greek New Testament. This feature is essential for consistent and accurate lexical analysis.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Notes

See also the following related features:

   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [unicode](unicode.md#start): Word as it appears in the text (in unicode)

   
The following snippet identifies all word nodes where feature text and normalized differ:
```python
Query = '''
w:word 
   w .text#normalized. w
'''

Results = A.search(Query)
```
This query returns 37182 results. The following table shows the frequency of the top ten differences between feature text and normalized:

| text        | normalized | frequency |
|-------------|-------------|-----------|
| καὶ         | καί        | 8545      |
| δὲ          | δέ         | 2620      |
| τὸ          | τό         | 1658      |
| τὸν         | τόν        | 1556      |
| τὴν         | τήν        | 1518      |
| γὰρ         | γάρ        | 921       |
| μὴ          | μή         | 902       |
| τὰ          | τά         | 817       |
| τοὺς        | τούς       | 722       |
| πρὸς        | πρός       | 670       |

The relation between the feature values for text, normalized and lemma can be demonstrated using the example from the third word in Matthew 1:2:

<pre>
        &lt;w ref="MAT 1:2!3"
             ...
             xml:id="n40001002003"
             lemma="ὁ"
             normalized="τόν"
             ...
             unicode="τὸν"&gt;τὸν&lt;/w&gt;
</pre>

## Source description

The `normalized` feature is taken from the XML attribute `normalized` of the `w` (word) tag.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: normalized

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

This feature provides the normalized Greek form of the surface text in the Nestle 1904 Greek New Testament. This feature is essential for consistent and accurate lexical analysis.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

The normalized form of the Greek surface text (see also the 'notes' section).

## Notes
  
The following snippet identifies all word nodes where feature text and normalized differ:
```python
Query = '''
w:word 
   w .text#normalized. w
'''

Results = A.search(Query)
```
This query returns 37182 results. The following table shows the frequency of the top ten differences between feature text and normalized:

| feature value text        | feature value normalized | frequency |
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

See also the following related features:

   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [unicode](unicode.md#start): Word as it appears in the text (in unicode)

## Source description

The `normalized` feature is taken from the XML attribute `normalized` of the `w` (word) tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


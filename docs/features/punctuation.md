<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: punctuation

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

This feature contains the punctuation character found after a word. If no punctuation, the feature value is empty.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values 

For [`word`](featuresbynodetype.md#word-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and [`wg-view`](../wg-view.md#start)):

Value | Description | Unicode codepoint | Frequency
---  |  --- | --- | ---
`,` | Comma |  [`&#44`](https://www.codetable.net/decimal/44)   | 9462
`.` | Full Stop | [`&#46`](https://www.codetable.net/decimal/46) | 5717
`·` | Midle Dot | [`&#183`](https://www.codetable.net/decimal/183) | 2359
`;` | Semicolon | [`&#59`](https://www.codetable.net/decimal/59) | 971
&lt;empty&gt; | No punctuation | | 119270 

For [`phrase`](featuresbynodetype.md#phrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Unicode codepoint | Frequency
---  |  --- | --- | ---
`,` | Comma |  [`&#44`](https://www.codetable.net/decimal/44)   | 3903
`.` | Full Stop | [`&#46`](https://www.codetable.net/decimal/46) | 2731
`·` | Midle Dot | [`&#183`](https://www.codetable.net/decimal/183) | 1189
`;` | Semicolon | [`&#59`](https://www.codetable.net/decimal/59) | 589
&lt;empty&gt; | No punctuation | | 60595 

For [`subphrase`](featuresbynodetype.md#subphrase-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start)):

Value | Description | Unicode codepoint | Frequency
---  |  --- | --- | ---
`,` | Comma |  [`&#44`](https://www.codetable.net/decimal/44)   | 9462
`.` | Full Stop | [`&#46`](https://www.codetable.net/decimal/46) | 5717
`·` | Midle Dot | [`&#183`](https://www.codetable.net/decimal/183) | 2359
`;` | Semicolon | [`&#59`](https://www.codetable.net/decimal/59) | 971
&lt;empty&gt; | No punctuation | | 106081 

## Notes

This feature enables easy testing for the presence of punctuation following a word. To retrieve all word nodes without trailing punctuation, use the following snippet:

```python
Query = '''
word
   punctuation#
'''

Results = A.search(Query)
```

The following image shows the features describing the material found after a word.

<img src="images/material_after_word.jpg" width="150px">

The following set of features describe the full surface text:
   * [after](after.md#start): All material found after a word (including critical signs).
   * [before](before.md#start): All material found before a word.
   * [criticalsign](criticalsign.md#start): Text-critical signs.
   * [normalized](normalized.md#start): Normalized Greek text.
   * punctuation (this feature): Punctuations found after a word.
   * [text](text.md#start): Word without punctuations and text-critical signs.
   * [trailer](trailer.md#start): All material found after a word (excluding critical signs).
   * [translit](translit.md#start): Transliteration of the word surface texts.
   * [unaccent](unaccent.md#start): Word without accents and diacritical markers.
   * [unicode](unicode.md#start): Unicode presentation including all material before and after word.

The following image shows the relation between these features.

<img src="images/details_surface_features.png" width="400" >

The following [text-formating options](../textformats.md#start) are defined in this dataset using this feature:
<pre>
  A.showFormats()
     format              level    template
     lex-orig-plain      word     {lemma}{trailer}
     lex-translit-plain  word     {lextranslit}{trailer}
     text-orig-full      word     {before}{text}{after}
     text-orig-plain     word     {text}{trailer}
     text-translit-plain word     {translit}{trailer}
     text-unaccent-plain word     {unaccent}{trailer}
</pre>

## Source description

Calculated from the from XML attribute `after` of tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*




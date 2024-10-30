<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: domain

Feature group | Feature type | Data type | Available for node types | Used in viewtypes
---  | --- | --- | --- | ---
[`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 
 
## Feature description

This feature specifies the semantic domain according to the Semantic Dictionary of Biblical Greek (SDBG). This feature helps to categorize words based on their meanings and semantic fields.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Value | Description | Frequency<sup>1</sup>
--- | --- | ---
xxxyyy  | Lexical Domain value| 126757
&lt;empty&gt; | Value not provided | 11022

<sup>1</sup> Frequency figures are listed for `word` nodes only.

## Interpreting the data

This feature is *to some extent* equivalent to a numerical representation of feature ['ln'](ln.md#start) and can be decoded using the following method. Take for example feature 'domain' has a value of '089007'. The 6-digit value '089007' first need to be split into two 3-digit parts: '087' and '007'. The second part should be interpreted as a alphabetic (A=1, B=2, C=3, D=4, E=5, ..., Z=26). Taken the two parts together, this will result in '89G', which points to an entry in Louw-Nida. For this example (i.e. 89G) this maps to main section ['Relations'](https://www.laparola.net/greco/louwnida.php?sezmag=89) and subsection ['Cause and/or Reason'](https://www.laparola.net/greco/louwnida.php?sezmag=89&sez1=15&sez2=38).

It is important to realize that the granularity of feature 'domain' is less than that of feature ['ln'](ln.md#readme). Consider for example the Greek word ἀρχή in John 1:1. According to Louw-Nida Lexicon this can map to either a:beginning (aspect)=>68.1 or b:beginning (time)=>67.65. In Text-Fabric one value is attached to feature 'domain', which is '067003'. Using the above explained method, this breaks down to '067' and '003' where the last part refers to section 'C', which is actualy a range [(67.65-67.72)](https://www.laparola.net/greco/louwnida.php#67) within Louw Nida's classification.

## Using the domain feature in Text-Fabric queries

Given that the domain feature may contain multiple entries, using a regular expression rather than a simple comparison is sensible. However, this approach requires caution; merely replacing `=` with `~` will yield all wanted matches but may also introduce unintended ones. To filter out these unwanted results, the following template can be used, illustrated here with the example value 088015.

```python
# The preceding 'r' before the template allows for a raw strings, preventing Python from altering the regex.
findDomain =r'''
phrase
    word domain~(^|\s)088015($|\s)
'''
domainResults=A.search(findDomain)
```

## Note

See also related feature [ln](ln.md#readme) (Louw-Nida lexical classification).

## Source description

This feature is derived from the XML attribute `domain` of the tag `w` (word). The word sense data for this feature was compiled by the United Bible Societies MARBLE project. See [Macula-Greek Licence](https://github.com/Clear-Bible/macula-greek/blob/main/LICENSE.md).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

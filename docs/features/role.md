<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: role

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactical`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features)  | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `role` feature indicates the syntactic role of a word or word group within a sentence. It provides information about whether the word or group is acting as a subject, object, verb, etc.

## Feature values

For `word` or `wg` (wordgroup) nodes:

Value | Description | Frequency
--- | --- | ---
o | Object | 26988
s | Subject | 22336
adv | Adverbial | 43154
v | Verb | 50344
p | Predicate | 7348
io | Indirect object | 5316
vc | Verbal Copula  | 5186
apposition | Apposition | 4878
aux | Auxiliar | 2112
o2 | Second object | 718

## Mapping between role and function feature

feature `role` ([`wg-view`](../wg-view.md#start)) | feature [`function`](function.md#start) ([`syntax-view`](../syntax-view.md#start))
---|---
io | Cmpl
o | Objc
o2 | Objc
p | PreD
s | Subj
vc (wg nodes) | Pred
v (word nodes) | Pred
apposition | Appo

## Note
See also the description in [MACULA Greek Treebank for the Nestle 1904 Greek New Testament.pdf](https://nbviewer.org/github/biblicalhumanities/greek-new-testament/blob/master/syntax-trees/nestle1904/doc/Nestle%201904%20Treebank%20Documentation.pdf) on page 4 and 5 (section 2.2. Syntactic Categories at Word Level: Part of Speech Labels).

## Source description

This feature is derived from the XML attribute `role` of the tag `w` (word) or `wg` (wordgroup).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

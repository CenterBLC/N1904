<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: function

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`Sentence`](featuresbynodetype.md#sentence-nodes) [`Clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

The `function` feature describes the syntactic functions of words, groups of words (phrases, clauses, etc.), or the composition of (sub)sentences. This feature mimicks BHSA nomenclature for feature [function](https://etcbc.github.io/bhsa/features/function/).

## Feature values

The values of this feature consist of one or more of the following functions:

Value|Description
---|---
Pred|Predicate
Cmpl|Complement
Objc|Object
Subj|Subject
PreC|Predicate-Complement
Adv|

### Frequency for nodetype [sentence](featuresbynodetype.md#sentence-nodes)

Value|Occurences<sup>1</sup>
---|---
Pred-Obj|51
Subj-PreC-PreC|42
Cmpl-Pred|38
Cmpl-Pred-Obj|34
Subj-PreC|29
PreC-Subj|28
Subj-Cmpl|23
Pred-Obj-Cmpl|22
Subj-Pred-Obj|20
Pred-Obj-Subj|19

<sup>1</sup> Only the first 10 items are shown in this list. 

### Frequency for nodetype [clause](featuresbynodetype.md#clause-nodes)

Value|Occurences<sup>2</sup>
---|---
Pred-Obj|2675
Pred-Cmpl|1897
Cmpl-Pred|1147
Obj-Pred|1065
Cmpl-Pred-Obj|650
Subj-Pred|626
Pred-Subj|603
Pred-Obj-Cmpl|596
Subj-PreC-PreC|595
PreC-PreC|554

<sup>2</sup> Only the first 10 items are shown in this list. 

### Frequency for nodetype [wg](featuresbynodetype.md#wordgroup-nodes)

Value|Occurences
---|---
Cmpl|11056
Subj|5740
Objc|4524
Pred-Obj|2726
Pred-Cmpl|1909
PreC|1610
Cmpl-Pred|1185
Obj-Pred|1077
Cmpl-Pred-Obj|684
Subj-Pred|639

### Frequency for nodetype [phrase](featuresbynodetype.md#phrase-nodes)

Value|Occurences
---|---
Pred|24767
Cmpl|18608
Subj|10198
Objc|9337
PreC|3514

### Frequency for nodetype [subphrase](featuresbynodetype.md#subphrase-nodes)

Value|Occurences
---|---
Pred|24767
Cmpl|18608
Subj|10198
Objc|9337
PreC|3514

### Frequency for nodetype [word](featuresbynodetype.md#word-nodes)

Value|Occurences
---|---
Pred|24767
Cmpl|7552
Objc|4813
Subj|4458
PreC|1904

## Source description

This feature is based upon the (optional) XML attribute `role` of the tag `wg` (wordgroup) or `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

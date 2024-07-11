<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: cltype

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`clause`](featuresbynodetype.md#clause-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

This feature provides classification for different types of clauses, specifically focusing on verbless, verb-elided, and minor clauses. 

All clauses without explicit value for this this feature are to be regarded verbal clauses. 

## Feature values

Frequency for [sentence](featurebynodetype.md#sentence-nodes) nodes:

value | description | Frequency
---  | --- | --- 
&lt;empty&gt; | Verbal clause type | 19703 
`Verbless` | Verbless clause type| 77
`VerbElided` |  Verb-elided clause type | 47
`Minor` |  Minor clause type | 1

Frequency for [`clause`](featuresbynodetype.md#clause-nodes) nodes:

value | description | Frequency
---  | --- | --- 
&lt;empty&gt; | Verbal clause type | 30814
`Verbless` | Verbless clause type| 1003
`VerbElided` |  Verb-elided clause type | 884
`Minor` |  Minor clause type | 831

Frequency for [`wg`](featuresbynodetype.md#wordgroup-nodes) nodes:

value | description | Frequency
---  | --- | --- 
&lt;empty&gt; | Verbal clause type | 106868
`Verbless` | Verbless clause type| 1050
`VerbElided` |  Verb-elided clause type | 961
`Minor` |  Minor clause type | 832

## Note

To select all verbal clauses for node type `sentence`, the following snippet can be used:

```python
Query = '''
sentence 
   cltype#1
'''
Results = A.search(Query)
```

## Additional information

The following description of the various clause types is taken from : Andi Wu and Randall K. Tan, *Documentation for the MACULA Greek Treebank for the Nestle 1904 Greek New Testament* (2022),7. Availabe at [MACULA Greek Treebank for the Nestle 1904 Greek New Testament.pdf](https://nbviewer.org/github/biblicalhumanities/greek-new-testament/blob/master/syntax-trees/nestle1904/doc/Nestle%201904%20Treebank%20Documentation.pdf).

  - Verbal Clause: The clause represents a grammatical unit that expresses a proposition. Verbal clauses are 
the most typical form of the clause, with an explicit verbal element as the head of the clause (i.e., the 
constituent on which all other clause constituents are dependent).  
  - Verbless Clause: Verbless clauses are relational clauses of identification or attribution without an explicit 
copula verb. Verbless clauses typically consist of a core of a Subject and a Predicate, with additional 
Adverbial clause constituents possible. 
  - Verb Elided Clause: Verb elided clauses are clauses that imply the carrying over of Verbal Function 
(usually from the previous clause). They are clauses without Verbal Function that are not clauses of 
identification or attribution. 
  - Minor Clause: Minor clauses are clauses without any predication (no Verbal Function or Predicate 
Function), i.e., contain no assertions or propositions. They function interpersonally (vocative direct 
address or interjection to gain attention/alert) or textually (left-dislocated focus noun phrases, e.g. as for 
the game, I did not get to watch it.).

## Source description

This feature is derived from the XML attribute `cltype` of the tag `wg` (wordgroup).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

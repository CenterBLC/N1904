<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: cls

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `cls` feature provides the part of speech (PoS) for `word` nodes and the category for other nodes. 
## Feature values

Frequency for nodetype [`word`](featuresbynodetype.md#word-nodes):

value | Part of Speech | frequency
--- | --- | ---
adj | adjective | 8452
adv | adverb | 6147
conj | conjunction | 18227
det | determiner | 19786
intj | interjection | 15
noun | noun | 28455
num | numeral | 476
prep | preposition | 10914
ptcl | particle | 773
pron | pronoun | 16177
verb | verb | 28357

Frequency for nodetype [`wg`](featuresbynodetype.md#wordgroup-nodes) (wordgroup) :

Value | Phrase Category | frequency
--- | --- | ---
adjp | adjective phrase | 168
advp | adverbial phrase | 166
np | nominal phrase | 30911
nump | numeral phrase | 7
pp | prepositional phrase | 11169
vp | verbal phrase | 207
adv | ? phrase | 7
cl | ? phrase | 30152
conj | conjuction phrase| 1

Frequency for nodetype [`phrase`](featuresbynodetype.md#phrase-nodes) :

Value | Phrase Category | frequency
--- | --- | ---
verb | verbal phrase|	24772
np	| nominal phrase |10935
pp | prepositional phrase |	9609
pron ||	8751
adv	| ? phrase | 4390
noun | |	2822
adj	|| 2304
det	|| 257
advp | adverbial phrase |	154
ptcl |participle phrase |	87
adjp | adjectival phrase | 168

Frequency for nodetype [`subphrase`](featuresbynodetype.md#subphrase-nodes) :

Value | Phrase Category | frequency
--- | --- | ---
np	| noun phrase | 30911
noun | noun | 28455
verb	| verb| 28357
det ||	19786
conj | conjunction |	18228
pron	| pronoun | 16177
pp | prepositional phrase|11169
prep| preposition | 10914
adj | adjectival phrase | 8452
adv	| adverbal | 6154

Frequency for nodetype [`clause`](featuresbynodetype.md#clause-nodes) :

Value | Phrase Category | frequency
--- | --- | ---
cl | Clause | 28676

Frequency for nodetype [`sentence`](featuresbynodetype.md#sentence-nodes) :

Value | Phrase Category | frequency
--- | --- | ---
cl | Clause | 1476

## Note
See also the description in [MACULA Greek Treebank for the Nestle 1904 Greek New Testament.pdf](https://nbviewer.org/github/biblicalhumanities/greek-new-testament/blob/master/syntax-trees/nestle1904/doc/Nestle%201904%20Treebank%20Documentation.pdf) on page 4 and 5 (section 2.2. Syntactic Categories at Word Level: Part of Speech Labels).

## Source description

This feature is derived from the XML attribute `class` of the tags `w` (word) and `wg` (wordgroup).

---
#### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

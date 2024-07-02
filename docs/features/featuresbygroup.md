<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Features (grouped by feature group) 
###### *(or browse by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), or [feature type](featuresbyfeaturetype.md#start))*

This is the key to the meaning of the features in this TextFabric dataset. The available features can be grouped together as following: 

* [Grid features](#grid-features): features pertaining to the arrangement and organization of the database.
* [Sectional features](#sectional-features): features related to structural divisions within the text.
* [Orthograpic features](#orthograpic-features): features related to the visual representation of the text.
* [Lexical features](#lexical-features): features related to individual words and their lexical properties.
* [Textcritical features](#textcritical-features): features related to textual critical issues.
* [Morphological features](#morphological-features): features related to the morphological form of words.
* [Syntactic features](#syntactic-features): features related to the syntactical arrangement of words and phrases.
* [Semantic features](#semantic-features): features related to semantic meaning and roles of words and phrases. 
* [Relational features](#relational-features): features describing relationships or connections between nodes.

## Grid features

<sup>These features pertains to the arrangement and organization of the database.</sup>

Name |  Feature type | Available on nodes | Description| Examples
---|---| ---|--- | ---
[oslots](oslots.md#start) | [`Edge`](featuresbyfeaturetype.md#edge-features) | *not applicable*  | slot containment | `1`&nbsp`1-11`&nbsp`2010-2015,2020-2030`
[otext](otext.md#start) |  [`Config`](featuresbyfeaturetype.md#config-features) | *not applicable*  | Textformatting and corpus segmenting configuration used by the text API | *no data, only specifications*  
[otype](otype.md#start)| [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`Sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`Book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`Group`](featuresbynodetype.md#group-nodes) [`Clause`](featuresbynodetype.md#clause-nodes) | mapping between node number and associated objecttype | 

## Sectional features

<sup>These features are related to structural divisions within the text.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
---|---|---|---|---|---
[book](book.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | Full book name | `Matthew`&nbsp`Mark` ... `Revelation`
[bookshort](bookshort.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | Short book name | `MAT`&nbsp`MAR` ... `REV`
[chapter](chapter.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) | Chapter number inside book | `1`&nbsp`2` ...
[id](id.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Unique identity of a word | `n40001003006`
[nodeid](nodeid.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | Node Id as in XML | `400010200010490`
[num](num.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`book`](featuresbynodetype.md#book-nodes) | Sequence number  | `1`&nbsp`2` ...   
[ref](ref.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Unique identity of a word | `1CO 10:1!1`
[verse](verse.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`verse`](featuresbynodetype.md#verse-nodes) | Verse number inside chapter | `1`&nbsp`2`

## Orthograpic features

<sup>These features are related to the visual representation of the text.</sup>

Name |  Data type |Feature type | Available on nodes| Description | Examples
--- | --- | --- | --- | --- | ---
[after](after.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | All material found after a word | `&nbsp` `. `&nbsp`; `
[before](before.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | text-critical characters before word | `(`&nbsp`[`
[normalized](normalized.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Normalized form of the surface text | `πρὸς`
[punctuation](punctuation.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Punctations after the word | `.`&nbsp`;`
[text](text.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word as it appears in the text | `Λόγος`&nbsp`Θεόν,`
[translit](translit.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Transliteration of the Greek word surface text | `estin`&nbsp`auton`
[unaccent](unaccent.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Surface word stripped of accents and diacritical markers | `εστιν`&nbsp`αυτον`
[unicode](unicode.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word in unicode format | `Λόγος`&nbsp`Θεόν,`

## Lexical features

<sup>These features are related to individual words and their lexical properties.</sup>

Name |  Data type |Feature type | Available on nodes | Description | Examples
---|---|---|--- | ---| ---
[gloss](gloss.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | English gloss (cf. BGVB) | `and, also, likewise`&nbsp`the`
[lemma](lemma.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical lemma (cf. BDAG) | `αὐτός`  `λέγω`
[strong](strong.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Strong's number | `5547`
[trans](trans.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | English translation (cf. Berean Study Bible) | `of the`&nbsp`to them`
[variant](variant.md#start) | [`string`](featuresbydatatype.md#string-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical variant of the lemma | `1`&nbsp`2`

## Textcritical features
<sup>These features are related to textual critical issues</sup>

Name |  Data type |Feature type | Available on nodes | Description | Examples
---|---|---|--- | ---| ---
[criticalsign](criticalsign.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | text-critical signs | `(`&nbsp`[`&nbsp`)`&nbsp`]`

## Morphological features
<sup>These features are related to the morphological form of words.</sup>
Name |  Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[case](case.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical case | `nominative`&nbsp`genitive`&nbsp`dative`
[degree](degree.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Degree of an comparative or superlative adjective | `superlative`&nbsp`comparative`
[gender](gender.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical gender | `masculine`&nbsp`feminine`&nbsp`neuter`
[mood](mood.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical mood of a verb | `indicative`&nbsp`optative `
[morph](morph.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)| Morphological tag | `V-AAI-3S`&nbsp`N-GSF`
[number](number.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical number | `singular`&nbsp`plural`
[person](person.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical person | `first`&nbsp`second`&nbsp`third`
[tense](tense.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical tense of the verb | `present`&nbsp`aorist`
[type](type.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`group`](featuresbynodetype.md#group-nodes) | Gramatical type of noun or pronoun | `common`&nbsp`personal`
[voice](voice.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical voice of the verb | `active`&nbsp`passive`

## Syntactic features
<sup>These features are related to the syntactical arrangement of words and phrases.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[appostioncontainer](appositioncontainer.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)  | Appostioncontainer information | `1` 
[articular](articular.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`sentence`](featuresbynodetype.md#sentence-nodes) [`group`](featuresbynodetype.md#group-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Articular information | `1`
[clausetype](clausetype.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Clause type information | `normalized`
[cls](cls.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word and WordGroup class (Part of Speech) | `noun`&nbsp`verb` / `np`&nbsp`cl`
[cltype](cltype.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) | Clause type | `Verbless`&nbsp`VerbElided`
[crule](crule.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Clause rule | `ClCl`&nbsp`ClCl2`
[discontinuous](discontinuous.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Discontinuous information | `1`
[junction](junction.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Junction information | `coordinate`&nbsp`subordinate`
[lang](lang.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`book`](bookgroupnodefeatures.md#readme) | Language of the corpus | `el`
[referent](referent.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Referent | `n40001011005`
[rela](rela.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Appostion information | `Appo` 
[role](role.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Role of word or wordgroup | `s`&nbsp`o`&nbsp`apposition`
[sp](sp.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`word`](featuresbynodetype.md#word-nodes)| Part of Speech | `verb`&nbsp`pron`&nbsp`intj`
[subjref](subjref.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes)  | Subject reference to one or more nodes | `512`&nbsp`821`
[subjrefspec](subjrefspec.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes)  | Subject reference to a node formated as id | `n46003022002`
[type](type.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`wg`](featuresbynodetype.md#wordgroup-nodes) | Syntactical type of wordgroup | `conjuncted-wg`&nbsp`apposition-group`

## Semantic features
<sup>These features are related to semantic meaning and roles of words and phrases.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[domain](domain.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical-Semantic domain according to SDBG | `092004`
[frame](frame.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0`&nbsp`A1`&nbsp`A2`
[framespec](framespec.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0:n63001005005 A1:n63001010014`
[ln](ln.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Louw-Nida lexical classification of semantic domains | `93.169a`

## Relational features
<sup>These features describe the relationships or connections between nodes.</sup>

Name | Data type | Feature type | Available on nodes |Description | Example
--- | --- | --- | --- | --- | ---
[note](note.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Annotation of linguistic nature | `discontinuous discourse`
[parent](parent.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes)  | Parent node | 
[sibling](sibling.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Sibling node | 

##### *(or browse by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), or [feature type](featuresbyfeaturetype.md#start))*

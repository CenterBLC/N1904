<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Features (grouped by feature group) 
#### *Or browse by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), or [feature type](featuresbyfeaturetype.md#start)*

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

<sup>These features pertains to the arrangement and organization of the database and its presentation.</sup>

Name |  Data type | Feature type | Available on nodes | Description| Examples
---|---| ---|--- | --- | ---
[oslots](oslots.md#start) |  [`String`](featuresbydatatype.md#string-datatype)| [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  | Represents set of slots associated with an object | `1` `1-11` `2010-2015,2020-2030`
[otext](otext.md#start) | *not applicable* | [`Config`](featuresbyfeaturetype.md#config-features) | *not applicable*  | Textformatting and corpus segmenting configuration used by the text API | *no data, only specifications*  
[otype](otype.md#start)| [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`clause`](featuresbynodetype.md#clause-nodes) | Maps node number to objecttype | `word` `sentence` `book` 

## Sectional features

<sup>These features are related to structural divisions within the text.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
---|---|---|---|---|---
[book](book.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | Full book name | `Matthew` `Mark` ... `Revelation`
[bookshort](bookshort.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | Short book name | `MAT` `MAR` ... `REV`
[chapter](chapter.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) | Chapter number inside book | `1` `2` ...
[id](id.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Node id as in XML | `n40001003006`
[nodeid](nodeid.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#word-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Reference to wg, clause, or sentence | `400010200010490`
[num](num.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`book`](featuresbynodetype.md#book-nodes) | Sequence number  | `1` `2` ... 
[ref](ref.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Unique identity of a word | `1CO 10:1!1`
[verse](verse.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`group`](featuresbynodetype.md#group-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`verse`](featuresbynodetype.md#verse-nodes) | Verse number inside chapter | `1` `2`

## Orthograpic features

<sup>These features are related to the visual representation of the text.</sup>

Name |  Data type |Feature type | Available on nodes| Description | Examples
--- | --- | --- | --- | --- | ---
[after](after.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | All material found after a word (incl. critical signs)| <span>` `</span> <span>`. `</span> <span>`; `</span>
[normalized](normalized.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Normalized form of the surface text | `πρὸς`
[punctuation](punctuation.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Punctations after the word | `.` `;`
[text](text.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word as it appears in the text | `Λόγος` `Θεόν,`
[trailer](trailer.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | All material found after a word (excl. critical signs) | `.` <span>` `</span>
[translit](translit.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Transliteration of the Greek word surface text | `estin` `auton`
[unaccent](unaccent.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Surface word stripped of accents and diacritical markers | `εστιν` `αυτον`
[unicode](unicode.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word in unicode format | `Λόγος` `Θεόν,`

## Lexical features

<sup>These features are related to individual words and their lexical properties.</sup>

Name |  Data type |Feature type | Available on nodes | Description | Examples
---|---|---|--- | ---| ---
[gloss](gloss.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | English gloss (cf. BGVB) | `and, also, likewise` `the`
[lemma](lemma.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical lemma (cf. BDAG) | `αὐτός`  `λέγω`
[lemmatranslit](lemmatranslit.md#start) | [`string`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Transliteration of the word lemma | `autos`  `lego`
[strong](strong.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Strong's number | `5547`
[trans](trans.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | English translation (cf. Berean Study Bible) | `of the` `to them`
[variant](variant.md#start) | [`String`](featuresbydatatype.md#string-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical variant of the lemma | `1` `2`

## Textcritical features
<sup>These features are related to textual critical issues</sup>

Name |  Data type |Feature type | Available on nodes | Description | Examples
---|---|---|--- | ---| ---
[before](before.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Text-critical characters before word | `(` `[`
[criticalsign](criticalsign.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Text-critical signs | `(` `[` `)` `]`

## Morphological features
<sup>These features are related to the morphological form of words.</sup>

Name |  Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[case](case.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical case | `nominative` `genitive` `dative`
[degree](degree.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Degree of an comparative or superlative adjective | `superlative` `comparative`
[gender](gender.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical gender | `masculine` `feminine` `neuter`
[mood](mood.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical mood of a verb | `indicative` `optative `
[morph](morph.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)| Morphological tag | `V-AAI-3S` `N-GSF`
[number](number.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical number | `singular` `plural`
[person](person.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical person | `first` `second` `third`
[tense](tense.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical tense of the verb | `present` `aorist`
[typems](typems.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  | Gramatical type of noun or pronoun | `common` `personal`
[voice](voice.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical voice of the verb | `active` `passive`

## Syntactic features
<sup>These features are related to the syntactical arrangement of words and phrases.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[appostioncontainer](appositioncontainer.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)  | Indicates whether a word group or phrase contains an apposition | <span title="1 = true">`1`</span> 
[articular](articular.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`sentence`](featuresbynodetype.md#sentence-nodes) [`group`](featuresbynodetype.md#group-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Articular information | <span title="1 = true">`1`</span>
[clausetype](clausetype.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Clause type information | `normalized`
[cls](cls.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word and WordGroup class (Part of Speech) | `noun` `verb` / `np` `cl`
[cltype](cltype.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) | Clause type | `Verbless` `VerbElided`
[crule](crule.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Clause rule | `ClCl` `ClCl2`
[discontinuous](discontinuous.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Discontinuous information | <span title="1 = true">`1`</span>
[junction](junction.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Junction information | `coordinate` `subordinate`
[lang](lang.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`book`](bookgroupnodefeatures.md#readme) | Language of the corpus | `el`
[referent](referent.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Referent | `n40001011005`
[rela](rela.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Appostion information | `Appo` 
[role](role.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Role of word or wordgroup | `s` `o` `apposition`
[rule](rule.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) | Rule for non-terminal node in syntax tree | `ClCl` `ClCl2`
[sp](sp.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`word`](featuresbynodetype.md#word-nodes)| Part of Speech | `verb` `pron` `intj`
[typ](typ.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`group`](featuresbynodetype.md#group-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`wg`](featuresbynodetype.md#wordgroup-nodes) [`group`](featuresbynodetype.md#group-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Syntactical type of group of words | `conjuncted-wg` `apposition-group`

## Semantic features
<sup>These features are related to semantic meaning and roles of words and phrases.</sup>

Name | Data type | Feature type | Available on nodes | Description | Examples
--- | --- | --- | --- | --- | ---
[domain](domain.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical-Semantic domain according to SDBG | `092004`
[frame](frame.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0` `A1` `A2`
[framespec](framespec.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0:n63001005005 A1:n63001010014`
[ln](ln.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Louw-Nida lexical classification of semantic domains | `93.169a`
[note](note.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Annotation of linguistic nature | `discontinuous discourse`
[subjref](subjref.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes)  | Subject reference to one or more nodes | `512` `821`
[subjrefspec](subjrefspec.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes)  | Subject reference to a node formated as id | `n46003022002`

## Relational features
<sup>These features describe the relationships or connections between nodes.</sup>

Name | Data type | Feature type | Available on nodes |Description | Example
--- | --- | --- | --- | --- | ---
[parent](parent.md#start) | [`String`](featuresbydatatype.md#string-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes)  | Parent node | 
[sibling](sibling.md#start) | [`Integer`](featuresbydatatype.md#integer-datatype) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`group`](featuresbynodetype.md#group-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`clause`](featuresbynodetype.md#clause-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Sibling node | 

#### *Or browse by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), or [feature type](featuresbyfeaturetype.md#start)*

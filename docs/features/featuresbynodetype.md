<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Features (grouped by node type) 

#### *Or browse by [name](featuresbyname.md#start), [feature type](featuresbyfeaturetype.md#start), [data type](featuresbydatatype.md#start), or [feature group](featuresbygroup.md#start)*

In  Text-Fabric 'features' provide a mapping of nodes of a specific type to its associated additional information. This Text-Fabric dataset contains the following node types:
* [137779 `word` nodes](#word-nodes): each node represents an individual word in the corpus. They consitute the the smallest linguistic entity in a query as they form the slots in the database.
* [106868 `wg` (wordgroup) nodes](#wordgroup-nodes): each node represents a group of words forming a cohesive unit. Many  word group nodes (namely the ones with an associated [cls](cls.md#start) value) are duplicated with a shadow node of one of the following types:
    * [72845 `subphrase` nodes](#subphrase-nodes): 
    * [113750 `phrase` nodes](#phrase-nodes): 
    * [30479 `clause` nodes](#clause-nodes): 
    * [8964 `group` nodes](#group-nodes):
* [18609 `sentence` nodes](#sentence-nodes): each node represents a single sentence.
* [7944 `verse` nodes](#verse-nodes): each node represents a single verse.
* [260 `chapter`nodes](#chapter-nodes): each node represents a single chapter.
* [27 `book` nodes](#book-nodes): each node represents a single book.

All node features are listed below grouped by node type: 

## Word nodes 

<sup>The `word` nodes represents individual word in the corpus. The features associated with this node type are used in both the [`wg-view`](../wg-view.md#start) and the [`syntax-view`](../syntax-view.md#start).</sup>

<sup>There are about fourty [optional features](../additions/featuresbyfeaturegroup.md#start) available for word nodes that can be [loaded as a module](../additions/README.md#adding-the-features).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[after](after.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | All material found after a word | `. ` `; ` <span>` `</span>
[before](before.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Text-critical signs before word | `[` `(` `—`
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Matthew` `Mark` ... `Revelation`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (abbreviated) | `MAT` `MAR` ... `REV`
[case](case.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical case | `nominative` `genitive` `vocative`
[chapter](chapter.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Chapter number inside book | `5` `7`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features)  | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word class: Part of Speech | `noun` `verb`
[criticalsign](criticalsign.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Text-critical signs | `(` `[` `)` `]`
[degree](degree.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Degree of an adjective | `comparative` `superlative`
[discontinuous](discontinuous.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Discontinuous information | `1`
[domain](domain.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical domain according to Semantic Dictionary of Biblical Greek, SDBG | `033006`
[frame](frame.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0` `A1`
[framespec](framespec.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0:n00000000000` `A1:n00000000000`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic function | `Pred` `Subj`
[gender](gender.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical gender | `masculine` `feminine` `neuter`
[gloss](gloss.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English gloss | `and, also, likewise` `the`
[id](id.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Unique identifier of a word | `n40001001001`
[lemma](lemma.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical lemma (cf. BDAG) | `αὐτός` `λέγω`
[lemmatranslit](lemmatranslit.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Transliteration of the word lemma | `αὐτός` `λέγω`
[ln](ln.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Louw-Nida lexical classification of semantic domains | `93.169a`
[morph](morph.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Morphological tag (Sandborg-Petersen morphology) | `V-PAI-3S` `PREP` `N-GSM`
[mood](mood.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical mood of a verb | `indicative` `optative`
[nodeid](nodeid.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String` ](featuresbydatatype.md#string-datatype) | Reference to wg, clause, or sentence | `400010200010490`
[normalized](normalized.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Normalized form of the surface text | `πρὸς`
[note](note.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Annotation of linguistic nature | `discontinuous discourse`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: word in verse) | `1` `2` ...
[number](number.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical number of the verb | `singular` `plural`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype |  `word`
[parent](parent.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Link to parent node
[person](person.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical person of the verb | `first` `second` `third`
[punctuation](punctuation.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Punctuation | ` ` `.`
[ref](ref.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`String`](featuresbydatatype.md#string-datatype) | Unique identity of a word | `1CO 10:1!1`
[sp](sp.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Part of Speech | `verb` `pron` `intj`
[strong](strong.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Strong's number | `5547`
[unicode](unicode.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word in unicode format | `Λόγος` `Θεόν,`
[sibling](sibling.md#start) | [`Relational`](featuresbygroup.md#relational-features) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | Sibling relationship between words | 
[subjrefspec](subjrefspec.md#start) | [`Relational`](featuresbygroup.md#relational-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Subject reference (to nodeID in XML source data) | `n40006028008`
[tense](tense.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical tense of the verb | `present` `aorist`
[text](text.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word as it appears in the text | `εὐαγγέλιον`
[trailer](trailer.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Material after the end of the word (excluding critical signs) | `.` <span>` `</span>
[trans](trans.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English translation (cf. Berean Study Bible) | `of the` `to them`
[translit](translit.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  |  Transliteration of the Greek word surface text | `estin` `auton`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[unaccent](unaccent.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Surface word stripped of accents and diacritical markers | `εστιν` `αυτον`
[unicode](unicode.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word in unicode format | `Λόγος` `Θεόν,`
[variant](variant.md#start) |  [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical variant | `1` `2`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter | `1` `4`
[voice](voice.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical voice of the verb | `active` `passive` `middle`

## Wordgroup nodes 

<sup>The `wg` nodes represents a group of words and/or wordgroups forming a cohesive unit. This node type is only associated with the [`wg-view`](../wg-view.md#start).</sup> 

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[appositioncontainer](appositioncontainer.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Indicates whether the word group contains an apposition | `1`
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates if wordgroup contains an article | `1`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (abbreviated) | `MAT` `MAR` ... `REV`
[clausetype](clausetype.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Clause type information | `normalized`)
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | WordGroup class | `np` `cl`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic function | `Pred` `Subj`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Junction details |  `coordinate` `subordinate`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: wordgroup in book) | `1` `2` ...
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | Maps node number to objecttype | `wg`
[parent](parent.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Link to parent node |
[rela](rela.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Appostion information | `Appo` 
[role](role.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Role wordgroup | `s` `o` `apposition`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[typ](typ.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Clause type | `Verbless` `VerbElided`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`

## Subphrase nodes

<sup>Note: this node type is only associated with the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[appositioncontainer](appositioncontainer.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer` ](featuresbydatatype.md#integer-datatype) | Indicates whether the subphrase contains an apposition | `1`
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates if subphrase contains an article | `1`
[after](after.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | All material found after a word | `. ` `; ` <span>` `</span>
[before](before.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Text-critical signs before word | `[` `(` `—`
[case](case.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical case | `nominative` `genitive` `vocative`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Class of the subphrase  | `np` `cl`
[criticalsign](criticalsign.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | text-critical signs | `(` `[` `)` `]`
[degree](degree.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Degree of an adjective | `comparative` `superlative`
[discontinuous](discontinuous.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Discontinuous information | `1` <span>` `</span>
[domain](domain.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical domain according to Semantic Dictionary of Biblical Greek, SDBG | `033006`
[framespec](framespec.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0:n00000000000` `A1:n00000000000`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | this is XML attribute function | `Pred` `Subj`
[gender](gender.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical gender | `masculine` `feminine` `neuter`
[gloss](gloss.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English gloss | `and, also, likewise` `the`
[id](id.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Unique identifier of a word | `n40001001001`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`String`](featuresbydatatype.md#string-datatype) | Junction |  `coordinate` `subordinate`
[lemma](lemma.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical lemma (cf. BDAG) | `αὐτός` `λέγω`
[lemmatranslit](lemmatranslit.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Transliteration of the word lemma | `autos` `lego`
[ln](ln.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Louw-Nida lexical classification of semantic domains | `93.169a`
[mood](mood.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical mood of a verb | `indicative` `optative`
[morph](morph.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | morphological code | `CONJ` `PREP`
[normalized](normalized.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Surface word stripped of punctations
[note](note.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Annotation of linguistic nature | `discontinuous discourse`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: subphrase in book) | `1` `2` ...
[number](number.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical number of the verb | `singular` `plural`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype | `subphrase`
[person](person.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical person of the verb | `first` `second` `third`
[punctuation](punctuation.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Punctuation | <span>` `</span> `.`
[ref](ref.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Unique identity of a word | `1CO 10:1!1`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[sp](sp.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Part of Speech | `verb` `pron` `intj`
[tense](tense.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical tense of the verb | `present` `aorist`
[text](text.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word as it appears in the text |
[trans](trans.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English translation (cf. Berean Study Bible) | `of the` `to them`
[translit](translit.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  |  Transliteration of the Greek word surface text | `estin` `auton`
[trailer](trailer.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Material after the end of the word (excluding critical signs) | `.` <span>` `</span>
[typ](typ.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[unaccent](unaccent.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Surface word stripped of accents and diacritical markers | `εστιν` `αυτον`
[unicode](unicode.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word in unicode format | `Λόγος` `Θεόν,`
[variant](variant.md#start) |  [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical variant | `1` `2`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`
[voice](voice.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical voice of the verb | `active` `passive` `middle`

## Phrase nodes

<sup>Note: this node type is only associated with the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[after](after.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | All material found after a word | `. ` `; ` ` `
[appositioncontainer](appositioncontainer.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer` ](featuresbydatatype.md#integer-datatype) |  appositioncontainer | `1`
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates whether the phrase contains an apposition | `1`
[before](before.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Text-critical signs before word | `[` `(` `—`
[case](case.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical case | `nominative` `genitive` `vocative`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Class of the phrase  | `np` `cl`
[criticalsign](criticalsign.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | text-critical signs | `(` `[` `)` `]`
[degree](degree.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Degree of an adjective | `comparative` `superlative`
[discontinuous](discontinuous.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Discontinuous information | `1`
[domain](domain.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical domain according to Semantic Dictionary of Biblical Greek, SDBG | `033006`
[framespec](framespec.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Semantic Role Labeling (reference to id of subject, object or idirect object) | `A0:n00000000000` `A1:n00000000000`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | this is XML attribute function | `Pred` `Subj`
[gender](gender.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical gender | `masculine` `feminine` `neuter`
[gloss](gloss.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English gloss | `and, also, likewise` `the`
[id](id.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Unique identifier of a word | `n40001001001`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`String`](featuresbydatatype.md#string-datatype) | Junction |  `coordinate` `subordinate`
[lemma](lemma.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical lemma (cf. BDAG) | `αὐτός` `λέγω`
[lemmatranslit](lemmatranslit.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Transliteration of the word lemma | `autos` `lego`
[ln](ln.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Louw-Nida lexical classification of semantic domains | `93.169a`
[note](note.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Annotation of linguistic nature | `discontinuous discourse`
[mood](mood.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical mood of a verb | `indicative` `optative`
[morph](morph.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | morphological code | `CONJ` `PREP`
[normalized](normalized.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Surface word stripped of punctations
[note](note.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Annotation of linguistic nature | `discontinuous discourse`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: phrase in book) | `1` `2` ...
[number](number.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical number of the verb | `singular` `plural`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype |  `phrase`
[person](person.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical person of the verb | `first` `second` `third`
[punctuation](punctuation.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Punctuation | <span>` `</span> `.`
[ref](ref.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Node`](featuresbyfeaturetype.md#node-features) | Unique identity of a word | `1CO 10:1!1`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[sp](sp.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Part of Speech | `verb` `pron` `intj`
[tense](tense.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical tense of the verb | `present` `aorist`
[text](text.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word as it appears in the text |
[trans](trans.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | English translation (cf. Berean Study Bible) | `of the` `to them`
[translit](translit.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  |  Transliteration of the Greek word surface text | `estin` `auton`
[trailer](trailer.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Material after the end of the word (excluding critical signs) | `.` <span>` `</span>
[typ](typ.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[unaccent](unaccent.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Surface word stripped of accents and diacritical markers | `εστιν` `αυτον`
[unicode](unicode.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Word in unicode format | `Λόγος` `Θεόν,`
[variant](variant.md#start) |  [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Lexical variant | `1` `2`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`
[voice](voice.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical voice of the verb | `active` `passive` `middle`

## Clause nodes

<sup>Note: this node type is only associated with the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates if wordgroup contains an article | `1`
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Luke` `Matthew` ... `Revelation`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (abbreviated) | `MAT` `MAR` ... `REV`
[clausetype](clausetype.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Clause type information | `normalized`)
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Class of the clause  | `np` `cl`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | this is XML attribute function | `Pred` `Subj`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Junction |  `coordinate` `subordinate`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: clause in book) | `1` `2` ...
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype | `clause`
[role](role.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Role wordgroup | `s` `o` `apposition`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[typ](typ.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`

## Group nodes

<sup>Note: thes node type is only associated with the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates if wordgroup contains an article | `1`
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Luke` `Matthew` ... `Revelation`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (abbreviated) | `MAT` `MAR` ... `REV`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: group in book) | `1` `2` ...
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | Maps node number to objecttype | `group`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of group | `conjuncted`
[role](role.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Role wordgroup | `s` `o` `apposition`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[typ](typ.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype)  | syntactic labels for textual elements | `NP` `AdjP`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`

## Sentence nodes 

<sup>The `sentence` nodes represents individual sentences in the corpus. This node type is associated with both the [`wg-view`](../wg-view.md#start) and the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[articular](articular.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Indicates if wordgroup contains an article | `1`
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Galatians`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (abbreviated) | `MAT` `MAR` ... `REV`
[clausetype](clausetype.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Clause type information | `normalized`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | WordGroup class | `np` `cl`
[function](function.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | this is XML attribute function | `Pred` `Subj`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Junction |  `coordinate` `subordinate`
[nodeid](nodeid.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Reference to wg, clause, or sentence | `400010200010490`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: sentence in book) | `1` `2` ...
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`String`](featuresbydatatype.md#string-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | mapping between node number and associated objecttype | `sentence`
[parent](parent.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Edge`](featuresbyfeaturetype.md#edge-features)  | [`String`](featuresbydatatype.md#string-datatype) | Link to parent node
[role](role.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Role wordgroup | `s` `o` `apposition`
[rule](rule.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Syntactic rule | `ClCl` `ClCl2`
[typems](typems.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Gramatical type of noun or pronoun | `common` `personal`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter where this item begins | `1` `4`

## Verse nodes 

<sup>The `verse` nodes represents individual versus in the corpus. This node type is associated with both the [`wg-view`](../wg-view.md#start) and the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Luke` `Matthew` ... `Revelation`
[chapter](chapter.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Chapter number inside book | `1` `2`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype | `verse`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Verse number inside chapter | `1` `4`

## Chapter nodes 

<sup>The `chapter` nodes represents individual chapters in the corpus. This node type is associated with both the [`wg-view`](../wg-view.md#start) and the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) |  Book name (full) | `Luke` `Matthew` ... `Revelation`
[chapter](chapter.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Chapter | `1` `2`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype | `chapter`

## Book nodes 

<sup>The `book` nodes represents individual books in the corpus. This node type is associated with both the [`wg-view`](../wg-view.md#start) and the [`syntax-view`](../syntax-view.md#start).</sup>

Feature | Feature group | Feature type | Data type | Short description | Examples
--- | --- | --- | --- | --- | ---
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Book name (full) | `Luke` `Matthew` ... `Revelation`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Book name (abbreviated) | `LUK` `ACT`
[lang](lang.md#start) |  [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | Language of the corpus | `el`
[num](num.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`Integer`](featuresbydatatype.md#integer-datatype) | Sequence number (here: book number) | `1` `2` ... `26`
[oslots](oslots.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype) | Represents set of slots associated with an object |  `1` `1-11` `2010-2015,2020-2030`
[otype](otype.md) | [`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) |   [`String`](featuresbydatatype.md#string-datatype) | Maps node number to objecttype | `book`

#### *Or browse by [name](featuresbyname.md#start), [feature type](featuresbyfeaturetype.md#start), [data type](featuresbydatatype.md#start), or [feature group](featuresbygroup.md#start)*

<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Features (grouped by data type)
###### *(or browse by [node type](featuresbynodetype.md#start), [feature group](featuresbygroup.md#start), or [feature type](featuresbyfeaturetype.md#start))*

The features in this Text-Fabric dataset can be grouped according to their datatype in the following manner: 

* [String datatype features](#string-datatype)
* [Integer datatype features](#integer-datatype)
* [Link datatype features](#link-datatype)
* [Configuration data](featuresbydatatype.md#configuration-data)

## String datatype
<sup>Python datatype: [str](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)</sup>

Name | Feature group | Feature type | Available on node | Description | Examples
--- | --- | --- | --- | --- | ---
[after](after.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)| All material after a word | ` ` `.` `,— ` `.]] `
[before](before.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | All material before a word | `—`  `[[`
[book](book.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`group`](featuresbynodetype.md#group-nodes) [`wg`](featuresbynodetype.md#wg-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes)  [`book`](featuresbynodetype.md#book-nodes) | Full book name | `Matthew` ... `Revelation`
[bookshort](bookshort.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`book`](featuresbynodetype.md#book-nodes) | Short book name | `MAT` `MAR` ... `REV`
[case](case.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical case | `nominative` `genitive` `dative`
[clausetype](clausetype.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`string`](featuresbydatatype.md#string-datatype) | [`clause`](featuresbynodetype.md#clause-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Clause type information | `normalized`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Part of Speech | `adv` `det` `verb`
[cls](cls.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes)  [`sentence`](featuresbynodetype.md#sentence-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes)  | phrase catagory | `adjp`  `np`
[degree](degree.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Degree of an comparative or superlative adjective | `superlative` `comparative`
[discontinuous](discontinuous.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | 1 if the word is out of sequence | ` ` `1` 
[domain](domain.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical domain according to SDBG | `092004`
[frame](frame.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) | Reference to the id of subject, object or idirect object | `A0` `A1` `A2`
[framespec](framespec.md#start) | [`Semantic`](featuresbygroup.md#senantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes)  [`phrase`](featuresbynodetype.md#phrase-nodes) | Reference to the id of subject, object or idirect object | `A0:n63001005005 A1:n63001010014`
[gloss](gloss.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | English gloss (cf. BGVB)| `faith`
[gender](gender.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)  | Gramatical gender | `masculine` `feminine` `neuter`
[nodeId](nodeId.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Node ID | `n56001015007`
[lemma](lemma.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical lemma (cf. BDAG) |
[ln](ln.md#start) | [`Semantic`](featuresbygroup.md#semantic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Louw-Nida lexical classification of semantic domains | `93.169a`
[mood](mood.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) |Gramatical mood of a verb | `indicative` `optative `
[morph](morph.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Morphological tag | `V-AAI-3S` `N-GSF`
[note](note.md#start) | ? | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes)  | Annotation of linguistic nature | `discontinuous discourse`
[normalized](normalized.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Normalized form of the surface text |
[number](number.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) |Gramatical number | `singular` `plural`
[person](person.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical person | `first` `second` `third`
[punctuation](punctuation.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) |[`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Punctuation after a word | ` ` `.`
[ref](ref.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Unique identity of a word | `1CO 10:1!1`
[junction](junction.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | Junction information | `coordinate` `subordinate`
[sp](sp.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`word`](featuresbynodetype.md#word-nodes)| Part of Speech | `verb` `pron` `intj`
[strong](strong.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Strongs number | `5547`
[tense](tense.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical tense of the verb | `present` `aorist`
[text](text.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word as it appears in the text | `λόγος`
[trans](trans.md#start) | [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | English translation (cf. Berean Study Bible) | `of the` `to them`
[translit](translit.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Transliteration of the Greek word surface text | `estin` `auton`
[type](type.md#start) | [`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes)  |Gramatical type of noun or pronoun | `common` `personal`
[type](type.md#start) | [`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`wg`](featuresbynodetype.md#wordgroup-nodes)  | Syntactical type. | `apposition-group` `wrapper-scope`
[unicode](unicode.md#start) | [`Orthograpic`](featuresbygroup.md#orthograpic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Word as it appears in the text (in unicode) | `λόγος`
[variant](variant.md#start) |  [`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Lexical variant | `1` `2`
[voice](voice.md#start) | [`Morphological`](featuresbygroup.md#morphological-features)| [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Gramatical voice of the verb | `active` `passive`

## Integer datatype
<sup>Python datatype: [int](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)</sup>

Name | Feature group | Feature type | Available on node | Description | Examples
--- | --- | --- | --- | --- | ---
[chapter](chapter.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) | Chapter number inside book | `1` `2` ...
[num](num.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) |  [`word`](featuresbynodetype.md#word-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) [`book`](featuresbynodetype.md#book-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) | Sequence number  | `1` `2` ...
[nodeId](nodeId.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) | Node Id as in XML | `400010200010490`
[sibling](sibling.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Sibling relationship between words | 
[strong](strong.md#start) | [`integer`](featuresbydatatype.md#integer-datatype) |  [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | Strong's number | `5547`
[verse](verse.md#start) | [`Sectional`](featuresbygroup.md#sectional-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`verse`](featuresbynodetype.md#verse-nodes)| Verse number inside chapter | `1` `2`

## Link datatype

Name | Feature type | Available on node | Description | Examples
--- | --- | --- | --- | ---
[subj_ref](subj_ref.md#start) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`word`](featuresbynodetype.md#word-nodes) | Subject reference |


## Configuration data

Name | Feature type | Available on node | Description | Examples
--- | --- | --- | --- | ---
[oslots](oslots.md) | [`Config`](featuresbyfeaturetype.md#config-features) | - | slot containment | `1` `1-11` `2010-2015,2020-2030`
[otext](otext.md) | [`Config`](featuresbyfeaturetype.md#config-features) |  - |  configuration for sections, structure, and text formats (textapi) | *no data, only specifications*  
[otype](otype.md) | [`Node`](featuresbyfeaturetype.md#node-features) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`Sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`Book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`Group`](featuresbynodetype.md#group-nodes) [`Clause`](featuresbynodetype.md#clause-nodes)  | mapping between node number and associated objecttype|

###### *(or browse by [node type](featuresbynodetype.md#start), [feature group](featuresbygroup.md#start), or [feature type](featuresbyfeaturetype.md#start))*

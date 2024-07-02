<a name="start"></a>
[`Transcription`](../transcription.md#start) | `Features` | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Features

In Text-Fabric, a 'feature' refers to attributes associated with a certain nodes type (like words, word groups, or sentences). The feature value provide additional information specific to the attribute of that node.

The full featureset of this Text-Fabric dataset can be viewed by different grouping methods:
* [Grouped by feature type](featuresbyfeaturetype.md#start)
     * [`Node`](featuresbyfeaturetype.md#node-features): the fundamental units or entities in the data model.
     * [`Edge`](featuresbyfeaturetype.md#edge-features): relationships or links, establishing connections between nodes in the data model.
     * [`Config`](featuresbyfeaturetype.md#config-features): contains the configuration or settings that define the behavior and parameters of the data processing or analysis.
* [Grouped by feature group](featuresbygroup.md#start):
     * [`Grid`](featuresbygroup.md#grid-features): features pertaining to the arrangement and organization of the database.
     * [`Sectional`](featuresbygroup.md#sectional-features): features related to structural divisions within the text.
     * [`Orthograpic`](featuresbygroup.md#orthograpic-features): features related to the visual representation of the text.
     * [`Lexical`](featuresbygroup.md#lexical-features): features related to individual words and their lexical properties.
     * [`Textcritical`](featuresbygroup.md#textcritical-features): features related to textual critical issues.
     * [`Morphological`](featuresbygroup.md#morphological-features): features related to the morphological form of words.
     * [`Syntactic`](featuresbygroup.md#syntactic-features): features related to the syntactical arrangement of words and phrases.
     * [`Semantic`](featuresbygroup.md#semantic-features): features related to semantic meaning and roles of words and phrases.
     * [`Relational`](featuresbygroup.md#relational-features): features describing relationships or connections between nodes.
* [Grouped by node type](featuresbynodetype.md#start):
     * [`word`](featuresbynodetype.md#word-nodes): represents individual words in the text.
     * [`wg`](featuresbynodetype.md#wordgroup-nodes) (wordgroup): refers to a collection or grouping of words that form a cohesive unit. Each individual word group node is accompanied by a shadow node of one of the following types: 
         * [`subphrase`](featuresbynodetype.md#subphrase-nodes): Nodes pertaining to a subphrase unit.
         * [`phrase`](featuresbynodetype.md#phrase-nodes): Nodes pertaining to a phrase unit.
         * [`clause`](featuresbynodetype.md#clause-nodes): Nodes pertaining to a clause unit.
         * [`group`](featuresbynodetype.md#group-nodes): Nodes pertaining to a group unit.
     * [`sentence`](featuresbynodetype.md#sentence-nodes): represents individual sentences in the text.
     * [`verse`](featuresbynodetype.md#verse-nodes): pertains to divisions within a larger textual unit, specificaly the biblical verse.
     * [`chapter`](featuresbynodetype.md#chapter-nodes): divisions within the text that group related content together, specificaly the biblical chapter.
     * [`book`](featuresbynodetype.md#book-nodes): the highest-level division within the text, corresponding to a bible book.
* [Grouped by datatype](featuresbydatatype.md#start):
     * [`string`](featuresbydatatype.md#string-datatype): Datatype of feature is string.
     * [`integer`](featuresbydatatype.md#integer-datatype): Datatype of feature is integer.
     * [`configuration`](featuresbydatatype.md#configuration-data): Configuration data.



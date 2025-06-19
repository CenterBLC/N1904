<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: frame

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Semantic`](featuresbygroup.md#semantic-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`String`](featuresbydatatype.md#string-datatype)  |  [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

The verbal frames are defined as the arguments of predicates. Hence, this feature provide Semantic Role Labeling (SRL) information. The feature is called `frame` since it follows Frame Semantics. It can be used to answer questions like "Who does what to whom?".

## Feature values:

Value | Description | Frequency
---|---|---
A0 | Agent or subject of the action (prototypical agent) | 25654
A1 | Direct object or the entity directly affected by the action (prototypical patient) | 15570
A2 | Indirect object or secondary entity affected by the action (prototypical recipient) | 2577
AA2 | Adverbial roles in a sentence | 92

## Note

The following image shows a query that will return the node [id](id.md#start) of the verb and its indirect object:

<img src="images/indirectobjectquery.png" width="600">

The following image shows the first returned clause (from Matthew 1:18):

<img src="images/indirectobjecttree.png" width="600">

Edges can be traversed in both directions. For more details, see the [TF documentation on edgefeatures](https://annotation.github.io/text-fabric/tf/core/edgefeature.html).


See also related node feature [framespec](framespec.md#start).

## Source description

The `frame` feature is based on the optional XML attribute `frame` of the `w` (word) tag.


---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

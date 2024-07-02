<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>
# Nestle 1904 GNT - Feature: otype

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Grid`](featuresbygroup.md#grid-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`wg`](featuresbynodetype.md#wordgroup-nodes) [`Sentence`](featuresbynodetype.md#sentence-nodes) [`verse`](featuresbynodetype.md#verse-nodes) [`chapter`](featuresbynodetype.md#chapter-nodes) [`Book`](featuresbynodetype.md#book-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`Group`](featuresbynodetype.md#group-nodes) [`Clause`](featuresbynodetype.md#clause-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

This feature provides a mapping between node number and associated objecttype. 

## Feature values

In Text-Fabric all objects are reprented by nodes. Each node has also an objecttype, which is just a label. This mapping is performed by feature otype.

## Notes

The two main usages of this feature are:

Generating a list of nodes of a certain type, e.g. `verse` nodes:
<pre>
for verse in F.otype.s('verse'):
    "do something with verse nodes" </pre>

 Determining the node type of a node id:
 <pre>
  F.otype.v(node) </pre>
 
For a more comprehensice list of usages for feature otype, see the [documentation on special node feature otype](https://annotation.github.io/text-fabric/tf/cheatsheet.html#special-node-feature-otype).

The information on which object occupies a specific slot is stored in the edge feature [oslots](oslots.md).

## Source description

 Calculated during datacreation.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: crule

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](featuresbygroup.md#syntactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`wg`](featuresbynodetype.md#wordgroup-nodes) [`clause`](featuresbynodetype.md#clause-nodes) [`sentence`](featuresbynodetype.md#sentence-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start) 

## Feature description

The `crule` feature provides the clause rule from the XML attribute `rule`. This feature can be assigned to a `wg`, `clause`, or `sentence` node.

## Feature values

For [`sentence`](featuresbynodetype.md#sentence-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start) and  [`wg-view`](../wg-view.md#start))

Value | Description | Frequency
--- | --- | ---
ClCl | Subordinate clause follows the main clause | 619
‎ClCl2 | Subordinate clause precedes the main clause | 219
&lt;empty&gt; | No subordinate clause pressent | 18865 

For [`clause`](featuresbynodetype.md#sentence-nodes) nodes (used in [`syntax-view`](../syntax-view.md#start))

Value | Description | Frequency
--- | --- | ---
ClCl | Subordinate clause follows the main clause | 3689
‎ClCl2 | Subordinate clause precedes the main clause | 1031
&lt;empty&gt; | No subordinate clause pressent | 26094


For [`wg`](featuresbynodetype.md#wordgroup-nodes) nodes (used in [`wg-view`](../wg-view.md#start))

Value | Description | Frequency
--- | --- | ---
ClCl | Subordinate clause follows the main clause | 4308
‎ClCl2 | Subordinate clause precedes the main clause | 1250
&lt;empty&gt; | No subordinate clause pressent | 101310

## Note

See also the related feature [junction](junction.md#readme).

## Source description

The `crule` feature is taken from the optional XML attribute `rule` of the `wg` (wordgroup) tag.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

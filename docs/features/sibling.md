<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: sibling

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Relational`](featuresbygroup.md#relational-features) | [`Edge`](featuresbyfeaturetype.md#edge-features) | [`Integer`](featuresbydatatype.md#integer-datatype)  | [`word`](featuresbynodetype.md#word-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `sibling` feature represents the edge between a node and its sibling nodes, labeled with the distance between them. This feature is used to understand the sequential relationships between items with the same parent node.


## Feature value

The value of this feature is an integer indicating the distance between the current node and its  sibling.


## Notes

See also the related feature [parent](parent.md#start).

## Usage Example

A typical usage scenario for the `sibling` feature might involve querying for nodes that have specific distances between them and their  siblings.

## Data Storage

Due to the large size of the `sibling.tf` file, it is stored in a compressed format (zip file) in the usual location on GitHub, specifically in the `tf/{version}` directory. However, this feature file is also included in unzipped format the `complete.zip` file, which is part of the release. Depending on how Text-Fabric is invoked, either the `complete.zip` file is downloaded or each individual .tf file is downloaded separately. If the `complete.zip` file has not been downloaded, the `sibling.tf` file can be manually downloaded as a zip file from GitHub. After download unzip the file and store the file `sibling.tf` in the same directory as the other .tf files.



## Source description

This feature is calculated during dataset creation.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

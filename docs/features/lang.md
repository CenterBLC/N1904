<a name="start"></a>
[`Transcription`](../transcription.md#start) | [`Features`](README.md#start) | [`Viewtypes`](../viewtypes.md#start) | [`Textformats`](../textformats.md#start) |  [`Syntaxtrees`](../syntaxtrees.md#start) | [`Tutorial`](../../tutorial/README.md#start) | [`Usecases`](../usecases/README.md#start) | [`About`](../about.md#start)

# Nestle 1904 GNT - Feature: lang

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](home.md#sytactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype) | [`book`](bookgroupnodefeatures.md#readme) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `lang` feature indicates the language of the text based on [ISO 639.2](https://www.loc.gov/standards/iso639-2/php/code_list.php) language codes.

## Feature values 

Value | Description | Frequency
--- | --- | ---
[`el`](https://www.loc.gov/standards/iso639-2/php/langcodes_name.php?iso_639_1=el) | Greek | 27

## Note

The current data source contains the value `el`, which corresponds to Modern Greek (after 1453) according to ISO 639.2. However, the correct language indicator should be `grc` for Ancient Greek (before 1453).

## Source description

This feature is derived from the XML attribute `lang` of the tag `book`.

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

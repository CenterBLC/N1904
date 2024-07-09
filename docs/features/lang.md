<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: lang

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Syntactic`](home.md#sytactic-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`book`](bookgroupnodefeatures.md#readme) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description 

The `lang` feature indicates the language of the text based on [ISO 639.2](https://www.loc.gov/standards/iso639-2/php/code_list.php) language codes.

## Feature values 

Value | Description | Frequency
--- | --- | ---
[`el`](https://www.loc.gov/standards/iso639-2/php/langcodes_name.php?iso_639_1=el) | Greek | 27

## Note

The current data source contains the value `el`, which corresponds to Modern Greek (after 1453) according to ISO 639.2. However, the correct language indicator should be `grc` for Ancient Greek (before 1453).

Since this feature is only available for `book` nodes, it can not be used to identify the language of individual words. By querying feature [morph](morph.md#start) a limited set of (transliterated) Hebrew words can be identified in the Greek text, see the following snippet:

```python
Query = '''
phrase
   morph~HEBR*
'''
Results = A.search(Query)
```

To select Aramaic words, replace 'HEBR' with 'ARAM' in the above query.

## Source description

This feature is derived from the XML attribute `lang` of the tag `book`.

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*

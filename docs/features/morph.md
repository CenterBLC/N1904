<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a>  | <a href="../additions/README.md#start">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a>  | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: morhp

Feature group | Feature type | Data type | Available for node types | Used in viewtypes
---  | --- | --- | --- | ---
[`Morphological`](featuresbygroup.md#morphological-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`String`](featuresbydatatype.md#string-datatype) | [`word`](featuresbynodetype.md#word-nodes) [`subphrase`](featuresbynodetype.md#subphrase-nodes) [`phrase`](featuresbynodetype.md#phrase-nodes) | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

The `morph` feature provides the morphological tag according to Sandborg-Petersen morphology. This feature helps in understanding the morphological properties of words, such as their part of speech, tense, mood, voice, case, gender, and number.

This feature is also populated for `phrase` or `subphrase`, but only if they consist of just one `word` node.

## Feature values

Morphological tag according to Sandborg-Petersen morphology.

Some examples:
 - T-DSN decodes as [cls](cls.md#start)=determiner (here: article), [case](case.md#start)=dative, [number](number.md#start)=singular, [gender](gender.md#start)=neuter.
 - V-AAI-3S decodes as [cls](cls.md#start)=verb, [tense](tense.md#start)=aorist, [voice](voice.md#start)=active, [mood](mood.md#start)=indicative, [person](person.md#start)=third, [number](number.md#start)=singular.

 <script>
    function openMinimalWindow() {
      window.open(
        'https://centerblc.github.io/N1904/features/SP-Morph-decode.html',
        '_blank',
        'toolbar=no,location=no,status=no,menubar=no,scrollbars=yes,resizable=yes,width=450,height=400'
      );
    }
  </script>
  
<button onclick="openMinimalWindow()">Open Morph decoder</button>

## Notes

For detailed information on how to decode the feature values, see [biblicalhumanities/Nestle1904/morph/parsing.txt](https://github.com/biblicalhumanities/Nestle1904/blob/master/morph/parsing.txt).

This feature enables selection based on a wide range of grammatical properties. For example, to find all Attic words, you can use the following snippet, which utilizes a regular expression:

```python
Query = '''
word
   morph~-ATT$
'''
Results = A.search(Query)  # this yealds 117 results
```

The morphological tag also provides indication of some Hebrew and Aramaic words. See also [notes section of feature 'lang'](lang.md#note).

## Source description

This feature is derived from the XML attribute `morph` of the tag `w` (word).

---
#### *Browse all features by [name](featuresbyname.md#start), [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*


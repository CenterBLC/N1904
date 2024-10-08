<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="../features/README.md#start">Features</a> | Additions | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Add-on features

The Text-Fabric research ecosystem is open by design, allowing for the optional inclusion of additional datasets. This repository offers a set of approximately 40 add-on features, all related to word nodes. These features can be integrated with the Nestle 1904 Text-Fabric database, as they use the same node numbers for each individual word. This ensures compatibility, even though the feature values come from different data sources.

The following pages provide an overview of these add-on features:
  * [by name](featuresbyname.md#start): alphabeticaly sorted.
  * [by node type](featuresbynodetype.md#start): (only) `word`.
  * [by data type](featuresbydatatype.md#start): `string` or `integer`.
  * [by feature group](featuresbyfeaturegroup.md#start): e.g., `Bible Online Learner` or `Aland Synoptics`.
  
# Adding the features

The additional features are not loaded by default upon invocation of the Nestle 1904 Text-Fabric dataset. They need to be loaded using the 'mod' option during invocation, as shown by the following example:

```python
# load the app and data
A = use ("CenterBLC/N1904", version="1.0", mod="CenterBLC/N1904/BOLcomplement/tf/", hoist=globals())
```

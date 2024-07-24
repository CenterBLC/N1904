<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="../features/README.md#start">Features</a> | Additions | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Additions

A set of about fourty additional features are available.

Sorted by:
  * [by name](featuresbyname.md#start)
  * [by node type](featuresbynodetype.md#start)
  * [by data type](featuresbydatatype.md#start)
  * [by feature group](featuresbyfeaturegroup.md#start)
  
# Adding the features

The additional features are not loaded by default upon invocation of the Nestle 1904 Text-Fabric dataset. They need to be loaded using the 'mod' option during invocation, as shown by the following example:

```python
# load the app and data
A = use ("CenterBLC/N1904", version="1.0", mod="CenterBLC/N1904/BOLcomplement/tf/", hoist=globals())
```

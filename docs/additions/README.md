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

By default, the additional features of the Nestle 1904 Text-Fabric dataset are not loaded. To include them, use the `mod` option during invocation, as shown below:

```python
# Load the app and data with additional features
A = use ("CenterBLC/N1904", version="1.0.0", mod="CenterBLC/N1904/BOLcomplement/tf/", hoist=globals())
```

To use this functionality, the Text-Fabric package must support downloading files from GitHub. If it was installed without GitHub functionality, you might encounter the following error when trying to load the additional features:

```
The requested data is not available offline
	~/text-fabric-data/github/CenterBLC/N1904/BOLcomplement/tf/1.0.0 not found
Backend provider github not supported.
Cannot reach online data on github
Try installing text-fabric one of the following:
pip install text-fabric[github]
pip install text-fabric[all]
```

To resolve this issue, ensure that GitHub support is added to Text-Fabric by running:

```
!pip install text-fabric[github]
```

Since GitHub implemented a API rate limit of 60 requests per hour, it is recommended to use a personal access token to increase this rate limit. Refer to the following resources for guidance:
- [Jupyter Notebook: Increase GitHub API Rate Limit](https://nbviewer.org/github/CenterBLC/N1904/blob/main/docs/tutorial/Increase_GitHub_rate_limit.ipynb)
- [Text-Fabric Documentation: Using GitHub Tokens](https://annotation.github.io/text-fabric/tf/advanced/repo.html#token-in-environment-variables)

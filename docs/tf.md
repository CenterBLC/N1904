<a name="start"></a>
<div class="hidden-content"> <a href="transcription.md#start">
Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="additions/README.md#start">Additions</a> | <a href="viewtypes.md#start">Viewtypes</a> | <a href="textformats.md#start">Textformats</a> |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="tutorial/README.md#start">Tutorial</a> | <a href="about.md#start">About</a>
</div>

# Nestle 1904 GNT - About Text-Fabric

Text-Fabric is a powerful Python library and framework designed to facilitate the analysis and manipulation of large-scale textual data, particularly in the context of ancient languages and biblical texts. It provides a comprehensive set of tools for processing and querying structured text data efficiently. Text-Fabric was developed by [Dirk Roorda](https://github.com/dirkroorda). The software package is accessible at [https://github.com/annotation/text-fabric](https://github.com/annotation/text-fabric).

## Data model

Text-Fabric, as its name suggests, employs a 'warp and weft' concept inspired by textile weaving. The 'warp' represents foundational structured data, like words, phrases, and clauses, depicted as nodes, while the 'weft' adds layers of information—features like lexical, morphological, or syntactic data. By weaving these features with the nodes, TF maintains a clear separation between structure and content.

TF's data model is structured as a graph of nodes, each identified by a node type (a string) and a corpus wide unique sequence number (an integer). Nodes support two feature types: ['node features'](features/featuresbyfeaturetype.md#node-features) providing information about individual nodes, while ['edge features'](featuresbyfeaturetype.md#edge-features) define relationships or links between nodes. Each feature's data is stored in separate plain text files, resulting in a flat data structure. This design enables multiple formats for displaying corpus text and allows unlimited annotation depth.

The TF Python package provides an [Application Programming Interface](https://annotation.github.io/text-fabric/tf/cheatsheet.html) (API) for accessing and manipulating corpus-specific data, making it easy to integrate with other analytical tools. Given Python's prominence in Biblical and Digital Humanities research, TF is a fitting choice. Users can load additional feature sets, provided they align at the node level, allowing for queries beyond existing annotations. For example, this TF dataset was enhanced with features like [Bible Online Learner (BibleOL)](additions/featuresbyfeaturegroup.md#bible-online-learner) data and [Aland's synoptic parallel data](additions/featuresbyfeaturegroup.md#aland-synoptics),  enabling more comprehensive analysis.


## Functions

The main functionalities of Text-Fabric include:

* **Data Conversion:** Text-Fabric allows users to convert and import various text formats (e.g., XML, CSV, plain text) into a unified, efficient data format optimized for large-scale text analysis.

* **Data Organization:** Text-Fabric organizes the textual data into a graph-like data model. This data model represents the text as a network of interconnected nodes, where nodes can represent words, phrases, sentences, or any other linguistic unit, and edges represent relationships between these units.

* **Text Annotation:** It enables users to add annotations or metadata to the text, providing additional information about the linguistic units, such as part-of-speech tags, lemma, morphological data, or any other attributes relevant to the analysis.

* **Querying and Filtering:** Text-Fabric allows users to perform complex queries and filters on the text data. These template based queries enable researchers to extract specific linguistic patterns, search for particular words or phrases, or find instances that match certain criteria.

* **Computational Analysis:** The library supports a wide range of computational linguistic operations, such as concordance analysis, collocation analysis, frequency distributions, and other statistical analyses to gain insights into the text.

* **Interoperability:** Text-Fabric provides seamless integration with other popular Python libraries, such as [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/), or [NetworkX](https://networkx.org/), enabling users to leverage additional data analysis capabilities.

* **Exporting and Serialization:** After analyzing the data, Text-Fabric allows users to export the results into various formats or serialize the processed data for future use.

Detailed information regarding Text-Fabric can be found at:
* [Text-Fabric Package description](https://annotation.github.io/text-fabric/tf/index.html)


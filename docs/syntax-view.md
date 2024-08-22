<a name="start"></a>
<div class="hidden-content">
<a href="transcription.md">Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="additions/README.md#start">Additions</a> |  Viewtypes | <a href="textformats.md#start">Textformats</a> |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="tutorial/README.md#start">Tutorial</a> | <a href="about.md#start">About</a>
</div>

# Nestle 1904 GNT - Viewtype: syntax-view

The syntax viewtype displays the syntax tree using separate node types for clauses, phrases and subphrases, while annotiting them with terms common for linguistic research. This is the default viewtype, so it is automaticaly set upon invocation of the TF dataset.

Swithing to a specific viewtype can be done by providing the proper argument to command A.viewtype(). This command is specific to this dataset and automaticaly loaded upon invocation of the TF dataset.

The relation between node types and view types is shown in the following table.

Viewtype | Invocation | Associated node types | 
--- | --- | ---
[`wg-view`](wg-view.md#start) | A.viewtype('wg') |  [`wg`](features/featuresbynodetype.md#wordgroup-nodes) 
`syntax-view` (this view) | A.viewtype('syntax') | [`subphrase`](features/featuresbynodetype.md#subphrase-nodes) [`phrase`](features/featuresbynodetype.md#phrase-nodes) [`clause`](features/featuresbynodetype.md#clause-nodes) [`group`](features/featuresbynodetype.md#group-nodes)

<sup>Note: the node types  [`Word`](features/featuresbynodetype.md#word-nodes), [`Sentence`](features/featuresbynodetype.md#sentence-nodes), [`verse`](features/featuresbynodetype.md#verse-nodes), [`chapter`](features/featuresbynodetype.md#chapter-nodes), and [`Book`](features/featuresbynodetype.md#book-nodes) are common for both views.</sup>

The following features are created to be specificaly used in this viewtype:

* [function](features/function.md#start): syntactic functions
* [sp](features/sp.md#start): part-of-speech (POS)


The following images show John 1:1 using the syntas-view:

<img src="features/images/John_1_1_syntax-view.png" width="650">

Note that for some features from the wg-view, such as cls, junction, role, rule, and type, are shown in parallel to the syntax-view information on the right side of the symbol \\, while on the left side, it shows the values of the features typ, function, and rela.

### Impact on using parent and sibling feature 

Understanding the distinctions between these views is especialy important when building queries that involve parent-child relations. E.g. when using the edge features [parent](features/parent.md#start) and [sibling](features/sibling.md#start). See following image for details:

<img src="features/images/wordgroup_syntactic_view.png" width="600">

This image compares the parent (arrows) and sibling features (connector with circle) for the first phrase of the book of John (John 1:1) for the [WordGroup view](wg-view.md#start) and the Syntax view for the data. The parent feature for a specific node can be obtained using *E.parent.f(node)* and the sibling feature can be calculated using *E.sibling.b(node)*, where node stands for the number of the node. The direction of the arrow indicates the parent node of a given node. The dotted lines indicate that the [`wg`](features/featuresbynodetype.md#wordgroup-nodes) nodes share the same data as the [`sentence`](features/featuresbynodetype.md#sentence-nodes), [`clause`](features/featuresbynodetype.md#clause-nodes), and [`phrase`](features/featuresbynodetype.md#phrase-nodes). The [`subphrase`](features/featuresbynodetype.md#subphrase-nodes), [`verse`](featuresbynodetype.md#verse-nodes), and [`chapter`](features/featuresbynodetype.md#chapter-nodes) nodes are not nested in the calculation of the parent and sibling features.

## Implementatation

The following actions are performed when the command A.viewtype('syntax') is issued:
  * wg (wordgroup) node types will be hidden.
  * The label for sentence nodes is updates with features matching a syntax view
  * The display parameter 'condensed' is set to True and 'queryFeatures' to False, respectively.

The code for the A.viewtype() command is located in file [app.py](../app/app.py). 

In this file, the line 'app.viewtype('syntax')' within the \__init__() function is called after loading all corpus data and creating the API object, to set the default viewtype to 'syntax'.

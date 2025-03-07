<a name="start"></a>
<div class="hidden-content">
<a href="transcription.md">Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="additions/README.md#start">Additions</a> | <a href="viewtypes.md#start">Viewtypes</a> | <a href="textformats.md#start">Textformats</a> |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="tutorial/README.md#start">Tutorial</a> | About
</div>

# Nestle 1904 GNT - About

## This Text-Fabric dataset

This is the [Text-Fabric](tf.md#start) version of the Nestle 1904 Greek New Testament (seventh edition: reprint 1913), containing the Greek text augmented with linguistic annotations. This Text-Fabric dataset was created by the 'N1904-TF Conversion Project,' a collaboration between the [Eep Talstra Centre for Bible and Computer (ETCBC)](https://github.com/ETCBC/) at the Vrije Universiteit (VU) Amsterdam, Netherlands, and the [Center of Biblical Languages and Computing (CBLC)](https://github.com/CenterBLC/) at Andrews University, Berrien Springs, MI, USA.

### The Text-Fabric research ecosystem

Text-Fabric, as described by its developer [Dirk Roorda](https://github.com/dirkroorda), is a "data model, a file format, and a tool on the one hand, and a strategy, even an ethos on the other hand."<sup>1</sup>  The Text-Fabric framework is designed to facilitate the analysis and manipulation of large-scale textual data, particularly in the context of ancient languages and biblical texts. The engine of Text-Fabric is its powerful Python library, which provides a comprehensive set of tools for processing and querying structured text data efficiently. The software package is accessible at [https://github.com/annotation/text-fabric](https://github.com/annotation/text-fabric).

A brief functional overview of Text-Fabric functions can be found [here](tf.md#start). 

More detailed information regarding Text-Fabric can be found in its [package description](https://annotation.github.io/text-fabric/tf/index.html).

### License

> Copyright (c) 2024 Center of Biblical Languages and Computing (CBLC).
For licence details [see here](https://github.com/CenterBLC/N1904/blob/main/LICENSE.md).

### Citation

When citing this dataset, please include reference to the DOI (either the generic or release specific). For example:

> Tony Jurg, Saulo de Oliveira Cantanhêde, & Oliver Glanz.  (2024). *CenterBLC/N1904: Nestle 1904 Text-Fabric data*. Zenodo. [DOI: 10.5281/zenodo.13117911](https://doi.org/10.5281/zenodo.13117911).

## Provenance

### The Nestle text

This Text-Fabric dataset is based upon the Greek New Testament, edited by Eberhard Nestle, published in 1904 by the British and Foreign Bible Society. See [here](https://archive.org/details/the-greek-new-testament-nestle-1904-us-edition/mode/2up) a scan of the orginal publication: Nestle, Eberhard. *Η Καινή Διαθήκη Novum Testamentum Graece* (New York: Fleming H. Revell Company, 1904).  The 1913 reprint is available [here](https://archive.org/details/hkainediathekete00lond/). Transcription by [Diego Santos](https://sites.google.com/site/nestle1904/home), morphology by Ulrik Sandborg-Petersen, markup by Jonathan Robie. 

It is worth noting that the current standard version used in academic settings is the [Nestle-Aland edition 28](https://www.academic-bible.com/en/online-bibles/novum-testamentum-graece-na-28/read-the-bible-text/). Despite this, the Nestle 1904 provided by this Text-Fabric implementation, is the closest version in terms of the ‘principal text’ available in the public domain which is suitable to perform syntactical analysis.

### MACULA Greek Linguistic Datasets

The Text-Fabric files were created based upon the LowFat trees XML files. The source data for the conversion are the XML node files representing the macula-greek version of the Nestle Aland 1904 Greek New Testment.  The most recent source data for the "MACULA Greek Linguistic Datasets is available at [Clear-Bible Github](https://github.com/Clear-Bible/macula-greek/tree/main/Nestle1904/lowfat).
This source dataset includes data from:

1. [Nestle1904](https://github.com/biblicalhumanities/Nestle1904) Greek New Testament, edited by Eberhard Nestle, published in 1904 by the British and Foreign Bible Society. Transcription by Diego Santos, morphology by Ulrik Sandborg-Petersen, markup by Jonathan Robie.
2.  **_Syntax trees_** developed by Clear Bible, Inc.
3. **_English glosses_** from the Berean Study Bible
4. **_Word sense data_** from the United Bible Societies [MARBLE](https://semanticdictionary.org/) project, based on Louw & Nida's semantic domains.
5. **_Semantic roles_**: Who does what to whom? (Agent, Verb, Patient …)
6. **_Participant referents_**: Who is “he,” “she,” or “it” in this sentence?

## Footnotes

> <sup>1</sup> Dirk Roorda. "Coding the Hebrew Bible" in *Research Data Journal for the Humanities and Social Sciences Volume 3: Issue 1*, 30 [DOI: 10.1163/24523666-01000011](https://doi.org/10.1163/24523666-01000011)

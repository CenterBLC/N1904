<a name="start"></a>
<div class="hidden-content">
<a href="transcription.md">Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="viewtypes.md#start">Viewtypes</a> | Textformats |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="about.md#start">About</a>
</div>

# Nestle 1904 GNT - Textformats 

Text-Fabric's data design allows for flexible representation of the corpus text but requires at least one text format to be specified as its default (in this dataset: text-orig-full). During the creation of the dataset, additional formats relevant to this corpus were defined, which are basically based on a subset of the following surface text-related features:

   * [after](features/after.md#start): All material found after a word.
   * [before](features/before.md#start): All material found before a word.
   * [criticalsign](features/criticalsign.md#start): Text-critical signs.
   * [normalized](features/normalized.md#start): Normalized Greek text.
   * [punctuation](features/punctuation.md#start): Punctuations found after a word.
   * [text](features/text.md#start): Word without punctuations and text-critical signs.
   * [translit](features/translit.md#start): Transliteration of the word surface texts.
   * [unaccent](features/unaccent.md#start): word without accents and diacritical markers.
   * [unicode](features/unicode.md#start): Unicode presentation including all material before and after word.

The relation between these features in relation to the surface text is shown in the following image.

<img src="features/images/details_surface_features.png" width="400" >

The text formats in this Text-Fabric database are identified by unique names that reflect their actual formats. These names follow a structured naming schema, consisting of a string of keywords separated by hyphens (-).

```
 `what`-`how`-`fullness`
```

In our database the following keywords are used:

keyword	| value | meaning
--- | --- | ---
what | text | words as they belong to the text
what | lex | lexemes of the words
how	| orig | the original Greek script (all Unicode)
how	| unaccent | the original Greek script without accents
how	| translit | transliteration into latin alphabeth
fullness | full |	complete text with text-critical markers
fullness | plain | complete text without text-critical markers

Not all possible combinations are defined or relevant. The following text-formatting options are defined:

Format | Usage | Template
--- | --- | ---
lex-orig-plain | Lexemes of the Greek surface text | {[lemma](features/lemma.md#start)}{[punctuation](features/punctuation.md#start)}
lex-translit-plain | Transliteration of the lexemes of the Greek surface text | {[lemmatranslit](features/lemmatranslit.md#start)}{[punctuation](features/punctuation.md#start)}
text-orig-full (default) | The Greek surface text in unicode including text-critical markers | {[before](features/before.md#start)}{[text](features/text.md#start)}{[after](features/after.md#start)}
text-orig-plain | The Greek surface text in unicode | {[text](features/text.md#start)}{[punctuation](features/punctuation.md#start)}
text-translit-plain | Transliteration of the Greek surface text | {[translit](features/translit.md#start)}{[punctuation](features/punctuation.md#start)}
text-unaccent-plain | The Greek surface text in unicode without accents | {[unaccent](features/unaccent.md#start)}{[punctuation](features/punctuation.md#start)}

Each text format is implemented as a template that maps the format to individual features. This mapping can be easily checked using the following command: A.showFormats().

## Example

This example illustrates how the different formats in this dataset affect the presentation of Mark 1:1.

```
# note: node 383782 is of type 'verse' and associated to Mark 1:1 
for formats in T.formats:
    print(f'fmt={formats}\t: {T.text(383782,formats)}')
fmt=lex-orig-plain       : ἀρχή ὁ εὐαγγέλιον Ἰησοῦς Χριστός υἱός θεός.
fmt=lex-translit-plain   : arkhe o euaggelion Iesous Khristos uios theos.
fmt=text-orig-full       : Ἀρχὴ τοῦ εὐαγγελίου Ἰησοῦ Χριστοῦ (Υἱοῦ Θεοῦ).
fmt=text-orig-plain      : Ἀρχὴ τοῦ εὐαγγελίου Ἰησοῦ Χριστοῦ Υἱοῦ Θεοῦ.
fmt=text-translit-plain  : Arkhe tou euaggeliou Iesou Khristou Uiou Theou.
fmt=text-unaccent-plain  : Αρχη του ευαγγελιου Ιησου Χριστου Υιου Θεου.
```

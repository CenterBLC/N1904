<a name="start"></a>
<div class="hidden-content"> <a href="transcription.md#start">
Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="additions/README.md#start">Additions</a> | <a href="viewtypes.md#start">Viewtypes</a> | <a href="textformats.md#start">Textformats</a> |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="tutorial/README.md#start">Tutorial</a> | <a href="about.md#start">About</a>
</div>

# Nestle 1904 GNT - Character encoding

A computer cannot interpret text without first converting it into a binary format. Historically, this was done using ASCII, which mapped Latin characters to 7-bit codes. Various schemes existed for encoding characters in non-Latin languages, such as Greek. To standardize the encoding of these non-Latin characters, Unicode was introduced. This standardization aims to ensure full portability of text across computers with different operating systems. All Greek text in this Text-Fabric dataset has been encoded in Unicode.

However, in practice, this is not without complications, especially for languages, like Greek, that use characters augmented with polytonic accents. These complexities can lead to inconsistencies in text representation and processing.

The information on this page in particular pertains to the following base features:

* [lemma](features/lemma.md#start): Lexical lemma (cf. BDAG).
* [normalized](features/normalized.md#start): Normalized form of the 
* [text](features/text.md#start): Word as it appears in the text.
* [unicode](features/unicode.md#start): Word in unicode format.
surface text.

The information is also relevant to the following [add-on features](..additions/README.md#start):

* [bol_lemma](additions/bol_lemma.md#start): Bible Online Learner (BOL) based lexeme.
* [bol_lemma_dict](additions/bol_lemma_dict.md#start): BOL based lexeme as it appears in the dictionary.
* [bol_surface](additions/bol_surface.md#start): BOL based word as it appears in the text.
* [lemma_dict](additions/lemma_dict.md#start): Lexeme as it appears in the dictionary.

# Unicode related matters of concern

## Background

The unicode, text, after, before, and punctuation data were encoded using polytonic accents over the vowels (oxia, varia, and perispomeni). For instance, considering the vowel η, we have, respectively, ή (U+1F75), ὴ (U+1F74), and ῆ (U+1F74). However, since 1982, in Modern Greek, polytonic accents should be replaced by the monotonic accent tonos ◌̍ (U+030D). Later, in 1986, the Greek government decreed that the tonos be represented as the acute accent ◌́ (U+0301).84 Therefore, it is not possible to distinguish visually the difference between the characters with tonos or the acute accent in the writing of ancient Greek. 

Unicode has two ways of representing a character: decomposed  and precomposed characters. For instance, the decomposed character ά (U+03AC, Greek small letter alpha with tonos) can be rendered by the character α (U+03B1) and the acute accent ◌́ (U+0301), or by equivalence, the precomposed character ά (U+1F71, Greek small letter alpha with oxia). Both of them should be rendered the same way. 

## Translation in this Text-Fabric dataset

However, TF makes a distinction between those characters. This issue due to the codification of characters is revealed, especially during the search for words in TF. A user can copy a Greek word for a search, and it does not appear in the results just because of the difference in the representation of characters.85 Therefore, we updated nine characters (ά, έ, ή, ί, ΐ, ό, ύ, ΰ, ώ) of the unicode, text, normalized, and lemma features using precomposed characters, as shown in the following table. 

Character | Unicode decomposed character (with acute accent) | Unicode precomposed character (with oxia) 
--- | --- | ---
ά | [U+03AC](https://www.codetable.net/hex/3ac) | [U+1F71](https://www.codetable.net/hex/1f71)
έ | [U+03AD](https://www.codetable.net/hex/3ad) | [U+1F73](https://www.codetable.net/hex/1f73)
ή | [U+03AE](https://www.codetable.net/hex/3ae) | [U+1F75](https://www.codetable.net/hex/1f75)
ί | [U+03AF](https://www.codetable.net/hex/3af) | [U+1F77](https://www.codetable.net/hex/1f77)
ΐ | [U+0390](https://www.codetable.net/hex/390) | [U+1FD3](https://www.codetable.net/hex/1fd3)
ό | [U+03CC](https://www.codetable.net/hex/3cc) | [U+1F79](https://www.codetable.net/hex/1f79)
ύ | [U+03CD](https://www.codetable.net/hex/3cd) | [U+1F78](https://www.codetable.net/hex/1f78)
ΰ | [U+038E](https://www.codetable.net/hex/38e) | [U+1FE3](https://www.codetable.net/hex/1fe3)
ώ | [U+03CE](https://www.codetable.net/hex/3ce) | [U+1F7D](https://www.codetable.net/hex/1f7d)



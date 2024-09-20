<a name="start"></a>
<div class="hidden-content"> <a href="transcription.md#start">
Transcription</a> | <a href="features/README.md#start">Features</a> | <a href="additions/README.md#start">Additions</a> | <a href="viewtypes.md#start">Viewtypes</a> | <a href="textformats.md#start">Textformats</a> |  <a href="syntaxtrees.md#start">Syntaxtrees</a> | <a href="tutorial/README.md#start">Tutorial</a> | <a href="about.md#start">About</a>
</div>

# Nestle 1904 GNT - Character encoding

A computer cannot interpret text without first converting it into a binary format. Historically, this was done using ASCII, which mapped Latin characters to 7-bit codes. Various schemes existed for encoding characters in non-Latin languages, such as Greek. To standardize the encoding of these non-Latin characters, Unicode was introduced. This standardization aims to ensure full portability of text across computers with different operating systems. All Greek text in this Text-Fabric dataset has been encoded in Unicode.

However, in practice, this is not without complications, especially for languages, like Greek, that use characters augmented with polytonic accents. These complexities can lead to inconsistencies in text representation and can lead to errors in querie results when working with the dataset.

The information on this page in particular pertains to the following base features:

* [lemma](features/lemma.md#start): Lexical lemma (cf. BDAG).
* [normalized](features/normalized.md#start): Normalized form of the 
* [text](features/text.md#start): Word as it appears in the text.
* [unicode](features/unicode.md#start): Word in unicode format.
surface text.

The information is also relevant to the following [add-on features](additions/README.md#start):

* [bol_lemma](additions/bol_lemma.md#start): Bible Online Learner (BOL) based lexeme.
* [bol_lemma_dict](additions/bol_lemma_dict.md#start): BOL based lexeme as it appears in the dictionary.
* [bol_surface](additions/bol_surface.md#start): BOL based word as it appears in the text.
* [lemma_dict](additions/lemma_dict.md#start): Lexeme as it appears in the dictionary.

# All used special characters

To view all the special characters used in this dataset, run the following command (e.g., in a Jupyter Notebook cell):

```python
A.specialCharacters()
```
This command will return the following details:

<pre>
<b>Special characters in</b> text-orig-full

· Α α ὰ ά ᾴ ἀ Ἀ ἂ ἄ Ἄ ᾄ ἆ Ἆ ἁ Ἁ ἃ Ἃ ἅ Ἅ ᾶ ᾷ ᾳ Β β Γ γ Δ δ Ε ε ὲ έ ἐ Ἐ ἔ Ἔ ἑ Ἑ ἓ Ἓ ἕ Ἕ Ζ ζ Η η ὴ
ή ῄ ἠ Ἠ ἢ Ἢ ἤ Ἤ ᾔ ἦ Ἦ ᾖ ᾐ ἡ ἣ ἥ Ἥ ἧ ᾗ ᾑ ῆ ῇ ῃ Θ θ Ι ι ὶ ί ϊ ῒ ΐ ἰ Ἰ ἴ Ἴ ἶ ἱ Ἱ ἳ ἵ Ἵ ἷ ῖ Κ κ Λ λ 
Μ μ Ν ν Ξ ξ Ο ο ὸ ό ὀ Ὀ ὂ ὄ Ὄ ὁ Ὁ ὃ Ὃ ὅ Ὅ Π π Ρ ρ ῥ Ῥ Σ ς σ Τ τ Υ υ ὺ ύ ϋ ῢ ΰ ὐ ὒ ὔ ὖ ὑ Ὑ ὓ ὕ Ὕ 
ὗ Ὗ ῦ Φ φ Χ χ Ψ ψ Ω ω ὼ ώ ῴ ὠ ὢ ὤ Ὤ ὦ Ὦ ᾠ ὡ Ὡ ὥ Ὥ ὧ Ὧ ᾧ ῶ ῷ ῳ — ’
</pre>

These characters can be used directly to build queries without the need to look up Unicode codepoints.

# Unicode related matters of concern

## Example of Unicode related mismatches 

There are some differences in Unicode encoding between the base features and certain add-on BOL features, particularly concerning homoglyphs—characters that look identical or very similar but have different Unicode values. These subtle differences can be difficult to spot on screen. However, using a small Python script, these distinctions can be revealed, such as in the word θεὸς in Romans 1:19. This following code snippet identifies the Unicode code points for each character in that word.

```python
for char in item:    # stores the unicode encoded string
    print(f"Character: '{char}'\tUnicode Code Point: {ord(char)}")
```
The Python code prints the following for the base data:
<pre>
Character: 'θ'	Unicode Code Point: 952
Character: 'ε'	Unicode Code Point: 949
Character: 'ό'	Unicode Code Point: 972
Character: 'ς'	Unicode Code Point: 962
</pre>
The Python code prints the following for the BOL based feature, where the differences are highlighted:
<pre>
Character: 'Θ'	Unicode Code Point: <span style="background-color: yellow;">920</span>
Character: 'ε'	Unicode Code Point: 949
Character: 'ό'	Unicode Code Point: <span style="background-color: yellow;">8057</span>
Character: 'ς'	Unicode Code Point: 962
</pre>

See also the following [notebook](https://nbviewer.org/github/tonyjurg/Nestle1904LFT/blob/main/add_features/verify_BOL_against_LFT.ipynb).

## Background

The [unicode](features/unicode.md#start), [text](features/text.md#start), [after](features/after.md#start), [before](features/before.md#start), and [punctuation](features/punctuation.md#start) features were encoded using polytonic accents over the vowels (oxia, varia, and perispomeni). For instance, considering the vowel η, we have, respectively, ή [(U+1F75)](https://www.codetable.net/hex/1f75), ὴ [(U+1F74)](https://www.codetable.net/hex/1f75), and ῆ [(U+1FC6)](https://www.codetable.net/hex/1fc6). However, since 1982, in Modern Greek, polytonic accents should be replaced by the monotonic accent tonos ◌̍  [(U+030D)](https://www.codetable.net/hex/30d). Later, in 1986, the Greek government decreed that the tonos be represented as the acute accent ◌́ (U+0301). Therefore, it is not possible to distinguish visually the difference between the characters with tonos or the acute accent in the writing of ancient Greek. 

Unicode has two ways of representing a character: decomposed  and precomposed characters. For instance, the decomposed character ά (U+03AC, Greek small letter alpha with tonos) can be rendered by the character α (U+03B1) and the acute accent ◌́ (U+0301), or by equivalence, the precomposed character ά (U+1F71, Greek small letter alpha with oxia). Both of them should be rendered the same way. 

## Transcription in this Text-Fabric dataset

However, Python, like any other programming language, performs binary comparisons, which means it distinguishes between characters based on their exact Unicode values. This distinction becomes particularly evident when executing queries in Text-Fabric. For example, a user might copy a Greek word for a search, only to find no results because of subtle differences in character encoding. Therefore, we updated nine characters (ά, έ, ή, ί, ΐ, ό, ύ, ΰ, ώ) of the unicode, text, normalized, and lemma features using precomposed characters, as shown in the following table. 

Character | Unicode decomposed character (with acute accent) | Unicode precomposed character (with oxia) | Character name 
--- | --- | --- | ---
ά | [U+03AC](https://www.codetable.net/hex/3ac) | [U+1F71](https://www.codetable.net/hex/1f71) | Small letter alpha with tonos
έ | [U+03AD](https://www.codetable.net/hex/3ad) | [U+1F73](https://www.codetable.net/hex/1f73) | Small letter epsilon with tonos
ή | [U+03AE](https://www.codetable.net/hex/3ae) | [U+1F75](https://www.codetable.net/hex/1f75) | Small letter eta with tonos
ί | [U+03AF](https://www.codetable.net/hex/3af) | [U+1F77](https://www.codetable.net/hex/1f77) | Small letter iota with tonos
ΐ | [U+0390](https://www.codetable.net/hex/390) | [U+1FD3](https://www.codetable.net/hex/1fd3) | Small letter iota with dialytika and tonos
ό | [U+03CC](https://www.codetable.net/hex/3cc) | [U+1F79](https://www.codetable.net/hex/1f79) | Small letter omicron with tonos
ύ | [U+03CD](https://www.codetable.net/hex/3cd) | [U+1F78](https://www.codetable.net/hex/1f78) | Small letter upsilon with tonos
ΰ | [U+038E](https://www.codetable.net/hex/38e) | [U+1FE3](https://www.codetable.net/hex/1fe3) | Small letter upsilon with dialytika and oxia
ώ | [U+03CE](https://www.codetable.net/hex/3ce) | [U+1F7D](https://www.codetable.net/hex/1f7d) | Small letter omega with tonos

## More information on Unicode

* Information on Unicode usage is available in [The Unicode Cookbook for Linguists](https://langsci-press.org/catalog/book/176/).
* [Unicode Group 'Greek Extended' (codetable.net)](https://www.codetable.net/Group/greek-extended).


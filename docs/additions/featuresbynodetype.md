<a name="start"></a>
<div class="hidden-content"><a href="../transcription.md">Transcription</a> | <a href="../features/README.md#start">Features</a> | <a href="README.md">Additions</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../tutorial/README.md#start">Tutorial</a>  | <a href="../about.md#start">About</a></div>

# Nestle 1904 GNT - Optional features (grouped by node type)

#### *Or browse by [name](featuresbyname.md#start), [data type](featuresbydatatype.md#start), or [feature group](featuresbyfeaturegroup.md#start)*

Note: These features are not loaded by default and must be invoked using the mod option when initializing the TF dataset. For more details, refer to this [guide](../additions#adding-the-features).

## word

Feature|Feature type|Data type|Description|Examples
---|---|---|---|---
[`AU_declension`](AU_declension.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Andrews University declension selection for exercises|<span>` `</span> `2nd` `3rd` `1st`
[`AU_exercise_selection`](AU_exercise_selection.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Andrews University declension selection for exercises|<span>` `</span> `NTST551_no1`
[`AU_vocab_builder_chapter`](AU_vocab_builder_chapter.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Andrews University vocab builder booklet chapter|`1a` `1b` `absent` `1c`
[`AlandSynopChapter`](AlandSynopChapter.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Aland Synoptic Parallel Chapter|<span>` `</span> `Jesus’ Ministry in Galilee Continued` `The Passion Narrative` `Last Journey to Jerusalem (According to Luke)`
[`AlandSynopChapterNr`](AlandSynopChapterNr.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|Aland Synoptic Parallel Number|`8` `16` `10` `13`
[`AlandSynopEvent`](AlandSynopEvent.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Aland Synoptic Parallel Event|<span>` `</span> `Jesus before the Sanhedrin (Peter’s Denial)` `The Healing at the Pool` `Jairus’ Daughter and the Woman with a Hemorrhage`
[`AlandSynopEventNr`](AlandSynopEventNr.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|Aland Synoptic Parallel Event|`332` `141` `95` `146`
[`AlandSynopNo`](AlandSynopNo.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Aland Synoptic Parallel Number|<span>` `</span> `8` `16` `10`
[`BGVB`](BGVB.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Chapter categoried vocab as it appears in Larry Richards Textbook "Learning Greek in 30 days"|`1a` `1b` `0` `1c`
[`abc_order`](abc_order.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|The dictionary position of a given word|`3418` `2493` `835` `4575`
[`bol_case`](bol_case.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based case|<span>` `</span> `nominative` `accusative` `genitive`
[`bol_dict_abc`](bol_dict_abc.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based dictionary position of a given word|`3438` `2506` `839` `4603`
[`bol_frequency_rank`](bol_frequency_rank.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|BibleOL based frequency rank of a given lexeme|`1` `2` `3` `4`
[`bol_gender`](bol_gender.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based gender|<span>` `</span> `masculine` `feminine` `neuter`
[`bol_gloss_EN`](bol_gloss_EN.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based English gloss|`the` `and, even, also, namely` `he, she, it, they, them, same` `you`
[`bol_gloss_PT`](bol_gloss_PT.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based Portuguese gloss|`a, o, as, os` `e, até mesmo, também, nomeadamente` `ele, ela, eles, elas, mesmo, mesma` `tu`
[`bol_lemma`](bol_lemma.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based lexeme|`ὁ` `καί` `αὐτός` `σύ`
[`bol_lemma_dict`](bol_lemma_dict.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based lexeme as it appears in the dictionary|`ὁ, ἡ, τό` `καί` `αὐτός, -ή, -ό` `σύ`
[`bol_lemma_occ`](bol_lemma_occ.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|BibleOL based number of occurence of a given lexeme|`19783` `8978` `5550` `2892`
[`bol_monad_num`](bol_monad_num.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based word order within corpus|`1` `10` `100` `1000`
[`bol_mood`](bol_mood.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based mood|<span>` `</span> `indicative` `participle` `infinitive`
[`bol_noun_declension`](bol_noun_declension.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based noun declension|<span>` `</span> `second_d` `third_d` `first_alpha_macron`
[`bol_noun_stem`](bol_noun_stem.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based noun stem/noun_type|<span>` `</span> `omicron` `alpha` `tau`
[`bol_number`](bol_number.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based number|`singular` <span>` `</span> `plural`
[`bol_person`](bol_person.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based person|<span>` `</span> `third_person` `second_person` `first_person`
[`bol_possessor_number`](bol_possessor_number.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based number of posessor|<span>` `</span> `singular` `plural`
[`bol_psp`](bol_psp.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based part of speech|`noun` `verb` `prep` `art`
[`bol_ref`](bol_ref.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based Bible reference|`Rev 20:4` `Rev 3:12` `Rev 5:13` `Rev 9:20`
[`bol_suffix`](bol_suffix.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based suffix|<span>` `</span> `negative` `comparative` `superlative`
[`bol_surface`](bol_surface.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based word as it appears in the text|`καὶ` `ὁ` `ἐν` `δὲ`
[`bol_tense`](bol_tense.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based tense|<span>` `</span> `present` `aorist` `second_aorist`
[`bol_verb_type`](bol_verb_type.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based verb_type|<span>` `</span> `epsilon` `irregular` `gamma`
[`bol_voice`](bol_voice.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|BibleOL based voice|<span>` `</span> `active` `middle_or_passive` `middle_or_passive_deponent`
[`clause_number`](clause_number.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|Clause number|`4040` `10990` `5327` `16796`
[`gloss_BGVB`](gloss_BGVB.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|English gloss|`the` `and, also, likewise` `he, she, it, himself, herself, itself; even, very; same` `you`
[`lemma_dict`](lemma_dict.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Lexeme as it appears in the dictionary|`ὁ, ἡ, τό` `καί` `αὐτός, -ή, -ό` `σύ`
[`lemma_noaccent`](lemma_noaccent.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Lemma stripped of accents|`ο` `και` `αυτος` `συ`
[`lemma_translit`](lemma_translit.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Lexeme transliterated|`o` `kai` `autos` `su`
[`normalized_noaccent`](normalized_noaccent.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Surface word stripped of punctations and accents|`και` `ο` `δε` `εν`
[`sentence_number`](sentence_number.md#start)|[`Node`](featuresbynodetype.md#Node)|[`Integer`](featuresbydatatype.md#Integer)|Sentence number|`2288` `7536` `7232` `7229`
[`vocab_ReadGreekin30Days`](vocab_ReadGreekin30Days.md#start)|[`Node`](featuresbynodetype.md#Node)|[`String`](featuresbydatatype.md#String)|Chapter categoried vocab as it appears in Larry Richards Textbook "Learning Greek in 30 days"|`3a` <span>` `</span> `3b` `4b`

#### *Or browse by [name](featuresbyname.md#start), [data type](featuresbydatatype.md#start), or [feature group](featuresbyfeaturegroup.md#start)*

# andi-dicts

This repository contains a digitalized version of Andi dictionary from (Kibrik, Kodzasov, 1990) [1]. It was made by Valeria Buntiakova (NRU HSE, valleriabun@gmail.com) as a part of course paper "Morphological Parser of Andi in lexd and twol". (Main repository of the project: https://github.com/vbunt/andi)

Nouns, adjectives and adverbs were digitalized. Latin script follows [2], cyrillic script follows [3]. Every entry consists of _id_ in the dictionary, _name of the dictionary entry_ and _diagnostic forms_. If there were either more than one lexeme or variants for one lexeme in the same entry, they were treated as different entries. 

### andi-nouns.csv
- id - entry's id in the dictionary
- word - name of the dictionary entry
- type - word's class/type
- abs_sg - absolutive stem
- obl_sg_stem - singular oblique stem
- abs_pl - plural absolutive stem
- abs_pl_suffix - plural absolutive affix
- obl_pl_stem - plural oblique stem; if not specified, the same as plural absolutive stem
- other columns contain transliterated versions of the columns

### andi-adjectives.csv
- id - entry's id in the dictionary
- rus - name of the dictionary entry
- type - class which the stem is used with
- no_class - stems that cannot take class affixes
- first_stem - the first part of the stem which class affix is infixated
- affix - class affix that is used with this stem
- stem - stems that take class affixes OR the second part of the stem which class affix is infixated
- other columns contain transliterated versions of the columns

### andi-adverbs.csv
- id - entry's id in the dictionary
- rus - name of the dictionary entry
- type - class which the stem is used with
- no_class_stem - stems that cannot take class affixes
- affix - class affix that is used with this stem
- stem - stems that take class affixes
- other columns contain transliterated versions of the columns

### andi-verbs.csv
- id - entry's id in the dictionary
- word - name of the dictionary entry
- roles - the verb's role structure
- andi_roles - the verb's role structure if special for Andi
- aorist, infinitive, imperative - diagnostic forms from the dictionary
- aorist_cyr, infinitive_cyr, imperative_cyr - diagnostic forms from the dictionary in Cyrillic script
- stem_type	- oral, nasal (see [2]) or -di
- class	- 1 if the verb does can attach a class marker, 0 if not, *infix* is the marker is infixated
- ablaut - 1 if the verb has vowel alterantion for number, 0 if not

### Bibliography
1. Кибрик, А. Е., & Кодзасов, С. В. (1990). Сопоставительное изучение дагестанских языков: имя, фонетика (Vol. 2). Издательство Московского университета.
2. Kaye, S., Martynova, A., Moroz, G., Rochant, N., Verhees, S., & Zakirova, A.. (forthcoming). A sketch of Andi (Zilo dialect). In Koryakov, Y. and Maisak, T. (eds) The Caucasian Languages. An International Handbook. De Gruyter Mouton: Berlin/New York.
3. Салимов Х.С. (2010). Гагатлинский говор андийского языка. ИЯЛИ.

enUS (American English) plus deDE (German Standard German) bilingual dictionary
===============================================================================

### This is a hunspell dictionary that supports both enUS (American English) and deDE (German Standard German).

Hunspell <https://hunspell.github.io/> is a spellchecking library used by LibreOffice, Mozilla Firefox, Thunderbird, and many other projects.
This dictionary for Hunspell simply combines a German Standard German and an American English dictionary.

### Why?

This dictionary is meant for users who regularly write in German and English.
If you load this dictionary, you will **not need to manually switch** between dictionaries for the two languages.

### Downside

With this dictionary, sentences that are half-German and half-English, but correct in neither language will erroneously be seen as correct by the spellchecker,
e.g. "Ich like dieses dictionary."
In other words, this dictionary will not warn you when you mix the two languages.


How has this been created?
--------------------------

This bilingual dictionary has been created based on the "igerman98" dictionary for German Standard German and the en_US Hunspell Dictionary for American English.

Both dictionaries were converted to UTF8.
Then, the enUS dictionary was reorganized so that its set of affixes (i.e. the letters used to refer to the rules in the `.aff` file) are disjoint from the set of affixes used by the deDE dictionary.
Finally, the two dictionaries were merged.


License & Copyright
-------------------

Copyright 2022 Sebastian Muskalla

This dictionary is free and open-source software,
licensed under the GPLv3 (GNU General Public License version 3), see [LICENSE](LICENSE).

This dictionary is based on the German dictionary "igerman98",
Copyright 1999-2016 Björn Jacke.
This dictionary is licensed under the GPLv3, see [deDE.LICENSE](deDE.LICENSE).

This dictionary is based on the en_US Hunspell Dictionary,
Copyright 2000-2018 Kevin Atkinson.
This dictionary is licensed under a GPLv3 compatible license,
see [enUS.LICENSE](enUS.LICENSE).

enUS (American English) plus deDE (German Standard German) bilingual dictionary
===============================================================================

### This is a Hunspell dictionary that supports both enUS (American English) and deDE (German Standard German).

Hunspell <https://hunspell.github.io/> is a spellchecking library used by LibreOffice, Mozilla Firefox, Thunderbird, and many other projects.
This dictionary for Hunspell simply combines dictionaries for German Standard German and American English.

### Why?

This dictionary is meant for users who regularly write in German and English.
If you load this dictionary, you will **not need to manually switch** between dictionaries for the two languages.

### Downside

With this dictionary, sentences that are half-German and half-English, but correct in neither language will erroneously be seen as correct by the spellchecker,
e.g. "Ich like dieses dictionary."
In other words, this dictionary will not warn you when you mix the two languages.


Installation instructions
-------------------------

We provide this dictionary as an add-on for Mozilla Firefox and Thunderbird.
With the files contained in this repository, one could also install it in any other software that supports Hunspell dictionaries.

**Note:** This dictionary will register as a dictionary for American English.
You will need to set your spell checking to American English for this dictionary to work.

### Firefox: Automatic installation

*tbd*

### Thunderbird: Automatic installation

This dictionary is available as an add-on for Thunderbird via the add-on gallery.

<https://addons.thunderbird.net/en-US/thunderbird/addon/enus-dede-bilingual-dictionary/>

Inside Thunderbird, you can open the Add-ons Manager (Click the "Tools" menu and select "Add-ons and Themes"), search e.g. for "bilingual", and then click "Add to Thunderbird".


### Firefox & Thunderbird: Manual installation via `.xpi` files

From the **Releases** section in the sidebar of this page, you can download this dictionary as an add-on for Mozilla Firefox and Thunderbird (in the form of a signed `.xpi` file).


### Mozilla Firefox: Manual installation (option 1)

Click the latest release in the sidebar, then click on the file
`firefox_enus_plus_dede_bilingual_dictionary-1.xpi`.
Firefox should ask you whether you want to install the add-on.
Click "Continue to installation" and "Add".

### Mozilla Firefox: Manual installation (option 2)

* Click the latest release in the sidebar, then download the archive `firefox_enus_plus_dede_bilingual_dictionary-1.zip`.
* Extract the file `firefox_enus_plus_dede_bilingual_dictionary-1.xpi ` contained in this archive to some location on your computer.
* In Firefox, open the menu "Tools" and select on "Add-ons and Themes".
  The Add-on manager will open.
* Select "Dictionaries" in the sidebar.
* Click the cog icon on the top right and select "Install Add-on from File".
* Find and choose the `.xpi` file that you have extracted.
* A popup will ask you to confirm the installation. Click "Add".

This has been tested using Mozilla Firefox 105.0.3 on Windows 10 21H2.

### Thunderbird: Manual installation

* Click the latest release in the sidebar, then download the archive `thunderbird_enus_plus_dede_bilingual_dictionary-1.zip`.
* Extract the file `thunderbird_enus_plus_dede_bilingual_dictionary-1.xpi` contained in this archive to some location on your computer.
* In Thunderbird, open the menu "Tools" and select on "Add-ons and Themes".
  The Add-on manager will open.
* Select "Dictionaries" in the sidebar.
* Click the cog icon on the top right and select "Install Add-on from File".
* Find and choose the `.xpi` file that you have extracted.
* A popup will ask you to confirm the installation. Click "Add".

This has been tested using Thunderbird 102.3.3 on Windows 10 21H2.

### Other software supporting Hunspell

The folder `bundle/dictionaries` contains the two files that are needed for the dictionary:

* [enusdede.dic](bundle/dictionaries/enusdede.dic), the word list.

* [enusdede.aff](bundle/dictionaries/enusdede.aff), the affix rules.

With these two files, it should be possible to install this dictionary in any software that supports Hunspell.


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

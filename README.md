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


Mozilla Firefox & Thunderbird: Installation via the browser
-----------------------------------------------------------

We provide this dictionary as an add-on for Mozilla Firefox and Thunderbird.
It can be found in the add-on gallery under the name "enUS deDE bilingual dictionary":

* <https://addons.mozilla.org/en-US/firefox/addon/enus-dede-bilingual-dictionary>
* <https://addons.thunderbird.net/en-US/thunderbird/addon/enus-dede-bilingual-dictionary>

### Step-by-step installation guide

* Open the hamburger menu (on the top-right) and select "Add-ons and Themes" to open the add-on manager.
* In the search bar next to "Find more add-ons", search for "bilingual dictionary".
* Find the add-on and click "Add to Firefox" (resp. "Add to Thunderbird").
* Confirm the Installation by clicking "Add" in the resulting pop-up.

### Note:

This dictionary will register as a dictionary for American English.
You will need to set your spell checking to American English for this dictionary to work.

Right-click in a text box, open the "Languages" sub-menu and select "English (United States)".


Manual installation
-------------------

From the **Releases** section in the sidebar of this page, you can download this dictionary as an add-on for Mozilla Firefox and Thunderbird (in the form of a signed `.xpi` file).


### Mozilla Firefox (Option 1)

On this page, click the latest release in the sidebar, then click on the file
`firefox_enus_plus_dede_bilingual_dictionary-1.xpi`.
Firefox should ask you whether you want to install the add-on.
Click "Continue to installation" and "Add".

### Mozilla Firefox (Option 2)

* On this page, click the latest release in the sidebar, then download the archive `firefox_enus_plus_dede_bilingual_dictionary-1.zip`.
* Extract the file `firefox_enus_plus_dede_bilingual_dictionary-1.xpi` contained in this archive to some location on your computer.
* In Firefox, open the hamburger menu and select on "Add-ons and Themes".
  The Add-on manager will open.
* Select "Dictionaries" in the sidebar.
* Click the cog icon on the top right and select "Install Add-on from File".
* Find and choose the `.xpi` file that you have extracted.
* A popup will ask you to confirm the installation. Click "Add".

This has been tested using Mozilla Firefox 105.0.3 on Windows 10 21H2.

### Thunderbird: Manual installation

* On this page, click the latest release in the sidebar, then download the archive `thunderbird_enus_plus_dede_bilingual_dictionary-1.zip`.
* Extract the file `thunderbird_enus_plus_dede_bilingual_dictionary-1.xpi` contained in this archive to some location on your computer.
* In Thunderbird, open the hamburger menu and select on "Add-ons and Themes".
  The Add-on manager will open.
* Select "Dictionaries" in the sidebar.
* Click the cog icon on the top right and select "Install Add-on from File".
* Find and choose the `.xpi` file that you have extracted.
* A popup will ask you to confirm the installation. Click "Add".

This has been tested using Thunderbird 102.3.3 on Windows 10 21H2.

### Other software supporting Hunspell

The folder `bundle/dictionaries` contains the two files that constitute the dictionary:

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

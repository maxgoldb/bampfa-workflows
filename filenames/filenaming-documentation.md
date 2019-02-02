# BAMPFA Filenaming Guidelines 

Updated 2019-02-01

This document should provide a pretty comprehensive guide to naming files at BAMPFA. A lot of it is image-focused, but it also applies to audiovisual material.

## Contents

* [General info](#general-information)
  * [Special Characters](#special-characters)
  * [Filename Sections](#filename-sections)
  * 
 
## General Information
 
### Length

Try to keep filenames under 64 characters, including hyphens (-), underscores (_), and file extensions (.jpg, .tif, .doc, etc.).

### Special Characters
***THIS IS REALLY, REALLY IMPORTANT***

Do not use ANY special characters or punctuation in a file name. It will cause havoc down the road. Examples :

( ) @ / \ : * ? " < > ' ; +=¨

Only use underscores, (_), hyphens (-), and alphanumerics (a-z, 0-9). If you have a special character in a title (I ♥ Huckabees, for example), spell out the word "heart" instead of using the special character.  Omit accents from áccented wórds or nämes; ¿leave.out.all.punctuation?: unnecessary apostrophe's, commas; colons + etc.
 
**AVOID USING ALL CAPS**
 
Avoid using periods in filenames other than a single period before the file type extension (.tif, .jpg, .doc, etc.). 

### Filename Sections
Divide "areas" of the filename (e.g., artist name, title of a work) with underscores and words within an "area" with hyphens. e.g. LastName_Title-of-work. Please do not use underscores between words unless they separate conceptually distinct "areas" of the file name. 

Example: 

> **Chase-Riboud_All-that-rises_001.jpg**

not 

> **Chase_Riboud_All_that_rises_001.jpg**

For multi-word last names, use hyphens between words.

Example: 

* For an image of Lars von Trier's *Breaking the Waves*
  * **von-Trier_Breaking-the-Waves_001.tif**

### Intial articles

Omit initial articles from a title in a filename, in all languages (the, an, a, der, los, les, etc.). Any articles later in the title itself should stay in the filename. The full title, with articles, should be entered in the Title field in the metadata. 

Examples: 

* For an image of Michael Powell's film *The Red Shoes*
  * **Powell_Red-Shoes_001.jpg**
  * The Piction metadata field `Title` should read "The Red Shoes"
* For an image of David Lean's film *The Bridge on the River Kwai*
  * **Lean_Bridge-on-the-River-Kwai_001.tif**
  * Metadata field `Title` should read "The Bridge on the River Kwai"
* For Pablo Picasso's *Les Desmoiselles d'Avignon*
  * **Picasso_Desmoiselles-d-Avignon_001.jpg**
  * Metadata field `Title` should read "Les Desmoiselles d'Avignon"
 
### Abbreviations

Don't.

Include the full name of an artwork whenever possible. If you need to truncate because of length, do not abbreviate words; instead, use as many entire words as possible.

Example: 
* For W.D. Richter's *The Adventures of Buckaroo Bonzai Across the 8th Dimension
  * **Richter_Adventures-of-Buckaroo-Bonzai-Across_001.jpg**
  * (not **Adv-Buck-Bonz-Acr-8th-Dim** not **Buckaroo-Bonzai** not **A-B-B-A-t-8th-D**)

### Alternative spellings
When the title of an artwork or the name of an artist has various forms or spellings, default to the form of the name/title used in the most recent BAMPFA program guide. If the name  or title has not appeared in the program guide and there is no preferred spelling/form indicated by the BAMPFA style guide, default to the form found in the [Getty Union List of Artist Names](http://www.getty.edu/research/tools/vocabularies/ulan/), the [Library of Congress Name Authority](http://authorities.loc.gov/), or another reference source: for film titles, try Variety or Film Index International (contact library staff for help connecting to these). 

Examples:
* For the artist 艾未未:
  * **Ai Weiwei** not **Ài Wèi wèi**
* For the director 侯孝賢:
  * **Hou Hsiao-Hsien** not **Hóu Xiàoxián**
* For the director Сергей Михайлович Эйзенштейн:
  * **Sergei Eisenstein** not **S. M. Ejzenstein**
* For the painting *La gioconda*
    * **Mona Lisa** not **La joconde**
* For the film *À bout de souffle*
  * **Breathless** not **À bout de souffle**

### Numbering
Use three digits to indicate the image sequence number or view number: 

Examples: **_001**, **_002**, etc. not **_1**, **_2**.

Use these numbers even if we currently have only one image for a particular work--there may well be more on the way!  If we have more than one image pertaining to a particular work, number them consecutively. 

Please check that we do not already have images of the same work in Piction before labeling your image _001. If there are already images, start your numbering where they leave off. Example: if we have 001-004, you would start at 005.

Example: 

**von-Trier_Breaking-the-Waves_001.tif**

**von-Trier_Breaking-the-Waves_002.tif**

**von-Trier_Breaking-the-Waves_003.tif**

### Date formatting

For single dates, use the format **YYYY-MM-DD**

For other date formats, such as specific months, three-month calendar periods, separate year from month or day with a hyphen and use underscores to separate other date information. For example 2011-07-08 means July 8, 2011 whereas 2011-07_08 means July–August 2011. *[MCQ note 2019/02: this is probably in need of revision]*

## Types of File Names
 
### Artworks NOT accessioned by BAMPFA

**General structure:**

> ArtistLastName_Title-Of-Work_Optional-date-if-known_number.filetype

Examples: 

> Baldesarri_I-Am-Making-Art_1971_001.tif

or: 

> Baldesarri_I-Am-Making-Art_001.tif


__Artworks where artist is unknown:__

> Unknown_Title-Of-Work_number.filetype

Example:

> Unknown_Bodhisattva-Padmapani_001.tif
>
> **(Be sure to include country of origin and/or identifying information in metadata)**


__Films by one director:__

> DirectorLastName_Title-of-film_number.filetype

Example: 

> Wyler_Roman-Holiday_001.jpg

__Films by more than one director__

Use the word "Collaboration" in place of the directors' names.

> Collaboration_Title-of-film_number.filetype

Example: 

> Collaboration_Kinshasa-Symphony_001.jpg

**(Be sure to include all director names in metadata)**

---

### BAMPFA permanent art collection

**General structure:**

> bampfa_accession-number_page number or view_derivative number.filetype

Example:  **bampfa_1960-69-2_003_1.tif**

For BAM collection items, replace periods in accession numbers with hyphens. 

Example: 
* For the painting with accession number 1998.42.5:
  * **bampfa_1998-42-5_001_1.tif**

The page number or view can be used for multiple pages of a document such as an artist book or multiple views (front, side, back, etc) of a work, or a different version of the same image (e.g. a view from a 4 x 5" slide vs. one from a digital scan would be different versions).

Use three numbers for a "view": 001, 002, etc.

Use the following derivative numbers:

|number|description|
|-|-|
|_1|master TIF with color bar|
|_4|TIF without color bar (full size version that is cropped)|
|_5|image of any format from a source other than the normal BAMPFA workflow, typically from a gallery, a donor, etc. Image is potentially ready for web display|
|_6|reference-only snapshot, primarily by BAMPFA staff; *NOT FOR WEB DISPLAY*|

We formerly used _2 and _3 to denote jpeg derivatives based on the original TIF. These numbers are no longer in use.

---

### Gallery installation images

**General structure:**

> Install_Exhibition-Name_YearOpened_view number.tif

Example: **Install_Create_2011_002.tif**

For the MFA exhibits, the exhibition name is just **MFA**

Example: **Install_MFA_2011_001.tif** 

For MATRIX exhibits, exhibition name is just "matrix" and the MATRIX exhibition number with a hyphen.

Example: **Install_matrix-239_2011_003.tif**

---

### Press Clippings for Exhibitions

General structure:

> Press_Exhibition-Name_YearOpened_view number.tif

---

### Institutional Images
**Events and other "museum life" images**

**General structure:**

> Type_Keyword_Descriptive-Name_full-date_number.filetype 

Example: **Event_Late_Early-the-sun-part-one_2012-02-05_001.jpg**

Choose an appropriate type and keyword from the lists below in addition to the name of the program, guest, or speaker.

**Types**
* Event
* Building
* Portrait
* Misc

**Keywords**
* Gala
* Gallery-talk
* In-person
* Late
* Full
* Member
* Opening
* School-family-programs [education programs]
* School-visits [field trips, etc.]
* Staff
* Student
* Student-committee
* Talk

Examples:

> Event_Gallery-talk_Padma-Maitland_2014-03-13_005.JPG

> Event_Late_Sir-Richard-Bishop_2011-08-12_001.jpg

> Event_Opening_State-of-mind-opening_2012-02-28_001.jpg

> Event_printing-plant-tour_2012-02-16_001.jpg

> Event_Late_early-the-sun-part-one_2012-02-05_001.jpg

> Event_Member_ten-at-ten_2012-01-18_001.jpg

> Building_Durant-entrance_2012-02-21_001.jpg

> Building_Ito-conceptual-design-F_2007_001.jpg

> Building_schematic-design_2011_001.jpg

> Portrait_Staff_Lawrence-Rinder_2010-04-14_001.jpg

> Misc_Chez-Panisse-40_2011-10-12_001.jpg

---

### Funder or Partner Institution Logos
 
**General Structure:**
> Institution-name_logo_other-information.filetype

Examples:
* **NEA-Artworks_logo_cmyk.eps**
* **East-Bay-Express_logo_white_small.jpg**
 
Retain any original information about the filetype, version, or size in which the logo came from the funding institution. Remove any characters or spacing that don't comply with our system. If an institution supplies new or updated logos over time, record the logo year as a subfolder and note it in the metadata.

---

### Audiovisual material cataloged in the PFA Collection database

Files created in-house, for example at the LaserGraphics ScanStation for film or at the video digitization tower, or created by vendors.

Metadata about these materials is found in the PFA FileMaker Collection Management System. The item accession number in the filename is parsed on ingest to our digital repository to link descriptive metadata with the files.

**General structure:**

> title-without-lead-article_last-5-digits-of-pfa-accession#_barcode_r##of##.extension

Examples:
* Battleship Potemkin, 6 reels of 35mm, PFA Accession number 3500-01-498: 
   * **battleship-potemkin_00498_pm0067890_r01of06.mov**

* A woman is a woman, 16mm, PFA Accession number 1620-01-14322
    * **woman-is-a-woman_14322_pm0045628_r02of03.mov**

---

### Audio material cataloged in the BAMPFA audio database (WIP)

Files can be either born-digital or digitized audio cassettes. Examples are primarily guest speakers in the BAMPFA film program (guest filmmakers in the theater, Q&A sessions, etc.). 

Metadata about these materials is found in the BAMFA audio FileMaker database . The recording ID number in the filename is parsed on ingest to our digital repository to link descriptive metadata with the files.

**THIS IS IN PROGRESS AS OF 02/2019**

**General structure:**

> bampfa-audio_5-digit recording ID_recording YYYYMMDD_first speaker name_optional part designator.extension

Examples:

* George Kuchar discussing his films on May 3rd 1983, with recording in side A and side B:
  * bampfa-audio_01456_19830503_George-Kuchar_a.wav
  * bampfa-audio_01456_19830503_George-Kuchar_b.wav
* 



---

### Born-digital moving images created in-house

Examples include Osher theater lectures, panels, guest filmmakers, etc.; event documentation; artist interviews; special productions for website, social media, etc.

**THIS ALSO NEEDS TO BE CONFIRMED WITH DIGITAL MEDIA AND COMMUNICATIONS STAFF**

**: P**

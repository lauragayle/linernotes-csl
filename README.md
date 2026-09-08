# linernotes-csl
CSL modified for liner notes, book reviews and scores.
First of all, your mileage may vary.
These files include modified CSL for CMOS 18 notes-bibliography AND author-date to accommodate tracking and citing liner notes; book reviews, hypothetically recording reviews; and music scores. CSL was modified to include the liner notes; the others formats have the type indicated in the extra field.
The RDF file includes templates for each of the additional formats. Duplicate those when entering new information for your citation. Another alternative is to use the format type listed at the top of the template, then copy the extra field information to your new citation.

If you have not installed a new citation style to your Zotero before, here are the necessary steps:
* download the csl file
* in your Zotero installation, go to Settings, then Cite, then Add from file
* choose the downloaded file; note the name displayed in the style list is either CMOS 18 liner notes author-date or CMOS 18 liner notes notes-bibliography
* next, download the template file
* in your Zotero installation, choose File, Import, A file then navaigate to the downloaded file
* these items will likely be in their own collection after import.
* Open any one of these from the collection and note the tag for the format and the information in the extra field. In the case of liner notes, I've completed a fake citation to help you complete your entry. More information regarding the liner note details in the code below.

If you have corrections or suggestions, please contact me. I'm a music librarian and passionate Zotero user. While I do limited coding, it's not my strong suit. I used Claude.ai to edit the XML. 

The critical bit of code is

~~~Enter print liner notes in Zotero as a Book Section:
         Author        = liner-notes author
         Title         = liner-notes essay/section title (optional)
         Book Title    = recording title
         Book Author   = composer
         Contributor   = performer(s), ensemble, conductor
         Publisher     = record label
         Date          = release year
         Extra         = genre: Liner notes
                         medium: compact disc
                         number: <label catalogue number>   (optional)
                         event-date: 2019-05-04             (recording date, optional; original-date also accepted)
       The liner-notes format is triggered by a Book Section that has both `genre` and `medium`

# Transfer Translator IT -> IT-YO
The aim of this project is to create a transfer translator from Italian to Italian-Yodish, that is from a Subject Verb OtherPosTags (SVX) structure, to a OtherPostTags Subject Verb (XSV) structure.

We then created a Context Free Grammar for Italian to parsify some simple sentences. This grammar is in the file `g1.fcfg` and is written in Chomsky Normal Form.
The translation is done with the CKY algorithm.

In case of ambiguity, the first translation is chosen.

The translator is built to translate the following sentences:
- Tu avrai novecento anni di età -> Novecento anni di età tu avrai
- Tu hai amici lì-> Amici hai tu lì
- Noi siamo illuminati-> Illuminati noi siamo

## How to
Execute: `python3 yodify.py g1.fcfg "<sentence in Italian>"`.

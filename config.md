## AJT Japanese &mdash; config

*Anki needs to be restarted for changes to be applied.*

****

### General

* `regenerate_readings`.
  When you run "Edit" > "Bulk-add readings"
  in the Anki Browser,
  readings for each card will be regenerated
  even if destination is already filled.
* `generate_on_note_add`.
  Automatically add readings and pronunciations to cards created via AnkiConnect.
  For example, cards created with Mpvacious, Yomichan, Rikaikun.
* `cache_lookups`.
  Size of cache.
  Used internally.
* `styles`.
  Style mappings. Edit this if you want different colors, etc.

### Profiles

Each profile defines
Note Type constraints,
fields to generate data for
and fields where the generated data should be placed.
By default, the add-on matches a note type
if it finds the text "japanese" in the note type name.
Case is ignored.

Default field names match the [TSC](https://ankiweb.net/shared/info/1557722832) note type.

### Furigana

* `skip_numbers`. Whether to add furigana to numbers or not.
* `prefer_literal_pronunciation`.
  The database has readings with the `ー` symbol in place of long vowels.
  Prioritize them, and use single kana to show equivalent sounds, e.g. `を` and `お`.
* `reading_separator`.  String used to separate multiple readings of one word. For example, `<br>` or `,`.
* `blocklisted_words`. Furigana won't be added to these words. Comma-separated.
* `mecab_only`. A comma-separated list of words that don't need to be looked up in the database.
* `counters`. List of counters. Used internally.
* `maximum_results`. Used when database lookups are enabled. Will abort if fetched more results than this number.

### Pitch accent

* `lookup_shortcut`.
  The shortcut to perform pronunciation lookup
  on the selected text ("Tools" > "NHK pitch accent lookup").
* `output_hiragana`.
  Print readings using hiragana instead of katakana.
* `kana_lookups`.
  If failed to find pitch accent for a word,
  make an attempt to look it up using its kana reading.
  Works better if `split_morphemes` is set to `true` in the profile.
* `skip_numbers`. Don't lookup numbers.
* `reading_separator`. String used to separate different readings of one word.
* `word_separator`. String used to separate words.
* `blocklisted_words`. A comma-separated list of words that you don't want to look up.
* `maximum_results`. Abort if fetched more results than this number.

### Context menu

You can enable or disable the following actions:

* `generate_furigana`.
  Paste furigana for selection.
* `to_katakana`.
  Convert selection to katakana.
* `to_hiragana`.
  Convert selection to hiragana.
* `literal_pronunciation`.
  Convert selection to a pronunciation format used in dictionaries (katakana form + certain character conversions).

### Toolbar

Controls additional buttons on the Anki Editor toolbar.

* "Furigana" button lets you generate furigana in the selected field.
* "Clean" button removes furigana in the selected field.
* "Regenerate all" button clears all destination fields and fills them again.

Parameters:

* `enable`.
  Control whether a button is shown.
* `shortcut`.
  Specify a keyboard shortcut for the button.
* `text`.
  Customize the button's label.

****

If you enjoy this add-on,
please consider [donating](https://tatsumoto.neocities.org/blog/donating-to-tatsumoto.html)
to help me continue to provide you with updates and new features.
Thank you so much for your support and for being a part of our journey!

# Simple Stemmer for Core Search

Provides partial word matching for entities in the core Search module.

Partial word matching is implemented by using ngrams. Each word is split into 3
(default) letter lengths, so 'apple' gets indexed with 3 smaller strings 'app',
'ppl', 'ple'. The effect of this is that as long as your search matches X
percentage of the word the entity will be pulled up in the results.

## Installation

Install this module using the official Backdrop CMS instructions at
  <https://backdropcms.org/guide/modules>.

## Configuration

- By default, the "Minimum word length to index" is used for the N-gram size,
  which can be overridden by setting `simplestemmer_ngram_size` in `settings.php`
- Then click the button for 'Invalidate Search Index'.

## Current Maintainers

- [Herb v/d Dool](https://github.com/herbdool)
- Seeking additional maintainers

## Credits

Created for Backdrop CMS by Herb v/d Dool. Inspired by Scott Reynolds' work
on https://www.drupal.org/node/103548 and the Fuzzy Search module for Search API.

## License

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

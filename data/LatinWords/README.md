# Latin Word List

## Source

The Latin word list is derived from the [Classical Language Toolkit (CLTK)](https://github.com/cltk/cltk) Latin lemmata dataset, hosted at [cltk/lat_models_cltk](https://github.com/cltk/lat_models_cltk).

The CLTK is an open-source Natural Language Processing (NLP) framework for pre-modern languages, developed by academic researchers. The Latin lemmata dataset contains ~270,000 word form-to-lemma mappings covering Classical and Medieval Latin.

## Processing

The word list (`latin_words.txt`) was extracted by collecting all unique word forms and lemma headwords from the CLTK dataset. Words were lowercased and filtered to include only alphabetic entries of 4 or more characters. The letter 'w' (not part of the Latin alphabet) was excluded.

## License

The CLTK project is licensed under the MIT License. See [cltk/lat_models_cltk LICENSE](https://github.com/cltk/lat_models_cltk/blob/master/LICENSE).

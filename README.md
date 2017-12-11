## Parsing Inter Language Links Out of Wikimedia Data Dumps

**Author**: Bill Thompson (biltho@mpi.nl)


#### Summary
A Simple python script to extract inter-language links from [Wikimedia](https://dumps.wikimedia.org) sql dumps. Writes out a csv with (page_id, target_language, page_title_in_target_language) columns

Usage:

```python -f avwiki-latest-langlinks.sql.gz```

The latest dumps for the English wikipedia, for example, can be found [here](https://dumps.wikimedia.org/enwiki/latest/). This script works on the sql version of the langlinks table dump (e.g.: [link](dumps.wikimedia.org/enwiki/latest/enwiki-latest-langlinks.sql.gz)). This repository contains an example dump (```avwiki-latest-langlinks.sql.gz```) and an example of the parsed result (```avwiki-latest-langlinks-parsed.csv```). The latest dumps in other languages can be found at:

dumps.wikimedia.org/[LANGUAGE]wiki/latest/[LANGUAGE]wiki-latest-langlinks.sql.gz

 where [LANGUAGE] is replaced by the language iso (e.g. en, ab, es, pt, fr, etc...)




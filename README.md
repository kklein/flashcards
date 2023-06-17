A collection of personal flashcards meant to be used with [Anki](https://apps.ankiweb.net/).

## Specification

* The separator between question and answer is a comma (`,`).
* Answers can be multi-lined when properly wrapped by double quotes (`"`).
* Answer can contain commas when properly wrapped by double quotes (`"`).

For more details on what a valid csv format looks like, see
https://github.com/kklein/anki-csv.

## Pre-commit hooks

Spellchecking and csv format validation are provided by this repository's pre-commit hooks.

In order to make use of them, run the following:

```console
git clone git@github.com:kklein/flashcards.git
cd flashcards
mamba env create -f environment.yaml
mamba activate flashcards
pre-commit install
```

Aside the `git commit` hook mechanisms, the pre-commit checks can be run proactively by
executing

```console
pre-commit run --all-files
```

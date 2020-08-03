## What is Fiction Publisher
**Fiction Publisher** is a fork of [Open Publisher](https://github.com/chrisanthropic/Open-Publisher), redesigned to work with [Manuskript](https://github.com/olivierkes/manuskript) projects. It is a PowerShell script that wraps Pandoc, KindleGen, and LaTeX and uses a set of custom Pandoc templates (created with a focus on fiction).

Write your manuscript in markdown, write a Pandoc [metadata](Metadata-Doc.md) file, run a script, and receive some beautifully formatted ePub, Mobi, and print-ready PDF books.

Full documentation on the [wiki](https://github.com/Blake-Eryx/Fiction-Publisher/wiki).

## Features

#### PowerShell build script which creates
  - [X] PDF (print)
  - [X] epub
  - [X] mobi
  - [X] Word (using a **Draft** template)

#### Input formats
- [X] Supports Markdown files within [Manuskript](https://github.com/olivierkes/manuskript) folder structure

#### Configurable components for output (PDF and epub)
- [X] Copyright page template
  - [X] creative-commons
- [X] Chapter heading templates
  - [X] default
  - [X] romance
  - [X] Or you can select styles from the **fncychap** latex package
- [X] Half-title page template
- [X] Series page template
- [X] Author biography page template

#### Adds formatting to output (PDF and epub)
- [X] Adds header to start of chapters if missing (based on parent folder name)
- [X] Formats start of chapter with drop cap and smart caps
- [X] Adds flourishes between scene breaks/POV changes (currently PDF only)
- [X] Unindents starting paragraph of new scenes/POV changes
- [X] Formats start of chapter with drop cap and smart caps
- [X] Supports [CriticMarkup](https://github.com/CriticMarkup/CriticMarkup-toolkit) syntax

#### Validation features
- [X] Checks for paragraphs not separated by blank lines (this is recommended over ending lines with double spaces because it makes the intention clearer and avoids possible errors)
- [X] Checks for straight quotes (proper smart quotes should be included in source markdown to avoid ambiguity)
- [X] Checks for '--' (en dashes and em dashes should be included in source markdown to avoid ambiguity)
- [X] Checks for correct ordering of closing quotation marks and commas/periods
- [X] Checks for Unicode ellipsis (should be spaced periods)
- [X] Checks for en dash at the end of a quote (should be an em dash)
- [X] Checks for hyphen between numbers (should be an en dash)
- [X] Checks for extra spaces
- [X] Checks for indenting spaces (these should not be hardcoded in source markdown files)
- [X] Checks for tabs
- [X] Checks for a line that ends with space(s), followed by single newline (indicates ambiguous intention as to whether this should be a new paragraph [a full blank line is recommended here] or the same paragraph [the newline should be removed])
- [X] Checks for items that should be italicized (items are user-defined in metadata)

## Fiction Publisher v2 Roadmap

- [ ] Remove YAML headers from markdowns files
- [ ] Add commercial copyright page template
- [ ] Add flourishes between scene breaks/POV changes in epub output
# Glossary for Markdown (GlossaryMD)

[Example VVSG Glossary Output](vvsg_living_glossary.md)

## Instructions for Running

This report expects one report variable (passed in from MagicDraw Report Wizard), called `NERMappingFile`. This should be a file system path to the `NER` entity list.

## Instructions for Generation

- Install [MDReportExtensions](https://github.com/HiltonRoscoe/MDReportExtensions)
- Export Word version of VVSG Glossary into Google Docs
- Export from Google Docs into XLSX
- Replace Bullets with Dashses
- Replace fancy quotes “ ” ->  " ",  ’ -> '
- Export as CSV (UTF-8)
- Import CSV into MagicDraw
- Export `NER` entity list (use `regexner.txt` template).
- Export package as MarkDown report

> NER may have issues with terms containing slashes. Remove such terms from NER list.

## Instructions for MD conversion

```bash
pandoc vvsg_living_glossary.md -o vvsg.docx --reference-doc styles.docx -f markdown_github
```

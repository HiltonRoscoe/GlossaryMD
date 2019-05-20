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
- Export as CSV
- Import CSV into MagicDraw
- Export `NER` entity list (use `regexner.txt` template).
- Export package as MarkDown report

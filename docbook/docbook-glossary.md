Analyze all files from the cody://repository repository that are referenced from @ASSEMBLY-FILE
to enhance the glossary in @GLOSSARY-FILE. Follow these rules:

* if the term has an acronym, insert the acronym first and delimit it from the literal version with a comma
* do not capitalize the literal part if not necessary
* do not use brackets around the acronym in the term definition
* do not repeat the term in its description if possible
* check for uniqueness of glossary entries

Sort the glossary entries alphabetically following these rules:

* entries should be ordered by their acronym (if present) or by the term name
* terms without acronyms would be sorted by their first letter
* maintaining the existing XML structure, attributes, and formatting

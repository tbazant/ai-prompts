Update cody://selection by replacing matching strings with corresponding entities found in the entity file referenced by the "include::" directive in  cody://current-file.

If the entity file contains line such as ":harbor: Harbor", replace all "Harbor" or "harbor" occurrences with {harbor}.

Replace only whole words, do not replace the string in the following cases:

* the string is part of a parameter as in "setTheValue.harbor"
* the string is enclosed in back-ticks as in   "`harbor`" or "`harbor.125`"
* the string is part of a URL string as in "://core.harbor.eu"
* the string is part of a compound word that includes dashes, such as 'harbor-trivy-adapter' or 'harbor-core'. Only replace whole words that are not part of such compounds.

When updating AsciiDoc tables, focus only in the content within the table cells.
Maintain newlines and spacing between sections and tables.
Do not update or merge the lines with table's starting and ending strings "|===".
Do not delete any newline character following the selection.
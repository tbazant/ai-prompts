* If a table is missing a title, infer and add a meaningful title based on the table's content.
* If a table is missing a row header, infer and add the appropriate header based on the corresponding table's row content.
* If a table is missing a column header, infer and add the appropriate header based on the corresponding table's column content.
* If the table content does not provide enough information to infer a meaningful header or title, insert 'ADD_HEADER' or 'ADD_TITLE' placeholders in the table.
* Do not replace a partial header completely, build upon the existing header structure.
* Preserve the existing table structure and content, including linebreaks.
* Output only the changes.

When inferring a title, consider the following:
* Look for keywords or phrases in the table's content that can be used as a title.
* Use a concise and descriptive title that summarizes the table's content.
* Avoid using generic titles such as "Table 1" or "Data".

If the updated file is AsciiDoc, respect the following:
* When adding a new column header, insert '[%header]' on a separate line before the table's starting string "|===".
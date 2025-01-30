Autocomplete table headers and title following these rules:
* If a table is missing a title, infer and add a meaningful title based on the table's content.
* If a table is missing a row header, infer and add the appropriate header based on the corresponding table's row content.
* If a table is missing a column header, infer and add the appropriate header based on the corresponding table's column content.
* If the table content does not provide enough information to infer a meaningful header or title, leave a comment explaining the missing header or title.

Maintain the structure:
* Output the whole updated file including the unmodified parts.
* Do not replace a partial header completely, build upon the existing header structure.
* Preserve the existing table structure and content.
* Do not add new rows or columns to the table.

When inferring a title, consider the following:
* Look for keywords or phrases in the table's content that can be used as a title.
* Use a concise and descriptive title that summarizes the table's content.
* Avoid using generic titles such as "Table 1" or "Data".

If the updated file is AsciiDoc, respect the following:
* When adding a new column header, indicate it by inserting `[options="header"]` on a separate line right between the table title and the table's starting string "|===". 
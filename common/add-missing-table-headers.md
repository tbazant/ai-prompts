Autocomplete table headers and titles, based on the following rules:

* If a table is missing a row header, infer and add the appropriate header based on the corresponding table's row content.
* If a table is missing a column header, infer and add the appropriate header based on the corresponding table's column content.
* If a table is missing a title, infer and add the table title based on the table's content.
* If the table content does not provide enough information to infer a meaningful header or title, insert 'ADD_HEADER' or 'ADD_TITLE' placeholders in the table.
* Preserve the existing table structure and content.
* Leave the rest of the table unchanged including ine breaks.
* Output the whole table including the unmodified table cells.
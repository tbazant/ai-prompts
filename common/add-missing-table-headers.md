# Autocomplete table headers and titles following these rules:

* If a table is missing a title, infer and add a meaningful one based on the table's content.
* If a table is missing row headers, infer and add appropriate ones based on the content of the corresponding rows.
* If a table is missing column headers, infer and add appropriate ones based on the content of the corresponding columns.
* If the table content does not provide enough context to infer a meaningful header or title, leave a comment explaining what is missing.

## Maintain the structure:

* Output the entire updated file, including unmodified parts.
* Do not completely replace an existing header—improve or expand upon its current structure.
* Preserve the table’s existing structure and content.
* Do not introduce new rows or columns.

## When inferring a title:

* Identify key terms or phrases within the table's content that could serve as a meaningful title.
* Choose a concise, descriptive title that accurately summarizes the table's subject.
* Avoid generic titles like "Table 1" or "Data."

## For AsciiDoc formatting:

* When adding a new column header, insert `[options="header"]` on a separate line between the table title and the `|===` table delimiter.

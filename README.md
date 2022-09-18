# RenamePDF
Renames PDF invoices with current date

Description: Sequence for renaming every invoice from a folder.
Invoices are contained in the project folder embedded in the 'Data > Invoices' directory.

Current Limitation:
- You have to delete the newly appended date from the PDF file name before running for demo purposes. Otherwise, It'll just keep appending a date to the old date.

Activities Used:
- Browse for folder
- For Each
- Assign
- Log Message
- Move File

Methods Used:
- Directory.GetFiles(<insert folder path variable>)
- fileName.Replace(".pdf", Now.ToString("_yyyy_MM_dd") + ".pdf")

Process (Updated: November 25, 2023)

1. Convert pdf files to txt files ([pdf_to_txt.py](code/pdf_to_txt.py))
0. Manually remove attachments and index from txt (top and bottom of the file)
0. Parse each file by itemized numbers ([cleaning.py](code/cleaning.py))
0. Some numbers are not properly ordered. Manually reorder them on txt file (cleaning.py ends where any number is not ordered properly and extracts the rest of the document as one item, which is very large and noticeable).
0. When documents are not numbered (image numbers or nonexistent), use \n\n as parsing ([cleaning_linebreak.py](code/cleaning_linebreak.py))
0. After cleaning txt files and converting them to csv files, put them together as a large file ([csv_binder.py](code/csv_binder.py))
0. Run any analysis on the large file.

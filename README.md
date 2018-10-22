# PDFManager


REQUIRED: ADOBE ACROBAT	
To add acrobat library, open Visual Basic, under Tools->References, check "acrobat" if "Adobe Acrobat" is unchecked.

	NOTE: The macros will not make changes to the SOURCE file. Any modified file is saved as a new OUTPUT file.	
	NOTE: The SOURCE file and OUTPUT file cannot have the same file path.	
	NOTE: To reference the last page of any pdf, either enter the word "Last" or the page number	
	NOTE: In the sheet "Rearrange PDFs", enter "AfterLast" in the 3rd column to move the specified to the end of the pdf	
		
	Macro Summary	
	i) List all the PDF files in a specified folder (including or excluding subfolders)	
	ii) Extract, rearrange or delete specified pages from a SOURCE pdf file (saved as a new OUTPUT file)	
		
	DIRECTIONS		
		
I.	OUTPUT FOLDER	
	In sheet "OUTPUT", enter the folder path in B2	
	Any newly created files or subfolders from any of the macros will be found in this folder	
		
II.	Get File Paths	
	Displays list of PDF files in the specified folder. 	
	In sheet "Get File Paths", enter Folder path in B1	
	Click the appropriate Button to list PDF files 	
		There are two buttons; one includes subfolders within the specified folder
		
III.	Extract PDFs	
	Copies a specified subsection of pages into a new pdf file	
	In sheet "Extract PDFs",  Column A, enter page number of the start of the subsection	
	In Column B, enter page number of the end of the subsection	
	Both start page and end page will be included in the new file.	
	In Column C, enter a filename for the new output containing the subsection	
	(optional) In Column D, enter a folder name to create a subfolder in the OUTPUT folder	
	In Column E, enter filepath of the source file that needs to be edited (filepaths can be obtained from Step II)	
		
	Click RUN	
		
IV.	Rearrange PDFs	
	Creates a new pdf file where a specified subsection is moved before another specified page.	
	In sheet "Rearrange PDFs", Column A, enter page number of the start of the subsection	
	In Column B, enter page number of the end of the subsection	
	Both start page and end page will be included in the new file.	
	In column C, enter the number of the page before which the the specified subsection will be moved.	
	In Column D, enter a filename for the new output containing the subsection	
	(optional) In Column E, enter a folder name to create a subfolder in the OUTPUT folder	
	In Column F, enter filepath of the source file that needs to be edited (filepaths can be obtained from Step II)	
		
	Click RUN	
		
V.	Delete Pages	
	Creates a new pdf file where a specifed subsection is removed.	
	In sheet "Delete Pages",  Column A, enter page number of the start of the subsection	
	In Column B, enter page number of the end of the subsection	
	Both start page and end page will be deleted in the new file.	
	In Column C, enter a filename for the new output containing the subsection	
	(optional) In Column D, enter a folder name to create a subfolder in the OUTPUT folder	
	In Column E, enter filepath of the source file that needs to be edited (filepaths can be obtained from Step II)	
		
	Click RUN	

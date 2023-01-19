MSC Fileman 1062 Release Notes
==============================

New Capability
--------------
- Add UNEDT on a field in an input template ensures that while a field can be entered initially in an Input Template, it cannot be edited.
- Reference Standard Mumps is now supported. See below for instructions.


Bug Fixes
---------
- Disallow storage of data into negative subscripts. This is a 40 year old bug. In the early days of Fileman, this would have been without issue; but now negative subscripts are used to indicate that an entry has been merged.
- Fileman erroneously interpreted a field as M code if the file name contained the letter "K". This caused undesirable effects in 'MODIFY FILE ATTRIBUTES', where all fields now were forced to be stored in Extract format. This is now fixed.
- Incorporate DI*22.2*14 fixes
- Incorporate DI*22.2*18 fixes
- Foreign languages with translations for Yes/No in the Dialog File, make sure that Fileman still accepts Y/N, as a lot of VistA code hardcodes that as a value. Previously, code such as DR="6///Y" would fail in such a case.
- German date/time output could not be accepted back into Fileman as a date input. That is now fixed.
- When deleting an entry in "Enter/Edit", users are normally asked if they wish to repoint pointing entries if pointers exist to the entry just deleted. A additional check has been added: If pointing files are empty, the question to repoint is not asked.
- The file verification utility now detects if the global storage location is missing. Previously, it didn't.
- Data Dictionary Listing/File ?? listings have a few cosmetic enhancements:
	- Condensed listing now displays the "Audit Security"
	- New Style Indexes now display their number in the data dictionary listings
	- Print Templates file Identifier is now cleaner
- Rename Entries in the Mumps Operating System file:
	- Add IRIS to Cache entry
	- Add YottaDB to GT.M entry
	- Add RSM to MUMPS V1 entry
- Update RSM Mumps Operating System file entry with code to allow Screenman to function
- Fix urnary + on functions in DICOMP. Previously, using +INTERNAL(#.02), for example, would add 1 to the entry.
- New Write Identifiers will now use EN^DDIOL by default now. Previously, they just used WRITE statements.
- The Meta Data Dictionary has two new computed fields, "File Number" and "File Name".

Instructions for Using REFERENCE STANDARD MUMPS
-----------------------------------------------
1. Create a database with a block size of AT LEAST 32k. 16k is not large enough for the Fileman compiled routines. E.g.

	rsm -v TST -b 32 -s 4096 tst.dat

2. Import the RSM utilities (including %RR).

3. Start the environment.

4. Import Fileman using %RR on the supplied .RSA file.

5. As the VistA Kernel isn't present, rename the kernel and helper routines like this:

	M ^$ROUTINE("%DT")=^$ROUTINE("DIDT")
	M ^$ROUTINE("%DTC")=^$ROUTINE("DIDTC")
	M ^$ROUTINE("%RCR")=^$ROUTINE("DIRCR")
	M ^$ROUTINE("%ZIS")=^$ROUTINE("DIIS")
	M ^$ROUTINE("%ZISS")=^$ROUTINE("DIISS")
	M ^$ROUTINE("%ZISC")=^$ROUTINE("DIISC")

6. Run ^DINIT, choosing RSM/MUMPS V1 as the operating system.
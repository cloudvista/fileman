MSC FILEMAN 1061

MSC FileMan has passed through many hands since it was donated to OSEHRA/VA in late 2014 (when the version number was 1051).  That process resulted in VA FileMan 22.2, the current VA version.  In the course of that process.... 
 
1. Prompts for key sequences that use the keys labelled "F1", "F2" etc on all modern keyboards were changed by VA  --backwards from MSC FileMan fixes -- to show "PF1", "PF2" etc.
 
2. Mouseclicks have been supported in ScreenMan screens for over a decade in MSC FileMan.  The code to enable these mouseclicks has made its way to VA FileMan 22.2, but this functionality is disabled by a PARAMETER when 22.2 is loaded.
 
3. In MSC FileMan, great care was taken so that wherever FileMan outputs dates, it does so in the same manner (invoking ^DD("DD")).  FileMan 22.2 removes this consistency by a change to the DIUTL routine.

4. First-line tags, like the one at the top of the DIALOG routine, have been altered.  Thus, developer code that calls ^DIALOG with parameters (as has been possible for ten years with MSC FileMan) will again encounter a backwards-incompatibility that generates a MUMPS error. 

In all these ways, FileMan 22.2 has been degraded from its source, MSC FileMan.   "MSC FileMan 1061" does NOT change earlier versions in these ways. 

Also,
  
5. The LANGUAGE File (File .85) got enhanced and restructured in VA FileMan. This is an unabashed backwards-incompatibility with all earlier versions of FileMan. Developer code that counts on what the .01 field of that File looks like will now work differently than intended.  MSC FileMan leaves the structure of File .85 as it was, while adding many fields similar to those now in VA FileMan.  If MSC FileMan is loaded on top of the "new" version of File .85, that new version will remain (unchanged by ^DINIT).

6. 22.2 creates its own implementation-specific 'kernel' code (in File .7), rather than looking at nodes in the ^%ZOSF global.  This innovation allows FileMan to run STAND-ALONE, without the presence of Kernel.   The drawback is that FileMan 22.2 system managers who want to change some Kernel code need to change it in two places  -- in a %Z routine and also in FileMan's MUMPS OPERATING SYSTEM File.  In MSC FileMan 1061, the stand-alone feature is preserved, but if the Kernel is present (as it is for 99% of all FileMan users), that Kernel code will continue to be used, in preference to what is in File .7.

On the other hand,

7. VA insisted that the full-screen word-processing editor should NOT exit when user typed two 'enters' successively at the bottom of the text.  The problem was that people would cut-and-paste hunks of text that included embedded double line feeds.  Since other (Medsphere) users had this problem, too, the "two-enters" feature of the word-processing module has been REMOVED in 1061.

The development of 22.2 revealed other bugs, which were fixed both in the VA version, and in the present MSC FileMan 1061.  1061 includes the forthcoming VA patch DI*22.2*10, which fixes other minor bugs.  Much internal documentation of FileMan files has also been added to both versions.   DINIT must be run for this documentation to be added to existing systems.

Several enhancements, not present in VA FileMan 22.2, are also included in 1061:

8. A new MUMPS OPERATING SYSTEM is defined in File .7.  This is "MUMPS V1", which Ray Newman down in Australia has been working on for years.  Might eventually be a usable small-scale open-source MUMPS OS.

9. The syntax VARIABLE-POINTER:FILE had a bug in it for decades.  If two entries in FILE have the same name, the user who enters the variable-pointer data picks between them.  But 'VARIABLE-POINTER:FILE' output didn't work, because the computed-field parser turned VARIABLE POINTER back into its EXTERNAL value and then tried to look it up in FILE.   Now, the stored, unambiguous internal value will be used. 

10. Sorting FileMan entries "backwards" (using a minus sign after the "SORT BY:" prompt) has been improved.   Sorting by reverse internal 'NUMBER' (highest number first) will be much more efficient.  And sorting by alphabetically-valued fields will finally work, showing entries from Z to A.

11. MSC FileMan 1061 introduces a new data-checking capability called CONSISTENCY CHECKS.  Developers may now add to any FileMan field one or more "checks" on data when it is input.  These optional checks are entered in "Computed Field" syntax, where each Computed-Field expression should be truth-valued.  For examples, see http://www.hardhats.org/fileman/u2/ut_input.htm .

12. MSC FileMan 1061 also introduces an interactive warning when a FileMan user tries to delete an entire entry in a File, using the syntax
         NAME: FIRST ONE// @
   If the data in the entry being deleted is sizeable, or includes any pointer to File 2, the user will have to answer an "ARE YOU SURE?" query in order to proceed with the deletion.
---
title: |
  VA FileMan 22.2

  Release Notes
---

<img src="images/media/image1.jpg" style="width:2.375in;height:2.375in"
alt="Department of Veterans Affairs official seal" />

August 2016

Department of Veterans Affairs (VA)

Office of Information and Technology (OI&T)

Enterprise Program Management Office (EPMO)

Revision History

<table>
<caption>Template Revision History showing date template was created or
revised, version number, description, and author.</caption>
<colgroup>
<col style="width: 18%" />
<col style="width: 10%" />
<col style="width: 45%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>Date</th>
<th>Version</th>
<th>Description</th>
<th>Author</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>08/15/2016</td>
<td>1.1</td>
<td><p>Tech Edits:</p>
<ul>
<li><p>Removed author notes in Section <u>2.2.1</u>.</p></li>
<li><p>Updated Section <u>2.2.1.2</u>.</p></li>
</ul></td>
<td>REDACTED</td>
</tr>
<tr class="even">
<td>08/07/2016</td>
<td>1.0</td>
<td>Initial release of VA FileMan 22.2 Release Notes.</td>
<td>VA FileMan 22.2 Development Team</td>
</tr>
</tbody>
</table>

Template Revision History showing date template was created or revised,
version number, description, and author.

Table of Contents

[1. Principal Enhancements
[1](#principal-enhancements)](#principal-enhancements)

[1.1. ScreenMan Enhancements
[1](#screenman-enhancements)](#screenman-enhancements)

[1.1.1. Use of Mouse in ScreenMan Forms
[1](#use-of-mouse-in-screenman-forms)](#use-of-mouse-in-screenman-forms)

[1.1.2. Record Selection as a Full ScreenMan Page
[1](#record-selection-as-a-full-screenman-page)](#record-selection-as-a-full-screenman-page)

[1.1.3. Expanded Multiples
[1](#expanded-multiples)](#expanded-multiples)

[1.1.4. Custom Colors Option
[1](#custom-colors-option)](#custom-colors-option)

[1.1.5. Quick Exit from Word Processing Pages
[1](#quick-exit-from-word-processing-pages)](#quick-exit-from-word-processing-pages)

[1.1.6. Indication of Word-Processing Data
[1](#indication-of-word-processing-data)](#indication-of-word-processing-data)

[1.1.7. Screen Print [1](#screen-print)](#screen-print)

[1.2. Internationalization
[2](#internationalization)](#internationalization)

[1.2.1. VA FileMan is Translation-Ready
[2](#va-fileman-is-translation-ready)](#va-fileman-is-translation-ready)

[1.2.2. New Entries in DIALOG File (#.84)
[2](#new-entries-in-dialog-file-.84)](#new-entries-in-dialog-file-.84)

[1.2.3. Many New Languages in File \#.85
[2](#many-new-languages-in-file-.85)](#many-new-languages-in-file-.85)

[1.2.4. New Dialog Framework for Data Dictionary Elements
[2](#new-dialog-framework-for-data-dictionary-elements)](#new-dialog-framework-for-data-dictionary-elements)

[1.2.5. New Entry Points to Help Translate DD Elements
[2](#new-entry-points-to-help-translate-dd-elements)](#new-entry-points-to-help-translate-dd-elements)

[1.2.6. Consistent Date Formatting
[2](#consistent-date-formatting)](#consistent-date-formatting)

[1.2.7. Date Internationalization Enhancement
[2](#date-internationalization-enhancement)](#date-internationalization-enhancement)

[1.2.8. Upper/Lowercase Translations are Consistent
[2](#upperlowercase-translations-are-consistent)](#upperlowercase-translations-are-consistent)

[1.2.9. Two- and Three-letter Language Abbreviations
[2](#two--and-three-letter-language-abbreviations)](#two--and-three-letter-language-abbreviations)

[1.3. Data Analysis Tools
[3](#data-analysis-tools)](#data-analysis-tools)

[1.3.1. Check all Pointers into a Given File
[3](#check-all-pointers-into-a-given-file)](#check-all-pointers-into-a-given-file)

[1.3.2. Automatic Auditing
[3](#automatic-auditing)](#automatic-auditing)

[1.3.3. Showing Past Changes to Data Dictionary
[3](#showing-past-changes-to-data-dictionary)](#showing-past-changes-to-data-dictionary)

[1.3.4. Showing Changes by a Specific User
[3](#showing-changes-by-a-specific-user)](#showing-changes-by-a-specific-user)

[1.3.5. Modified Auditing Menu
[3](#modified-auditing-menu)](#modified-auditing-menu)

[1.3.6. Entry Access Audit
[3](#entry-access-audit)](#entry-access-audit)

[1.3.7. Update The Meta Data Dictionary
[3](#update-the-meta-data-dictionary)](#update-the-meta-data-dictionary)

[1.3.8. Improvements to the Verify Fields Utility
[3](#improvements-to-the-verify-fields-utility)](#improvements-to-the-verify-fields-utility)

[1.3.8.1. Checks for Duplicates and Dangling Pointers
[4](#checks-for-duplicates-and-dangling-pointers)](#checks-for-duplicates-and-dangling-pointers)

[1.3.8.2. Checks Index Values Do Not Exceed Thirty-Character Limit
[4](#checks-index-values-do-not-exceed-thirty-character-limit)](#checks-index-values-do-not-exceed-thirty-character-limit)

[1.3.8.3. Output Displays Translated Field Label
[4](#output-displays-translated-field-label)](#output-displays-translated-field-label)

[1.3.8.4. Suppresses Accidental Echo of dates
[4](#suppresses-accidental-echo-of-dates)](#suppresses-accidental-echo-of-dates)

[1.3.9. Comparing Data and Data Dictionaries across Environments
[4](#comparing-data-and-data-dictionaries-across-environments)](#comparing-data-and-data-dictionaries-across-environments)

[1.4. Ability to Edit Export Template
[4](#ability-to-edit-export-template)](#ability-to-edit-export-template)

[2. Other Enhancements [4](#other-enhancements)](#other-enhancements)

[2.1. User Interface Changes
[4](#user-interface-changes)](#user-interface-changes)

[2.1.1. Select Prompt: Extended Selection by IEN
[4](#select-prompt-extended-selection-by-ien)](#select-prompt-extended-selection-by-ien)

[2.1.2. Printing Multiples in Sorted Order
[4](#printing-multiples-in-sorted-order)](#printing-multiples-in-sorted-order)

[2.1.3. VA FileMan Browser Enhancements
[4](#va-fileman-browser-enhancements)](#va-fileman-browser-enhancements)

[2.2. API Changes [5](#api-changes)](#api-changes)

[2.2.1. Enhancements to FIND^DIC and LIST^DIC
[5](#enhancements-to-finddic-and-listdic)](#enhancements-to-finddic-and-listdic)

[2.2.1.1. Third Argument (Fields)
[5](#third-argument-fields)](#third-argument-fields)

[2.2.1.2. New E Flag Returns the Complete List of Matches
[5](#new-e-flag-returns-the-complete-list-of-matches)](#new-e-flag-returns-the-complete-list-of-matches)

[2.2.1.3. Eighth Parameter (Index) of LISTˆDIC
[5](#eighth-parameter-index-of-listˆdic)](#eighth-parameter-index-of-listˆdic)

[2.2.2. New API to Create Sort Templates Silently
[5](#new-api-to-create-sort-templates-silently)](#new-api-to-create-sort-templates-silently)

[2.3. Data Dictionary Changes
[5](#data-dictionary-changes)](#data-dictionary-changes)

[2.3.1. Auditable Word Processing Fields
[5](#auditable-word-processing-fields)](#auditable-word-processing-fields)

[2.3.2. Word Processing Fields Can be Made Uneditable
[5](#word-processing-fields-can-be-made-uneditable)](#word-processing-fields-can-be-made-uneditable)

[2.3.3. Set Explicit Maximum Length for Free-text Fields
[5](#set-explicit-maximum-length-for-free-text-fields)](#set-explicit-maximum-length-for-free-text-fields)

[2.3.4. Override of Character Limit in Globals
[5](#override-of-character-limit-in-globals)](#override-of-character-limit-in-globals)

[2.4. Installation and Distribution Changes
[5](#installation-and-distribution-changes)](#installation-and-distribution-changes)

[2.4.1. DIFROM: Keys and New-Style Indexes
[5](#difrom-keys-and-new-style-indexes)](#difrom-keys-and-new-style-indexes)

[2.4.2. DINIT: Virgin Install
[6](#dinit-virgin-install)](#dinit-virgin-install)

[3. Bug Fixes [6](#bug-fixes)](#bug-fixes)

[3.1. Computed Expressions: Multiple Contains with Word-processing
Fields
[6](#computed-expressions-multiple-contains-with-word-processing-fields)](#computed-expressions-multiple-contains-with-word-processing-fields)

[3.2. Uppercasing [6](#uppercasing)](#uppercasing)

[3.3. DIFROM Maximum Routine Size
[6](#difrom-maximum-routine-size)](#difrom-maximum-routine-size)

[3.4. DIFROM Routine Size Calculation
[6](#difrom-routine-size-calculation)](#difrom-routine-size-calculation)

[3.5. Browser Display Routines Did Not Work on Caché
[6](#browser-display-routines-did-not-work-on-caché)](#browser-display-routines-did-not-work-on-caché)

[3.6. Maximum Routine Size
[6](#maximum-routine-size)](#maximum-routine-size)

[3.7. Browser Now Works without Kernel
[7](#browser-now-works-without-kernel)](#browser-now-works-without-kernel)

[3.8. Replace/With Maximum Length
[7](#replacewith-maximum-length)](#replacewith-maximum-length)

[3.9. Reverse Collation on Complex New Style Indexes When Doing Partial
Matches
[7](#reverse-collation-on-complex-new-style-indexes-when-doing-partial-matches)](#reverse-collation-on-complex-new-style-indexes-when-doing-partial-matches)

[3.10. Q Flag on LIST^DIC and FIND^DIC and Partial Numeric Matches on
Pointer Values
[7](#q-flag-on-listdic-and-finddic-and-partial-numeric-matches-on-pointer-values)](#q-flag-on-listdic-and-finddic-and-partial-numeric-matches-on-pointer-values)

[3.11. DDS3-1 New Options at Command Line
[7](#dds3-1-new-options-at-command-line)](#dds3-1-new-options-at-command-line)

[3.12. DDS3-2 New Dialog on Existing Form
[7](#dds3-2-new-dialog-on-existing-form)](#dds3-2-new-dialog-on-existing-form)

[3.13. DDS3-3 New Capabilities from Record Selection Page
[7](#dds3-3-new-capabilities-from-record-selection-page)](#dds3-3-new-capabilities-from-record-selection-page)

[3.14. DIB Warning-Data Global does Not Exist
[7](#dib-warning-data-global-does-not-exist)](#dib-warning-data-global-does-not-exist)

[3.15. DIKCUTL Non deleteable index
[8](#dikcutl-non-deleteable-index)](#dikcutl-non-deleteable-index)

[3.16. DIUTL NOW Returns Minutes
[8](#diutl-now-returns-minutes)](#diutl-now-returns-minutes)

[4. Unit Tests [8](#unit-tests)](#unit-tests)

# Principal Enhancements

## ScreenMan Enhancements

### Use of Mouse in ScreenMan Forms

ScreenMan does support the use of a mouse for emulators that support
ANSI standard control sequences to turn the mouse on and off. However,
the Department of Veterans Affairs has elected to turn this feature off
due to support complications with Attachmate Reflection. The parameter
DI SCREENMAN NO MOUSE needs to be established for SYSTEM and set to
“**Yes**”. The DI SCREENMAN NO MOUSE parameter will be set to “**YES**”
during the VA FileMan (FM) 22.2 installation.

### Record Selection as a Full ScreenMan Page

The ScreenMan Record Selection page can now be a full ScreenMan page
using a computed multiple pointer, so that the user can select an entry
by scrolling up or down. This new feature lets forms contain embedded
lookups.

You can set this up automatically when you create a form. At the query
“Do you want your Form to begin with a display of all entries, for
selection,” answer “**Yes**.” The initial position can be set to be the
user’s last selection, rather than first, last, or new.

### Expanded Multiples

Multiples within a single ScreenMan page can now be more than one line
deep.

### Custom Colors Option

The “Customize Colors” sub option within ScreenMan allows selection of
ANSI colors for all ScreenMan presentations, on a parameterized basis
(user, institution, etc.) using Kernel parameters.

### Quick Exit from Word Processing Pages

While Editing/Adding a ScreenMan word processing document, the user can
enter two carriage returns (press **Enter** twice) at the end of the
document to exit ScreenMan. This is new functionality, the user is no
longer required to use **\<PF1\>E** to exit ScreenMan.

### Indication of Word-Processing Data

A **+** now indicates, in a ScreenMan form, whether a word-processing
field already contains data. If users have their PREFERRED EDITOR field
set to “SCREEN EDITOR – VA FILEMAN”, the previous message “No existing
Text” has been modified to “THERE ARE NO LINES!” if a word-processing
field has no data.

### Screen Print

**\<PF1\>P** allows printing of the screen (including all multiples).

## Internationalization

### VA FileMan is Translation-Ready

VA FileMan is in the process of converting all *non*-developer dialogues
to use FM dialogues framework, so that translations can be table-driven.

### New Entries in DIALOG File (#.84)

Many new entries have been added to the DIALOG file (#.84) to handle
end-user interactions.

### Many New Languages in File \#.85

The LANGUAGE file (#.85) now includes entries for all ISO 639-2:1998
languages, as of the 11/21/2012 update to the standard.

### New Dialog Framework for Data Dictionary Elements

File names, field labels, set values, and help messages can be entered
into the ^DD schema for any of the **living** languages listed in the
LANGUAGE file (#.85).

### New Entry Points to Help Translate DD Elements

A new direct mode tool has been created to help translate the file name,
field names, and help prompts. The call is DO LANG^DIALOGZ().

### Consistent Date Formatting

Formatting of date output is now consistently done throughout all the
end-user routines. Changing the global node ^DD(“DD”) changes the way
all VA FileMan dates are output. Re­running ^DINIT does not change this
node.

### Date Internationalization Enhancement

The Date Internationalization has been enhanced so that when the
international format is specified using the "**I**" flag, the returned
display output is in the form DD MON YYYY instead of MON, DD YYYY.

### Upper/Lowercase Translations are Consistent

VA FileMan’s internationalization framework has been made consistently
independent of the ASCII character set, to improve support for
international case conversion.

### Two- and Three-letter Language Abbreviations

The LANGUAGE file (#.85) now can store two and three letter
abbreviations for languages.

## Data Analysis Tools

### Check all Pointers into a Given File

A fourth Data Dictionary utility (“find pointers into a file”) checks
all files with pointers into a given File. The utility gives four kinds
of output (here using PATIENT file \[#2\] as an example):

### Automatic Auditing

To improve version control for data dictionaries, DD changes are always
audited in the DD AUDIT file (#.6). There is no need to turn on DD
auditing file­by­file.

### Showing Past Changes to Data Dictionary

The “Show Past Changes to DDs” auditing option shows most DD changes
since a certain date.

<img src="images/media/image2.png"
style="width:0.33333in;height:0.33333in" alt="Note" /> **NOTE:** This
will be added in a future release and a ticket has been created in the
VA SDM system. Service Desk Ticket has been opened to fix this issue as
a VA FileMan Maintenance issue. Ticket number I7740738FY16 created on
2/26/16.

### Showing Changes by a Specific User

“Monitor a User” is now the second auditing option. It shows every entry
in an audited file touched by a given user in an audited file.

### Modified Auditing Menu

The auditing menu has been modified to be better organized and more
intuitive.

### Entry Access Audit

The ACCESSED^DIET function has been modified to replace a call that
killed the variable DIC.

### Update The Meta Data Dictionary

Use the Update The Meta Data Dictionary option on the Data Dictionary
Utilities menu to create the new META DATA DICTIONARY file (#.9). The
Meta Data Dictionary lists all fields in all files in a searchable
format.

### Improvements to the Verify Fields Utility

A number of improvements have been made to the Verify Fields Utility.

#### Checks for Duplicates and Dangling Pointers

Verify Fields checks for duplicates and dangling pointers in
cross-references. There is no new Verify Data menu and no new Verify
Pointers option. The verify pointers functionality is invoked by the
Verify Fields option on the Utilities menu.

#### Checks Index Values Do Not Exceed Thirty-Character Limit

Verify Fields checks that the index values do not exceed the
thirty-character limit.

#### Output Displays Translated Field Label

If a user's language is set to a *non*-English language, and if a
translation of a field label exists for that language, then Verify
Fields output displays the translated field label.

#### Suppresses Accidental Echo of dates

A bug was fixed to suppress the accidental echo of dates in the Verify
Fields output.

### Comparing Data and Data Dictionaries across Environments

A new Transfer menu option, Namespace Compare, lets you identify
differences in data and DDs between different MUMPS environments (on the
same server), to help with version control.

## Ability to Edit Export Template

In prior versions of VA FileMan, if a user created an Export Template
they were unable to edit that template like they could with a Sort,
Print, and Edit Templates; with VA FileMan 22.2, the user is now able to
edit an Export Template.

# Other Enhancements

## User Interface Changes

### Select Prompt: Extended Selection by IEN

Lookup enhancement: if the .01 field of the file being selected from is
a pointer to another file, you can use a double accent grave (**\`\`**)
to pick a pointed­to entry by its internal entry number (IEN).

### Printing Multiples in Sorted Order

Until now, when printing sorted records, any subentries within those
records were displayed unsorted, in order by internal entry number. A
new **B** print specifier will ensure that subentries are displayed in
order.

### VA FileMan Browser Enhancements

You can now print the text being browsed using **PF1­PF1­P**.

## API Changes

### Enhancements to FIND^DIC and LIST^DIC

#### Third Argument (Fields)

Third argument (fields) can now be a computed expression, not just a
field.

#### New E Flag Returns the Complete List of Matches

Fourth argument (flags) can now contain **E**, and it will return the
complete list of matches even if errors are encountered during the
generation of the results.

#### Eighth Parameter (Index) of LISTˆDIC

Eighth parameter (index) of LISTˆDIC can now be a sort template, a
field, or a computed expression, if the new **X** flag is included.

### New API to Create Sort Templates Silently

The BUILDNEW^DIBTED API silently creates a sort template.

## Data Dictionary Changes

### Auditable Word Processing Fields

VA FileMan security has been improved by allowing word-processing fields
to be audited.

### Word Processing Fields can be Made Uneditable

Reference files and clinically significant text can now be protected
from subsequent change.

### Set Explicit Maximum Length for Free-text Fields

The Maximum Length of output for a Free Text field can now be set; it is
not dependent on the input Transform. The Maximum Length value truncates
the stored data during output if necessary. The Maximum Length can be
set in the input Transform (Syntax) option on the VA FileMan's Utility
Options sub-menu.

### Override of Character Limit in Globals

^DD(“STRING_LIMIT”), if set, overrides the standard 255-character limit
throughout VA FileMan.

<img src="images/media/image2.png" title="Note"
style="width:0.33333in;height:0.33333in" alt="Note" /> **NOTE**: The
Post Install sets the limit to 4094.

## Installation and Distribution Changes

### DIFROM: Keys and New-Style Indexes

DIFROM has been extended to be able to transport keys and New Style
indexes.

<img src="images/media/image2.png" title="Note"
style="width:0.33333in;height:0.33333in" alt="Note" /> **NOTE**: This is
specific to standalone VA FileMan (FM). The Department of Veterans
Affairs does not use FM in this capacity.

### DINIT: Virgin Install

VA FileMan has been changed to restore its ability to run correctly
without any of the rest of Veterans Health Information Systems and
Technology Architecture (VistA) being installed.

<img src="images/media/image2.png" title="Note"
style="width:0.33333in;height:0.33333in" alt="Note" /> **NOTE**: This is
specific to standalone VA FileMan. The Department of Veterans Affairs
does not use FM in this capacity. A virgin install of FM 22.2 does not
include the META DATA DICTIONARY file (#.9) and will not include all the
languages in the LANGUAGE file (#.85).

# Bug Fixes

## Computed Expressions: Multiple Contains with Word-processing Fields

Computed Expressions with Multiple Contains, such as
(WP1\["GREEN")!(WP2\["GREEN"), are now handled correctly for
Word-processing Fields.

## Uppercasing

VA FileMan uppercasing code in DILIBF is now User Language aware.
Previously, it worked for English only.

## DIFROM Maximum Routine Size

DIFROM did not use ^DD(“ROU”) to determine the maximum routine size, but
rather had it hard­coded to 9999.

## DIFROM Routine Size Calculation

DIFROM did not correctly count the size of routines it created making
routines larger than the maximum size.

## Browser Display Routines Did Not Work on Caché

DR^DDBRU did not work on Caché due to the way %RSEL works on Caché.

## Maximum Routine Size

Maximum routine size did not get set with the first installation of VA
FileMan. The node ^DD(“ROU”) does not get initialized when installing VA
FileMan for the first time.

## Browser Now Works without Kernel

The VA FileMan Browser now works without the DEVICE file (#3.5) and can
be invoked from VA FileMan directly.

<img src="images/media/image2.png" title="Note"
style="width:0.33333in;height:0.33333in" alt="Note" /> **NOTE:** This is
specific to standalone VA FileMan. The Department of Veterans Affairs
does not use FM in this capacity.

## Replace/With Maximum Length

The replace prompt only supported input up to 245 characters long. Now,
it supports any length such that the sum of the replace length, overhead
of the field and existing characters do not exceed ˆDD("STRING_LIMIT").

## Reverse Collation on Complex New Style Indexes When Doing Partial Matches

Previously, a compound New Style index configured to sort in reverse
order still sorted in forward order upon partial matches even when it
sorted in reverse when listing entries using “**??**”. Now, it correctly
sorts in reverse order when displaying partial matches.

## Q Flag on LIST^DIC and FIND^DIC and Partial Numeric Matches on Pointer Values

Previously, using **Q** flag on DBS DIC calls caused numeric matches on
pointer fields to be partially matched a la text matches. Now, partial
numeric matches are not allowed in these circumstances.

## DDS3-1 New Options at Command Line 

Two new items are available for selection at the “COMMAND:” prompt at
the bottom of a ScreenMan screen: **Quit** and **Previous Page**. These
commands are the equivalent of the previously available **\<PF1\>Q** and
**\<PF1\>\<ArrowUp\>**.

## DDS3-2 New Dialog on Existing Form

When entering **EXIT** at the Command Line after editing data, the form
is exited and changes saved without asking a verifying question;
question has been removed. Now **\<PF1\>-E** and **EXIT** at Command
Line work the same way.

## DDS3-3 New Capabilities from Record Selection Page

You can **Exit** or **Save** data from the Record Selection page.

## DIB Warning-Data Global does Not Exist

When ENTERING or EDITing a file, the user is notified by message “DATA
GLOBAL DOES NOT EXIST” if the file header does not exist rather than
just returning to the menu.

## DIKCUTL Non deleteable index

Programmers may set the 666 node to “null” to protect a New Style index
from being deleted. For example, programmers can issue the following
command:

**S ^DD("IX",321,666)=""**

Where 321 is the assigned index number that needs to be protected from
being deleted.

## DIUTL NOW Returns Minutes

The \$\$NOWˆDIUTL function now returns the date and the minutes in the
format as defined in ˆDD(“DD”).

# Unit Tests

VA FileMan 22.2 comes with Unit Tests for classical date/time calls and
new features of the DBS LISTER and FINDER. All unit tests are under the
namespace DMU.

Per SRP 3.5, DMU is not planned to be released part of VA FileMan 22.2.

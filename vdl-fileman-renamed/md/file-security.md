<img src="images/media/image1.png" style="width:2.5in;height:1.875in"
alt="VistA" />

**VA FILEMAN (Version 22.0)**

**and KERNEL (Version 8.0)**

**FILE ACCESS SECURITY  
**

**July 2007**

Department of Veterans Affairs

Veterans Health Information Technology (VHIT)

Common Services

## Documentation Revision History

The following table displays the revision history for this document.
Revisions to the documentation are based on a continuous dialogue with
the Security Services Technical Writers and evolving industry standards
and styles.

| **Date** | **Description**            | **Author** |
|----------|----------------------------|------------|
| 7/2007   | First release of document. | REDACTED   |

<span id="_Toc172441709" class="anchor"></span>Table i: Documentation
Revision History

Contents

[Documentation Revision History
[iii](#documentation-revision-history)](#documentation-revision-history)

[Figures and Tables [vi](#figures-and-tables)](#figures-and-tables)

[Orientation [vii](#orientation)](#orientation)

[Introduction [1](#introduction)](#introduction)

[VA FileMan Reserved Symbols Used to Implement File Access Security
[1](#va-fileman-reserved-symbols-used-to-implement-file-access-security)](#va-fileman-reserved-symbols-used-to-implement-file-access-security)

[What Type of File Access Security is Your Site Using?
[3](#what-type-of-file-access-security-is-your-site-using)](#what-type-of-file-access-security-is-your-site-using)

[How to Use the File Access Security at Your Site
[6](#how-to-use-the-file-access-security-at-your-site)](#how-to-use-the-file-access-security-at-your-site)

[Classic VA FileMan File Access Security
[6](#classic-va-fileman-file-access-security)](#classic-va-fileman-file-access-security)

[File Level Security Properties
[6](#file-level-security-properties)](#file-level-security-properties)

[Kernel File Access Security
[9](#kernel-file-access-security)](#kernel-file-access-security)

[File Level Security Properties
[9](#file-level-security-properties-1)](#file-level-security-properties-1)

[Index [11](#index)](#index)

## Figures and Tables

[Table i: Documentation Revision History
[iii](#_Toc172441709)](#_Toc172441709)

[Table ii: Documentation Symbol Descriptions
[vii](#_Toc172441710)](#_Toc172441710)

[Figure 1: Example─Use VA FileMan to determine if your site is using
Kernel File Access Security [4](#_Ref168761732)](#_Ref168761732)

[Figure 2: Example─Security property values in the NEW PERSON file
(#200) [4](#_Ref168883552)](#_Ref168883552)

[Table 3: File level security properties in Classic VA FileMan file
access security [8](#_Ref168826189)](#_Ref168826189)

[Table 4: File level security properties in Kernel File Access Security
[10](#_Ref168826234)](#_Ref168826234)

## Orientation

This manual is intended for use in conjunction with the VA FileMan
Version 22.0 as it relates to access security in VistA.

**How to Use this Manual**

This manual uses several methods to highlight different aspects of the
material. The following symbols are used in the manual to alert the
reader about special information:

- Various symbols are used throughout the documentation to alert the
  > reader to special information. The following table gives a
  > description of each of these symbols:

| **Symbol**                                             | **Description**                                                                                      |
|--------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | Used to inform the reader of general information including references to additional reading material |
| ![](images/media/image3.png)                           | **Used to caution the reader to take special notice of critical information**                        |

<span id="_Toc172441710" class="anchor"></span>Table ii: Documentation
Symbol Descriptions

- Descriptive text is presented in a proportional font (as represented
  by this font).

- "Snapshots" of computer online displays (i.e., character-based screen
  captures/dialogs) and computer source code are shown in a
  *non*-proportional font and enclosed within a box. Also included are
  Graphical User Interface (GUI) Microsoft Windows images (i.e., dialogs
  or forms).

<!-- -->

- User's responses to online prompts will be boldface type.

- The "**\<Enter\>**" found within these snapshots indicate that the
  > user should press the Enter or Return key on their keyboard.

- Author's comments are displayed in italics.

<!-- -->

- All uppercase is reserved for the representation of M code, variable
  > names, or the formal name of options, field and file names, and
  > security keys (e.g., the XUPROGMODE key).

<!-- -->

- Conventions for displaying TEST data when used in this document are as
  > follows:

<!-- -->

- The first three digits (prefix) of any Social Security Numbers (SSN)
  > will begin with either "000" or "666".

- Patient and user names will be formatted as follows: \[Application
  > Name\]PATIENT,\[N\] and \[Application Name\]USER,\[N\] respectively,
  > where "Application Name" is defined in the Approved Application
  > Abbreviations document, located on the Web site listed below, and
  > where "N" represents the first name as a number spelled out and
  > incremented with each new entry.

<table>
<caption><p><span id="_Ref168826189" class="anchor"></span>Table 3: File
level security properties in Classic VA FileMan file access
security</p></caption>
<colgroup>
<col style="width: 8%" />
<col style="width: 91%" />
</colgroup>
<tbody>
<tr class="odd">
<td><img src="images/media/image2.png"
style="width:0.34722in;height:0.33333in" alt="Note" /></td>
<td><p>The list of Approved Application Abbreviations can be found at
the following Web site:</p>
<blockquote>
<p><mark>REDACTED</mark></p>
</blockquote></td>
</tr>
</tbody>
</table>

<span id="_Ref168826189" class="anchor"></span>Table 3: File level
security properties in Classic VA FileMan file access security

**Who Should Read this Manual?**

This manual has been written for personnel responsible for implementing
security at the Veterans Integrated Service Networks (VISN), to include
Information Resource Management (IRM) personnel involved with
implementing the same. If you need more information, it is suggested
that you look at the various VA OI Health Systems Design & Development
(HSD&D) home web pages for a general orientation to VistA at this
address:

> <http://vaww.vista.med.va.gov>

**Reference Materials**

Readers who wish to learn more about VA FileMan should consult the
manuals listed below located on the VHA Software Document Library in
MS-Word and PDF formats:

> <http://www.va.gov/vdl/application.asp?appid=5>

- *VA FileMan V. 22.0 Release Notes*

- *VA FileMan V. 22.0 Installation Guide*

- *VA FileMan V. 22.0 Technical Manual*

<!-- -->

- *VA FileMan V. 22.0 Getting Started Manual*

- *VA FileMan V. 22.0 Advanced User Manual*

- *VA FileMan V. 22.0 Programmer Manual*

VA FileMan documentation can also be accessed in HTML format at the
following Web site:

> <span class="mark">REDACTED</span>

VistA documentation is made available online in Microsoft Word format
and in Adobe Acrobat Portable Document Format (PDF). Adobe Acrobat
Portable (PDF) documents *must* be read using the Adobe Acrobat Reader
(i.e., ACROREAD.EXE), which is freely distributed by Adobe Systems
Incorporated at the following web address:

<http://www.adobe.com/>

|                                                        |                                                                                                                                                                                        |
|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | For more information on the use of Adobe Acrobat Reader, please refer to the "Adobe Acrobat Quick Guide" at the following web address: <http://vista.med.va.gov/iis/acrobat/index.asp> |

<span id="_Ref168826234" class="anchor"></span>Table 4: File level
security properties in Kernel File Access Security

VistA documentation and software can also be downloaded from the
Enterprise VistA Support (EVS) anonymous directories:

- **Preferred Method download.vista.med.va.gov**

|                                                        |                                                                      |
|--------------------------------------------------------|----------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.33333in;height:0.33333in" alt="Note" />  | This method transmits the files from the first available FTP server. |

- Albany OIFO REDACTED

- Hines OIFO REDACTED

- Salt Lake City OIFO REDACTED

**How to Obtain Technical Information Online**

**Obtaining Data Dictionary Listings**

Technical information about VistA M-based files and their associated
fields is stored in data dictionaries. You can use the List File
Attributes option on the Data Dictionary Utilities submenu in VA FileMan
to print formatted data dictionaries.

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 92%" />
</colgroup>
<tbody>
<tr class="odd">
<td><img src="images/media/image2.png"
style="width:0.33333in;height:0.33333in" alt="Note" /></td>
<td><p>For details about obtaining data dictionaries and about the
formats available, please refer to the "List File Attributes" chapter in
the "File Management" section of the <em>VA FileMan Advanced User
Manual</em> located at the following address:</p>
<blockquote>
<p><a
href="http://www.va.gov/vdl/application.asp?appid=5">http://www.va.gov/vdl/application.asp?appid=5</a></p>
</blockquote></td>
</tr>
</tbody>
</table>

|                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|-----------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image4.png"                        
 style="width:0.45139in;height:0.45139in" alt="Caution" />  | **DISCLAIMER: The appearance of external hyperlink references in this manual does not constitute endorsement by the Department of Veterans Affairs (VA) of this Web site or the information, products, or services contained therein. The VA does not exercise any editorial control over the information you may find at these locations. Such links are provided and are consistent with the stated purpose of this VA Intranet Service.** |

## Introduction

VA FileMan is VistA's database management system. VA FileMan APIs are
divided up into two categories:

- Classic VA FileMan─Certain modules within VA FileMan are callable by
  > other M routines or when using the VA FileMan exported menu options.
  > File access security checking is performed via Classic FileMan APIs.

|                                                        |                                                                                                                                                        |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | Another implementation of file access security checking is done via Kernel File Access Security. This topic is detailed further in this documentation. |

- Database Server (DBS)─No file access security checking is performed on
  > VA FileMan Database Server (DBS) calls because they separate
  > interactions with the database created by programmers. They are
  > "silent," meaning there is no interaction with the end-user.

|                                                        |                                                                                                        |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | There is no further discussion about the VA FileMan Database Server (DBS) calls in this documentation. |

### VA FileMan Reserved Symbols Used to Implement File Access Security

VA FileMan recognizes the two symbols listed below. All other symbols
are available to use in order to implement site file access security via
Classic FileMan APIs at the developer or VA Facilities discretion.
DUZ(0) is set after the user has been validated by the Kernel. The value
for any user's DUZ(0) can be found in the NEW PERSON file (#200), FILE
MANAGER ACCESS CODE field (#3).

- At-sign (@)─Programmer access in VistA is defined as DUZ(0)="@". It
  grants the privilege to become a programmer in VistA. Programmer
  access allows you to work outside many of the security controls
  enforced by VA FileMan, enables access to all VA FileMan files, access
  to modify data dictionaries, etc. It is important to proceed with
  caution when having access to the system in this way.

- Caret (^)─The caret (^) trumps the at-sign (@). For example, if the
  user's DUZ(0)="@", but WR ACCESS is set to a caret (^), that user
  cannot write (e.g., via the VA FileMan Enter Or Edit File Entries
  option) to that file. This is often used at the field level,
  obstructing all DUZ(0) access to that field.

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 92%" />
</colgroup>
<tbody>
<tr class="odd">
<td><img src="images/media/image2.png"
style="width:0.34722in;height:0.33333in" alt="Note" /></td>
<td><p>For information about DUZ(0)="@" programmer access in VistA,
consult the <em>VA FileMan V. 22.0 Programmer Manual</em>, located on
the VHA Software Document Library:</p>
<blockquote>
<p><a
href="http://www.va.gov/vdl/application.asp?appid=5">http://www.va.gov/vdl/application.asp?appid=5</a></p>
</blockquote></td>
</tr>
</tbody>
</table>

## 

# What Type of File Access Security is Your Site Using?

Security control for file access at VA Facilities is implemented via
either of the following two methods:

- Classic VA FileMan file access security

- Kernel File Access Security

In order to know how to manage file security at your site, it is first
necessary to determine which security implementation your site is using.
An easy way to determine if the Kernel File Access Security option
\[XUFILEACCESS\] has been implemented is to use the VA FileMan Data
Dictionary Utilities option \[DI DDU\], as shown in Figure 1.

Select the List File Attributes option \[DILIST\]. At the "START WITH
WHAT FILE:" prompt, select a VistA Fileman file from which to display
the data dictionary. If your site is using Kernel File Access Security,
the following message will appear after the file description and
security access information is displayed, Figure 1:

> (NOTE: Kernel's File Access Security has been installed in this UCI.)

|                                                        |                                                                                                                      |
|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | The file used to create the screen capture in Figure 1 is fictitious and used only for the purposes of this example. |

VA FileMan 22.0

Select OPTION: **?**

Answer with OPTION NUMBER, or NAME

Choose from:

1 ENTER OR EDIT FILE ENTRIES

2 PRINT FILE ENTRIES

3 SEARCH FILE ENTRIES

4 MODIFY FILE ATTRIBUTES

5 INQUIRE TO FILE ENTRIES

6 UTILITY FUNCTIONS

7 OTHER OPTIONS

8 DATA DICTIONARY UTILITIES

9 TRANSFER ENTRIES

Select OPTION: **8 \<Enter\>** DATA DICTIONARY UTILITIES

Select DATA DICTIONARY UTILITY OPTION: **?**

Answer with DATA DICTIONARY UTILITY OPTION NUMBER, or NAME

Choose from:

1 LIST FILE ATTRIBUTES

2 MAP POINTER RELATIONS

3 CHECK/FIX DD STRUCTURE

Select DATA DICTIONARY UTILITY OPTION: **1 \<Enter\>** LIST FILE
ATTRIBUTES

START WITH WHAT FILE: FILE// **EXAMPLE \<Enter\>**

GO TO WHAT FILE: EXAMPLE// **\<Enter\>**

Select SUB-FILE: **\<Enter\>**

Select LISTING FORMAT: STANDARD// **\<Enter\>**

Start with field: FIRST// **\<Enter\>**

DEVICE: **\<Enter\>** Right Margin: 80// **\<Enter\>**

STANDARD DATA DICTIONARY \#123 -- EXAMPLE FILE JUN 5,2007@15:57:14 PAGE
1

STORED IN ^MYGLOBAL(123, (999 ENTRIES) SITE: NVS.FO-ANYSITE.MED.VA.GOV
UCI: NVS,NOU (VERSION 8.0)

DATA NAME GLOBAL DATA

ELEMENT TITLE LOCATION TYPE

-------------------------------------------------------------------------------

This is an example file.

DD ACCESS: @

RD ACCESS: D

WR ACCESS: d

DEL ACCESS: d

LAYGO ACCESS: d

AUDIT ACCESS: @

(NOTE: Kernel's File Access Security has been installed in this UCI.)

*\[Data Dictionary listing continues as it would normally…\]*

<span id="_Ref168761732" class="anchor"></span>Figure 1: Example─Use VA
FileMan to determine if your site is using Kernel File Access Security

If your VA Facility has implemented Kernel File Access Security, it is
not using Classic VA FileMan file access security.

|                                                        |                                                                                                                                                                                  |
|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | Developers can also verify Kernel File Access Security by checking for the ^VA(200,"AFOF") cross-reference. If it exists, then Kernel File Access Security has been implemented. |

Figure 2 shows user field values in the NEW PERSON file (#200) using the
same fictitious EXAMPLE file (#123) from Figure 1.

NEW PERSON LIST JUN 6,2007 06:18 PAGE 1

FILE MANAGER

NAME ACCESS CODE

DD DEL LAYGO RD WR AUDIT

FILE ACCESS ACCESS ACCESS ACCESS ACCESS ACCESS

---------------------------------------------------------------------------------------------

FMUSER,ONE dS

EXAMPLE YES

<span id="_Ref168883552" class="anchor"></span>Figure 2:
Example─Security property values in the NEW PERSON file (#200)

A Null value is equal to a "NO." In Figure 2, the DUZ(0) for the user
named ONE FMUSER is equal to “dS.” Based on the security access shown in
Figure 1, this indicates that the user does not have READ (RD) access.

|                                                        |                                                                                                                                                                                                                                                       |
|--------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | For information on the difference between Kernel and VA Classic FileMan file access security, see the following topic "Difference in Behavior Between Kernel File Access Security and Classic VA FileMan File Access Security" in this documentation. |

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 92%" />
</colgroup>
<tbody>
<tr class="odd">
<td><img src="images/media/image2.png"
style="width:0.34722in;height:0.33333in" alt="Note" /></td>
<td><p>For information about Kernel File Access Security, consult the
<em>Kernel Systems Management Guide, Version 8.0</em>, in the "File
Access Security" chapter, located on the VHA Software Document
Library:</p>
<blockquote>
<p><a
href="http://www.va.gov/vdl/application.asp?appid=10">http://www.va.gov/vdl/application.asp?appid=10</a></p>
</blockquote></td>
</tr>
</tbody>
</table>

# How to Use the File Access Security at Your Site

- If your VA Facility is *not* using Kernel File Access Security, read
  > the section titled "Classic VA FileMan File Access Security"

- If your VA Facility *is* using Kernel File Access Security, read the
  > section titled "Kernel File Access Security"

### Classic VA FileMan File Access Security

Given the example in Figure 1, if you *do not* see the message "(NOTE:
Kernel's File Access Security has been installed in this UCI.)" when
displaying a VistA file in the VA FileMan Data Dictionary Utilities
option, then your site has not implemented Kernel File Access Security.
This means that file access security at your site is implemented based
on VA FileMan symbol(s) that are set into the security access property
for a particular file via Classic FileMan APIs. User file access is
based upon the VA FileMan symbols contained in the DUZ(0) value.

**Example**

In this example, the RD ACCESS for the fictitious file, EXAMPLE file
(#123), in Figure 1 is equal to "D," and the user’s DUZ(0) is equal to
"AaZz." This means that the user will not be able to view the data via
VA FileMan’s exported menus because the DUZ(0) does not contain the
symbol "D." If that same user’s DUZ(0) was equal to Aa**D**Zz, then the
user *is* authorized to view the file's data via the VA FileMan’s
exported menus because the DUZ(0) contains the symbol "D."

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 92%" />
</colgroup>
<tbody>
<tr class="odd">
<td><img src="images/media/image2.png"
style="width:0.34722in;height:0.33333in" alt="Note" /></td>
<td><h5
id="difference-in-behavior-between-kernel-file-access-security-and-classic-va-fileman-file-access-security">Difference
in Behavior Between Kernel File Access Security and Classic VA FileMan
File Access Security </h5>
<p>In the Classic VA FileMan file access security environment, the user
(shown in the previous example) would <em>not</em> be authorized to view
the data contained in the EXAMPLE file (#123) via the VA FileMan
exported menu option(s) because the user's (ONE FMUSER) FILEMANAGER
ACCESS CODE field (#3) does not contain the symbol "D." However, in a
Kernel File Access Security environment, the file RD ACCESS is set to
Yes for the user. Hence the user <em>would be able</em> to view the
data.</p></td>
</tr>
</tbody>
</table>

#### File Level Security Properties

There are six security properties involved with file access security,
Table 3. If a security property is not defined, the value is null. In
the Classic VA FileMan file access security environment, properties with
null values open up full user access to the VA FileMan exported menu
option(s) for that property.

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 44%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Access</strong></th>
<th><strong>Security Property Description</strong></th>
<th><strong>Property Location (Classic VA FileMan)</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>AUDIT</td>
<td><p>The AUDIT security property controls the setting of auditing
characteristics and the deletion of audit trails. Examples of the VA
FileMan options that this property controls are as follows:</p>
<ul>
<li><p>Fields Being Audited [DIAUDITED FIELDS]</p></li>
<li><p>Data Dictionaries Being Audited [DIAUDIT DD]</p></li>
<li><p>Purge Data Audits [DIAUDIT PURGE DATA]</p></li>
<li><p>Purge DD Audits [DIAUDIT PURGE DD]</p></li>
<li><p>Turn Data Audit On/Off [DIAUDIT TURN ON/OFF]</p></li>
</ul></td>
<td>^DIC(&lt;file number&gt;,0,”AUDIT”)=&lt;value&gt;</td>
</tr>
<tr class="even">
<td>DATA DICTIONARY<br />
"DD"</td>
<td><p>The DATA DICTIONARY security property controls who has access to
modify the data dictionary. Examples of the VA FileMan options that this
property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Modify File Attributes [DIMODIFY]</p>
</blockquote></li>
<li><blockquote>
<p>Utility Functions [DIUTILITY]/(Data Dictionary [DIDDU])</p>
</blockquote></li>
</ul></td>
<td>^DIC(&lt;file number&gt;,0,”DD”)=&lt;value&gt;</td>
</tr>
<tr class="odd">
<td>DELETE "DEL"</td>
<td><p>The DELETE security property controls who can delete an existing
record that is contained within the file. Examples of the VA FileMan
options that this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer Entries [DITRANSFER]</p>
</blockquote></li>
</ul></td>
<td>^DIC(&lt;file number&gt;,0,”DEL”)=&lt;value&gt;</td>
</tr>
<tr class="even">
<td>LAYGO</td>
<td><p>The LAYGO (Learn As You Go) security property controls who can
add a new record to the file. Examples of the VA FileMan options that
this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
</ul>
<p>NOTE: You must have LAYGO and WRITE access to a file to add new
entries. In addition, you must have WRITE access at the field level for
all required identifier fields.</p></td>
<td>^DIC(&lt;file number&gt;,0,”LAYGO”)=&lt;value&gt;</td>
</tr>
<tr class="odd">
<td>READ "RD"</td>
<td><p>The Read security property controls who has access to read data
contained within a file. Examples of the VA FileMan options that this
property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Print File Entries [DIPRINT]</p>
</blockquote></li>
<li><blockquote>
<p>Search File Entries [DISEARCH]</p>
</blockquote></li>
<li><blockquote>
<p>Inquire to File Entries [DIINQUIRE]</p>
</blockquote></li>
<li><blockquote>
<p>Statistics [DISTATISTICS], List File Attributes [DILIST]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer File Entries [DITRANSFER] (transfer-from file)</p>
</blockquote></li>
</ul></td>
<td>^DIC(&lt;file number&gt;,0,”RD”)=&lt;value&gt;</td>
</tr>
<tr class="even">
<td>WRITE "WR"</td>
<td><p>The WRITE security property controls who can alter data in an
existing record that is contained within the file. Examples of the VA
FileMan options that this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer [File] Entries [DITRANSFER] (transfer-to file)</p>
</blockquote></li>
</ul></td>
<td>^DIC(&lt;file number&gt;,0,”WR”)=&lt;value&gt;</td>
</tr>
</tbody>
</table>

###  Kernel File Access Security

Given the example in Figure 1, if you *do* see the message "(NOTE:
Kernel's File Access Security has been installed in this UCI.)" when
displaying a VistA file in the VA FileMan Data Dictionary Utilities
option, file access security is controlled by the ACCESSIBLE FILE
multiple (#32) in the NEW PERSON file (#200). This means that file
access security to a particular file is *not* based on the VA FileMan
Access Code DUZ(0) value. Rather, a lookup is done on the user’s
ACCESSIBLE FILE multiple (#32) record in the NEW PERSON file (#200) to
determine which accesses are allowed to the file in question via VA
FileMan exported menus. If the users VA FileMan Access Code \[i.e.,
DUZ(0)\] is equal to the at-sign (**@**), they are allowed access to all
files.

|                                                        |                                                                                  |
|--------------------------------------------------------|----------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | Kernel File Access Security is known as an Access Control List in other systems. |

#### File Level Security Properties

There are six security properties involved with file access security
that are equivalent to the Classic VA FileMan file access security,
Table 4. Unlike Classic VA FileMan file access security, in a Kernel
File Access Security environment, if the security property is not
defined, the VA FileMan exported menu option(s) for that property are
*not* open to full access for users.

|                                                        |                                                                                                                                                                                         |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                     
 style="width:0.34722in;height:0.33333in" alt="Note" />  | These same security properties left undefined in a Classic VA FileMan file access security environment open the related VA FileMan exported menu option(s) up to full access for users. |

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 49%" />
<col style="width: 34%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Access</strong></th>
<th><strong>Security Property Description</strong></th>
<th><strong>Property Location (Kernel File<br />
Access Security)</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>AUDIT</td>
<td><p>The AUDIT security property controls the setting of auditing
characteristics and the deletion of audit trails. Examples of the VA
FileMan options that this property controls are as follows:</p>
<ul>
<li><p>Fields Being Audited [DIAUDITED FIELDS]</p></li>
<li><p>Data Dictionaries Being Audited [DIAUDIT DD]</p></li>
<li><p>Purge Data Audits [DIAUDIT PURGE DATA]</p></li>
<li><p>Purge DD Audits [DIAUDIT PURGE DD]</p></li>
<li><p>Turn Data Audit On/Off [DIAUDIT TURN ON/OFF]</p></li>
</ul></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: AUDIT ACCESS (#6)</p></td>
</tr>
<tr class="even">
<td>DATA DICTIONARY<br />
"DD"</td>
<td><p>The DATA DICTIONARY security property controls who has access to
modify the data dictionary. Examples of the VA FileMan options that this
property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Modify File Attributes [DIMODIFY]</p>
</blockquote></li>
<li><blockquote>
<p>Utility Functions [DIUTILITY]/(Data Dictionary [DIDDU])</p>
</blockquote></li>
</ul></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: DATA DICTIONARY ACCESS (#1)</p></td>
</tr>
<tr class="odd">
<td>DELETE "DEL"</td>
<td><p>The DELETE security property controls who can delete an existing
record that is contained within the file. Examples of the VA FileMan
options that this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer Entries [DITRANSFER]</p>
</blockquote></li>
</ul></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: DELETE ACCESS (#2)</p></td>
</tr>
<tr class="even">
<td>LAYGO</td>
<td><p>The LAYGO (Learn As You Go) security property controls who can
add a new record to the file. Examples of the VA FileMan options that
this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
</ul>
<p>NOTE: You must have LAYGO as well as WRITE access to a file to add
new entries. Additionally, you must have WRITE access at the field level
for all required identifier fields.</p></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: LAYGO ACCESS (#3)</p></td>
</tr>
<tr class="odd">
<td>READ "RD"</td>
<td><p>The READ security property controls who has access to read data
contained within a file. Examples of the VA FileMan options that this
property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Print File Entries [DIPRINT]</p>
</blockquote></li>
<li><blockquote>
<p>Search File Entries [DISEARCH]</p>
</blockquote></li>
<li><blockquote>
<p>Inquire to File Entries [DIINQUIRE]</p>
</blockquote></li>
<li><blockquote>
<p>Statistics [DISTATISTICS], List File Attributes [DILIST]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer File Entries [DITRANSFER] (transfer-from file)</p>
</blockquote></li>
</ul></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: READ ACCESS (#4)</p></td>
</tr>
<tr class="even">
<td>WRITE "WR"</td>
<td><p>The WRITE security property controls who can alter data in an
existing record that is contained within the file. Examples of the VA
FileMan options that this property controls are as follows:</p>
<ul>
<li><blockquote>
<p>Enter or Edit File Entries [DIEDIT]</p>
</blockquote></li>
<li><blockquote>
<p>Transfer [File] Entries [DITRANSFER] (transfer-to file)</p>
</blockquote></li>
</ul></td>
<td><p>File: NEW PERSON (#200)</p>
<p>Multiple: ACCESSIBLE FILE (#32)</p>
<p>Property: WRITE ACCESS (#5)</p></td>
</tr>
</tbody>
</table>

## Index

A

ACCESSIBLE FILE multiple (#32), 10

Adobe Acrobat Reader, x

Anonymous Directories, xi

Approved Application Abbreviations, x

AUDIT security properties, 7, 10

C

Classic VA FileMan APIs, 1

Classic VA FileMan file access security, 3, 7, 12

Is Your Site Using Classic VA FileMan File Access Security?, 7

Security Access and Properties, 7

Contents, v

D

Data Dictionary

Data Dictionary Utilities Menu, xi, 3

Listings, xi

DATA DICTIONARY security properties, 8, 10

Database Server (DBS) APIs, 1

DELETE "DEL" security properties, 8, 11

Document History, iii

Documentation Symbols, ix

DUZ(0)="@", 1

E

EVS Anonymous Directories, xi

F

Figures, vii

File Access Security

Classic VA FileMan file access security, 3, 7, 12

Kernel File Access Security, 3, 10, 12

Security Access and Properties, 7, 10

file access security via Classic FileMan APIs

at-sign (@), 1

caret (^), 1

File Access Security, VA FileMan Symbols Used to Implement, 1

File Level Security Properties, 7, 10

FILE MANAGER ACCESS CODE field (#3), 1

FileMan

Classic VA FileMan APIs, 1

Database Server (DBS), 1

symbols used to implement file access security, 1

VistA's database management system, 1

FILEMANAGER ACCESS CODE field (#3), 7

FTP directories, xi

H

How to

Obtain Technical Information Online, xi

How to Use this Manual, ix

I

Introduction, 1

Is Your Site Using Classic VA FileMan File Access Security?, 7

Is Your Site Using Kernel File Access Security?, 10

K

Kernel File Access Security, 3, 10, 12

DI DDU, 3

Is Your Site Using Kernel File Access Security?, 10

Security Access and Properties, 10

VA FileMan Data Dictionary Utilities, 3

XUFILEACCESS, 3

L

LAYGO security properties, 8, 11

List File Attributes Option, xi, 3

M

menu text

List File Attributes, xi, 3

N

NEW PERSON file (#200)

ACCESSIBLE FILE multiple (#32), 10

FILE MANAGER ACCESS CODE field (#3), 1

O

Online

Technical Information, How to Obtain, xi

Orientation, ix

conventions for displaying TEST data, ix

EVS Anonymous Directories, xi

P

patient & user names

test data, ix

Programmer access

DUZ(0)="@", 1

R

READ "RD" security properties, 8, 11

Reference Materials, x

Revision History, iii

S

security properties

AUDIT, 7, 10

DATA DICTIONARY, 8, 10

DELETE "DEL", 8, 11

LAYGO, 8, 11

READ "RD", 8, 11

WRITE "WR", 9, 11

Social Security Numbers

test data, ix

Symbols Found in the Documentation, ix

T

test data

patient & user names, ix

Social Security Numbers, ix

V

VA FileMan file access security, Classic, 3, 7, 12

Is Your Site Using Classic VA FileMan File Access Security?, 7

Security Access and Properties, 7

VA FileMan Symbols Used to Implement File Access Security, 1

VistA's database management system, FileMan, 1

W

Who Should Read this Manual?, x

WRITE "WR" security properties, 9, 11

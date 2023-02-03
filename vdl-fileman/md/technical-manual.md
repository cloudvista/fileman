---
title: |
  VA FileMan 22.2

  Technical Manual
---

<img src="images/media/image1.jpeg"
style="width:2.34722in;height:2.34722in"
alt="Department of Veterans Affairs official seal" />

July 2022

Department of Veterans Affairs (VA)

Office of Information and Technology (OIT)

Development, Security, and Operations (DSO)

<span id="_Toc41989686" class="anchor"></span>

Revision History

<table>
<caption><p><span id="_Ref386465892" class="anchor"></span>Table :
Documentation Symbol Descriptions</p></caption>
<colgroup>
<col style="width: 15%" />
<col style="width: 13%" />
<col style="width: 42%" />
<col style="width: 27%" />
</colgroup>
<thead>
<tr class="header">
<th>Date</th>
<th>Revision</th>
<th>Description</th>
<th>Author</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>07/06/2022</td>
<td>1.9</td>
<td><p>Updates:</p>
<ul>
<li><p>Section <u>4.1</u>, "<u>Routines and Callable Entry Points</u>:"
<u>Table 5</u>:</p></li>
</ul>
<ul>
<li><p>Updated <strong>DDE*</strong> entry: Changed "<strong>Entity
Mapping</strong>" menu to "<strong>Data Mapping</strong>" menu.</p></li>
<li><p>Updated <strong>DDE1A</strong> entry: Changed "<strong>Entity
Enter/Edit</strong>" to "<strong>Enter/Edit an
Entity</strong>".</p></li>
</ul>
<ul>
<li><p>Section <u>4.5</u>, "<u>Direct Mode VA FileMan</u>:"</p></li>
</ul>
<ul>
<li><p>Changed "<strong>ENTITY MAPPING</strong>" to "<strong>DATA
MAPPING</strong>".</p></li>
<li><p>Changed "<strong>AUTO GEN ENTITY FOR A DD #</strong>" to
"<strong>GENERATE AN ENTITY FOR A FILE</strong>”.</p></li>
<li><p>Changed <strong>"INQUIRE TO ENTITY FILE</strong>" to
"<strong>PRINT AN ENTITY</strong>”.</p></li>
<li><p>Changed "<strong>ENTITY ENTER/EDIT</strong>" to
"<strong>ENTER/EDIT AN ENTITY</strong>".</p></li>
</ul>
<ul>
<li><p>Section <u>4.6</u>, “<u>VA FileMan Options</u>:” Updated Menu
Text for the following DDE option: <strong>Enter/Edit an Entity</strong>
[DDE ENTITY ENTER/EDIT] Option.</p></li>
</ul></td>
<td>Vista Infrastructure Shared Services (VISS) Development Team</td>
</tr>
<tr class="even">
<td>11/10/2021</td>
<td>1.8</td>
<td><p>Added DDE* components to the following sections:</p>
<ul>
<li><p>Section <u>4.1</u>, “<u>Routines and Callable Entry Points</u>:”
Added <strong>DDE*</strong> routine descriptions and added
<strong>DDEPRT</strong> routine to <u>Table 5</u>.</p></li>
<li><p>Section <u>4.6</u>, “<u>VA FileMan Options</u>:” Added
<strong>DDE*</strong> options attached to the <strong>Other
Options</strong> [DIOTHER] menu branch in <u>Figure 3</u>:</p></li>
</ul>
<ul>
<li><p><strong>Entity Mapping</strong> [DDE ENTITY MAPPING]
Menu.</p></li>
<li><p><strong>Auto Gen Entity for a DD #</strong> [DDE AUTO GEN ENTITY
FOR A DD #] Option.</p></li>
<li><p><strong>Entity Enter/Edit</strong> [DDE ENTITY ENTER/EDIT]
Option.</p></li>
<li><p><strong>Inquire to Entity File</strong> [DDE ENTITY INQUIRE]
Option.</p></li>
</ul></td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="odd">
<td>02/04/2019</td>
<td>1.7</td>
<td>Updated Section <u>4.5</u> to add menu option numbers.</td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="even">
<td>01/30/2019</td>
<td>1.6</td>
<td><p>Changes for Patch DI*22.2*9:</p>
<ul>
<li><p>Added ENTITY (#1.5) file global in <u>Table 3</u> and Section
<u>10</u>.</p></li>
<li><p>Added ENTITY (#1.5) file and description in <u>Table
4</u>.</p></li>
<li><p>Added DDE routines to <u>Table 5</u>.</p></li>
<li><p>Updated Section <u>4.5</u> to add DDE menu and submenu
options.</p></li>
<li><p>Added Section <u>5.18</u> with a list of cross-references for the
ENTITY (#1.5) file.</p></li>
</ul></td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="odd">
<td>10/01/2018</td>
<td>1.5</td>
<td><p>Reviewer Feedback Edits:</p>
<ul>
<li><p>Added the <strong>DDERR</strong> routine to <u>Table
5</u>.</p></li>
<li><p>Added field numbers to <u>Table 23</u>.</p></li>
</ul></td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="even">
<td>05/16/2018</td>
<td>1.4</td>
<td><p>Updated <u>Figure 3: VA FileMan Exported Options Diagrams</u> in
Section 4.5 - VA FileMan with Kernel. Removed references to the
following options, since they have been deleted with Patch
DI*22.2*10:</p>
<ul>
<li><p>DI DATA TYPE OPTIONS</p></li>
<li><p>DI DATA TYPE FILE</p></li>
<li><p>DI DATA TYPE METHOD FILE</p></li>
<li><p>DI DATA TYPE PROPERTY FILE</p></li>
</ul></td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="odd">
<td>08/07/2017</td>
<td>1.3</td>
<td>Changes for patch DI*22.2*6 (Data Sync functionality)</td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="even">
<td>08/07/2017</td>
<td>1.2</td>
<td><p>Tech edits for patch DI*22.2*8, Data Access Control (DAC):</p>
<ul>
<li><p>Added new Data Access Control (DAC) files to the “<u>Files</u>”
section.</p></li>
<li><p>Added new DAC routines to the “<u>Routines, Application
Programming Interfaces (APIs), and Options</u>” section.</p></li>
<li><p>Added new DAC options to the “<u>VA FileMan Options</u>”
section.</p></li>
<li><p>Reformatted display of file and field names throughout; moved
file/field number immediately following the file/field name.</p></li>
</ul></td>
<td>VistA Kernel (VistA Infrastructure [VI]) Development Team</td>
</tr>
<tr class="odd">
<td>01/17/2017</td>
<td>1.1</td>
<td><p>Changes for patch DI*22.2*2:</p>
<ul>
<li><p>Updated <u>Table 3: VA FileMan Routine Global References</u> in
Orientation section. Added ^DIT.</p></li>
<li><p>Updated <u>Table 4: VA FileMan File List</u> in Section 3 –
Files. Added .86, .87, 1.71 and 1.72., and updated .9.</p></li>
<li><p>Updated <u>Figure 2: VA FileMan Pointer Map</u> in Section 3.1 –
Pointer Map. Added .86 and .87.</p></li>
<li><p>Updated <u>Table 5: VA FileMan Routines and Callable Entry
Points</u> in Section 4 – Routines and Callable Routines/Entry
Points/Application Programming Interfaces (APIs). Added DDPA2, DDSRP,
DICATTD8, DICATTUD, DIETLIB, DIFMEDT1, DITIME, DIUTC, and updated DDD
and DIALOGZ.</p></li>
<li><p>Updated <u>Figure 3: VA FileMan Exported Options Diagrams</u> in
Section 4.5 - VA FileMan with Kernel. Added DI DATA TYPE
OPTIONS.</p></li>
<li><p>Update global list in Section 10 <u>Globals</u>. Added
<strong>^DIT</strong>.</p></li>
</ul></td>
<td>VA FileMan 23.0 Development Team</td>
</tr>
<tr class="even">
<td>08/03/2016</td>
<td>1.0</td>
<td>Initial release of VA FileMan 22.2 Release Notes.</td>
<td>VA FileMan 22.2 Development Team</td>
</tr>
</tbody>
</table>

<span id="_Ref386465892" class="anchor"></span>Table : Documentation
Symbol Descriptions

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For the
current patch history related to this software, see the Patch Module
(i.e., Patch User Menu \[A1AE USER\]) on FORUM.

Table of Contents

[Revision History [ii](#_Toc41989686)](#_Toc41989686)

[List of Figures [vii](#_Toc108021444)](#_Toc108021444)

[List of Tables [viii](#_Toc108021445)](#_Toc108021445)

[Orientation [ix](#_Toc108021446)](#_Toc108021446)

[1 Introduction [1](#introduction)](#introduction)

[2 Implementation and Maintenance
[1](#implementation-and-maintenance)](#implementation-and-maintenance)

[3 Files [3](#files)](#files)

[3.1 Pointer Map [12](#pointer-map)](#pointer-map)

[4 Routines, Application Programming Interfaces (APIs), and Options
[17](#routines-application-programming-interfaces-apis-and-options)](#routines-application-programming-interfaces-apis-and-options)

[4.1 Routines and Callable Entry Points
[17](#routines-and-callable-entry-points)](#routines-and-callable-entry-points)

[4.2 Direct Mode Utilities
[38](#direct-mode-utilities)](#direct-mode-utilities)

[4.3 ScreenMan-Specific Utilities
[38](#screenman-specific-utilities)](#screenman-specific-utilities)

[4.4 Mapping Routines [39](#mapping-routines)](#mapping-routines)

[4.5 Direct Mode VA FileMan
[39](#direct-mode-va-fileman)](#direct-mode-va-fileman)

[4.6 VA FileMan Options [43](#va-fileman-options)](#va-fileman-options)

[5 Cross-References [50](#cross-references)](#cross-references)

[5.1 INDEX (#.11) File [50](#index-.11-file)](#index-.11-file)

[5.2 KEY (#.31) File [51](#key-.31-file)](#key-.31-file)

[5.3 PRINT TEMPLATE (#.4) File
[52](#print-template-.4-file)](#print-template-.4-file)

[5.4 SORT TEMPLATE (#.401) File [53](#_Toc108021462)](#_Toc108021462)

[5.5 INPUT TEMPLATE (#.402) File [53](#_Toc108021463)](#_Toc108021463)

[5.6 FORM (#.403) File [54](#form-.403-file)](#form-.403-file)

[5.7 BLOCK (#.404) File [54](#_Toc108021465)](#_Toc108021465)

[5.8 FOREIGN FORMAT (#.44) File
[55](#foreign-format-.44-file)](#foreign-format-.44-file)

[5.9 IMPORT TEMPLATE (#.46) File
[55](#import-template-.46-file)](#import-template-.46-file)

[5.10 DD AUDIT (#.6) File [55](#dd-audit-.6-file)](#dd-audit-.6-file)

[5.11 DATA TYPE (#.81) File
[55](#data-type-.81-file)](#data-type-.81-file)

[5.12 COMPILED ROUTINE (#.83) File
[56](#compiled-routine-.83-file)](#compiled-routine-.83-file)

[5.13 LANGUAGE (#.85) File [56](#language-.85-file)](#language-.85-file)

[5.14 META DATA DICTIONARY (#.9) File
[56](#meta-data-dictionary-.9-file)](#meta-data-dictionary-.9-file)

[5.15 FILE (#1) of Files [57](#_Toc108021473)](#_Toc108021473)

[5.16 AUDIT (#1.1) File [57](#audit-1.1-file)](#audit-1.1-file)

[5.17 ARCHIVAL ACTIVITY (#1.11) File
[58](#archival-activity-1.11-file)](#archival-activity-1.11-file)

[5.18 ENTITY (#1.5) File [58](#_Toc108021476)](#_Toc108021476)

[5.19 SQLI_TABLE_ELEMENT (#1.5216) File
[58](#sqli_table_element-1.5216-file)](#sqli_table_element-1.5216-file)

[5.20 SQLI_COLUMN (#1.5217) File [59](#_Toc108021478)](#_Toc108021478)

[5.21 SQLI_PRIMARY_KEY (#1.5218) File
[59](#_Toc108021479)](#_Toc108021479)

[6 Archiving and Purging
[60](#archiving-and-purging)](#archiving-and-purging)

[6.1 Archiving [60](#archiving)](#archiving)

[6.2 Purging [60](#purging)](#purging)

[7 External Relationships
[61](#external-relationships)](#external-relationships)

[7.1 DBA Approvals and Database Integration Control Registrations (ICRs)
[62](#dba-approvals-and-database-integration-control-registrations-icrs)](#dba-approvals-and-database-integration-control-registrations-icrs)

[7.1.1 ICRs—Current List for VA FileMan as Custodian
[62](#icrscurrent-list-for-va-fileman-as-custodian)](#icrscurrent-list-for-va-fileman-as-custodian)

[7.1.2 ICRs—Detailed Information
[63](#icrsdetailed-information)](#icrsdetailed-information)

[7.1.3 ICRs—Current List for VA FileMan as Subscriber
[63](#icrscurrent-list-for-va-fileman-as-subscriber)](#icrscurrent-list-for-va-fileman-as-subscriber)

[8 Internal Relationships
[63](#internal-relationships)](#internal-relationships)

[9 Package-Wide Variables
[64](#package-wide-variables)](#package-wide-variables)

[9.1 Standards and Conventions (SAC) Exemptions
[65](#standards-and-conventions-sac-exemptions)](#standards-and-conventions-sac-exemptions)

[9.1.1 STANDARD SECTION: 4B–Package-wide variables
[65](#standard-section-4bpackage-wide-variables)](#standard-section-4bpackage-wide-variables)

[9.1.2 STANDARD SECTION: 6D–FM compatibility
[65](#_Toc108021492)](#_Toc108021492)

[10 Globals [65](#globals)](#globals)

[10.1 Global Journaling, Translation, and Replication
[67](#global-journaling-translation-and-replication)](#global-journaling-translation-and-replication)

[11 Security [67](#security)](#security)

[11.1 Security Management
[68](#security-management)](#security-management)

[11.2 Mail Groups and Alerts
[68](#mail-groups-and-alerts)](#mail-groups-and-alerts)

[11.3 Remote Systems [68](#remote-systems)](#remote-systems)

[11.4 Interfacing [68](#interfacing)](#interfacing)

[11.5 Electronic Signatures
[68](#electronic-signatures)](#electronic-signatures)

[11.6 Security Keys [68](#security-keys)](#security-keys)

[11.7 File Security [69](#file-security)](#file-security)

[11.8 References [69](#references)](#references)

[11.9 Official Policies [69](#official-policies)](#official-policies)

[12 Troubleshooting [70](#troubleshooting)](#troubleshooting)

[12.1 How to Obtain Technical Information Online
[70](#how-to-obtain-technical-information-online)](#how-to-obtain-technical-information-online)

[12.2 Help at Prompts [70](#help-at-prompts)](#help-at-prompts)

[Glossary [71](#_Toc108021508)](#_Toc108021508)

[Index [75](#_Toc108021509)](#_Toc108021509)

<span id="_Toc108021444" class="anchor"></span>List of Figures

[Figure 1: Type of M System Prompt
[xiv](#_Toc343519945)](#_Toc343519945)

[Figure 2: VA FileMan Pointer Map [13](#_Ref343695917)](#_Ref343695917)

[Figure 3: VA FileMan Exported Options Diagrams
[43](#_Ref343690295)](#_Ref343690295)

<span id="_Toc108021445" class="anchor"></span>List of Tables

[Table 1: Documentation Symbol Descriptions
[xii](#_Ref386465892)](#_Ref386465892)

[Table 2: VA FileMan Routine Variables and Default Values
[xv](#_Ref514251138)](#_Ref514251138)

[Table 3: VA FileMan Routine Global References
[xvi](#_Ref443482297)](#_Ref443482297)

[Table 4: VA FileMan File List (listed by file number)
[3](#_Ref345487413)](#_Ref345487413)

[Table 5: VA FileMan Routines and Callable Entry Points
[17](#_Ref345487248)](#_Ref345487248)

[Table 6: INDEX (#.11) File—Cross-References
[50](#_Toc108021518)](#_Toc108021518)

[Table 7: KEY (#.31) File—Cross-References
[51](#_Toc108021519)](#_Toc108021519)

[Table 8: PRINT TEMPLATE (#.4) File—Cross-References
[52](#_Toc108021520)](#_Toc108021520)

[Table 9: SORT TEMPLATE (#.401) File—Cross-References
[53](#_Toc108021521)](#_Toc108021521)

[Table 10: INPUT TEMPLATE (#.402) File—Cross-References
[53](#_Toc108021522)](#_Toc108021522)

[Table 11: FORM (#.403) File—Cross-References
[54](#_Toc108021523)](#_Toc108021523)

[Table 12: BLOCK (#.404) File—Cross-References
[54](#_Toc108021524)](#_Toc108021524)

[Table 13: FOREIGN FORMAT (#.44) File—Cross-References
[55](#_Toc108021525)](#_Toc108021525)

[Table 14: IMPORT TEMPLATE (#.46) File—Cross-References
[55](#_Toc108021526)](#_Toc108021526)

[Table 15: DD AUDIT (#.6) File—Cross-References
[55](#_Toc108021527)](#_Toc108021527)

[Table 16: DATA TYPE (#.81) File—Cross-References
[55](#_Toc108021528)](#_Toc108021528)

[Table 17: COMPILED ROUTINE (#.83) File—Cross-References
[56](#_Toc108021529)](#_Toc108021529)

[Table 18: LANGUAGE (#.85) File—Cross-References
[56](#_Toc108021530)](#_Toc108021530)

[Table 19: META DATA DICTIONARY (#.9) File—Cross-References
[56](#_Toc108021531)](#_Toc108021531)

[Table 20: FILE (#1) of Files—Cross-References
[57](#_Toc108021532)](#_Toc108021532)

[Table 21: AUDIT (#1.1) File—Cross-References
[57](#_Toc108021533)](#_Toc108021533)

[Table 22: ARCHIVAL ACTIVITY (#1.11) File—Cross-References
[58](#_Toc108021534)](#_Toc108021534)

[Table 23: ENTITY (#1.5) File—Cross-References
[58](#_Ref526166676)](#_Ref526166676)

[Table 24: SQLI_TABLE_ELEMENT (#1.5216) File—Cross-References
[58](#_Toc108021536)](#_Toc108021536)

[Table 25: SQLI_COLUMN (#1.5217) File—Cross-References
[59](#_Toc108021537)](#_Toc108021537)

[Table 26: SQLI_PRIMARY_KEY (#1.5218) File—Cross-References
[59](#_Toc108021538)](#_Toc108021538)

[Table 27: Package-Wide Variables [64](#_Ref514251199)](#_Ref514251199)

[Table 28: Package-Wide Variables—DISY (Special Meaning)
[64](#_Ref514251240)](#_Ref514251240)

[Table 29: List of Variables VA FileMan is Exempted from KILLing
[65](#_Toc108021541)](#_Toc108021541)

[Table 30: VA FileMan Security Keys
[68](#_Ref345487626)](#_Ref345487626)

[Table 31: Glossary [71](#_Toc108021543)](#_Toc108021543)

<span id="_Toc108021446" class="anchor"></span>Orientation

What is VA FileMan?

VA FileMan is the database management system for the Veterans Health
Information Systems and Technology Architecture user (VistA)
environment. VA FileMan creates and maintains a database management
system that includes features such as:

- Report writer

- Data dictionary manager

- Scrolling and screen-oriented data entry

- Text editors

- Programming utilities

- Tools for sending data to other systems

- File archiving

VA FileMan can be used as a:

- Standalone database

- Set of interactive or “silent” routines

- Set of application utilities; in all modes

It is used to define, enter, and retrieve information from a set of
computer-stored files, each of which is described by a data dictionary.

VA FileMan is a public domain software package that is developed and
maintained by the Department of Veterans Affairs (VA). It is widely used
by VA medical centers and in clinical, administrative, and business
settings in this country and abroad.

<img src="images/media/image3.png"
style="width:0.44444in;height:0.44444in" alt="Caution" /> CAUTION:
Programmer access in VistA is defined as DUZ(0)=“@”. It grants the
privilege to become a developer in VistA. Programmer access allows you
to work outside many of the security controls enforced by VA FileMan,
enables access to all VA FileMan files, access to modify data
dictionaries, etc. It is important to *proceed with caution* when having
access to the system in this way.

How to Use this Manual

The *VA FileMan Technical Manual* provides information about the
technical structure of VA FileMan. It includes the following information
about VA FileMan:

- <u>Implementation and Maintenance</u>

- <u>Files</u>

- <u>Routines, Application Programming Interfaces (APIs), and
  Options</u>

- <u>Cross-References</u>

- <u>Archiving and Purging</u>

- <u>External Relationships</u>

- <u>Internal Relationships</u>

- <u>Package-Wide Variables</u>

- <u>Globals</u>

- <u>Security</u>

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For VA
FileMan installation instructions in the VistA environment, see the *VA
FileMan Installation Guide* and any national patch description of the
patch being released.

Intended Audience

The intended audience of this manual is all key stakeholders. The
stakeholders include the following: It also contains material
specifically intended for VA’s Veterans Health Information Systems and
Technology Architecture (VistA) systems managers and application
developers.

- System Administrators—System administrators at Department of Veterans
  Affairs (VA) sites who are responsible for computer management and
  system security on the VistA M Servers.

- Development, Security, and Operations (DSO)—VistA development teams.

- Product Support (PS).

Disclaimers

Software Disclaimer

This software was developed at the Department of Veterans Affairs (VA)
by employees and contractors of the Federal Government in the course of
their official duties with significant input from the larger open source
community. Pursuant to title 17 Section 105 of the United States Code
this software is *not* subject to copyright protection and is in the
public domain. VA assumes no responsibility whatsoever for its use by
other parties, and makes no guarantees, expressed or implied, about its
quality, reliability, or any other characteristic. We would appreciate
acknowledgement if the software is used. This software can be
redistributed and/or modified freely provided that any derivative works
bear some notice that they are derived from it, and any modified
versions bear some notice that they have been modified.

<img src="images/media/image3.png"
style="width:0.44444in;height:0.44444in" alt="Caution" /> CAUTION: To
protect the security of VistA systems, distribution of this software for
use on any other computer system by VistA sites is prohibited. All
requests for copies of this software for *non*-VistA use should be
referred to the VistA site’s local Office of Information Field Office
(OIFO).

Documentation Disclaimer

This manual provides an overall explanation of VA FileMan and the
functionality contained in VA FileMan 22.2; however, no attempt is made
to explain how the overall VistA programming system is integrated and
maintained. Such methods and procedures are documented elsewhere. We
suggest you look at the various VA Internet and Intranet Websites for a
general orientation to VistA. For example, visit the Office of
Information and Technology (OIT) VistA Development Intranet website.

<img src="images/media/image3.png" title="Caution"
style="width:0.44444in;height:0.44444in" alt="Caution" /> DISCLAIMER:
The appearance of any external hyperlink references in this manual does
*not* constitute endorsement by the Department of Veterans Affairs (VA)
of this Website or the information, products, or services contained
therein. The VA does *not* exercise any editorial control over the
information you find at these locations. Such links are provided and are
consistent with the stated purpose of this VA Intranet Service.

Documentation Conventions

This manual uses several methods to highlight different aspects of the
material:

- Various symbols are used throughout the documentation to alert the
  reader to special information. <u>Table 1</u> gives a description of
  each of these symbols:

| Symbol                                                    | Description                                                                                                           |
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| <img src="images/media/image2.png"                        
 style="width:0.29167in;height:0.3125in" alt="Note" />      | **NOTE / REF:** Used to inform the reader of general information including references to additional reading material. |
| <img src="images/media/image3.png"                        
 style="width:0.45833in;height:0.45833in" alt="Caution" />  | **CAUTION / RECOMMENDATION / DISCLAIMER:** Used to caution the reader to take special notice of critical information. |

<span id="_Ref514251138" class="anchor"></span>Table : VA FileMan
Routine Variables and Default Values

- Descriptive text is presented in a proportional font (as represented
  by this font).

- Conventions for displaying TEST data in this document are as follows:

<!-- -->

- The first three digits (prefix) of any Social Security Numbers (SSN)
  begin with either “**000**” or “**666**”.

- Patient and user names are formatted as follows:

<!-- -->

- *\<Application Name/Abbreviation/Namespace\>*PATIENT,\[*N*\] and

- *\<Application Name/Abbreviation/Namespace\>*USER,\[*N*\]

Where “\<*Application Name/Abbreviation/Namespace*\>” is defined in the
Approved Application Abbreviations document and “*N*” represents the
first name as a number value or spelled out and incremented with each
new entry. For example, in VA FileMan (FM) test patient and user names
would be documented as follows:

- FMPATIENT,ONE; FMPATIENT,TWO; FMPATIENT,THREE; FMPATIENT,14, etc.

- FMUSER,ONE; FMUSER,TWO; FMUSER,THREE; FMUSER,14, etc.

<!-- -->

- “Snapshots” of computer online displays (i.e., screen
  captures/dialogues) and computer source code, if any, are shown in a
  *non*-proportional font and enclosed within a box.

<!-- -->

- User’s responses to online prompts are **bold** typeface and
  highlighted in yellow (e.g., **\<Enter\>**).

- Emphasis within a dialogue box is **bold** typeface and highlighted in
  blue (e.g., STANDARD LISTENER: RUNNING).

- Some software code reserved/key words are **bold** typeface with
  alternate color font.

- References to “**\<Enter\>**” within these snapshots indicate that the
  user should press the **Enter** key on the keyboard. Other special
  keys are represented within **\< \>** angle brackets. For example,
  pressing the **PF1** key can be represented as pressing **\<PF1\>**.

- Author’s comments are displayed in italics or as “callout” boxes.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** Callout
boxes refer to labels or descriptions usually enclosed within a box,
which point to specific areas of a displayed image.

- All uppercase is reserved for the representation of M code, variable
  names, or the formal name of options, field/file names, and security
  keys (e.g., DIEXTRACT).

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** Other
software code (e.g., Delphi/Pascal and Java) variable names and
file/folder names can be written in lower or mixed case
(e.g., CamelCase).

Documentation Navigation

This document uses Microsoft® Word’s built-in navigation for internal
hyperlinks. To add **Back** and **Forward** navigation buttons to your
toolbar, do the following:

1.  Right-click anywhere on the customizable Toolbar in Word (*not* the
    > Ribbon section).

2.  Select **Customize Quick Access Toolbar** from the secondary menu.

3.  Select the drop-down arrow in the “Choose commands from:” box.

4.  Select **All Commands** from the displayed list.

5.  Scroll through the command list in the left column until you see the
    > **Back** command (green circle with arrow pointing left).

6.  Select/Highlight the **Back** command and select **Add** to add it
    > to your customized toolbar.

7.  Scroll through the command list in the left column until you see the
    > **Forward** command (green circle with arrow pointing right).

8.  Select/Highlight the Forward command and select **Add** to add it to
    > your customized toolbar.

9.  Select **OK**.

You can now use these **Back** and **Forward** command buttons in your
Toolbar to navigate back and forth in your Word document when clicking
on hyperlinks within the document.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** This is
a one-time setup and is automatically available in any other Word
document once you install it on the Toolbar.

VA FileMan Coding Conventions

*Non*-Standard M Features

**Z**-commands and **Z**-functions are avoided throughout VA FileMan
routines. For certain purposes (e.g., allowing terminal breaking and
spooling to a Standard Disk Processor \[SDP\] disk device), VA FileMan
executes lines of *non*-standard M code out of the MUMPS OPERATING
SYSTEM (#.7) file. The *non*-standard code used (if any) depends on the
answer to the prompt:

<span id="_Toc343519945" class="anchor"></span>Figure : Type of M System
Prompt

TYPE OF MUMPS SYSTEM YOU ARE USING:

This prompt appears during the **DINIT** initialization routine.
Answering **OTHER** to this question ensures that VA FileMan uses only
standard M code.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** When
installed with the VA’s KIDS build, use of the Caché operating is
assumed. You will not see the TYPE OF MUMPS SYSTEM YOU ARE USING:
prompt.

VA FileMan also makes use of *non*-standard M code that is stored in the
**%ZOSF** global:

- If VA FileMan is installed on a system that contains Kernel, it uses
  the **%ZOSF** global created by Kernel.

- If it is being used without Kernel (i.e., standalone), the necessary
  **%ZOSF** nodes are set for many operating systems by running
  **DINZMGR** in the Manager account.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
details, see the “System Management” section in the *VA FileMan Advanced
User Manual*.

String-valued subscripts (up to **30** characters long) are used
extensively but only in the **\$ORDER** collating sequence approved by
the MUMPS Development Committee (MDC). Non-negative integer and
fractional canonic numbers collate ahead of all other strings.

The **\$ORDER** function is used at several points in VA FileMan’s code.
VA FileMan routines assume that reference to an undefined global
subscript level sets the naked indicator to that level, rather than
leaving it undefined. In all other respects, the VA FileMan code
conforms to the 1995 ANSI Standard for the M language with Type **A**
extensions.

Routine, Variable, and Global Names

In keeping with the convention that all programs that are a part of the
same application or utility package should be namespaced, all VA FileMan
routine names begin with **DI**, **DD**, or **DM**. (The “Device
Handling for Standalone VA FileMan” section in the VA *FileMan Advanced
User Manual* explains that some **DI\*** routines are renamed in the
Manager account.) The **DINIT** routine initializes VA FileMan. The
**DINIT** routine is run automatically with no user interaction during
the KIDS install. The **DI** routine itself is the main option reader.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on the DI routine, see the “^DI: Programmer Access” section
in the *VA FileMan Developer’s Guide*.

Except in **DI**, the routines do *not* contain unargumented or
exclusive **KILL** commands. Most multi-character local variable names
created by VA FileMan routines begin with **%** or the letter **D** or
consist of one uppercase letter followed by one numeral \[except that
**IO(0)**, by convention, contains the **\$I** value of the signon
device\]. Since VA FileMan uses single character variable names
extensively, do *not* use them in code that is executed from within VA
FileMan programming hooks unless their use is documented in the hook’s
description or you NEW them. Also, do *not* expect single character
variables to return unchanged after calling a VA FileMan entry point.

<u>Table 2</u> lists the local variables that are of special importance
in the VA FileMan routines:

<table>
<caption><p><span id="_Ref443482297" class="anchor"></span>Table : VA
FileMan Routine Global References</p></caption>
<colgroup>
<col style="width: 11%" />
<col style="width: 57%" />
<col style="width: 30%" />
</colgroup>
<thead>
<tr class="header">
<th>Variable</th>
<th>Description</th>
<th>Default Value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>DT</strong></td>
<td><p>If defined, it is assumed to be the current date. For
example:</p>
<blockquote>
<p>June 1, 1987 is DT=2870601.</p>
</blockquote></td>
<td>Today’s date; derived from <strong>$H</strong></td>
</tr>
<tr class="even">
<td><strong>DTIME</strong></td>
<td>If defined, it is the integer value of the number of seconds the
user <em>must</em> respond to a timed read.</td>
<td><strong>300</strong></td>
</tr>
<tr class="odd">
<td><strong>DUZ</strong></td>
<td>If defined, it is assumed to be the User Number; a positive number
uniquely identifying the current user.</td>
<td><strong>0</strong></td>
</tr>
<tr class="even">
<td><strong>DUZ(0)</strong></td>
<td><p>If defined, it is assumed to be the FileMan Access Code, which is
a character string describing the user’s security clearance with regard
to files, templates, and data fields within a file.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> See the “Data Security” section in the <em>VA
FileMan Advanced User Manual</em>.</p>
<p>Setting <strong>DUZ(0)</strong> equal to the at-sign
(<strong>@</strong>) overrides all security checks and allows special
programmer features that are described later. If the user’s M
implementation supports terminal break, a developer is allowed to break
execution at any point, whereas a user who does <em>not</em> have
programmer access can only break during output routines.</p></td>
<td><strong>“”</strong></td>
</tr>
<tr class="odd">
<td><strong>U</strong></td>
<td>If defined, it is equal to a single caret (<strong>^</strong>)
character.</td>
<td><strong>^</strong></td>
</tr>
</tbody>
</table>

<span id="_Ref443482297" class="anchor"></span>Table : VA FileMan
Routine Global References

VA FileMan routines explicitly refer to the globals in <u>Table 3</u>:

| Global     | Description                                                                           |
|------------|---------------------------------------------------------------------------------------|
| **^DD**    | All attribute dictionaries, Keys, Functions, and MUMPS operating systems.             |
| **^DDA**   | Data dictionary audit trail.                                                          |
| **^DDD**   | Meta Data Dictionary.                                                                 |
| **^DDE**   | Entity File                                                                           |
| ^DI        | Data types, Languages, Dialogs.                                                       |
| **^DIA**   | Data audit trail.                                                                     |
| **^DIAR**  | Archival activity and Filegrams.                                                      |
| **^DIBT**  | Sort templates and the results of file searches.                                      |
| **^DIC**   | Dictionary of files.                                                                  |
| **^DIE**   | Input templates.                                                                      |
| **^DIPT**  | Print templates and Filegram templates.                                               |
| **^DIST**  | ScreenMan forms and blocks, Import Templates, Foreign Formats, and Alternate Editors. |
| **^DISV**  | Most recent lookup value in any file or subfile (by **DUZ**).                         |
| **^DIT**   | Files needed for UTC Data Type.                                                       |
| **^DIZ**   | Default location for new data files as they are created.                              |
| **^DOPT**  | Option lists.                                                                         |
| **^DOSV**  | Statistical results.                                                                  |
| **^%ZOSF** | M vendor-specific executable code.                                                    |

<span id="_Ref345487413" class="anchor"></span>Table : VA FileMan File
List (listed by file number)

The routines use the **^UTILITY** and **^TMP** globals for temporary
scratch space. The **^XUTL** global is also used if you are running some
M implementations.

Delimiters within Strings

The caret (**^**) character is conventionally used to delimit data
elements that are strung together to be stored in a single global node.
A corollary of this rule is that the routines almost never allow input
data to contain carets; the user types a caret (**^**) to change or
terminate the sequence of questions being asked. Within **^**-pieces,
semicolons (**;**) are usually used as secondary delimiters, and colons
(**:**) as tertiary delimiters.

VA FileMan routines use the local variable **U** as equal to the single
caret (**^**) character.

Canonic Numbers

VA FileMan recognizes only canonic numbers. A canonic number is a number
that does *not* begin or end with meaningless zeroes. For example, **7**
is a canonic number, whereas **007** and **7.0** are *not* canonic
numbers.

How to Obtain Technical Information Online

Exported VistA M Server-based software file, routine, and global
documentation can be generated through the use of Kernel, MailMan, and
VA FileMan utilities.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** Methods
of obtaining specific technical information online are indicated where
applicable under the appropriate section.

Help at Prompts

VistA M Server-based software provides online help and commonly used
system default prompts. Users are encouraged to enter question marks at
any response prompt. At the end of the help display, you are immediately
returned to the point from which you started. This is an easy way to
learn about any aspect of the software.

Obtaining Data Dictionary Listings

Technical information about VistA M Server-based files and the fields in
files is stored in data dictionaries (DD). You can use the List File
Attributes option \[DILIST\] on the Data Dictionary Utilities menu \[DI
DDU\] in VA FileMan to print formatted data dictionaries.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
details about obtaining data dictionaries and about the formats
available, see the “List File Attributes” section in the “File
Management” section in the *VA FileMan Advanced User Manual*.

Assumptions

This manual is written with the assumption that the reader is familiar
with the following:

- VistA computing environment:

<!-- -->

- Kernel—VistA M Server software

- VA FileMan data structures and terminology—VistA M Server software

<!-- -->

- Microsoft<sup>®</sup> Windows environment

- M programming language

Reference Materials

Readers who wish to learn more about VA FileMan should consult the
following documents:

- *VA FileMan Release Notes*

- *VA FileMan Installation Guide*

- *VA FileMan Technical Manual* (this manual)

- *VA FileMan User Manual* (PDF and HTML format)

- *VA FileMan Advanced User Manual* (PDF and HTML format)

- *VA FileMan Developer’s Guide* (PDF and HTML format)

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** Zip files
of the VA FileMan documentation in HTML format are located on the VA
FileMan Intranet Product website and VDL at:
<http://www.va.gov/vdl/application.asp?appid=5>.  
  
Using a Web browser, open the **HTML** documents “table of contents”
page (i.e., index.shtml). The *VA FileMan User Manual*, the *VA FileMan
Advanced User Manual*, and the *VA FileMan Developer’s Guide* are all
linked together.

VistA documentation is made available online in Microsoft<sup>®</sup>
Word format and in Adobe<sup>®</sup> Acrobat Portable Document Format
(PDF). The PDF documents *must* be read using the Adobe<sup>®</sup>
Acrobat Reader, which is freely distributed by Adobe<sup>®</sup> Systems
Incorporated at: <http://www.adobe.com/>

VistA software documentation can be downloaded from the VA Software
Document Library (VDL) at: <http://www.va.gov/vdl/>

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** VA
FileMan manuals are located on the VDL at:
<http://www.va.gov/vdl/application.asp?appid=5>

VistA documentation and software can also be downloaded from the Product
Support (PS) Anonymous Directories.

# Introduction

VA FileMan is a database management system (DBMS) consisting of computer
routines written in American National Standards Institute (ANSI)
Standard M, along with associated files. Developed with portability as a
goal, VA FileMan runs on all major implementations of ANSI M and on
hardware platforms ranging from PCs to mainframes.

Developers and non-developers use VA FileMan alike. VA FileMan can be
used as a standalone database or as a set of application utilities. In
either mode, it is used to define, enter, and retrieve information from
a set of computer-stored files, each of which is described by the data
dictionary.

VA FileMan is a public domain software package and is widely used in
clinical, administrative, and business settings in the United States and
abroad.

# Implementation and Maintenance

VA FileMan 22.2 is initialized by an install using the Kernel
Distribution and Installation system (KIDS) as directed in the *VA
FileMan Installation Guide*. In previous versions **DINIT** was used to
initialize VA FileMan. Now, **DINIT** is run automatically with no user
intervention during the KIDS install. **DINIT** should *not* be run from
the command line after the KIDS install is done. Standalone VA FileMan
installs on systems without Kernel is not addressed by this
documentation.

VA FileMan routines and globals occupy approximately **3.5 MB** of disk
space. The size of the globals, particularly those that store
application data, increases when VA FileMan is used.

Since VA FileMan provides the DBMS upon which all files in Veterans
Health Information Systems and Technology Architecture (VistA) are
based, it *must* be present on all VistA systems. The current version of
VA FileMan is designed for complete backward compatibility; files and
applications developed under prior versions remain usable.

If used with Kernel, all or part of the VA FileMan options can be given
to users. Those who are able to use programmer mode can also invoke the
main menu from the M prompt. Anyone can use applications developed with
VA FileMan, whether or not direct access to VA FileMan itself is
allowed.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on programmer mode, see the “^DI: Programmer Access” section
in the “Developer’s Tools” section in the *VA FileMan Developer’s
Guide*.

When used with Kernel, VA FileMan allows the user to print multiple
copies. In order to do this, a temporary storage location *must* be
allocated on the system with a corresponding DEVICE (#3.5) file entry
that uses a sequential disk processor (SDP) device type.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** The
*Kernel 8.0 and Kernel Toolkit 7.3 Systems Management Guide* contains
specific instructions on how to set up an SDP device for different
operating systems.

The **^DISV** global contains the most recent lookup value for files and
subfiles; it is used to process **\<Spacebar\>\<Enter\>** input. The
**^DOSV** global contains results of statistical operations. These
globals can grow to considerable size and should be monitored. It is
safe to periodically **KILL** these globals. Users should *not* be
logged on to the system when the globals are **KILL**ed in order to
minimize inconvenience and avoid data corruption.

The site manager *must* monitor the proliferation of routines with names
like **^DISZ*nnnn*** where “***nnnn***” is a four-digit number with
leading zeros. These routines are created when compiled sorts are run.
Ordinarily, they are deleted after the sort completes, but, if the
system goes down or the job fails with an error, they can remain. When
users are *not* on the system, the routine ENRLS^DIOZ can be run to
clean up these routines and to release the “***nnnn***” numbers for
reuse.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on the ENRLS^DIOZ utility, see the “COMPILED ROUTINE File
Cleanup: ENRLS^DIOZ( )” section in the “System Management” section in
the “Tools” section in the *VA FileMan Advanced User Manual*.

# Files

This section lists all the VA FileMan files, file numbers, global
locations, and a brief description of each. Data exported with VA
FileMan 22.2 is described for some files:

- VA FileMan uses files numbered between **0** and **2**.

- VA FileMan files should *not* be altered, per VHA Directive 6402.

<table>
<caption><p><span id="_Ref345487248" class="anchor"></span>Table : VA
FileMan Routines and Callable Entry Points</p></caption>
<colgroup>
<col style="width: 10%" />
<col style="width: 29%" />
<col style="width: 17%" />
<col style="width: 41%" />
</colgroup>
<thead>
<tr class="header">
<th>File #</th>
<th>File Name</th>
<th>Global Location</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>.11</td>
<td>INDEX</td>
<td>^DD(“IX”,</td>
<td>The INDEX file stores information about New-Style cross-references
defined on a file. Whereas Traditional cross-references are stored under
the <strong>1</strong> nodes of the ^DD for a particular field,
New-Style cross-references are stored in this file and can consist of
one field (simple cross-references), as well as more than one field
(compound cross-references).</td>
</tr>
<tr class="even">
<td>.2</td>
<td>Destination</td>
<td>^DIC(.2</td>
<td>The DESTINATION file documents the location where data is used.</td>
</tr>
<tr class="odd">
<td>.31</td>
<td>KEY</td>
<td>^DD(“KEY”,</td>
<td>The KEY file stores information about keys on a file or subfile. A
key is a set of one or more fields that uniquely identifies a record in
a file. If more than one set of fields can uniquely identify a record,
one of those sets should be designated the primary key; all others
should be designated secondary keys. The primary key is the principal
means of identifying records in the file. To allow VA FileMan to enforce
key uniqueness, the database designer <em>must</em> define a regular
index that consists of all the fields that make up the key. This index
is called the uniqueness index. All key fields <em>must</em> have
values. They cannot be <strong>NULL</strong>.</td>
</tr>
<tr class="even">
<td>.4</td>
<td>Print Template</td>
<td>^DIPT(</td>
<td><p>The PRINT TEMPLATE file stores VA FileMan PRINT templates.
Exported PRINT templates include:</p>
<ul>
<li><p>CAPTIONED</p></li>
<li><p>FILE SECURITY CODES</p></li>
<li><p>DI-PKG-DEFAULT-DEFINITION</p></li>
<li><p>DDXP FORMAT DOC</p></li>
<li><p>DDXP FORMAT DOC HDR</p></li>
</ul></td>
</tr>
<tr class="odd">
<td>.401</td>
<td>Sort Template</td>
<td>^DIBT(</td>
<td>The SORT TEMPLATE file stores VA FileMan SORT, SEARCH, and INQUIRE
templates.</td>
</tr>
<tr class="even">
<td>.402</td>
<td>Input Template</td>
<td>^DIE(</td>
<td>The INPUT TEMPLATE file stores VA FileMan INPUT templates.</td>
</tr>
<tr class="odd">
<td>.403</td>
<td>FORM</td>
<td>^DIST(.403</td>
<td>The FORM file stores forms used by VA FileMan to display screens.
The DDXP FF FORM1 and various forms used by ScreenMan’s Form Editor
utility are exported.</td>
</tr>
<tr class="even">
<td>.404</td>
<td>BLOCK</td>
<td>^DIST(.404</td>
<td>The BLOCK file stores blocks used to build forms for screen display.
Blocks are exported for use with the forms sent with VA FileMan.</td>
</tr>
<tr class="odd">
<td>.44</td>
<td>FOREIGN FORMAT</td>
<td>^DIST(.44</td>
<td>The FOREIGN FORMAT file holds specifications for sending data to an
application outside of M. Several Foreign Formats are exported.</td>
</tr>
<tr class="even">
<td>.46</td>
<td>IMPORT TEMPLATE</td>
<td>^DIST(.46,</td>
<td>The IMPORT TEMPLATE file holds specifications for importing
information from an application outside of M into a VA FileMan
file.</td>
</tr>
<tr class="odd">
<td>.5</td>
<td>Function</td>
<td>^DD(“FUNC”</td>
<td><p>The FUNCTION file stores the computed functions available in VA
FileMan. The functions described in the <em>VA FileMan Advanced User
Manual</em> are exported.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For more information on functions, see the “VA
FileMan Functions” section in the “Tools” section in the VA <em>FileMan
Advanced User Manual</em>.</p></td>
</tr>
<tr class="even">
<td>.6</td>
<td>DD AUDIT</td>
<td>^DDA(</td>
<td>The DD AUDIT file stores the changes made to data dictionaries.</td>
</tr>
<tr class="odd">
<td>.7</td>
<td>MUMPS Operating System</td>
<td>^DD(“OS”</td>
<td>The MUMPS OPERATING SYSTEM file stores the operating systems
recognized by VA FileMan along with operating system-specific data. This
data is exported.</td>
</tr>
<tr class="even">
<td>.81</td>
<td>DATA TYPE</td>
<td>^DI(.81</td>
<td>The DATA TYPE file stores information about the DATA TYPEs known to
VA FileMan. Several DATA TYPEs are exported.</td>
</tr>
<tr class="odd">
<td>.83</td>
<td>COMPILED ROUTINE</td>
<td>^DI(.83</td>
<td>The COMPILED ROUTINE file contains a list of numbers (to be used to
create compiled sort routines) and a flag to indicate whether a number
is currently in use.</td>
</tr>
<tr class="even">
<td>.84</td>
<td>DIALOG</td>
<td>^DI(.84</td>
<td>The DIALOG file contains text used to “talk” to the user (error
messages, help text, prompts). Entries under IEN <strong>10,000</strong>
are exported by VA FileMan and are used in VA FileMan routines.</td>
</tr>
<tr class="odd">
<td>.85</td>
<td>LANGUAGE</td>
<td>^DI(.85</td>
<td>The LANGUAGE file is used to reference data dictionary elements and
subentries in the DIALOG file for user dialogue in foreign languages and
contains M code used to perform data transformations for such things as
dates and numbers to non-English formats. All the languages in ISO
639-2:1998 (as revised 11/21/2012; International Organization for
Standardization) are exported.</td>
</tr>
<tr class="even">
<td>.86</td>
<td>DATA TYPE PROPERTY</td>
<td>^DI(.86</td>
<td>The DATA TYPE PROPERTY file stores the names of different kinds of
STRINGS that describe data.</td>
</tr>
<tr class="odd">
<td>.87</td>
<td>DATA TYPE METHOD</td>
<td>^DI(.87</td>
<td>The DATA TYPE METHOD file stores the names of different kinds of
lines of MUMPS code that are used in the definitions of DATA TYPES.</td>
</tr>
<tr class="even">
<td>.9</td>
<td>Meta data Dictionary</td>
<td>^DDD(</td>
<td>The META DATA DICTIONARY file stores the file and field definitions
of all files and fields in a VA FileMan instance.</td>
</tr>
<tr class="odd">
<td>1</td>
<td>File</td>
<td>^DIC(</td>
<td>The FILE file stores the name, number, global name or location,
package name, security access, and developer of VA FileMan created
files. Data for the VA FileMan files is exported.</td>
</tr>
<tr class="even">
<td>1.1</td>
<td>Audit</td>
<td>^DIA(</td>
<td>The AUDIT file stores the date and time, user’s name, and old and
new data values of changes made to audited fields.</td>
</tr>
<tr class="odd">
<td>1.11</td>
<td>ARCHIVAL ACTIVITY</td>
<td>^DIAR(1.11</td>
<td>The ARCHIVAL ACTIVITY file stores information about and status of
archiving and extract activities.</td>
</tr>
<tr class="even">
<td>1.12</td>
<td>FILEGRAM HISTORY</td>
<td>^DIAR(1.12</td>
<td>The FILEGRAM HISTORY file stores information and status of
Filegrams.</td>
</tr>
<tr class="odd">
<td>1.13</td>
<td>FILEGRAM ERROR LOG</td>
<td>^DIAR(1.13</td>
<td>The FILEGRAM ERROR LOG file stores information about Filegram errors
and the text of the affected Filegram.</td>
</tr>
<tr class="even">
<td>1.2</td>
<td>ALTERNATE EDITOR</td>
<td>^DIST(1.2</td>
<td>The ALTERNATE EDITOR file stores information about the editors that
can be used to edit VA FileMan’s WORD-PROCESSING-type fields. Data for
the Line Editor and the Screen Editor is exported.</td>
</tr>
<tr class="odd">
<td>1.5</td>
<td>ENTITY</td>
<td>^DDE(</td>
<td><p>The ENTITY file maps VistA data to entities or resources, which
can be exposed RESTfully to standard web methods and formats. It can
support various data models; for example:</p>
<ul>
<li><p>Fast Healthcare Interoperability Resources (FHIR)</p></li>
<li><p>InterSystems' Summary Document Architecture (SDA)</p></li>
</ul></td>
</tr>
<tr class="even">
<td>1.521</td>
<td>SQLI_SCHEMA</td>
<td>^DMSQ(“S”,</td>
<td>The SQLI_SCHEMA file stores a set of tables and domains; a subset of
catalog and environment.</td>
</tr>
<tr class="odd">
<td>1.52101</td>
<td>SQLI_KEY_WORD</td>
<td>^DMSQ(“K”,</td>
<td>The SQLI_KEY_WORD file stores the SQL identifiers that
<em>cannot</em> be used for column and table names. SQL, ODBC, and
vendors all have lists of restricted words, which should be put in this
table before SQLI table generation.</td>
</tr>
<tr class="even">
<td>1.5211</td>
<td>SQLI_DATA_TYPE</td>
<td>^DMSQ(“DT”,</td>
<td><p>The SQLI_DATA_TYPE file stores a set of values from which all
domains of that type can be drawn:</p>
<ul>
<li><p>PRIMARY_KEY—Set of all primary keys (in SQLI_TABLE_ELEMENT
[#1.5216] file, type P).</p></li>
<li><p>CHARACTER—Set of all character strings of length less than
256.</p></li>
<li><p>INTEGER—Set of all cardinal numbers.</p></li>
<li><p>NUMERIC—Set of all real numbers.</p></li>
<li><p>DATE—Set of all date valued tokens.</p></li>
<li><p>TIME—Set of all time valued tokens.</p></li>
<li><p>MOMENT—Set of all tokens that have both a date and a time
value.</p></li>
<li><p>BOOLEAN—Set of all tokens that evaluate to true or false
only.</p></li>
<li><p>MEMO—Set of all character strings of length greater than
255.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td>1.5212</td>
<td>SQLI_DOMAIN</td>
<td>^DMSQ(“DM”,</td>
<td><p>The SQLI_DOMAIN file stores the set from which all objects of
that domain <em>must</em> be drawn. In SQLI, all table elements
(SQLI_TABLE_ELEMENT [#1.5216] file) have a domain that restricts them to
their domain set. For each DATA TYPE there is a domain of the same name,
representing the same set. Other domains have different set membership
restrictions.</p>
<p>Each domain has a DATA TYPE, which determines the rules for comparing
values from different domains, and the operators that can be used on
them.</p>
<p>The PRIMARY_KEY DATA TYPE and domain is unique to SQLI. It is used to
relate primary keys to foreign keys unambiguously.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For information on table elements, see the
SQLI_TABLE_ELEMENT (#1.5216) file.</p></td>
</tr>
<tr class="even">
<td>1.5213</td>
<td>SQLI_KEY_FORMAT</td>
<td>^DMSQ(“KF”,</td>
<td>The SQLI_KEY_FORMAT file stores strategies for converting base
values into key values. Soundex and uppercase conversion are common
examples. This implies that comparisons of key values with base values
<em>must</em> be preceded by conversion of the base value to a key
value. Key formats are frequently lossy; they <em>cannot</em> be
converted uniquely back to base format.</td>
</tr>
<tr class="odd">
<td>1.5214</td>
<td>SQLI_OUTPUT_FORMAT</td>
<td>^DMSQ(“OF”,</td>
<td><p>The SQLI_OUTPUT_FORMAT file stores strategies for converting base
values to external values. In VA FileMan, they are used to convert
references to pointers to their text values. They are also used for the
SET OF CODES type.</p>
<p>SQLI projects POINTER TO A FILE and SET OF CODES as calls to
$$GET1^DIQ, VARIABLE-POINTERs into calls to $$EXTERNAL^DILFD.</p>
<p>Vendors and other users of SQLI can implement their own conversions
to improve performance.</p></td>
</tr>
<tr class="even">
<td>1.5215</td>
<td>SQLI_TABLE</td>
<td>^DMSQ(“T”,</td>
<td><p>The SQLI_TABLE file stores the descriptor of a set of table
elements, which includes name and file number (see the
SQLI_TABLE_ELEMENT [#1.5216] file). Each ^DD(DA) represents a table in a
relational model of VA FileMan. Further, each index represents a
table.</p>
<p>Each schema contains multiple tables. Each table contains just one
primary key, but multiple columns, foreign keys and indices.</p></td>
</tr>
<tr class="odd">
<td>1.5216</td>
<td>SQLI_TABLE_ELEMENT</td>
<td>^DMSQ(“E”,</td>
<td><p>The SQLI_TABLE_ELEMENT file contains the names and domains of
primary keys, columns, and foreign keys. Each represents the relational
concept of an attribute; whose essential characteristics are a name
(unique by relation) and a domain.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For more information, see the SQLI_PRIMARY_KEY,
SQLI_COLUMN, and SQLI_FOREIGN KEY files.</p></td>
</tr>
<tr class="even">
<td>1.5217</td>
<td>SQLI_COLUMN</td>
<td>^DMSQ(“C”,</td>
<td><p>The SQLI_COLUMN file stores a set of formatting and physical
structure specifications. Each column specification has a column type
table element (SQLI_TABLE_ELEMENT file) that contains the relational
specifications, name, and domain. The column specification contains
those attributes required to locate the value in the global structure
and to project the value to the user.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For information on table elements, see the
SQLI_TABLE_ELEMENT (#1.5216) file.</p></td>
</tr>
<tr class="odd">
<td>1.5218</td>
<td>SQLI_PRIMARY_KEY</td>
<td>^DMSQ(“P”,</td>
<td><p>The SQLI_PRIMARY_KEY file stores a chosen set of columns that
uniquely identify a table. In the relational model (as in set theory)
the columns of a primary key are <em>not</em> ordered. In SQLI, they
<em>must</em> be, in order to map to the quasi-hierarchical model of M
globals.</p>
<p>VA FileMan subfiles (Multiples) have a primary key element for each
parent plus one for the subfile. Each contains a pointer to its primary
key table element (SQLI_TABLE-ELEMENT file), a sequence, and a column in
the local base table (SQLI_COLUMN file).</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For information, see the SQLI_TABLE_ELEMENT and
SQLI_COLUMN files above.</p></td>
</tr>
<tr class="even">
<td>1.5219</td>
<td>SQLI_FOREIGN_KEY</td>
<td>^DMSQ(“F”,</td>
<td><p>The SQLI_FOREIGN_KEY file stores a set of columns in a table that
match the primary key of another table. They represent an explicit join
of the two tables. Each foreign key element points to its table element
(SQLI_TABLE_ELEMENT [#1.5216] file), a column in the local table
(SQLI_COLUMN file), and a primary key element of a foreign table
(SQLI_PRIMARY_KEY file). The primary key table element of the foreign
table has the domain of that table, which makes the connection.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For more information, see the SQLI_TABLE_ELEMENT,
SQLI_COLUMN, and SQLI_PRIMARY_KEY files.</p></td>
</tr>
<tr class="odd">
<td>1.52191</td>
<td>SQLI_ERROR_TEXT</td>
<td>^DMSQ(“ET”,</td>
<td>The SQLI_ERROR_TEXT file stores a numbered list of error messages,
auto-generated by ERR^DMSQU.</td>
</tr>
<tr class="even">
<td>1.52192</td>
<td>SQLI_ERROR_LOG</td>
<td>^DMSQ(“EX”,</td>
<td><p>The SQLI_ERROR_LOG file stores a log of all errors encountered
while compiling SQLI. It generates the error text table (SQLI_ERROR_TEXT
file) on a LAYGO basis; errors are added only when they occur. If DBS
errors triggered the error, the DIALOG file reference is also saved.</p>
<p><img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" />
<strong>REF:</strong> For more information, see the SQLI_ERROR_TEXT and
DIALOG files.</p></td>
</tr>
<tr class="odd">
<td>1.6</td>
<td>POLICY</td>
<td>^DIAC(1.6,</td>
<td>The POLICY file is a self-referring, namespaced file, which is
similar to the OPTION (#19) file. Rules are stored in a sub-file, much
like menu items, and evaluated in sequence. If more complex policies are
needed, policy sets can be created by grouping other policies or sets,
drilling down the levels in sequence like a menu tree.</td>
</tr>
<tr class="even">
<td>1.61</td>
<td>APPLICATION ACTION</td>
<td>^DIAC(1.6,</td>
<td>The APPLICATION ACTION file stores the list of actions that can be
taken on a file or sub-file (e.g., read, cancel, sign, etc.). Each
action can be mapped to a policy that is evaluated when that kind of
access to data is requested.</td>
</tr>
<tr class="odd">
<td>1.62</td>
<td>POLICY FUNCTION</td>
<td>^DIAC(1.6,</td>
<td>Supporting M code for policies is implemented as M functions and
stored as entries in the POLICY FUNCTION file.</td>
</tr>
<tr class="even">
<td>1.71</td>
<td>WORLD TIMEZONES</td>
<td>^DIT(1.71,</td>
<td>The WORLD TIMEZONES file stores time zone designations used
throughout the world.</td>
</tr>
<tr class="odd">
<td>1.72</td>
<td>WORLD DAYLIGHT SAVINGS</td>
<td>^DIT(1.72,</td>
<td>The WORLD DAYLIGHT SAVINGS file tracks which countries have periods
during the year in which they follow DAYLIGHT SAVING TIME, STANDARD
TIME, or SUMMER TIME.</td>
</tr>
<tr class="even">
<td>1.75</td>
<td>DATA SYNCHRONIZATION HISTORY</td>
<td>^DIFS(1.75</td>
<td>The DATA SYNCHRONIZATION HISTORY file is used to capture information
from DATA SYNCHRONIZATION processing. Information logged allows an
administrator to see if the process completed successfully or if there
were issues and what errors were reported by the processing.</td>
</tr>
</tbody>
</table>

<span id="_Ref345487248" class="anchor"></span>Table : VA FileMan
Routines and Callable Entry Points

Installing the KIDS build for VA FileMan 22.2 loads the files listed in
<u>Table 4</u>. Two files (LANGUAGE \[#.85\] and META DATA DICTIONARY
\[#.9\]) are carried by the KIDS build in the standard fashion; the
other files are installed when KIDS runs **DINIT**.

The PACKAGE (#9.4) file init routines (DIPKINIT) are no longer sent with
VA FileMan 22.2. The PACKAGE (#9.4) file is necessary to build inits
using **DIFROM**.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on DIFROM, see the “DIFROM” section in the “Developer’s
Tools” section in the *VA FileMan Developer’s Guide.*

<img src="images/media/image3.png"
style="width:0.44444in;height:0.44444in" alt="Caution" /> CAUTION: The
Kernel Installation and Distribution System (KIDS) replaced the use of
DIFROM as the method of exporting software packages in the VA. The
version of DIFROM released with VA FileMan 22.2 will transport the new
Key and Index structures.

## Pointer Map

Figure 2<u>Figure 2</u> is a diagram of the pointer relationships
between fields in VA FileMan’s files. This pointer map reflects the
relationships that exist in a VA FileMan environment running Kernel 8.0.
As files are added to a system, new pointer relationships can be
created; thus, the actual map for different operational systems can
vary.

The diagram in <u>Figure 2</u> was created using the Map Pointer
Relations option on the Data Dictionary Utilities submenu.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information about creating and reading this map, see the “Map Pointer
Relations option” section in the “List File Attributes” section in the
“File Management” section in the *VA FileMan Advanced User Manual*.

<span id="_Ref343695917" class="anchor"></span>Figure : VA FileMan
Pointer Map

File/Package: Date: MAR 10,2016

FILE (#) POINTER (#) FILE

POINTER FIELD TYPE POINTER FIELD FILE POINTED TO

--------------------------------------------------------------------------------

L=Laygo S=File not in set N=Normal Ref. C=Xref.

\*=Truncated m=Multiple v=Variable Pointer

---------------------

KEY (#.31) \| \|

UNIQUENESS INDEX ..... (N )-\> \| .11 INDEX \|

---------------------

---------------------

ARCHIVAL ACTIVITY (#1.11) \| \|

PRINT TEMPLATE ....... (N )-\> \| .4 PRINT TEMPLA\* \|

FILEGRAM HISTORY (#1.12) \| \|

FILEGRAM ............. (N )-\> \| FILE \|-\> FILE

\| DESTINATION FI\* \|-\> FILE

---------------------

---------------------

ARCHIVAL ACTIVITY (#1.11) \| \|

SEARCH TEMPLATE ...... (N L)-\> \| .401 SORT TEMPL\* \|

\| FILE \|-\> FILE

---------------------

---------------------

KERNEL SITE PARAMETE (#4.3) \| \|

USER CHARACTERISTICS T\* (N S )-\> \| .402 INPUT TEMP\* \|

KERNEL SYSTEM PARAME (#8989.3) \| \|

USER CHARACTERISTICS T\* (N S )-\> \| FILE \|-\> FILE

---------------------

---------------------

FORM (#.4031) \| \|

PAGE:HEADER BLOCK .... (N L)-\> \| .404 BLOCK \|

PAGE:BLOCK:BLOCK NAME (N C L)-\> \| \|

---------------------

---------------------

PRINT TEMPLATE (#.4) \| \|

EXPORT FORMAT ........ (N )-\> \| .44 FOREIGN FOR\* \|

---------------------

---------------------

\| .46 IMPORT TEMP\* \|

\| PRIMARY FILE \|-\> FILE

\| CREATOR \|-\> NEW PERSON

\| IMPORT:FILE\* \|-\> FILE

---------------------

---------------------

\| .6 DD AUDIT \|

\| USER \|-\> NEW PERSON

---------------------

---------------------

SORT TEMPLATE (#.4014) \| \|

SORT FIELD:DATA TYPE F\* (N )-\> \| .81 DATA TYPE \|

PRINT TEMPLATE (#.42) \| \|

EXPORT FIELD:DATA TYPE (N )-\> \| \|

DATA TYPE PROPERTY (#.86) \| \|

DATA TYPE ............ (N )-\> \| \|

---------------------

---------------------

SQLI_ERROR_LOG (#1.52192) \| .84 DIALOG \|

FILEMAN_ERROR ……. (N C)-\> \| PACKAGE \|-\> PACKAGE

---------------------

---------------------

DATA TYPE (#.81) \| \|

PROPERTY:PROPERTY .... (N C L)-\> \| .86 DATA TYPE P\* \|

---------------------

---------------------

DATA TYPE (#.81) \| \|

METHOD:METHOD ........ (N C L)-\> \| .87 DATA TYPE M\* \|

---------------------

---------------------

PRINT TEMPLATE (#.4) \| \|

LANGUAGE OF HEADING .. (N S L)-\> \| \|

LANGUAGE IN WHICH COMP\* (N S L)-\> \| \|

DIALOG (#.84) \| \|

TRANSLATION:LANGUAGE . (N C )-\> \| .85 LANGUAGE \|

LANGUAGE (#.85) \| \|

LINGUISTIC CATEGORY .. (N )-\> \| \|

MEMBER OF LANGUAGE SET (N )-\> \| \|

FILE (#1) \| \|

TRANSLATION:LANGUAGE . (N S L)-\> \| \|

NEW PERSON (#200) \| \|

LANGUAGE ............. (N S )-\> \| \|

KERNEL SITE PARAMETE (#8989.3) \| \|

DEFAULT LANGUAGE ..... (N S )-\> \| \|

---------------------

---------------------

VARIABLE-POINTER (#.12) \| \|

. . . . . . . . . . . (N S)-\> \| \|

PRINT TEMPLATE (#.4) \| 1 FILE \|

FILE ................. (N )-\> \| \|

DESTINATION FILE ... . (N )-\> \| \|

SORT TEMPLATE (#.401) \| DEVELOPER \|-\> NEW PERSON

FILE ................. (N )-\> \| \|

INPUT TEMPLATE (#.402) \| \|

FILE ................. (N )-\> \| \|

IMPORT TEMPLATE (#.46) \| \|

PRIMARY FILE ......... (N )-\> \| \|

IMPORT FIELDS:FILE ... (N )-\> \| \|

ARCHIVAL ACTIVITY (#1.11) \| \|

FILE ................. (N )-\> \| \|

DESTINATION FILE ..... (N )-\> \| \|

FILEGRAM HISTORY (#1.12) \| \|

FILE ................. (N )-\> \| \|

PACKAGE (#9.402) \| \|

AFFECTS R:FILE AFFECT\* (N S C )-\> \| \|

\*FILE ................ (N S )-\> \| \|

\*PRINT TEMPLATE:FILE.. (N S )-\> \| \|

\*INPUT TEMPLATE:FILE.. (N S )-\> \| \|

\*SORT TEMPLATE:FILE .. (N S )-\> \| \|

\*SCREEN TE:FILE\* ..... (N S )-\> \| \|

BUILD (#9.64) \| \|

FILE ................. (N S )-\> \| \|

BUILD COM:BUILD COMPO\* (N S )-\> \| \|

BUILD:ENTRIES:FILE\* .. (N S )-\> \| \|

INSTALL (#9.714) \| \|

FILE ................. (N S C )-\> \| \|

BUILD COM:BUILD COMPO\* (N S C )-\> \| \|

DUPLICATE RESOLUTION (#15.1) \| \|

FILE TO BE CHECKED ... (N S C )-\> \| \|

DUPLICATE:FILE FOR IN\* (N S C )-\> \| \|

DINUM FIL:DINUM FILE \* (N S C )-\> \| \|

NEW PERSON (#200.032) \| \|

ACCESSIBLE FILE ...... (N S C )-\> \| \|

PKI Digital Signatur (#8980.2) \| \|

DATA FILE ............ (N S )-\> \| \|

LOCAL KEYWORD (#8984.1) \| \|

ASSOCIATED FILE ...... (N S C )-\> \| \|

LOCAL SYNONYM (#8984.3) \| \|

ASSOCIATED FILE ...... (N S C )-\> \| \|

LOCAL LOOKUP (#8984.4) \| \|

NAME ................. (N S C )-\> \| \|

PARAMETER TEMPLATE (#8989.52) \| \|

USE ENTITY FROM ...... (N S )-\> \| \|

---------------------

---------------------

\| 1.1 AUDIT \|

\| USER \|-\> NEW PERSON

\| MENU OPTION US\* \|-\> OPTION

\| v PROTOCOL or OP\* \|-\> OPTION

\| \|-\> PROTOCOL

---------------------

---------------------

\| 1.11 ARCHIVAL A\* \|

\| FILE \|-\> FILE

\| ARCHIVER \|-\> NEW PERSON

\| SELECTOR \|-\> NEW PERSON

\| PURGER \|-\> NEW PERSON

\| USER PERFORMIN\* \|-\> NEW PERSON

\| DESTINATION FI\* \|-\> FILE

---------------------

---------------------

\| 1.12 FILEGRAM H\* \|

\| FILE \|-\> FILE

\| MESSAGE \|-\> MESSAGE

---------------------

---------------------

NEW PERSON (#200) \| \|

PREFERRED EDITOR .... (N S ) -\> \| 1.2 ALTERNATE E\* \|

---------------------

---------------------

SQLI_TABLE (#1.5215) \| \|

T_SCHEMA ............. (N L)-\> \| 1.521 SQLI_SCHE\* \|

---------------------

---------------------

SQLI_DOMAIN (#1.5212) \| \|

DM_DATA_TYPE ......... (N C )-\> \| 1.5211 SQLI_DAT\* \|

SQLI_KEY_FORMAT (#1.5213) \| \|

KF_DATA_TYPE ......... (N C )-\> \| D_OUTPUT_FORMAT
\|-\>SQLI_OUTPUT_FO\*

SQLI_OUTPUT_FORMAT (#1.5214) \| \|

OF_DATA_TYPE ......... (N )-\> \| \|

---------------------

---------------------

SQLI_TABLE_ELEMENT (#1.5216) \| \|

E_DOMAIN ............. (N C )-\> \| 1.5212 SQLI_DOM\* \|

\| DM_DATA_TYPE \|-\> SQLI_DATA_TYPE

\| DM_TABLE \|-\> SQLI_TABLE

\| DM_OUTPUT_FORM\* \|-\>SQLI_OUTPUT_FO\*

---------------------

---------------------

SQLI_PRIMARY_KEY (#1.5218) \| \|

P_KEY_FORMAT ......... (N )-\> \| 1.5213 SQLI_KEY\* \|

\| KF_DATA_TYPE \|-\> SQLI_DATA_TYPE

---------------------

---------------------

SQLI_DATA_TYPE (#1.5211) \| \|

D_OUTPUT_FORMAT ...... (N )-\> \| 1.5214 SQLI_OUT\* \|

SQLI_DOMAIN (#1.5212) \| \|

DM_OUTPUT_FORMAT ..... (N )-\> \| OF_DATA_TYPE \|-\> SQLI_DATA_TYPE

SQLI_COLUMN (#1.5217) \| \|

C_OUTPUT_FORMAT ...... (N C )-\> \| \|

---------------------

---------------------

SQLI_DOMAIN (#1.5212) \| \|

DM_TABLE ............. (N C )-\> \| 1.5215 SQLI_TAB\* \|

SQLI_TABLE (#1.5215) \| \|

T_MASTER_TABLE ....... (N C )-\> \| T_SCHEMA \|-\> SQLI_SCHEMA

SQLI_TABLE_ELEMENT (#1.5216) \| \|

E_TABLE .............. (N C )-\> \| T_MASTER_TABLE \|-\> SQLI_TABLE

---------------------

---------------------

SQLI_COLUMN (#1.5217) \| \|

C_TABLE_ELEMENT ...... (N C )-\> \| 1.5216 SQLI_TAB\* \|

SQLI_PRIMARY_KEY (#1.5218) \| \|

P_TBL_ELEMENT ........ (N C )-\> \| E_DOMAIN \|-\> SQLI_DOMAIN

SQLI_FOREIGN_KEY (#1.5219) \| \|

F_TBL_ELEMENT ........ (N C )-\> \| E_TABLE \|-\> SQLI_TABLE

---------------------

---------------------

SQLI_COLUMN (#1.5217) \| \|

C_PARENT ............. (N C )-\> \| 1.5217 SQLI_COL\* \|

SQLI_PRIMARY_KEY (#1.5218) \| \|

P_COLUMN ............. (N C )-\> \| C_TABLE_ELEMENT
\|-\>SQLI_TABLE_ELE\*

SQLI_FOREIGN_KEY (#1.5219) \| \|

F_CLM_ELEMENT ........ (N )-\> \| C_PARENT \|-\> SQLI_COLUMN

\| C_OUTPUT_FORMAT \|-\>SQLI_OUTPUT_FO\*

---------------------

---------------------

SQLI_FOREIGN_KEY (#1.5219) \| \|

F_PK_ELEMENT ......... (N )-\> \| 1.5218 SQLI_PRI\* \|

\| P_TBL_ELEMENT \|-\>SQLI_TABLE_ELE\*

\| P_COLUMN \|-\> SQLI_COLUMN

\| P_KEY_FORMAT \|-\>SQLI_KEY_FORMAT

---------------------

---------------------

\| 1.5219 SQLI_FOR\* \|

\| F_TBL_ELEMENT \|-\>SQLI_TABLE_ELE\*

\| F_PK_ELEMENT \|-\>SQLI_PRIMARY_K\*

\| F_CLM_ELEMENT \|-\> SQLI_COLUMN

---------------------

---------------------

SQLI_ERROR_LOG (#1.52192) \| \|

ERROR ................ (N C L)-\> \| 1.52191 SQLI_ER\* \|

---------------------

---------------------

\| 1.52192 SQLI_ER\* \|

\| ERROR \|-\> SQLI_ERROR_TE\*

---------------------

# Routines, Application Programming Interfaces (APIs), and Options

## Routines and Callable Entry Points

<u>Table 5</u> lists and briefly describes the VA FileMan routines and
Application Programming Interfaces (APIs; aka callable routines and
entry points).

<img src="images/media/image3.png" title="Caution"
style="width:0.44444in;height:0.44444in" alt="Caution" /> CAUTION VA
FileMan routines should *not* be altered, per Veterans Health
Administration (VHA) Directive 6402.

The Application Programming Interfaces (APIs; aka callable routines and
entry points) for those VA FileMan routines that can be invoked from
other applications are shown in the “Callable Entry Point” column in
<u>Table 5</u>.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** The APIs,
ScreenMan, and Database Server (DBS) calls are described in detail
(including their function, required variables, and any restrictions) in
the *VA FileMan Developer’s Guide*:

APIs—See the “Major APIs” and “Other APIs” sections in the *VA FileMan
Developer’s Guide*.

ScreenMan—See the “ScreenMan” section in the *VA FileMan Developer’s
Guide*.

Database Server (DBS) calls—See the “Database Server (DBS)” section in
the “Major APIs” section in the *VA FileMan Developer’s Guide*.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** The
Direct mode utilities, which can only be called directly from M and
ScreenMan-specific utilities, are listed in Sections <u>4.2</u> and
<u>4.3</u>, and are also described in the *VA FileMan Developer’s
Guide*.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** Routine
mapping is described in Section <u>4.4</u>.

<table>
<caption><p><span id="_Toc108021518" class="anchor"></span>Table : INDEX
(#.11) File—Cross-References</p></caption>
<colgroup>
<col style="width: 16%" />
<col style="width: 25%" />
<col style="width: 57%" />
</colgroup>
<thead>
<tr class="header">
<th>Routine</th>
<th>Callable Entry Point</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>%DT</strong></td>
<td></td>
<td>See DIDT for callable entry points and description.</td>
</tr>
<tr class="even">
<td><strong>%DTC</strong></td>
<td></td>
<td>See DIDTC for callable entry points and description.</td>
</tr>
<tr class="odd">
<td><strong>%RCR</strong></td>
<td></td>
<td>See DIRCR for callable entry points and description.</td>
</tr>
<tr class="even">
<td><strong>DDBR</strong></td>
<td><p>EN^DDBR</p>
<p>WP^DDBR</p>
<p>BROWSE^DDBR</p>
<p>DOCLIST^DDBR</p></td>
<td>Routines responsible for displaying ASCII text on a terminal screen,
for viewing only.</td>
</tr>
<tr class="odd">
<td><p><strong>DDBR0</strong></p>
<p><strong>DDBR1</strong></p>
<p><strong>DDBR2</strong></p>
<p><strong>DDBR3</strong></p>
<p><strong>DDBR4</strong></p>
<p><strong>DDBRAHT</strong></p>
<p><strong>DDBRAHTE</strong></p>
<p><strong>DDBRAHTJ</strong></p>
<p><strong>DDBRAHTR</strong></p>
<p><strong>DDBRAP</strong></p>
<p><strong>DDBRGE</strong></p>
<p><strong>DDBRP</strong></p>
<p><strong>DDBRS</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>DDBRT</strong></td>
<td>$$TEST^DDBRT</td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DDBRU</strong></p>
<p><strong>DDBRU2</strong></p>
<p><strong>DDBRWB</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>DDBRZIS</strong></td>
<td><p>CLOSE^DDBRZIS</p>
<p>OPEN^DDBRZIS</p>
<p>POST^DDBRZIS</p></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DDD</strong></td>
<td><p>^DDD</p>
<p>FILELIST^DDD</p>
<p>PARTIAL1^DDD</p>
<p>PARTIAL2^DDD</p></td>
<td>Routine that creates a full META DATA DICTIONARY (#.9) file. Other
entry points to be used to update partial portions of the META DATA
DICTIONARY (#.9) file.</td>
</tr>
<tr class="even">
<td><strong>DDE*</strong></td>
<td><p>$$GET1^DDE</p>
<p>GET^DDE</p></td>
<td>Entity main driver. Routines used to enter/edit entries in the
ENTITY (#1.5) file, VA FileMan Data Mapping [DDE ENTITY MAPPING] menu
options, and other DD utilities.</td>
</tr>
<tr class="odd">
<td><strong>DDE1A</strong></td>
<td></td>
<td>Enter/Edit an Entity via VA FileMan.</td>
</tr>
<tr class="even">
<td><strong>DDEG</strong></td>
<td></td>
<td>Entity <strong>GET</strong> Extract.</td>
</tr>
<tr class="odd">
<td><strong>DDEGET</strong></td>
<td></td>
<td>Entity <strong>GET</strong> Handler.</td>
</tr>
<tr class="even">
<td><strong>DDEMAP</strong></td>
<td></td>
<td>Auto-Generate Data Mapping.</td>
</tr>
<tr class="odd">
<td><strong>DDEOPT</strong></td>
<td></td>
<td>DDE Options.</td>
</tr>
<tr class="even">
<td><strong>DDEPRT</strong></td>
<td></td>
<td>Entity Print Utilities.</td>
</tr>
<tr class="odd">
<td><strong>DDERR</strong></td>
<td></td>
<td>Entity Error Handler.</td>
</tr>
<tr class="even">
<td><strong>DDEX</strong></td>
<td></td>
<td>Entity Data Dictionary Utilities.</td>
</tr>
<tr class="odd">
<td><strong>DDFIX</strong></td>
<td></td>
<td>Routine that checks nodes in the data dictionary and the FILE (#1)
file.</td>
</tr>
<tr class="even">
<td><p><strong>DDGF</strong></p>
<p><strong>DDGF0</strong></p>
<p><strong>DDGF1</strong></p>
<p><strong>DDGF2</strong></p>
<p><strong>DDGF3</strong></p>
<p><strong>DDGF4</strong></p>
<p><strong>DDGFADL</strong></p>
<p><strong>DDGFAPC</strong></p>
<p><strong>DDGFASUB</strong></p>
<p><strong>DDGFBK</strong></p>
<p><strong>DDGFBSEL</strong></p>
<p><strong>DDGFEL</strong></p>
<p><strong>DDGFFLD</strong></p>
<p><strong>DDGFFLDA</strong></p>
<p><strong>DDGFFM</strong></p>
<p><strong>DDGFH</strong></p>
<p><strong>DDGFHBK</strong></p>
<p><strong>DDGFLOAD</strong></p>
<p><strong>DDGFORD</strong></p>
<p><strong>DDGFPG</strong></p>
<p><strong>DDGFSV</strong></p>
<p><strong>DDGFU</strong></p>
<p><strong>DDGFUPDB</strong></p>
<p><strong>DDGFUPDP</strong></p></td>
<td></td>
<td>Routines used to create and edit ScreenMan forms.</td>
</tr>
<tr class="odd">
<td><p><strong>DDGLBXA</strong></p>
<p><strong>DDGLBXA1</strong></p>
<p><strong>DDGLCBOX</strong></p>
<p><strong>DDGLIB0</strong></p>
<p><strong>DDGLIBH</strong></p>
<p><strong>DDGLIBW</strong></p>
<p><strong>DDGLIBW1</strong></p></td>
<td></td>
<td>Routines that manage the screen for VA FileMan’s screen-oriented
utilities.</td>
</tr>
<tr class="even">
<td><strong>DDIOL</strong></td>
<td>EN^DDIOL</td>
<td><p>Routine that any of the following:</p>
<ul>
<li><p>Writes text to the screen.</p></li>
<li><p>Writes text in ScreenMan’s Command Area.</p></li>
<li><p>Loads text into an array, depending on the environment in which
it is called.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>DDMAP</strong></p>
<p><strong>DDMAP1</strong></p>
<p><strong>DDMAP2</strong></p></td>
<td></td>
<td>Routines that generate a graphic display of the pointer
relationships among a specified group of package files to an output
device.</td>
</tr>
<tr class="even">
<td><strong>DDMOD</strong></td>
<td><p>DELIX^DDMOD</p>
<p>DELIXN^DDMOD</p>
<p>CREIXN^DDMOD</p>
<p>FILESEC^DDMOD</p></td>
<td>Routine supporting calls for modifying DD attributes.</td>
</tr>
<tr class="odd">
<td><p><strong>DDMP</strong></p>
<p><strong>DDMP1</strong></p>
<p><strong>DDMP2</strong></p>
<p><strong>DDMPSM</strong></p>
<p><strong>DDMPSM1</strong></p>
<p><strong>DDMPU</strong></p></td>
<td>FILE^DDMP</td>
<td>Routines used by the Import Tool.</td>
</tr>
<tr class="even">
<td><strong>DDPA2</strong></td>
<td></td>
<td>Routine finds any sort templates that have a sort field with a range
that is <strong>FROM</strong> or <strong>TO</strong> a
<em>non</em>-canonic number.</td>
</tr>
<tr class="odd">
<td><p><strong>DDR</strong></p>
<p><strong>DDR0</strong></p>
<p><strong>DDR1</strong></p>
<p><strong>DDR2</strong></p>
<p><strong>DDR3</strong></p>
<p><strong>DDR4</strong></p></td>
<td></td>
<td>Routines that contain the RPCs for the VA FileMan Delphi
components.</td>
</tr>
<tr class="even">
<td><p><strong>DDS</strong></p>
<p><strong>DDS0</strong></p>
<p><strong>DDS01</strong></p>
<p><strong>DDS02</strong></p>
<p><strong>DDS1</strong></p>
<p><strong>DDS10</strong></p>
<p><strong>DDS11</strong></p>
<p><strong>DDS2</strong></p>
<p><strong>DDS3</strong></p>
<p><strong>DDS4</strong></p>
<p><strong>DDS41</strong></p>
<p><strong>DDS5</strong></p>
<p><strong>DDS6</strong></p>
<p><strong>DDS7</strong></p>
<p><strong>DDSBOX</strong></p>
<p><strong>DDSCAP</strong></p>
<p><strong>DDSCLONE</strong></p>
<p><strong>DDSCLONF</strong></p>
<p><strong>DDSCOM</strong></p>
<p><strong>DDSCOMP</strong></p>
<p><strong>DDSDBLK</strong></p>
<p><strong>DDSDEL</strong></p>
<p><strong>DDSDFRM</strong></p>
<p><strong>DDSFO</strong></p>
<p><strong>DDSIT</strong></p>
<p><strong>DDSLIB</strong></p>
<p><strong>DDSM</strong></p>
<p><strong>DDSM1</strong></p>
<p><strong>DDSMSG</strong></p>
<p><strong>DDSOPT</strong></p>
<p><strong>DDSPRNT</strong></p>
<p><strong>DDSPRNT1</strong></p>
<p><strong>DDSPRNT2</strong></p>
<p><strong>DDSPTR</strong></p>
<p><strong>DDSR</strong></p>
<p><strong>DDSR1</strong></p>
<p><strong>DDSRP</strong></p>
<p><strong>DDSRSEL</strong></p>
<p><strong>DDSRUN</strong></p>
<p><strong>DDSSTK</strong></p>
<p><strong>DDSU</strong></p></td>
<td>DDS</td>
<td>Routines used to compile and run forms for data viewing and
editing—ScreenMan.</td>
</tr>
<tr class="odd">
<td><strong>DDSUTL</strong></td>
<td><p>MSG^DDSUTL</p>
<p>REFRESH^DDSUTL</p>
<p>REQ^DDSUTL</p>
<p>UNED^DDSUTL</p></td>
<td></td>
</tr>
<tr class="even">
<td><strong>DDSVAL</strong></td>
<td><p>$$GET^DDSVAL</p>
<p>PUT^DDSVAL</p></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DDSVALF</strong></td>
<td><p>$$GET^DDSVALF</p>
<p>PUT^DDSVALF</p></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DDSVALM</strong></p>
<p><strong>DDSWP</strong></p>
<p><strong>DDSZ</strong></p>
<p><strong>DDSZ1</strong></p>
<p><strong>DDSZ2</strong></p>
<p><strong>DDSZ3</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DDU</strong></p>
<p><strong>DDUCHK</strong></p>
<p><strong>DDUCHK1</strong></p>
<p><strong>DDUCHK2</strong></p>
<p><strong>DDUCHK3</strong></p>
<p><strong>DDUCHK4</strong></p>
<p><strong>DDUCHK5</strong></p></td>
<td></td>
<td>Routines responsible for running the data dictionary checking
utility.</td>
</tr>
<tr class="even">
<td><p><strong>DDW</strong></p>
<p><strong>DDW1</strong></p>
<p><strong>DDW2</strong></p>
<p><strong>DDW3</strong></p>
<p><strong>DDW4</strong></p>
<p><strong>DDW5</strong></p>
<p><strong>DDW6</strong></p>
<p><strong>DDW7</strong></p>
<p><strong>DDW8</strong></p>
<p><strong>DDW9</strong></p>
<p><strong>DDWC</strong></p>
<p><strong>DDWC1</strong></p>
<p><strong>DDWF</strong></p>
<p><strong>DDWG</strong></p>
<p><strong>DDWH</strong></p>
<p><strong>DDWK</strong></p>
<p><strong>DDWT1</strong></p></td>
<td></td>
<td>Routines responsible for full screen text editing.</td>
</tr>
<tr class="odd">
<td><p><strong>DDXP</strong></p>
<p><strong>DDXP1</strong></p>
<p><strong>DDXP2</strong></p>
<p><strong>DDXP3</strong></p>
<p><strong>DDXP31</strong></p>
<p><strong>DDXP32</strong></p>
<p><strong>DDXP33</strong></p>
<p><strong>DDXP4</strong></p>
<p><strong>DDXP41</strong></p>
<p><strong>DDXP5</strong></p>
<p><strong>DDXPLIB</strong></p></td>
<td></td>
<td>Routines responsible for the data export to a Foreign Format
tool.</td>
</tr>
<tr class="even">
<td><strong>DI</strong></td>
<td></td>
<td>Routine for direct entry into VA FileMan.</td>
</tr>
<tr class="odd">
<td><p><strong>DI222ENV</strong></p>
<p><strong>DI222POS</strong></p>
<p><strong>DI222PRE</strong></p></td>
<td></td>
<td>These routines are removed after the install.</td>
</tr>
<tr class="even">
<td><p><strong>DIA</strong></p>
<p><strong>DIA1</strong></p>
<p><strong>DIA2</strong></p>
<p><strong>DIA3</strong></p></td>
<td></td>
<td>Routines responsible for gathering fields to be edited.</td>
</tr>
<tr class="odd">
<td><strong>DIAC</strong></td>
<td>DIAC</td>
<td>Routine that determines file access.</td>
</tr>
<tr class="even">
<td><strong>DIAC1</strong></td>
<td>$$CANDO^DIAC1</td>
<td>Data Access Control (DAC): Policy Evaluation API.</td>
</tr>
<tr class="odd">
<td><strong>DIAC1T</strong></td>
<td></td>
<td>Data Access Control (DAC): Test utility for Policies.</td>
</tr>
<tr class="even">
<td><strong>DIACLM</strong></td>
<td></td>
<td>Data Access Control (DAC): Policy Editor driver.</td>
</tr>
<tr class="odd">
<td><strong>DIACLM1</strong></td>
<td></td>
<td>Data Access Control (DAC): Policy Editor actions.</td>
</tr>
<tr class="even">
<td><strong>DIACOPT</strong></td>
<td></td>
<td>Data Access Control (DAC): Data Access Control Options.</td>
</tr>
<tr class="odd">
<td><strong>DIACP</strong></td>
<td></td>
<td>Data Access Control (DAC): Print Policy Reports.</td>
</tr>
<tr class="even">
<td><strong>DIACX</strong></td>
<td></td>
<td>Data Access Control (DAC): Policy utilities.</td>
</tr>
<tr class="odd">
<td><strong>DIALOG</strong></td>
<td><p>BLD^DIALOG</p>
<p>$$EZBLD^DIALOG</p></td>
<td>Routines to build VA FileMan dialogues and their functions.</td>
</tr>
<tr class="even">
<td><strong>DIALOGU</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIALOGZ</strong></td>
<td>LANG^DIALOGZ</td>
<td>Routine that creates and uses foreign-language additions to the data
dictionary.</td>
</tr>
<tr class="even">
<td><p><strong>DIAR</strong></p>
<p><strong>DIARA</strong></p>
<p><strong>DIARB</strong></p>
<p><strong>DIARCALC</strong></p>
<p><strong>DIARR</strong></p>
<p><strong>DIARR1</strong></p>
<p><strong>DIARR2</strong></p>
<p><strong>DIARR3</strong></p>
<p><strong>DIARR4</strong></p>
<p><strong>DIARR5</strong></p>
<p><strong>DIARR6</strong></p>
<p><strong>DIARU</strong></p>
<p><strong>DIARX</strong></p></td>
<td></td>
<td>Routines responsible for VA FileMan archiving.</td>
</tr>
<tr class="odd">
<td><p><strong>DIAU</strong></p>
<p><strong>DIAUTL</strong></p></td>
<td></td>
<td>Routines used for auditing.</td>
</tr>
<tr class="even">
<td><p><strong>DIAX</strong></p>
<p><strong>DIAXD</strong></p>
<p><strong>DIAXERR</strong></p>
<p><strong>DIAXF</strong></p>
<p><strong>DIAXM</strong></p>
<p><strong>DIAXM1</strong></p>
<p><strong>DIAXM2</strong></p>
<p><strong>DIAXM3</strong></p>
<p><strong>DIAXMS</strong></p>
<p><strong>DIAXP</strong></p>
<p><strong>DIAXT</strong></p>
<p><strong>DIAXU</strong></p></td>
<td>EN^DIAXU</td>
<td>Routines responsible for extracting data to a VA FileMan file.</td>
</tr>
<tr class="odd">
<td><strong>DIB</strong></td>
<td>EN^DIB</td>
<td>Routine that creates a new file.</td>
</tr>
<tr class="even">
<td><p><strong>DIBT</strong></p>
<p><strong>DIBT1</strong></p>
<p><strong>DIBTEDT</strong></p></td>
<td></td>
<td>Routine that stores a SORT template.</td>
</tr>
<tr class="odd">
<td><strong>DIC</strong></td>
<td><p>DIC</p>
<p>FIND^DIC</p>
<p>$$FIND1^DIC</p>
<p>IX^DIC</p>
<p>LIST^DIC</p></td>
<td>Routines that perform VA FileMan lookups or return an ordered list
of records.</td>
</tr>
<tr class="even">
<td><strong>DIC0</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIC1</strong></td>
<td><p>MIX^DIC1</p>
<p>DO^DIC1</p></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DIC11</strong></p>
<p><strong>DIC2</strong></p>
<p><strong>DIC3</strong></p>
<p><strong>DIC4</strong></p>
<p><strong>DIC5</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DICA</strong></p>
<p><strong>DICA1</strong></p>
<p><strong>DICA2</strong></p>
<p><strong>DICA3</strong></p></td>
<td></td>
<td>Routines responsible for DBS Updater functions.</td>
</tr>
<tr class="even">
<td><p><strong>DICATT</strong></p>
<p><strong>DICATT0</strong></p>
<p><strong>DICATT1</strong></p>
<p><strong>DICATT2</strong></p>
<p><strong>DICATT22</strong></p>
<p><strong>DICATT3</strong></p>
<p><strong>DICATT4</strong></p>
<p><strong>DICATT5</strong></p>
<p><strong>DICATT6</strong></p></td>
<td></td>
<td>Routines responsible for the Modify File Attributes option.</td>
</tr>
<tr class="odd">
<td><strong>DICATTA</strong></td>
<td></td>
<td>Routine responsible for data dictionary audits.</td>
</tr>
<tr class="even">
<td><p><strong>DICATTD</strong></p>
<p><strong>DICATTD0</strong></p>
<p><strong>DICATTD1</strong></p>
<p><strong>DICATTD2</strong></p>
<p><strong>DICATTD3</strong></p>
<p><strong>DICATTD4</strong></p>
<p><strong>DICATTD5</strong></p>
<p><strong>DICATTD6</strong></p>
<p><strong>DICATTD7</strong></p>
<p><strong>DICATTD8</strong></p>
<p><strong>DICATTD9</strong></p>
<p><strong>DICATTDD</strong></p>
<p><strong>DICATTDE</strong></p>
<p><strong>DICATTDK</strong></p>
<p><strong>DICATTDM</strong></p>
<p><strong>DICATTUD</strong></p></td>
<td></td>
<td>Routines responsible for Modify File Attributes option in Screen
oriented format.</td>
</tr>
<tr class="odd">
<td><strong>DICD</strong></td>
<td>WAIT^DICD</td>
<td>Routine for selecting, displaying, editing, or deleting a
cross-reference.</td>
</tr>
<tr class="even">
<td><p><strong>DICE</strong></p>
<p><strong>DICE0</strong></p>
<p><strong>DICE1</strong></p>
<p><strong>DICE2</strong></p>
<p><strong>DICE3</strong></p>
<p><strong>DICE4</strong></p>
<p><strong>DICE7</strong></p></td>
<td></td>
<td>Routines responsible for creating cross-references.</td>
</tr>
<tr class="odd">
<td><p><strong>DICF</strong></p>
<p><strong>DICF0</strong></p>
<p><strong>DICF1</strong></p>
<p><strong>DICF2</strong></p>
<p><strong>DICF3</strong></p>
<p><strong>DICF4</strong></p>
<p><strong>DICF5</strong></p>
<p><strong>DICFIX</strong></p>
<p><strong>DICFIX1</strong></p></td>
<td></td>
<td>Routines responsible for DBS Finder functions.</td>
</tr>
<tr class="even">
<td><p><strong>DICL</strong></p>
<p><strong>DICL1</strong></p>
<p><strong>DICL10</strong></p>
<p><strong>DICL2</strong></p>
<p><strong>DICL3</strong></p>
<p><strong>DICLGFT</strong></p>
<p><strong>DICLIB</strong></p>
<p><strong>DICLIX</strong></p>
<p><strong>DICLIX0</strong></p>
<p><strong>DICLIX1</strong></p></td>
<td></td>
<td>Routines responsible for DBS Lister functions.</td>
</tr>
<tr class="odd">
<td><p><strong>DICM</strong></p>
<p><strong>DICM0</strong></p>
<p><strong>DICM1</strong></p>
<p><strong>DICM2</strong></p>
<p><strong>DICM3</strong></p></td>
<td></td>
<td>Routines responsible for performing transforms on the lookup value
to attempt to find a match on the lookup indexes. For example,
transforms date to internal format.</td>
</tr>
<tr class="even">
<td><strong>DICN</strong></td>
<td><p>FILE^DICN</p>
<p>YN^DICN</p></td>
<td>Routines that allow adding a new entry to a file.</td>
</tr>
<tr class="odd">
<td><p><strong>DICN0</strong></p>
<p><strong>DICN1</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DICOMP</strong></p>
<p><strong>DICOMP0</strong></p>
<p><strong>DICOMP1</strong></p>
<p><strong>DICOMPU</strong></p>
<p><strong>DICOMPV</strong></p>
<p><strong>DICOMPW</strong></p>
<p><strong>DICOMPX</strong></p>
<p><strong>DICOMPY</strong></p>
<p><strong>DICOMPZ</strong></p></td>
<td></td>
<td>Routines that evaluate computed field expressions.</td>
</tr>
<tr class="odd">
<td><p><strong>DICQ</strong></p>
<p><strong>DICQ1</strong></p></td>
<td>DQ^DICQ</td>
<td>Routines responsible for help on lookups.</td>
</tr>
<tr class="even">
<td><strong>DICR</strong></td>
<td></td>
<td>Routine responsible for recursive calls for cross-references on
triggered fields.</td>
</tr>
<tr class="odd">
<td><p><strong>DICRW</strong></p>
<p><strong>DICRW1</strong></p></td>
<td>DT^DICRW</td>
<td>Routines that select a file.</td>
</tr>
<tr class="even">
<td><p><strong>DICU</strong></p>
<p><strong>DICU1</strong></p>
<p><strong>DICU11</strong></p>
<p><strong>DICU2</strong></p>
<p><strong>DICUF</strong></p>
<p><strong>DICUIX</strong></p>
<p><strong>DICUIX1</strong></p>
<p><strong>DICUIX2</strong></p></td>
<td></td>
<td>Routines containing utilities used during lookups.</td>
</tr>
<tr class="odd">
<td><strong>DID</strong></td>
<td><p>EN^DID</p>
<p>FIELD^DID</p>
<p>FIELDLST^DID</p>
<p>FILE^DID</p>
<p>FILELST^DID</p>
<p>$$GET1^DID</p></td>
<td>Routines for data dictionary listings.</td>
</tr>
<tr class="even">
<td><strong>DID1</strong></td>
<td></td>
<td>Standard data dictionary listing.</td>
</tr>
<tr class="odd">
<td><strong>DID2</strong></td>
<td></td>
<td>Modified data dictionary listing.</td>
</tr>
<tr class="even">
<td><strong>DIDC</strong></td>
<td></td>
<td>Condensed data dictionary listing.</td>
</tr>
<tr class="odd">
<td><strong>DIDG</strong></td>
<td></td>
<td>Global Map data dictionary listing.</td>
</tr>
<tr class="even">
<td><strong>DIDGFTPT</strong></td>
<td></td>
<td>Find pointers into a file utility.</td>
</tr>
<tr class="odd">
<td><strong>DIDH</strong></td>
<td></td>
<td>Headers for the data dictionary listings.</td>
</tr>
<tr class="even">
<td><strong>DIDH1</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIDT</strong></td>
<td><p>%DT</p>
<p>DD^%DT</p></td>
<td>Routine responsible for the Date/Time validation. <em>Must</em> be
stored in the Manager account as <strong>%DT</strong>.</td>
</tr>
<tr class="even">
<td><strong>DIDTC</strong></td>
<td><p>%DTC</p>
<p>C^%DTC</p>
<p>NOW^%DTC</p>
<p>H^%DTC</p>
<p>DW^%DTC</p>
<p>YMD^%DTC</p>
<p>COMMA^%DTC</p>
<p>S^%DTC</p>
<p>YX^%DTC</p>
<p>HELP^%DTC</p></td>
<td>Routine responsible for the Date/Time operations. <em>Must</em> be
stored in the Manager account as <strong>%DTC</strong>.</td>
</tr>
<tr class="odd">
<td><p><strong>DIDU</strong></p>
<p><strong>DIDU1</strong></p>
<p><strong>DIDU2</strong></p></td>
<td></td>
<td>Routines responsible for data dictionary functions.</td>
</tr>
<tr class="even">
<td><strong>DIDX</strong></td>
<td></td>
<td>Brief data dictionary listing.</td>
</tr>
<tr class="odd">
<td><strong>DIE</strong></td>
<td><p>DIE</p>
<p>CHK^DIE</p>
<p>FILE^DIE</p>
<p>HELP^DIE</p>
<p>$$KEYVAL^DIE</p>
<p>UPDATE^DIE</p>
<p>VAL^DIE</p>
<p>VALS^DIE</p>
<p>WP^DIE</p></td>
<td>Routines responsible for the Enter or Edit File Entries option and
for DBS filing and help retrieval functions.</td>
</tr>
<tr class="even">
<td><p><strong>DIE0</strong></p>
<p><strong>DIE1</strong></p>
<p><strong>DIE17</strong></p>
<p><strong>DIE2</strong></p>
<p><strong>DIE3</strong></p>
<p><strong>DIE9</strong></p>
<p><strong>DIED</strong></p>
<p><strong>DIEF</strong></p>
<p><strong>DIEF1</strong></p>
<p><strong>DIEFU</strong></p>
<p><strong>DIEFW</strong></p>
<p><strong>DIEH</strong></p>
<p><strong>DIEH1</strong></p>
<p><strong>DIEKMSG</strong></p>
<p><strong>DIEQ</strong></p>
<p><strong>DIEQ1</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DIENV</strong></p>
<p><strong>DIENVSTP</strong></p>
<p><strong>DIENVWRN</strong></p></td>
<td></td>
<td>Environment check routines.</td>
</tr>
<tr class="even">
<td><p><strong>DIET</strong></p>
<p><strong>DIETED</strong></p></td>
<td></td>
<td>Routine that displays an INPUT template and performs VA FileMan
auditing function.</td>
</tr>
<tr class="odd">
<td><strong>DIETLIB</strong></td>
<td></td>
<td>Library of APIs for user-defined data types.</td>
</tr>
<tr class="even">
<td><strong>DIETLIBF</strong></td>
<td></td>
<td>Library for field attributes.</td>
</tr>
<tr class="odd">
<td><p><strong>DIEV</strong></p>
<p><strong>DIEV1</strong></p>
<p><strong>DIEVK</strong></p>
<p><strong>DIEVK1</strong></p>
<p><strong>DIEVS</strong></p></td>
<td></td>
<td>Routines responsible for data validation functions.</td>
</tr>
<tr class="even">
<td><p><strong>DIEZ</strong></p>
<p><strong>DIEZ0</strong></p>
<p><strong>DIEZ1</strong></p>
<p><strong>DIEZ2</strong></p>
<p><strong>DIEZ3</strong></p>
<p><strong>DIEZ4</strong></p></td>
<td><p>DIEZ</p>
<p>EN^DIEZ</p></td>
<td>Routines that compile INPUT templates.</td>
</tr>
<tr class="odd">
<td><p><strong>DIFG</strong></p>
<p><strong>DIFG0</strong></p>
<p><strong>DIFG0A</strong></p>
<p><strong>DIFG0B</strong></p>
<p><strong>DIFG1</strong></p>
<p><strong>DIFG2</strong></p>
<p><strong>DIFG3</strong></p>
<p><strong>DIFG3A</strong></p>
<p><strong>DIFG4</strong></p>
<p><strong>DIFG4A</strong></p>
<p><strong>DIFG5</strong></p>
<p><strong>DIFG6</strong></p>
<p><strong>DIFG7</strong></p>
<p><strong>DIFGA</strong></p>
<p><strong>DIFGA1</strong></p>
<p><strong>DIFGB</strong></p></td>
<td>DIFG</td>
<td>Routines responsible for Filegrams.</td>
</tr>
<tr class="even">
<td><strong>DIFGG</strong></td>
<td>EN^DIFGG</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIFGG2</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DIFGG4</strong></p>
<p><strong>DIFGGI</strong></p>
<p><strong>DIFGGSB</strong></p>
<p><strong>DIFGGSB1</strong></p>
<p><strong>DIFGGSB2</strong></p>
<p><strong>DIFGGU</strong></p>
<p><strong>DIFGO</strong></p>
<p><strong>DIFGSRV</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIFMEDT1</strong></td>
<td><p>ENP81^DIFMEDT1</p>
<p>ENP86^DIFMEDT1</p>
<p>ENP87^DIFMEDT1</p></td>
<td><p>Routine to enter/edit entries in the following files:</p>
<ul>
<li><p>DATA TYPE (#.81)</p></li>
<li><p>DATA TYPE PROPERTY (#.86)</p></li>
<li><p>DATA TYPE METHOD (#.87)</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>DIFROM</strong></p>
<p><strong>DIFROM0</strong></p>
<p><strong>DIFROM1</strong></p>
<p><strong>DIFROM11</strong></p>
<p><strong>DIFROM12</strong></p>
<p><strong>DIFROM2</strong></p>
<p><strong>DIFROM3</strong></p>
<p><strong>DIFROM4</strong></p>
<p><strong>DIFROM41</strong></p>
<p><strong>DIFROM42</strong></p>
<p><strong>DIFROM5</strong></p>
<p><strong>DIFROM6</strong></p>
<p><strong>DIFROM7</strong></p>
<p><strong>DIFROMH</strong></p>
<p><strong>DIFROMH1</strong></p>
<p><strong>DIFROMS</strong></p>
<p><strong>DIFROMS1</strong></p>
<p><strong>DIFROMS2</strong></p>
<p><strong>DIFROMS3</strong></p>
<p><strong>DIFROMS4</strong></p>
<p><strong>DIFROMS5</strong></p>
<p><strong>DIFROMSB</strong></p>
<p><strong>DIFROMSC</strong></p>
<p><strong>DIFROMSD</strong></p>
<p><strong>DIFROMSE</strong></p>
<p><strong>DIFROMSI</strong></p>
<p><strong>DIFROMSK</strong></p>
<p><strong>DIFROMSL</strong></p>
<p><strong>DIFROMSO</strong></p>
<p><strong>DIFROMSP</strong></p>
<p><strong>DIFROMSR</strong></p>
<p><strong>DIFROMSS</strong></p>
<p><strong>DIFROMSU</strong></p>
<p><strong>DIFROMSV</strong></p>
<p><strong>DIFROMSX</strong></p>
<p><strong>DIFROMSY</strong></p></td>
<td>DIFROM</td>
<td>Routines responsible for generating init packages for export and
supporting Kernel’s KIDS functions.</td>
</tr>
<tr class="odd">
<td><strong>DIFSBLD</strong></td>
<td>JSON1^DIFSBLD</td>
<td>Routine to accept a JSON formatted file, process the data in it, and
insert the data into a FileMan file, logging the results into a new Data
Synchronization History file (#1.75).</td>
</tr>
<tr class="even">
<td><strong>DIG</strong></td>
<td></td>
<td>Routine responsible for the Scattergram option on the Statistics
submenu.</td>
</tr>
<tr class="odd">
<td><strong>DIH</strong></td>
<td></td>
<td>Routine responsible for the Histogram option on the Statistics
submenu.</td>
</tr>
<tr class="even">
<td><p><strong>DII</strong></p>
<p><strong>DII1</strong></p></td>
<td></td>
<td>Routines responsible for the main menu in standalone VA FileMan and
for the Inquire to File Entries option.</td>
</tr>
<tr class="odd">
<td><p><strong>DIIS</strong></p>
<p><strong>DIISC</strong></p>
<p><strong>DIISS</strong></p></td>
<td></td>
<td>Routines responsible for device selection for standalone VA FileMan.
Stored in the Manager account as <strong>%ZIS</strong>,
<strong>%ZISC</strong>, and <strong>%ZISS</strong>.</td>
</tr>
<tr class="even">
<td><strong>DIK</strong></td>
<td><p>DIK</p>
<p>IXALL^DIK</p>
<p>IX^DIK</p>
<p>IX1^DIK</p>
<p>ENALL^DIK</p>
<p>EN^DIK</p>
<p>EN1^DIK</p></td>
<td>Routines that perform file re-indexing and entry deletion.</td>
</tr>
<tr class="odd">
<td><strong>DIK1</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DIKC</strong></p>
<p><strong>DIKC1</strong></p>
<p><strong>DIKC2</strong></p>
<p><strong>DIKCBLD</strong></p>
<p><strong>DIKCDD</strong></p>
<p><strong>DIKCFORM</strong></p>
<p><strong>DIKCP</strong></p>
<p><strong>DIKCP1</strong></p>
<p><strong>DIKCP2</strong></p>
<p><strong>DIKCP3</strong></p>
<p><strong>DIKCR</strong></p>
<p><strong>DIKCU</strong></p>
<p><strong>DIKCU1</strong></p>
<p><strong>DIKCU2</strong></p>
<p><strong>DIKCUTL</strong></p>
<p><strong>DIKCUTL1</strong></p>
<p><strong>DIKCUTL2</strong></p>
<p><strong>DIKCUTL3</strong></p>
<p><strong>DIKD</strong></p>
<p><strong>DIKD1</strong></p>
<p><strong>DIKD2</strong></p></td>
<td>DIKCBLD</td>
<td>Routines responsible for defining, deleting, printing, and executing
the logic for New-Style indices.</td>
</tr>
<tr class="odd">
<td><p><strong>DIKK</strong></p>
<p><strong>DIKK1</strong></p>
<p><strong>DIKK2</strong></p>
<p><strong>DIKKDD</strong></p>
<p><strong>DIKKFORM</strong></p>
<p><strong>DIKKP</strong></p>
<p><strong>DIKKUTL</strong></p>
<p><strong>DIKKUTL1</strong></p>
<p><strong>DIKKUTL2</strong></p>
<p><strong>DIKKUTL3</strong></p>
<p><strong>DIKKUTL4</strong></p></td>
<td></td>
<td>Routines responsible for defining, printing, and verifying the
integrity of Keys.</td>
</tr>
<tr class="even">
<td><p><strong>DIKZ</strong></p>
<p><strong>DIKZ0</strong></p>
<p><strong>DIKZ1</strong></p>
<p><strong>DIKZ11</strong></p>
<p><strong>DIKZ2</strong></p></td>
<td><p>DIKZ</p>
<p>EN^DIKZ</p></td>
<td>Routines responsible for VA FileMan’s cross-reference compiler.</td>
</tr>
<tr class="odd">
<td><p><strong>DIL</strong></p>
<p><strong>DIL0</strong></p>
<p><strong>DIL1</strong></p>
<p><strong>DIL11</strong></p>
<p><strong>DIL2</strong></p>
<p><strong>DILL</strong></p></td>
<td></td>
<td>Routines responsible for processing PRINT templates or fields.</td>
</tr>
<tr class="even">
<td><strong>DILF</strong></td>
<td><p>CLEAN^DILF</p>
<p>$$CREF^DILF</p>
<p>DA^DILF</p>
<p>DT^DILF</p>
<p>FDA^DILF</p>
<p>$$IENS^DILF</p>
<p>$$OREF^DILF</p>
<p>$$VALUE1^DILF</p>
<p>VALUES^DILF</p></td>
<td>Routine that contains VA FileMan’s library of functions.</td>
</tr>
<tr class="odd">
<td><strong>DILFD</strong></td>
<td><p>$$EXTERNAL^DILFD</p>
<p>$$FLDNUM^DILFD</p>
<p>PRD^DILFD</p>
<p>RECALL^DILFD</p>
<p>$$ROOT^DILFD</p>
<p>$$VFIELD^DILFD</p>
<p>$$VFILE^DILFD</p></td>
<td></td>
</tr>
<tr class="even">
<td><strong>DILIBF</strong></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DIM</strong></p>
<p><strong>DIM1</strong></p>
<p><strong>DIM2</strong></p>
<p><strong>DIM3</strong></p>
<p><strong>DIM4</strong></p></td>
<td>DIM</td>
<td>Routines responsible for the M syntax checker.</td>
</tr>
<tr class="even">
<td><strong>DINIT</strong></td>
<td></td>
<td>Routines that initialize VA FileMan.</td>
</tr>
<tr class="odd">
<td><strong>DINIT*</strong></td>
<td></td>
<td>Numerous routines starting with “DINIT” are used in the
initialization process.</td>
</tr>
<tr class="even">
<td><p><strong>DINVGTM</strong></p>
<p><strong>DINVGUX</strong></p>
<p><strong>DINVONT</strong></p>
<p><strong>DINZONT</strong></p></td>
<td></td>
<td>Routines containing operating system specific code.</td>
</tr>
<tr class="odd">
<td><p><strong>DIO</strong></p>
<p><strong>DIO0</strong></p>
<p><strong>DIO1</strong></p></td>
<td></td>
<td>Routines responsible for building sort logic, executing the sort,
and performing output functions.</td>
</tr>
<tr class="even">
<td><strong>DIO2</strong></td>
<td>DT^DIO2</td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DIO3</strong></p>
<p><strong>DIO4</strong></p>
<p><strong>DIOS</strong></p>
<p><strong>DIOS1</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>DIOC</strong></td>
<td></td>
<td>Routine responsible for checking code to check query
conditions.</td>
</tr>
<tr class="odd">
<td><strong>DIOQ</strong></td>
<td></td>
<td>Routine responsible for determining sort (query) optimization
numbers.</td>
</tr>
<tr class="even">
<td><strong>DIOU</strong></td>
<td></td>
<td>Routines responsible for generic VA FileMan code generation
utilities.</td>
</tr>
<tr class="odd">
<td><strong>DIOZ</strong></td>
<td>^DIOZ</td>
<td>Routines responsible for compiling SORT templates.</td>
</tr>
<tr class="even">
<td><p><strong>DIP</strong></p>
<p><strong>DIP0</strong></p>
<p><strong>DIP1</strong></p>
<p><strong>DIP10</strong></p>
<p><strong>DIP100</strong></p>
<p><strong>DIP11</strong></p>
<p><strong>DIP12</strong></p>
<p><strong>DIP2</strong></p>
<p><strong>DIP21</strong></p>
<p><strong>DIP22</strong></p>
<p><strong>DIP23</strong></p>
<p><strong>DIP3</strong></p>
<p><strong>DIP31</strong></p>
<p><strong>DIP4</strong></p>
<p><strong>DIP5</strong></p></td>
<td>EN1^DIP</td>
<td>Routines that: process sorting specifications, edit SORT templates,
process the <strong>FROM</strong> and <strong>TO</strong> sort range,
edit PRINT templates, process PRINT templates, and initialize the
printing process.</td>
</tr>
<tr class="odd">
<td><strong>DIPT</strong></td>
<td><p>DIPT</p>
<p>DIBT^DIPT</p></td>
<td>Routine that displays PRINT and SORT templates.</td>
</tr>
<tr class="even">
<td><strong>DIPTED</strong></td>
<td></td>
<td>Routine used for the ScreenMan-based PRINT template editor.</td>
</tr>
<tr class="odd">
<td><strong>DIPZ</strong></td>
<td><p>DIPZ</p>
<p>EN^DIPZ</p></td>
<td>Routines that compile PRINT templates.</td>
</tr>
<tr class="even">
<td><p><strong>DIPZ0</strong></p>
<p><strong>DIPZ1</strong></p>
<p><strong>DIPZ2</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIQ</strong></td>
<td><p>EN^DIQ</p>
<p>Y^DIQ</p>
<p>D^DIQ</p>
<p>DT^DIQ</p>
<p>$$GET1^DIQ</p>
<p>GETS^DIQ</p></td>
<td>Routines that retrieve data and support DBS Retriever and DD
Retriever functions.</td>
</tr>
<tr class="even">
<td><strong>DIQ1</strong></td>
<td>EN^DIQ1</td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>DIQG</strong></p>
<p><strong>DIQGDD</strong></p>
<p><strong>DIQGDD0</strong></p>
<p><strong>DIQGDDF</strong></p>
<p><strong>DIQGDDT</strong></p>
<p><strong>DIQGDDU</strong></p>
<p><strong>DIQGQ</strong></p>
<p><strong>DIQGU</strong></p>
<p><strong>DIQGU0</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DIQQ</strong></p>
<p><strong>DIQQ1</strong></p>
<p><strong>DIQQQ</strong></p></td>
<td></td>
<td>Routines that provide help on various subjects.</td>
</tr>
<tr class="odd">
<td><p><strong>DIR</strong></p>
<p><strong>DIR0</strong></p>
<p><strong>DIR01</strong></p>
<p><strong>DIR02</strong></p>
<p><strong>DIR03</strong></p>
<p><strong>DIR0H</strong></p>
<p><strong>DIR0K</strong></p>
<p><strong>DIR0W</strong></p>
<p><strong>DIR1</strong></p>
<p><strong>DIR2</strong></p>
<p><strong>DIR3</strong></p>
<p><strong>DIRQ</strong></p></td>
<td>DIR</td>
<td>Routines responsible for the standard reader used in VA
FileMan.</td>
</tr>
<tr class="even">
<td><strong>DIRCR</strong></td>
<td>XY^%RCR</td>
<td>Routine that moves arrays. <em>Must</em> be stored in the Manager
account as <strong>%RCR</strong>.</td>
</tr>
<tr class="odd">
<td><strong>DIS</strong></td>
<td>EN^DIS</td>
<td>Routines responsible for the Search File Entries option.</td>
</tr>
<tr class="even">
<td><p><strong>DIS0</strong></p>
<p><strong>DIS1</strong></p>
<p><strong>DIS2</strong></p>
<p><strong>DIS3</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DISZ*</strong></td>
<td></td>
<td>Temporary routines compiled for SORT templates and deleted after use
(<em>not</em> exported with VA FileMan routines).</td>
</tr>
<tr class="even">
<td><p><strong>DIT</strong></p>
<p><strong>DIT0</strong></p>
<p><strong>DIT1</strong></p>
<p><strong>DIT2</strong></p>
<p><strong>DIT3</strong></p>
<p><strong>DITP</strong></p>
<p><strong>DITR</strong></p>
<p><strong>DITR1</strong></p></td>
<td></td>
<td>Routines responsible for the Transfer Entries option. Also used by
the Compare/Merge option and by <strong>DIFROM</strong>.</td>
</tr>
<tr class="odd">
<td><p><strong>DITC</strong></p>
<p><strong>DITC0</strong></p>
<p><strong>DITC1</strong></p>
<p><strong>DITC2</strong></p>
<p><strong>DITC3</strong></p></td>
<td></td>
<td>Routines responsible for allowing a user to select data values
during the compare/merge process.</td>
</tr>
<tr class="even">
<td><p><strong>DITCP</strong></p>
<p><strong>DITCP0</strong></p>
<p><strong>DITCPL</strong></p></td>
<td></td>
<td>Routines enabling comparison of data and data dictionaries across
environments.</td>
</tr>
<tr class="odd">
<td><strong>DITIME</strong></td>
<td></td>
<td>Input Transform for “TIME” Data Type.</td>
</tr>
<tr class="even">
<td><p><strong>DITM</strong></p>
<p><strong>DITM1</strong></p>
<p><strong>DITM2</strong></p>
<p><strong>DITMGM1</strong></p>
<p><strong>DITMGM2</strong></p>
<p><strong>DITMGM2A</strong></p>
<p><strong>DITMGM2B</strong></p>
<p><strong>DITMGM2C</strong></p>
<p><strong>DITMGMRG</strong></p>
<p><strong>DITMGMRI</strong></p>
<p><strong>DITMU1</strong></p>
<p><strong>DITMU2</strong></p>
<p><strong>DITMU3</strong></p>
<p><strong>DITMU4</strong></p></td>
<td></td>
<td>Routines used to compare/merge two records located within a single
file.</td>
</tr>
<tr class="odd">
<td><strong>DITP</strong></td>
<td></td>
<td>Routine responsible for transferring pointers.</td>
</tr>
<tr class="even">
<td><p><strong>DIU</strong></p>
<p><strong>DIU0</strong></p>
<p><strong>DIU1</strong></p></td>
<td></td>
<td>Routines responsible for the Utility Functions option.</td>
</tr>
<tr class="odd">
<td><strong>DIU2</strong></td>
<td>EN^DIU2</td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>DIU20</strong></p>
<p><strong>DIU21</strong></p>
<p><strong>DIU3</strong></p>
<p><strong>DIU31</strong></p>
<p><strong>DIU4</strong></p>
<p><strong>DIU5</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIUCANON</strong></td>
<td></td>
<td>Routine containing utilities for Canonic Templates.</td>
</tr>
<tr class="even">
<td><strong>DIUTC</strong></td>
<td>$$UTC^DIUTC</td>
<td>Routine to convert a VA FileMan date/time into Coordinated Universal
Time (UTC).</td>
</tr>
<tr class="odd">
<td><strong>DIUTL</strong></td>
<td></td>
<td>General utility routines used internally by VA FileMan.</td>
</tr>
<tr class="even">
<td><p><strong>DIV</strong></p>
<p><strong>DIVC</strong></p>
<p><strong>DIVR</strong></p>
<p><strong>DIVR1</strong></p>
<p><strong>DIVU</strong></p></td>
<td></td>
<td>Routines that verify field data.</td>
</tr>
<tr class="odd">
<td><p><strong>DIVRE</strong></p>
<p><strong>DIVRE1</strong></p></td>
<td></td>
<td>Routine that checks for required field data.</td>
</tr>
<tr class="even">
<td><strong>DIVRPTR</strong></td>
<td>DIVRPTR</td>
<td>Routine called from programmer mode to check pointers.</td>
</tr>
<tr class="odd">
<td><strong>DIWE</strong></td>
<td>EN^DIWE</td>
<td>Routines responsible for VA FileMan’s Line Editor and display of
word processing output. They also provide for use of Alternate
Editors.</td>
</tr>
<tr class="even">
<td><p><strong>DIWE1</strong></p>
<p><strong>DIWE11</strong></p>
<p><strong>DIWE12</strong></p>
<p><strong>DIWE2</strong></p>
<p><strong>DIWE3</strong></p>
<p><strong>DIWE4</strong></p>
<p><strong>DIWE5</strong></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>DIWF</strong></td>
<td><p>DIWF</p>
<p>EN1^DIWF</p>
<p>EN2^DIWF</p></td>
<td>Routine used for printing forms.</td>
</tr>
<tr class="even">
<td><p><strong>DIWP</strong></p>
<p><strong>DIWW</strong></p></td>
<td><p>DIWP</p>
<p>DIWW</p></td>
<td>Routines responsible for display of word processing output.</td>
</tr>
<tr class="odd">
<td><p><strong>DIX</strong></p>
<p><strong>DIXC</strong></p></td>
<td></td>
<td><p>Routines used for the Statistics option.</p>
<p>Routine used for the Descriptive Statistics option.</p></td>
</tr>
<tr class="even">
<td><p><strong>DMSQ</strong></p>
<p><strong>DMSQD</strong></p>
<p><strong>DMSQE</strong></p>
<p><strong>DMSQF</strong></p>
<p><strong>DMSQF1</strong></p>
<p><strong>DMSQF2</strong></p>
<p><strong>DMSQP</strong></p>
<p><strong>DMSQP1</strong></p>
<p><strong>DMSQP2</strong></p>
<p><strong>DMSQP3</strong></p>
<p><strong>DMSQP4</strong></p>
<p><strong>DMSQP5</strong></p>
<p><strong>DMSQP6</strong></p>
<p><strong>DMSQS</strong></p>
<p><strong>DMSQT</strong></p>
<p><strong>DMSQT1</strong></p>
<p><strong>DMSQU</strong></p></td>
<td></td>
<td>Routines used to build and maintain an SQL mapping to VA FileMan
data. Allows access to VA FileMan data using an SQL interface.</td>
</tr>
</tbody>
</table>

<span id="_Toc108021518" class="anchor"></span>Table : INDEX (#.11)
File—Cross-References

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
details on all VA FileMan callable routines/entry points/APIs, see the
*VA FileMan Developer’s Guide*.

## Direct Mode Utilities

In addition to the callable entry points shown in <u>Table 5</u>, there
are a few other entry points into VA FileMan routines. Unlike the
callable entry points, these entries ***cannot be used within
application programs***. Only users with programmer access can invoke
the following direct mode utilities from the M prompt:

- **C^DI**

- **D^DI**

- **P^DI**

- **Q^DI**

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on these direct mode utilities, see the “^DI: Programmer
Access” section in the “Developer Tools” section in the *VA FileMan
Developer’s Guide*.

## ScreenMan-Specific Utilities

The following are ScreenMan-specific utilities:

- ^DDGF

- CLONE^DDS

- PRINT^DDS

- RESET^DDS

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on these ScreenMan-specific utilities, see the “Programmer
Mode Utilities” section in the “ScreenMan Forms” section in the
“ScreenMan” section in the *VA FileMan Developer’s Guide*.

## Mapping Routines

No VA FileMan-specific routine mapping actions are needed in the VA
environment.

## Direct Mode VA FileMan

The exported menu structure of VA FileMan is displayed in <u>Figure
3</u>.

The following options are accessible from the MUMPS command prompt using
the calls described in Section <u>4.2</u>, “<u>Direct Mode
Utilities</u>:”

- Enter or Edit File Entries

- Print File Entries

- Search File Entries

- Modify File Attributes

- Inquire To File Entries

Utility Functions:

- Verify Fields

- Cross-Reference A Field or File

- Identifier

- Re-Index File

- Input Transform (Syntax)

- Edit File

- Output Transform

- Template Edit

- Uneditable Data

- Mandatory/Required Field Check

- Key Definition

Other Options:

- Filegrams:

<!-- -->

- Create/Edit Filegram Template

- Display Filegram Template

- Generate Filegram

- View Filegram

- Specifiers

- Install/Verify Filegram

<!-- -->

- Archiving:

<!-- -->

- Select Entries to Archive

- Add/Delete Selected Entries

- Print Selected Entries

- Create Filegram Archiving Template

- Write Entries to Temporary Storage

- Move Archived Data to Permanent Storage

- Purge Stored Entries

- Cancel Archival Selection

- Find Archived Entries

<!-- -->

- Auditing:

<!-- -->

- Fields Being Audited

- MONITOR A USER

- Purge Data Audits

- Purge DD Audits

- Turn Data Audit On/Off

<!-- -->

- ScreenMan:

<!-- -->

- Edit/Create a Form

- Run a Form

- Delete a Form

- Purge Unused Blocks

- PRINT A FORM

- CUSTOMIZE COLORS

- CLONE A FORM

<!-- -->

- Statistics:

<!-- -->

- Descriptive Statistics

- Scattergram

- Histogram

<!-- -->

- Extract Data to FileMan File:

<!-- -->

- Select Entries to Extract

- Add/Delete Selected Entries

- Print Selected Entries

- Modify Destination File

- Create Extract Template

- Update Destination File

- Purge Extracted Entries

- Cancel Extract Selection

- Validate Extract Template

<!-- -->

- Data Export To Foreign Format:

<!-- -->

- Define Foreign File Format

- Select Fields For Export

- Create Export Template

- Export Data

- Print Format Documentation

<!-- -->

- Import Data

- Browser

- DATA ACCESS CONTROL:

<!-- -->

- SET UP APPLICATION ACTIONS

- EDIT/CREATE AN ACTION POLICY

- TEST A POLICY

- DISABLE A POLICY

- DELETE A POLICY

- PRINT ACTIONS/POLICIES

- POLICY FUNCTIONS

<!-- -->

- DATA TYPE OPTIONS:

<!-- -->

- ENTER OR EDIT DATA TYPE FILE

- ENTER OR EDIT DATA TYPE METHOD FILE

- ENTER OR EDIT DATA TYPE PROPERTY FILE

<!-- -->

- DATA MAPPING:

<!-- -->

- ENTER/EDIT AN ENTITY

- GENERATE AN ENTITY FOR A FILE

- PRINT AN ENTITY

DATA DICTIONARY UTILITIES:

- LIST FILE ATTRIBUTES

- mAP POINTER RELATIONS

- CHECK/FIX DD STRUCTURE

- FIND POINTERS INTO A FILE

- UPDATE THE META DATA DICTIONARY

TRANSFER ENTRIES:

- TRANSFER FILE ENTRIES

- COMPARE/MERGE FILE ENTRIES

- NAMESPACE COMPARE

## VA FileMan Options

VA FileMan exports the options listed in <u>Figure 3</u>. They are
installed during the KIDS install. The top-level **VA FileMan**
\[DIUSER\] menu option can be found on Kernel’s EVE menu. The top-level
menu option, DMSQ MENU, is *not* attached to any other existing menu; it
is standalone and can be assigned as needed.

<span id="_Ref343690295" class="anchor"></span>Figure : VA FileMan
Exported Options Diagrams

VA FileMan (DIUSER)

\*\*ENTRY ACTION:

W !!?10,"VA FileMan Version "\_^DD("VERSION")

\|

\|

--------------------------------------------------------- Enter or Edit

File Entries

\[DIEDIT\]

\*\*ENTRY ACTION:

D ^DIB

--------------------------------------------------------- Print File

Entries

\[DIPRINT\]

\*\*ENTRY ACTION:

D ^DIP

--------------------------------------------------------- Search File

Entries

\[DISEARCH\]

\*\*ENTRY ACTION:

D ^DIS

--------------------------------------------------------- Modify File

Attributes

\[DIMODIFY\]

\*\*ENTRY ACTION:

D ^DICATT

--------------------------------------------------------- Inquire to
File

Entries

\[DIINQUIRE\]

\*\*ENTRY ACTION:

D INQ^DII

----- Utility ------------------------------------------- Verify Fields

Functions \[DIVERIFY\]

\[DIUTILITY\] \*\*ENTRY ACTION:

\| S DI=1 G EN^DIU

\|

\|---------------------------------------------- Cross-Reference

\| A Field \[DIXREF\]

\| \*\*ENTRY ACTION:

\| S DI=2 G EN^DIU

\|

\|---------------------------------------------- Identifier

\| \[DIIDENT\]

\| \*\*ENTRY ACTION:

\| S DI=3 G EN^DIU

\|

\|---------------------------------------------- Re-Index File

\| \[DIRDEX\]

\| \*\*ENTRY ACTION:

\| S DI=4 G EN^DIU

\|

\|---------------------------------------------- Input Transform

\| (Syntax)

\| \[DIITRAN\]

\| \*\*ENTRY ACTION:

\| Q:DUZ(0)'="@" S

\| DI=5 G EN^DIU

\|

\|---------------------------------------------- Edit File

\| \[DIEDFILE\]

\| \*\*ENTRY ACTION:

\| S DI=6 G EN^DIU

\|

\|---------------------------------------------- Output Transform

\| \[DIOTRAN\]

\| \*\*ENTRY ACTION:

\| S DI=7 G EN^DIU

\|

\|---------------------------------------------- Template Edit

\| \[DITEMP\]

\| \*\*ENTRY ACTION:

\| S DI=8 G EN^DIU

\|

\|---------------------------------------------- Uneditable Data

\| \[DIUNEDIT\]

\| \*\*ENTRY ACTION:

\| S DI=9 G EN^DIU

\|

\|---------------------------------------------- Mandatory/Requir

\| ed Field Check

\| \[DIFIELD CHECK\]

\| \*\*ENTRY ACTION:

\| S DI=10 G EN^DIU

\|

\|---------------------------------------------- Key Definition

\[DIKEY\]

\*\*ENTRY ACTION:

S DI=11 D EN^DIU

----- Data Dictionary ----------------------------------- List File

Utilities \[DI Attributes

DDU\] \[DILIST\]

\| \*\*ENTRY ACTION:

\| D ^DID

\|

\|---------------------------------------------- Map Pointer

\| Relations \[DI

\| DDMAP\]

\|

\|---------------------------------------------- Check/Fix DD

\| Structure \[DI

\| DDUCHK\]

\|

\|---------------------------------------------- Find Pointers

\| into a File \[DDU

\| FIND POINTERS

\| INTO A FILE\]

\|

\|---------------------------------------------- Update the META

Data Dictionary

\[DDU UPDATE META

DD\]

--------------------------------------------------------- Transfer
Entries

\[DITRANSFER\]

\*\*ENTRY ACTION:

D ^DIT

Other Options (DIOTHER)

\|

\|

----- Filegrams \[DIFG\] ---------------------- Create/Edit Filegram
Template

\*\*LOCKED: XUFILEGRAM\*\* \[DIFG CREATE\]

\| \*\*LOCKED: XUFILEGRAM\*\*

\|

\|---------------------------------- Display Filegram Template

\| \[DIFG DISPLAY\]

\| \*\*LOCKED: XUFILEGRAM\*\*

\|

\|---------------------------------- Generate Filegram \[DIFG

\| GENERATE\]

\| \*\*LOCKED: XUFILEGRAM\*\*

\|

\|---------------------------------- View Filegram \[DIFG VIEW\]

\|

\|---------------------------------- Specifiers \[DIFG SPECIFIERS\]

\| \*\*LOCKED: XUFILEGRAM\*\*

\|

\|---------------------------------- Install/Verify Filegram \[DIFG

INSTALL\]

\*\*LOCKED: XUFILEGRAM\*\*

----- Audit Menu \[DIAUDIT\] ------------------ Fields Being Audited

\*\*LOCKED: XUAUDITING\*\* \[DIAUDITED FIELDS\]

\|

\|---------------------------------- Monitor a User \[DIAUDIT

\| MONITOR USER\]

\|

\|---------------------------------- Purge Data Audits \[DIAUDIT

\| PURGE DATA\]

\|

\|---------------------------------- Purge DD Audits \[DIAUDIT PURGE

\| DD\]

\|

\|---------------------------------- Turn Data Audit On/Off

\| \[DIAUDIT TURN ON/OFF\]

\|

\|---------------------------------- Show Past Changes To Data

Dictionaries \[DIAUDIT SHOW

PAST CHG TO DDs\]

----- ScreenMan \[DDS SCREEN MENU\] ----------- Edit/Create a Form \[DDS

\*\*LOCKED: XUSCREENMAN\*\* EDIT/CREATE A FORM\]

\|

\|---------------------------------- Run a Form \[DDS RUN A FORM\]

\|

\|---------------------------------- Delete a Form \[DDS DELETE A

\| FORM\]

\|

\|---------------------------------- Purge Unused Blocks \[DDS PURGE

\| UNUSED BLOCKS\]

\|

\|---------------------------------- Print a Form \[DDS PRINT A

\| FORM\]

\|

\|---------------------------------- Customize Colors \[DDS

\| CUSTOMIZE COLORS\]

\|

\|---------------------------------- Clone a Form \[DDS CLONE A

FORM\]

--------------------------------------------- Statistics
\[DISTATISTICS\]

----- VA FileMan Management \[DI MGMT -------- Data Dictionary

MENU\] Cross-reference

\*\*LOCKED: XUMGR\*\* Compile/Uncompile \[DI DD

\| COMPILE\]

\|

\|---------------------------------- Input Template

\| Compile/Uncompile \[DI INPUT

\| COMPILE\]

\|

\|---------------------------------- Print Template

\| Compile/Uncompile \[DI PRINT

\| COMPILE\]

\|

\|---------------------------------- Sort Template

\| Compile/Uncompile \[DI SORT

\| COMPILE\]

\|

\|---------------------------------- Re-Initialize VA FileMan \[DI

\| REINITIALIZE\]

\|

\|---------------------------------- Set Type of Mumps Operating

\| System \[DI SET MUMPS OS\]

\|

\|---------------------------------- Forms Print \[DIWF\]

----- Data Export to Foreign Format --------- Define Foreign File Format

\[DDXP EXPORT MENU\] \[DDXP DEFINE FORMAT\]

\| \*\*LOCKED: DDXP-DEFINE\*\*

\|

\|---------------------------------- Select Fields for Export \[DDXP

\| SELECT EXPORT FIELDS\]

\|

\|---------------------------------- Create Export Template \[DDXP

\| CREATE EXPORT TEMPLATE\]

\|

\|---------------------------------- Export Data \[DDXP EXPORT DATA\]

\|

\|---------------------------------- Print Format Documentation

\[DDXP FORMAT DOCUMENTATION\]

----- Extract Data To Fileman File ---------- Select Entries to Extract

\[DIAX EXTRACT MENU\] \[DIAX SELECT\]

\*\*LOCKED: DIEXTRACT\*\* \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Add/Delete Selected Entries

\| \[DIAX ADD/DELETE\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Print Selected Entries \[DIAX

\| PRINT\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Modify Destination File \[DIAX

\| MODIFY\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Create Extract Template \[DIAX

\| CREATE\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Update Destination File \[DIAX

\| UPDATE\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Cancel Extract Selection \[DIAX

\| CANCEL\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Purge Extracted Entries \[DIAX

\| PURGE\]

\| \*\*LOCKED: DIEXTRACT\*\*

\|

\|---------------------------------- Validate Extract Template

\[DIAX VALIDATE\]

\*\*LOCKED: DIEXTRACT\*\*

--------------------------------------------- Import Data \[DDMP
IMPORT\]

--------------------------------------------- Browser \[DDBROWSER\]

----- Data Access Control \[DIACCESS\] -------- Set Up Application
Actions

\| \[DIAC ACTIONS\]

\|

\|---------------------------------- Edit/Create an Action Policy

\| \[DIAC EDIT\]

\|

\|---------------------------------- Test a Policy \[DIAC TEST\]

\|

\|---------------------------------- Disable a Policy \[DIAC

\| DISABLE\]

\|

\|---------------------------------- Delete a Policy \[DIAC DELETE\]

\|

\|---------------------------------- Print Actions/Policies \[DIAC

\| PRINT\]

\|

\|---------------------------------- Policy Functions \[DIAC

FUNCTIONS\]

----- Data Mapping \[DDE ENTITY -------------- Enter/Edit an Entity
\[DDE ENTITY

MAPPING\] ENTER/EDIT\]

\|

\|---------------------------------- Print an Entity \[DDE ENTITY

\| INQUIRE\]

\|

\|---------------------------------- Generate an Entity for a File

\[DDE AUTO GEN ENTITY FOR A DD

\#\]

SQLI (VA FileMan) (DMSQ MENU)

\|

\|

------------------------------------------RUN Regenerate SQLI Projection

\[DMSQ PROJECT\]

\*\*LOCKED: XUPROGMODE\*\*

------------------------------------------WHY Find Out SQLI Status
\[DMSQ

DIAGNOSTICS\]

------------------------------------------ERR Print Errors from Last

Projection \[DMSQ PRINT ERRORS\]

--------------------------------------------X Purge SQLI Data \[DMSQ
PURGE\]

\*\*LOCKED: XUPROGMODE\*\*

---DD Table Statistics Reports \[DMSQ -----DD1 Field Listing by File
(Brief)

TS MENU\] \[DMSQ TS FIELDS BRIEF\]

\|

\|-------------------------------DD2 Field Listing by File (Full)

\| \[DMSQ TS FIELDS FULL\]

\|

\|-------------------------------IN1 List Subfile Links (Brief)

\| \[DMSQ TS SUBFILE BRIEF\]

\|

\|-------------------------------IN2 List Incoming Pointer/Subfile

\| Links (Full) \[DMSQ TS PTR

\| SUBFILE FULL\]

\|

\|------------------------------OUT1 List Pointer and Parent Links

\| (Brief) \[DMSQ TS PTR PARENT

\| BRIEF\]

\|

\|------------------------------OUT2 List Pointer and Parent Links

\| (Full) \[DMSQ TS PTR PARENT

\| FULL\]

\|

\|------------------------------CNT1 Pointer Statistics by

\| Individual Table \[DMSQ TS PTR

\| STATS\]

\|

\|------------------------------CNT2 Pointer Statistics (Summary)

\| \[DMSQ TS PTR STATS SUMMARY\]

\|

\|------------------------------NAME Table Name Listing (VA FileMan

vs. SQLI) \[DMSQ TS NAMES\]

-CNTS Site Statistics Reports \[DMSQ ------TBL Table Total (Excluding
Index

PS MENU\] Tables) \[DMSQ PS TOTAL TABLES\]

\|

\|--------------------------------1C Column Total (All Tables)

\| \[DMSQ PS TOTAL COLUMNS\]

\|

\|------------------------------INDX Index Table Total \[DMSQ PS

\| TOTAL INDEXES\]

\|

\|------------------------------ELEM Table Element Totals, By Type

\| \[DMSQ PS TOTAL TABLE ELEMENTS\]

\|

\|--------------------------------2C Column Totals, by Table \[DMSQ

\| PS TOTAL TABLE COLS\]

\|

\|--------------------------------3C Column Totals, by Table

\| (Ordered by \# of Columns)

\| \[DMSQ PS TOTAL TABLE COLS A\]

\|

\|--------------------------------4C Columns in Regular Tables

\| Total \[DMSQ PS TOTAL COLUMNS

\| REG\]

\|

\|------------------------------FLDS Columns in Regular Tables,

\| Excluding ID Columns \[DMSQ PS

\| COLUMNS REG NOID\]

\|

\|-------------------------------DOM Columns by Domain \[DMSQ PS

COLUMNS BY DOMAIN\]

------------------------------------------GRP Suggest Table Groupings
\[DMSQ

SUGGEST TABLE GROUPINGS\]

# Cross-References

This section contains a description of the MUMPS-type cross-references
that exist on fields in VA FileMan files. There are no bulletin or
trigger cross-references in these files. All other cross-references are
regular types used for lookup or sorting, or both.

The cross-references are grouped by file. The field affected is
identified along with the cross-reference’s name (or subscript location
if there is no name) and a brief description. Many of these
cross-references are described in more detail in the data dictionaries.
Standard “B” cross-references are not shown. New-Style Indexes are
identified by as asterisk (\*). No Regular cross-references are shown
for the SQLI files (1.521-1.52192).

## INDEX (#.11) File

| Field (Subfile: Field)                   | X-Ref ID | Description                                                                                                                                                                                         |
|------------------------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ROOT FILE                                | **AC**   | VA FileMan finds indexes defined on fields from a particular file.                                                                                                                                  |
| FILE, NAME                               | **BB\*** | The BB index, on the key of the INDEX (#.11) file, lets VA FileMan test potential key values for uniqueness. It is a regular compound index with two fields, the **.01** (FILE) and **.02** (NAME). |
| NAME                                     | **IX\*** | This “Regular” index on the NAME (#.02) field allows users to select an index by its name.                                                                                                          |
| CROSS-REFERENCE VALUES: SUBSCRIPT NUMBER | **AC\*** | VA FileMan finds cross reference values by subscript.                                                                                                                                               |
| CROSS-REFERENCE VALUES: ORDER NUMBER     | **BB\*** | The uniqueness index of the CROSS-REFERENCE VALUES Multiple field of the INDEX (#.11) file.                                                                                                         |
| CROSS-REFERENCE VALUES: FILE, FIELD      | **F**    | The **F** index is a whole file compound cross-reference on two fields in the CROSS-REFERENCE VALUES Multiple: FILE (#2) and FIELD (#3).                                                            |

<span id="_Toc108021519" class="anchor"></span>Table : KEY (#.31)
File—Cross-References

## KEY (#.31) File

| Field                               | X-Ref ID    | Description                                                                                                                                                                                                                                                                                       |
|-------------------------------------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FILE, PRIORITY                      | **AP\***    | VA FileMan determines the primary key of a file.                                                                                                                                                                                                                                                  |
| UNIQUENESS INDEX                    | **AU\***    | VA FileMan determines whether an index is a uniqueness index for a key.                                                                                                                                                                                                                           |
| FILE, NAME                          | **BB\***    | The **BB** index, the uniqueness index for the Key file's key, lets VA FileMan test potential key values for uniqueness. It is a regular compound index with two fields, the **.01** (File) and **.02** (Key Name).                                                                               |
| FIELD: FIELD                        | **Trigger** | The FILE (.01) of the parent record is triggered into FILE (.02) when FIELD (.01) is edited.                                                                                                                                                                                                      |
| FIELD: FIELD, FILE                  | **BB\***    | The **BB** index, on the key of the FIELDS Multiple of the KEY (#.31) file, allows VA FileMan to test potential key values for uniqueness. It is a regular compound index with two fields.                                                                                                        |
| FIELD: FILE, FIELD                  | **F\***     | The **F** index, a whole file compound cross-reference on the key of the FIELDS Multiple of the KEY (#.31) file, allows VA FileMan to determine the keys of which a field is part. This is essential for identifying the key value uniqueness tests that must be done when a field value changes. |
| FIELD: SEQUENCE NUMBER, FIELD, FILE | **S\***     | The **S** index, a compound index on all fields of the FIELDS Multiple of the KEY (#.31) file, allows VA FileMan to step through the key fields in sequence. This is essential for prompting, returning values, as well as for the generation of each key's uniqueness index.                     |

<span id="_Toc108021520" class="anchor"></span>Table : PRINT TEMPLATE
(#.4) File—Cross-References

## PRINT TEMPLATE (#.4) File

<table>
<caption><p><span id="_Toc108021521" class="anchor"></span>Table : SORT
TEMPLATE (#.401) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>NAME</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all PRINT templates
associated with a particular file.</td>
</tr>
<tr class="even">
<td></td>
<td><strong>AF</strong></td>
<td><p>This cross-reference sets up an “<strong>AF</strong>”
cross-reference node for each field in a compiled PRINT template. The
cross-reference has the form:</p>
<p>^DIPT(“AF”,file#,field#,print template#)=““</p></td>
</tr>
<tr class="odd">
<td>FILE</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all PRINT templates
associated with a particular file.</td>
</tr>
<tr class="even">
<td>TEMPLATE TYPE</td>
<td><strong>FG</strong></td>
<td>This cross-reference is used to do a quick lookup of FILEGRAM-type
of PRINT templates.</td>
</tr>
<tr class="odd">
<td></td>
<td><strong>EX</strong></td>
<td>This cross-reference is used to do a quick lookup of EXTRACT-type
PRINT templates.</td>
</tr>
<tr class="even">
<td>CANONIC FOR THIS FILE</td>
<td><strong>CANONIC</strong></td>
<td><p>This cross-reference is used to identify files that have a
Canonic Print Template assigned. The structure of the cross-reference
is:</p>
<p><strong>^DIPT("CANONIC", File#, IEN)</strong></p>
<p>Where <strong>File#</strong> identifies the file that has a Canonic
PRINT template and IEN is the internal entry number of the Canonic PRINT
template assigned to that file.</p></td>
</tr>
</tbody>
</table>

<span id="_Toc108021521" class="anchor"></span>Table : SORT TEMPLATE
(#.401) File—Cross-References

## SORT TEMPLATE (#.401) File

<table>
<caption><p><span id="_Toc108021522" class="anchor"></span>Table : INPUT
TEMPLATE (#.402) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>NAME</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all SORT templates
associated with a particular file.</td>
</tr>
<tr class="even">
<td>FILE</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all SORT templates
associated with a particular file.</td>
</tr>
<tr class="odd">
<td>CANONIC FOR THIS FILE</td>
<td><strong>CANONIC</strong></td>
<td><p>This cross-reference is used to identify files that have a
Canonic Sort Template assigned. The structure of the cross-reference
is:</p>
<p><strong>^DIBT("CANONIC", File#, IEN)</strong></p>
<p>Where <strong>File#</strong> identifies the file that has a Canonic
SORT template and IEN is the internal entry number of the Canonic SORT
template assigned to that file.</p></td>
</tr>
</tbody>
</table>

<span id="_Toc108021522" class="anchor"></span>Table : INPUT TEMPLATE
(#.402) File—Cross-References

## INPUT TEMPLATE (#.402) File

<table>
<caption><p><span id="_Toc108021523" class="anchor"></span>Table : FORM
(#.403) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>NAME</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all INPUT templates
associated with a particular file.</td>
</tr>
<tr class="even">
<td></td>
<td><strong>AF</strong></td>
<td><p>This cross-reference sets up an “<strong>AF</strong>”
cross-reference node for each field in a compiled INPUT template. The
cross-reference has the form:</p>
<p><strong>^DIE(“AF”,file#,field#,input template#)=“”</strong></p></td>
</tr>
<tr class="odd">
<td>FILE</td>
<td><strong>F_file#</strong></td>
<td>This cross-reference is used to quickly find all INPUT templates
associated with a particular file.</td>
</tr>
<tr class="even">
<td>CANONIC FOR THIS FILE</td>
<td><strong>CANONIC</strong></td>
<td><p>This cross-reference is used to identify files that have a
Canonic Edit Template assigned. The structure of the cross-reference
is:</p>
<p><strong>^DIE(“CANONIC”, File#, IEN)</strong></p>
<p>Where <strong>File#</strong> identifies the file that has a Canonic
EDIT template and IEN is the internal entry number of the Canonic EDIT
template assigned to that file.</p></td>
</tr>
</tbody>
</table>

<span id="_Toc108021523" class="anchor"></span>Table : FORM (#.403)
File—Cross-References

## FORM (#.403) File

<table>
<caption><p><span id="_Toc108021524" class="anchor"></span>Table : BLOCK
(#.404) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>NAME</td>
<td><strong>F1</strong></td>
<td>This cross-reference is used to quickly find all ScreenMan forms
associated with a particular file.</td>
</tr>
<tr class="even">
<td></td>
<td><strong>AY</strong></td>
<td>This cross-reference merely documents the existence of data stored
under <strong>^DIST(.403,form IEN,“AY”)</strong>. This is where the
compiled data for a form is stored.</td>
</tr>
<tr class="odd">
<td>PAGE NAME<br />
(subfield of PAGE Multiple)</td>
<td><strong>C</strong></td>
<td>This cross-reference stores the PAGE NAME converted to uppercase
characters.</td>
</tr>
<tr class="even">
<td>PRIMARY FILE</td>
<td><strong>F</strong></td>
<td>This cross-reference is used to quickly find all ScreenMan forms
associated with a particular file.</td>
</tr>
<tr class="odd">
<td>PAGE: IS THIS A POP UP PAGE?</td>
<td></td>
<td>This MUMPS cross-references ensures that no Header block is present
if it is a pop-up page.</td>
</tr>
<tr class="even">
<td>PAGE: HEADER BLOCK</td>
<td><strong>AC</strong></td>
<td>This cross-reference ensures that no header block, next page, or
previous page is associated with a pop-up page.</td>
</tr>
<tr class="odd">
<td>PAGE: BLOCK: BLOCK NAME</td>
<td><strong>AB</strong></td>
<td>This cross-reference facilitates identifying the Forms on which a
Block is used.</td>
</tr>
<tr class="even">
<td>PAGE: BLOCK: BLOCK ORDER</td>
<td><strong>AC</strong></td>
<td>This cross-reference ensures that Block Order Numbers are unique
within a page.</td>
</tr>
</tbody>
</table>

<span id="_Toc108021524" class="anchor"></span>Table : BLOCK (#.404)
File—Cross-References

## BLOCK (#.404) File

<table>
<caption><p><span id="_Toc108021525" class="anchor"></span>Table :
FOREIGN FORMAT (#.44) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>CAPTION<br />
(subfield of FIELD Multiple)</td>
<td><strong>C</strong></td>
<td>This cross-reference is used for lookup of fields by CAPTION. It is
also used for ^-jumping.</td>
</tr>
<tr class="even">
<td>UNIQUE NAME<br />
(subfield of FIELD Multiple)</td>
<td><strong>D</strong></td>
<td>This cross-reference stores the UNIQUE NAME converted to uppercase
characters.</td>
</tr>
</tbody>
</table>

<span id="_Toc108021525" class="anchor"></span>Table : FOREIGN FORMAT
(#.44) File—Cross-References

## FOREIGN FORMAT (#.44) File

| Field                                        | X-Ref ID | Description                                                                      |
|----------------------------------------------|----------|----------------------------------------------------------------------------------|
| OTHER NAME FOR FORMAT: OTHER NAME FOR FORMAT | **C**    | This cross-reference allows look-ups for formats based on OTHER NAME FOR FORMAT. |

<span id="_Toc108021526" class="anchor"></span>Table : IMPORT TEMPLATE
(#.46) File—Cross-References

## IMPORT TEMPLATE (#.46) File

| Field        | X-Ref ID | Description                                                                               |
|--------------|----------|-------------------------------------------------------------------------------------------|
| NAME         | **F1**   | Creates an index under **F_file#** that is used for lookup when the file number is known. |
| PRIMARY FILE | **F**    | Same as **F1**.                                                                           |

<span id="_Toc108021527" class="anchor"></span>Table : DD AUDIT (#.6)
File—Cross-References

## DD AUDIT (#.6) File

| Field        | X-Ref ID | Description                                                             |
|--------------|----------|-------------------------------------------------------------------------|
| DATE UPDATED | **D**    | A regular cross-reference supporting lookups on the DATE UPDATED field. |
| USER         | **E**    | A regular cross-reference supporting lookups on the USER field.         |

<span id="_Toc108021528" class="anchor"></span>Table : DATA TYPE (#.81)
File—Cross-References

## DATA TYPE (#.81) File

| Field                   | X-Ref ID | Description                                                                        |
|-------------------------|----------|------------------------------------------------------------------------------------|
| INTERNAL REPRESENTATION | **C**    | A regular cross-reference supporting lookups on the INTERNAL REPRESENTATION field. |

<span id="_Toc108021529" class="anchor"></span>Table : COMPILED ROUTINE
(#.83) File—Cross-References

## COMPILED ROUTINE (#.83) File

| Field  | X-Ref ID | Description                                                                                                                                                   |
|--------|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| IN USE | **C**    | This cross-reference is used to control when a routine number is available for use in creating a compiled sort routine, during the FileMan sort/print option. |

<span id="_Toc108021530" class="anchor"></span>Table : LANGUAGE (#.85)
File—Cross-References

## LANGUAGE (#.85) File

| Field                          | X-Ref ID | Description                                                                                |
|--------------------------------|----------|--------------------------------------------------------------------------------------------|
| TWO LETTER CODE                | **C**    | Regular new style index on two letter language codes                                       |
| THREE LETTER CODE              | **D**    | Regular new-style index for three letter abbreviations for languages                       |
| ALTERNATE THREE LETTER CODE    | **E**    | This adds entries to the **D** index for the three-letter code a la the mnemonic style.    |
| ALTERNATE NAME: ALTERNATE NAME | **F**    | Whole file cross-reference for ALTERNATE NAME Multiple allowing look-up by ALTERNATE NAME. |

<span id="_Toc108021531" class="anchor"></span>Table : META DATA
DICTIONARY (#.9) File—Cross-References

## META DATA DICTIONARY (#.9) File

<table>
<caption><p><span id="_Toc108021532" class="anchor"></span>Table : FILE
(#1) of Files—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>DATA DICTIONARY NUMBER</td>
<td><strong>AFF</strong></td>
<td><p>The <strong>AFF</strong> cross-reference is a multi-field MUMPS
cross-reference based on the DATA DICTIONARY NUMBER and FIELD NUMBER
fields. It stores data into the same location as the
<strong>AFF2</strong> cross-reference on the FIELD NUMBER field. Its
structure is:</p>
<p><strong>^DDD(“AFF”,file_number,field_number,IEN)</strong></p></td>
</tr>
<tr class="even">
<td>FIELD NUMBER</td>
<td><strong>AFF2</strong></td>
<td><p>The <strong>AFF2</strong> cross-reference is a multi-field MUMPS
cross-reference based on the DATA DICTIONARY NUMBER and FIELD NUMBER
fields. It stores data into the same location as the
<strong>AFF</strong> cross-reference on the DATA DICTIONARY NUMBER
field. Its structure is:</p>
<p><strong>^DDD(“AFF”,file_number,field_number,IEN)</strong></p></td>
</tr>
<tr class="odd">
<td>LOOKUP TERM</td>
<td><strong>C</strong></td>
<td>The <strong>C</strong> cross-reference is a regular cross-reference
on the LOOKUP TERM field, supporting lookups on field labels.</td>
</tr>
</tbody>
</table>

<span id="_Toc108021532" class="anchor"></span>Table : FILE (#1) of
Files—Cross-References

## FILE (#1) of Files

<table>
<caption><p><span id="_Toc108021533" class="anchor"></span>Table : AUDIT
(#1.1) File—Cross-References</p></caption>
<colgroup>
<col style="width: 26%" />
<col style="width: 13%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>X-Ref ID</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>NAME</td>
<td><strong>AD</strong></td>
<td><p>This cross-reference sets and kills the “<strong>GL</strong>”
node for the file. This node has the form:</p>
<p><strong>^DIC(file#,0,”GL”)=file’s global location</strong></p></td>
</tr>
<tr class="even">
<td></td>
<td><strong>AE</strong></td>
<td><p>This cross-reference sets and kills the “<strong>NM</strong>”
node for the file. This node has the form:</p>
<p><strong>^DIC(file#,0,”NM”)=file’s name</strong></p></td>
</tr>
<tr class="odd">
<td>APPLICATION GROUP: APPLICATION GROUP</td>
<td><strong>AC</strong></td>
<td>This whole file cross-reference allows file look-ups by Application
Group (Package).</td>
</tr>
<tr class="even">
<td>TRANSLATION: TRANSLATION</td>
<td><strong>ALANG</strong></td>
<td><p>This cross-reference facilitates checking if a particular
language has a translation of the file name. Its structure is:</p>
<p><strong>^DIC(“ALANAG”_LanguageFileIEN,Translation,FileNumber)</strong></p></td>
</tr>
</tbody>
</table>

<span id="_Toc108021533" class="anchor"></span>Table : AUDIT (#1.1)
File—Cross-References

## AUDIT (#1.1) File

| Field              | X-Ref ID | Description                                                             |
|--------------------|----------|-------------------------------------------------------------------------|
| DATE/TIME RECORDED | **C**    | The cross-reference allows looking up an Audit record by date and time. |
| USER               | **D**    | The cross-reference allows looking up an Audit record by user.          |

<span id="_Toc108021534" class="anchor"></span>Table : ARCHIVAL ACTIVITY
(#1.11) File—Cross-References

## ARCHIVAL ACTIVITY (#1.11) File

| Field | X-Ref ID | Description                                                     |
|-------|----------|-----------------------------------------------------------------|
| FILE  | **C**    | This cross-reference allows looking up an Archive by File name. |

<span id="_Ref526166676" class="anchor"></span>Table : ENTITY (#1.5)
File—Cross-References

## ENTITY (#1.5) File

| Field                      | X-Ref ID | Description                                                                                                                                |
|----------------------------|----------|--------------------------------------------------------------------------------------------------------------------------------------------|
| ENTITY (#.08)              | **AD**   | The cross-reference allows looking up an ENTITY record for Input Transform, to look back up the tree and ensure item is *not* an ancestor. |
| NAME (#.01)                | **B**    | The cross-reference allows looking up an ENTITY record by name.                                                                            |
| NUMBER (#.02)              | **F**    | The cross-reference allows finding entities by primary file number.                                                                        |
| DISPLAY NAME (#.1)         | **FHIR** | Compound cross-reference. Retrieves FHIR entities by display name and file number.                                                         |
| DEFAULT FILE NUMBER (#.02) |          |                                                                                                                                            |
| DISPLAY NAME (#.1)         | **SDA**  | Compound cross-reference. Retrieves SDA entities by display name and file number.                                                          |
| DEFAULT FILE NUMBER (#.02) |          |                                                                                                                                            |

<span id="_Toc108021536" class="anchor"></span>Table :
SQLI_TABLE_ELEMENT (#1.5216) File—Cross-References

## SQLI_TABLE_ELEMENT (#1.5216) File

| Field   | X-Ref ID | Description                      |
|---------|----------|----------------------------------|
| E_TABLE | **G**    | Table element by table, by name. |
| E_TYPE  | **F**    | Table element by table, by type. |

<span id="_Toc108021537" class="anchor"></span>Table : SQLI_COLUMN
(#1.5217) File—Cross-References

## SQLI_COLUMN (#1.5217) File

| Field   | X-Ref ID | Description                                        |
|---------|----------|----------------------------------------------------|
| C_FIELD | **D**    | Column by VA FileMan file number, by field number. |

<span id="_Toc108021538" class="anchor"></span>Table : SQLI_PRIMARY_KEY
(#1.5218) File—Cross-References

## SQLI_PRIMARY_KEY (#1.5218) File

| Field      | X-Ref ID | Description                        |
|------------|----------|------------------------------------|
| P_SEQUENCE | **C**    | Primary key by table, by sequence. |

<span id="_Ref514251199" class="anchor"></span>Table : Package-Wide
Variables

# Archiving and Purging

## Archiving

There are no package-specific archiving procedures in VA FileMan.

The generic archiving tool for VistA is a part of VA FileMan. It is
described in the *VA FileMan Advanced User Manual*.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on archiving, see the “Archiving” section in the VA *FileMan
Advanced User Manual*.

The Extract Tool provides a means of archiving data into a VA FileMan
file. It is also described in the *VA FileMan Advanced User Manual*.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For more
information on the Extract Tool, see the “Extract Tool” section in the
“Archiving” section in the VA *FileMan Advanced User Manual*.

## Purging

Within VA FileMan, the only files that might grow large enough to
require purging of data are the audit files:

- AUDIT (#1.1)

- DD AUDIT (#.6)

These files capture information about changes to data and to data
dictionaries, respectively. The user audit is started and stopped by
using the Monitor a User option on the Auditing submenu. Starting with
VA FileMan 22.2, the data dictionary audit will always be on. The amount
of data accumulated is dependent both on the scope of the audit and its
duration. Options are available to purge the AUDIT (#1.1) (Purge Data
Audits) and the DD AUDIT (#.6) file (Purge DD Audits). Purging the audit
files is optional. Decisions to purge *must* be made based on the size
of the files and any need to retain the audit data.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
instructions on the use of the Auditing options, see the “Auditing”
section in the VA *FileMan Advanced User Manual*.

The Purge Stored Entries option on the Archiving submenu removes the
data archived from the primary file and from the ARCHIVAL ACTIVITY
(#1.11) file when the archiving process is complete. The Purge Stored
Entries option should be run when each archiving action is finished in
order to remove the archived data and clean up the files.

The Purge Extracted Entries option on the Extract Tool submenu removes
extracted data from the primary file and from the ARCHIVAL ACTIVITY
(#1.11) file when the extract process is complete. This option should be
run when using the Extract Tool for archiving purposes to remove
extracted data.

# External Relationships

As distributed with a Kernel Installation and Distribution System (KIDS)
build, VA FileMan 22.2 is dependent on a pre-existing installation of
Kernel. The VA FileMan 22.2 Installation Guide does not describe how to
install VA FileMan without the Kernel. In other words, a so-called
standalone installation is not explicitly supported. However, almost all
of the functionality of VA FileMan can be implemented without Kernel by
installing the VA FileMan 22.2 routines and running **^DINIT**.
Describing how to accomplish a standalone install is beyond the scope of
this documentation set.

VA FileMan must be installed on a system running an implementation of
ANSI Standard M. The KIDS distribution described here assumes
installation on a Caché system. Information in the MUMPS OPERATING
SYSTEM (#.07) file and Kernel-supplied **%ZOSF** nodes is used to
perform functions that are operating-system dependent. Operating Systems
other than Caché can be accommodated based on entries in the MUMPS
OPERATING SYSTEM (#.07) file. Again, processes for running VA FileMan on
operating systems other than Caché are beyond the scope of these
documents.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
details of installing VA FileMan, see the *VA FileMan 22.2 Installation
Guide.*

Although not part of VA FileMan, the Kernel’s PACKAGE (#9.4) file *must*
be present on your system to use the DIFROM routines to export software
packages. The Package file installation is *not* included in this
distribution of VA FileMan 22.2

<img src="images/media/image3.png"
style="width:0.44444in;height:0.44444in" alt="Caution" /> CAUTION: The
Kernel Installation and Distribution System (KIDS) replaced the use of
DIFROM as the method of exporting software packages in the VA. The
version of DIFROM released with VA FileMan 22.2 will transport the new
Key and Index structures.

VA FileMan’s capability is augmented when it is installed with Kernel
and MailMan. Specifically, VA FileMan 22.2 is designed to work with
Kernel 8.0 or later. For example, the following additional functionality
is available when VA FileMan is installed with Kernel:

- User security via the NEW PERSON (#200) file

- Control of file access

- More sophisticated menu presentation

- Device control

- Queuing

The following additional functionality is available when VA FileMan is
installed with MailMan:

- Bulletins, one of VA FileMan’s cross-references, become operational
  when MailMan is installed to deliver the messages.

- Filegram options also require MailMan.

Kernel allows networking two CPUs with different operating systems.
Kernel provides this ability by retrieving the type of operating system
from **^%ZOSF(“OS”)**. This global does *not* have to be replicated or
translated; thus, a separate copy of the global can be stored on each
CPU. When running standalone VA FileMan, the type of operating system is
retrieved either from the second piece of **^%ZOSF(“OS”)**, if the
**DINZMGR** was run, or from **^DD(“OS”)**. **^DD(“OS”)** is the global
location of the MUMPS OPERATING SYSTEM (#.7) file. The **^DD** global
*must* always be either replicated or translated across systems. In any
case, VA FileMan uses the local **DISYS** variable to store the value of
the current operating system. VA FileMan finds some operating
system-specific code in nodes descending from **^DD(“OS”,DISYS)**; other
code is found in **^%ZOSF** nodes.

VA FileMan exports options and security keys with the **DI** and **DD**
namespace for use by Kernel.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:**
Throughout the VA FileMan manuals, specific reference is made to Kernel
or MailMan when either is needed for a function to work.

## DBA Approvals and Database Integration Control Registrations (ICRs)

The Database Administrator (DBA) maintains a list of Integration Control
Registrations (ICRs) or mutual agreements between software developers
allowing the use of internal entry points or other software-specific
features that are *not* available to the general programming public.

### ICRs—Current List for VA FileMan as Custodian

To obtain the current list of ICRs, if any, to which the VA FileMan
software (DI) is a custodian, perform the following procedures:

1.  Sign onto the **FORUM** system (forum.va.gov).

<!-- -->

1.  Go to the **DBA** menu \[DBA\].

2.  Select the **Integration Agreements Menu** option \[DBA IA ISC\].

3.  Select the **Custodial Package Menu** option \[DBA IA CUSTODIAL
    > MENU\].

4.  Choose the A**CTIVE by Custodial Package** option \[DBA IA
    > CUSTODIAL\].

5.  When this option prompts you for a package, enter **VA FILEMAN** or
    > **DI**.

6.  All current ICRs to which the VA FileMan software is a custodian are
    > listed.

### ICRs—Detailed Information

To obtain detailed information on a specific integration control
registration, perform the following procedures:

1.  Sign onto the **FORUM** system (forum.va.gov).

<!-- -->

7.  Go to the **DBA** menu \[DBA\].

8.  Select the **Integration Agreements Menu** option \[DBA IA ISC\].

9.  Select the **Inquire** option \[DBA IA INQUIRY\].

10. When prompted for “INTEGRATION REFERENCES,” enter the specific
    > integration control registrations number of the ICR you would like
    > to display.

11. The option then lists the full text of the ICR you requested.

### ICRs—Current List for VA FileMan as Subscriber

To obtain the current list of ICRs, if any, to which the VA FileMan
software (DI) is a subscriber, perform the following procedures:

1.  Sign onto the **FORUM** system (forum.va.gov).

<!-- -->

12. Go to the **DBA** menu \[DBA\].

13. Select the **Integration Agreements Menu** option \[DBA IA ISC\].

14. Select the **Subscriber Package Menu** option \[DBA IA SUBSCRIBER
    > MENU\].

15. Choose the **Print ACTIVE by Subscribing Package** option \[DBA IA
    > SUBSCRIBER\].

16. When prompted with “START WITH SUBSCRIBING PACKAGE,” enter **VA
    > FILEMAN** (uppercase). When prompted with “GO TO SUBSCRIBING
    > PACKAGE,” enter **VA FILEMAN** (uppercase).

17. All current ICRs to which the VA FileMan software is a subscriber
    > are listed.

# Internal Relationships

All options can be independently invoked.

None of the options require any special setup in order to run
successfully.

# Package-Wide Variables

VA FileMan package-wide or key variables that can be assumed to be
defined at all times are listed in <u>Table 27</u>:

| Variable        | Description                                                                               |
|-----------------|-------------------------------------------------------------------------------------------|
| **DUZ**         | The internal entry number from the NEW PERSON (#200) file.                                |
| **DUZ(0)**      | The variable defining the user’s access.                                                  |
| **DUZ(“LANG”)** | If running Kernel 8.0 or later, this variable refers to the language of the current user. |
| **DT**          | The current date in VA FileMan internal format.                                           |
| **DTIME**       | The integer value of the number of seconds the user has to respond to a timed read.       |
| **U**           | The up-arrow (caret).                                                                     |

<span id="_Ref514251240" class="anchor"></span>Table : Package-Wide
Variables—DISY (Special Meaning)

In addition, the variable in <u>Table 28</u> has a special meaning for
VA FileMan although it is *not* always defined:

| Variable  | Description                                                                                                                                                                                  |
|-----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **DISYS** | The current M operating system—pointer to the MUMPS OPERATING SYSTEM (#.7) file contained in the first piece of **^DD(“OS”)** and, if using Kernel, in the second piece of **^%ZOSF(“OS”)**. |

<span id="_Toc108021541" class="anchor"></span>Table : List of Variables
VA FileMan is Exempted from KILLing

## Standards and Conventions (SAC) Exemptions

Beginning January 1, 1995, VA FileMan has been granted exemptions from
the following standards by the Programming Standards and Conventions
Committee (SACC).

### STANDARD SECTION: 4B–Package-wide variables

Beginning December 22, 1994, VA FileMan is exempted from **KILL**ing the
listed variables in the following calls:

| Supported Reference | Variables                   |
|---------------------|-----------------------------|
| DIC                 | **DA**                      |
| FILE^DICN           | **DA**                      |
| DIE                 | **%,D,D0,DI,DQ,X,D1,%X,%Y** |
| DIK                 | **%,DA,DIC, X, Y**          |
| EN1^DIP             | **X**                       |
| EN^DIQ1             | **%,D0,I,J,X,Y,C**          |

<span id="_Ref345487626" class="anchor"></span>Table : VA FileMan
Security Keys

### STANDARD SECTION: 6D–FM compatibility

- The following globals are exempt from VA FileMan compatibility:

<!-- -->

- **^DISV**

- **^DOSV**

<!-- -->

- VA FileMan may set a *non*-VA FileMan compatible node
  \[e.g., **^XXX(File#, IEN,-9)**\] to record information about archival
  activity and may set *non*-VA FileMan compatible nodes **^(3)** and
  **^(2)** to store old and new values of any audited field.

# Globals

VA FileMan’s globals are listed below:

- **^DD**

- **^DDD**

- **^DDA**

- **^DDE**

- **^DI**

- **^DIA**

- **^DIAR**

- **^DIBT**

- **^DIC**

- **^DIE**

- **^DIPT**

- **^DIST**

- **^DISV**

- **^DIT**

- **^DIZ**

- **^DMSQ**

- **^DOPT**

- **^DOSV**

- **^TMP**

- **^UTILITY**

- **^%ZOSF**

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For a
description of these globals, see <u>Table 3</u>.

The **^UTILITY** and **^TMP** globals are temporary globals used and
then **KILL**ed by many VA FileMan options. If VA FileMan is used with
Kernel, nodes in **^%ZOSF** are set up during Kernel’s installation.

There is a supported entry point to the **^DD** global: **^DD(“DD”)**.
Its use is explained in the “X ^DD(“DD”)—Another Way to Convert Dates”
section in the “Date/Time Utilities” section found in the “Classic
FileMan” section (listed by category) in the “Major APIs” section in the
*VA FileMan Developer’s Guide*.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
specific information on **^%DT**, see the “^%DT” section in the “Classic
FileMan API” section in the “Major APIs” section in the *VA FileMan
Developer’s Guide*.

**^DD(“VERSION”)** can be read to get the version number of the VA
FileMan package that exists in the system.

## Global Journaling, Translation, and Replication

No VA FileMan-specific actions are needed for global journaling,
translation, or replication in the VA environment.

# Security

VA FileMan (aka File Manager) is the database management system for
Veterans Health Information Systems and Technology Architecture (VistA).
As such, it provides security on a file, field, and template level. This
security is based on a string of characters stored in the **DUZ(0)**
local variable. You can find the details of the data security system
imposed by VA FileMan in the *VA FileMan Advanced User Manual*. The
security mechanisms described apply to the files and data sent with the
VA FileMan software as well as to the files created by other
applications and by users.

VA FileMan is a collection of routines written in MUMPS (M) that allow
the user the capability of reading and writing to files. The routines
are pre-written for users to access in creating APIs for access to data
in their "namespace". The modifications were all pertaining to these
routines and did *not* change the security boundary nor any methods of
access to the data that did *not* already exist under an authority to
operate (ATO) sustained by the Regions. VA FileMan experts extensively
tested and verified all fixes and ran existing utilities, such as
"**XINDEX**" to verify the validity of said routines.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For
specific information on VA FileMan’s data security, see the “Data
Security” section in the “Security” section in the *VA FileMan Advanced
User Manual*.

When used with Kernel, other types of access control are available. If
Kernel’s File Access Security system has been implemented on your
system, you can use it to control user access to files.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** Kernel’s
Sign-on/Security component is described in the *Kernel 8.0 and Kernel
Toolkit 7.3 Systems Management Guide*.

When you use VA FileMan within the Kernel’s menu system, you are subject
to the Kernel’s security requirements:

- You *must* enter correct Access and Verify codes.

- You can only use menus and options to which you have been granted
  access.

- You *must* have the proper security keys to use certain locked
  options.

Most VA FileMan options are accessed through the DIUSER menu. This menu
is usually located on the EVE menu distributed with Kernel.
SQLI-specific options are found on DMSQ menu.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **REF:** For a
diagram of the complete menu tree for VA FileMan, see <u>Figure 3</u> in
the “[VA FileMan Kernel Options](#va-fileman-options)” section.

## Security Management

This software was developed at the Department of Veterans Affairs (VA)
by employees of the Federal Government in the course of their official
duties. Pursuant to title 17 Section 105 of the United States Code this
software is *not* subject to copyright protection and is in the public
domain. VA assumes no responsibility whatsoever for its use by other
parties, and makes no guarantees, expressed or implied, about its
quality, reliability, or any other characteristic. We would appreciate
acknowledgement if the software is used. This software can be
redistributed and/or modified freely provided that any derivative works
bear some notice that they are derived from it, and any modified
versions bear some notice that they have been modified.

## Mail Groups and Alerts

VA FileMan does *not* make use of mail groups or alerts.

## Remote Systems

VA FileMan does *not* transmit data to any remote system, facility, or
database.

## Interfacing

No *non*-VA products are embedded in or required by VA FileMan, other
than those provided by the underlying operating systems.

## Electronic Signatures

Electronic signatures are *not* used within VA FileMan.

## Security Keys

VA FileMan options are locked with the security keys described in
<u>Table 30</u>. The security keys in the XU namespace are distributed
by Kernel; however, they lock VA FileMan options. The two remaining
security keys are distributed by VA FileMan and are installed when DINIT
is run:

| Security Key    | Description                                                                                                                                                                          |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **XUAUDITING**  | Use this security key to access the Auditing menu or to run any of the Auditing options.                                                                                             |
| **XUFILEGRAM**  | Use this security key to access the Filegram menu or to run any of the Filegram options; except the View Filegram option, for which no security key is required.                     |
| **XUMGR**       | Use this security key for users who act as site management staff. It is required in order to access the VA FileMan Management menu. It is also needed to access many Kernel options. |
| **XUPROGMODE**  | Use this security key to access the SQLI Regenerate SQLI Projection and Purge SQLI Data options.                                                                                     |
| **XUSCREENMAN** | Use this security key to access the ScreenMan menu.                                                                                                                                  |
| **DDXP-DEFINE** | Use this security key to access the Export Tool’s Define Foreign File Format option.                                                                                                 |
| **DIEXTRACT**   | Use this security key to access the Extract Data to FileMan File menu.                                                                                                               |

<span id="_Toc108021543" class="anchor"></span>Table : Glossary

## File Security

Files with numbers less than **two** (**2**) belong to VA FileMan. In
general, these files *cannot* be directly accessed. You can access them
only through the menu options. Those users who are granted programmer
access \[**DUZ(0)=“@”**\] can directly read and manipulate data in VA
FileMan files. However, it is *strongly recommended* that changes to
data in such files only be made through documented VA FileMan utilities.

## References

The following directive specifies that VA FileMan routines and files
should *not* be altered:

Veterans Health Administration (VHA) Directive 6402

## Official Policies

Modification of any part of the VA FileMan software is *not permitted*
as per VHA Directive 6402.

Distribution of the VA FileMan software is unrestricted (see the
“<u>Software Disclaimer</u>” section).

# Troubleshooting

For product support, contact the National Help Desk.

## How to Obtain Technical Information Online

Exported VistA M Server-based software file, routine, and global
documentation can be generated through the use of Kernel, MailMan, and
VA FileMan utilities.

<img src="images/media/image2.png"
style="width:0.29167in;height:0.3125in" alt="Note" /> **NOTE:** Methods
of obtaining specific technical information online are indicated where
applicable under the appropriate section.

## Help at Prompts

VistA M Server-based software provides online help and commonly used
system default prompts. Users are encouraged to enter question marks at
any response prompt. At the end of the help display, you are immediately
returned to the point from which you started. This is an easy way to
learn about any aspect of the software.

<span id="_Toc108021508" class="anchor"></span>Glossary

| Term                              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ANSI STANDARD MUMPS               | American National Standards Institute (ANSI) computer language used by VA FileMan. Also called M. The acronym MUMPS stands for Massachusetts General Hospital Utility Multiprogramming System.                                                                                                                                                                                                                                                                                                              |
| ARCHIVING                         | The storing of historical or little used data offline (often on tape).                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| AUDITING                          | The monitoring and recording of computer use. VA FileMan audits can log changes to data values in files and to the structure of the file itself.                                                                                                                                                                                                                                                                                                                                                            |
| BROWSER                           | An interactive application in VA FileMan that displays ASCII text on a terminal that supports a scroll region. The text can be in the form of a VA FileMan WORD-PROCESSING-type field or sequential local or global array. The user is allowed to navigate freely within the document.                                                                                                                                                                                                                      |
| CALLABLE ENTRY POINTS             | Places in a VA FileMan routine that can be called from an application program.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| CHECKSUM VALUE                    | A number computed for each routine in a package. The number is used to verify that the routine is uncorrupted and unchanged. Any coding change to a routine changes its checksum value.                                                                                                                                                                                                                                                                                                                     |
| CROSS-REFERENCE                   | In VA FileMan, an attribute of a field that identifies an action to take place when the value of the field is changed. Often, the action is the placement of the field’s value into an index. Beginning in Version 22.0 of VA FileMan, the INDEX file allows creation of indexes that contain more than one data field. Thus, they become an attribute of the file, rather than of a single field. The action described in the INDEX file entry happens when any of the involved fields is changed.         |
| DATA DICTIONARY                   | A data dictionary (DD) contains the definitions of a file’s elements (fields or data attributes), relationships to other files, and structure or design.                                                                                                                                                                                                                                                                                                                                                    |
| DATABASE MANAGEMENT SYSTEM        | A collection of software that handles the storage, retrieval and updating of records in a database.                                                                                                                                                                                                                                                                                                                                                                                                         |
| DBS                               | Database Server: An Application Programming Interface (API) for VA FileMan that updates the database in a non-interactive mode. VA FileMan passes information that needs to be displayed to the user to the calling routine in arrays.                                                                                                                                                                                                                                                                      |
| DBMS                              | Database Management System.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| DEVICE                            | A terminal, printer, modem or other type of hardware or equipment associated with a computer. A Host file of an underlying operating system may be treated like a device in that it can be written to (e.g., for spooling).                                                                                                                                                                                                                                                                                 |
| DHCP                              | The Decentralized Hospital Computer Program, see “VistA.”                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| DIRECT MODE UTILITY               | An entry point into a routine that can only be called from programmer mode, see “Callable Entry Points.”                                                                                                                                                                                                                                                                                                                                                                                                    |
| DSM FOR OPENVMS                   | The current name for **VAX DSM(V6)**. One of the M operating systems supported by VA FileMan.                                                                                                                                                                                                                                                                                                                                                                                                               |
| ENTRY                             | For VA FileMan, an instance of a file; a set of logically related data in a file; a record.                                                                                                                                                                                                                                                                                                                                                                                                                 |
| FIELD                             | In an entry, a specified area used for the value of a data attribute. The data specifications of each VA FileMan field are documented in the file’s data dictionary.                                                                                                                                                                                                                                                                                                                                        |
| FILE                              | A set of related records (or entries) treated as a unit.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| FILEGRAMS                         | A VA FileMan feature that stores file information in a sequential format in preparation for archiving or for sending it to a corresponding database in another computing location.                                                                                                                                                                                                                                                                                                                          |
| GLOBAL                            | In M, global may refer to a variable stored on disk (“global variable”) or the array to which the global variable may belong (“global array”).                                                                                                                                                                                                                                                                                                                                                              |
| HELP FRAMES                       | Online screens of documentation made possible by the Kernel’s Help Processor.                                                                                                                                                                                                                                                                                                                                                                                                                               |
| IMPLICITING                       | Term used by M/SQL operating system for global translation.                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| INIT                              | A step in the installation process that builds VA FileMan files from a set of routines (the “init routines”). Shortened form for “initialization.”                                                                                                                                                                                                                                                                                                                                                          |
| INDEX                             | A part of the data global whose subscripts are one or more fields from a single record in the file, along with the internal entry number (or numbers) that locate the record. An ordered list of all or a subset of the records in the file used to facilitate lookup and sorting.                                                                                                                                                                                                                          |
| INDEX FILE                        | This file was introduced with VA FileMan 22.0. Contains the information that describes an index on a file. Old-style index information is stored descendent from the description of the indexed field in the data dictionary. The INDEX file allows the creation of more complex indexes.                                                                                                                                                                                                                   |
| JOURNALING                        | The capturing of changes to files in order to facilitate the restoring of files from a known prior state.                                                                                                                                                                                                                                                                                                                                                                                                   |
| KERNEL                            | A set of VistA software utilities that function as an intermediary between the host operating system and VistA application packages (e.g., Laboratory, Pharmacy, IFCAP, etc.). Kernel provides a standard and consistent user and programmer interface between application packages and the underlying M implementation.                                                                                                                                                                                    |
| KEY                               | A group of one or more fields that together uniquely identifies a record in a file. Each key field *must* have a value, and fields that make up a key *must* in combination be unique for all records in the file. VA FileMan enforces key integrity.                                                                                                                                                                                                                                                       |
| KEY VARIABLE                      | See “Package-Wide Variable” below.                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **LAYGO** ACCESS                  | A user’s authorization to create a new entry when editing a computer file. **L**earn **A**s **Y**ou **GO**: the ability to create new entries.                                                                                                                                                                                                                                                                                                                                                              |
| MAILMAN                           | An electronic mail system (e-mail) that allows you to send messages to and receive them from other users via the computer. It is part of VistA.                                                                                                                                                                                                                                                                                                                                                             |
| MAPPING                           | See “Routine Mapping.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| OPERATING SYSTEM                  | A basic program that runs on the computer, controls the peripherals, allocates computing time to each user, and communicates with terminals. Some M implementations take over the functions of an operating system completely; others run on top of another host operating system.                                                                                                                                                                                                                          |
| PACKAGE                           | The set of programs, files, documentation, online help, and installation procedures required for a given software application package identified by a unique namespace. Elements include routines, files, and file entries from the OPTION, KEY, HELP FRAME, BULLETIN, FUNCTION, SORT TEMPLATE, PRINT TEMPLATE, INPUT TEMPLATE, FORM, and BLOCK files. Packages are transported using VA FileMan’s DIFROM routine, which creates initialization (init) routines to bundle the files and entries for export. |
| PACKAGE-WIDE VARIABLE             | For VistA, a variable that, for a particular application package, has a standard and documented meaning. Some package-wide variables may need to be defined at all times during package use. Also called Key Variable.                                                                                                                                                                                                                                                                                      |
| POINTER RELATIONSHIPS             | In VA FileMan, links between files that are created by use of the POINTER TO A FILE or VARIABLE-POINTER DATA TYPEs.                                                                                                                                                                                                                                                                                                                                                                                         |
| PROGRAMMER ACCESS                 | The ability to utilize VA FileMan features that are reserved for application developers. Referred to as “having the at-sign (**@**)”, because **@** is the **DUZ(0)** value that grants programmer access.                                                                                                                                                                                                                                                                                                  |
| PROGRAMMER MODE                   | Entry into VA FileMan directly from the M prompt instead of from Kernel’s menu system (e.g., by entering **D P^DI** at the M prompt).                                                                                                                                                                                                                                                                                                                                                                       |
| REPLICATION (OF GLOBALS)          | The practice of keeping and maintaining identical copies of the same global in different physical locations.                                                                                                                                                                                                                                                                                                                                                                                                |
| ROUTINE                           | A program or a sequence of instructions called by a program that may have some general or frequent use. M routines are groups of program lines that are saved, loaded, and called as a single unit via a specific name.                                                                                                                                                                                                                                                                                     |
| ROUTINE MAPPING                   | The placement of routines into main memory. Frequently used routines are mapped to reduce disk access and thereby increase efficiency.                                                                                                                                                                                                                                                                                                                                                                      |
| SAC EXEMPTION                     | An exception specifically granted by the Standards and Conventions Committee of the Programming Standards and Conventions requirements.                                                                                                                                                                                                                                                                                                                                                                     |
| SCREENMAN                         | A VA FileMan screen-oriented utility that supports creation, alteration, and presentation of screens for data editing and data display.                                                                                                                                                                                                                                                                                                                                                                     |
| SDP SPACE                         | Sequential Disk Processor space is an area on disk set aside for temporary storage of data during copying of the data. SDP is implemented by some M systems.                                                                                                                                                                                                                                                                                                                                                |
| SPACEBAR RETURN or SPACEBAR ENTER | The use of the key combination **\<Spacebar\>\<Return\>** or **\<Spacebar\>\<Enter\>** at a prompt. VA FileMan retrieves the user’s last response to that prompt.                                                                                                                                                                                                                                                                                                                                           |
| STANDALONE                        | Referring to VA FileMan, the use of VA FileMan without the complete Kernel. The rest of Kernel adds functionality; however, VA FileMan can be used alone.                                                                                                                                                                                                                                                                                                                                                   |
| TEMPLATE                          | A means of storing report formats, data entry formats, and sorted entry sequences. A template is a permanent place to store selected field specifications for use at a later time.                                                                                                                                                                                                                                                                                                                          |
| TRANSLATION (OF GLOBALS)          | The pointing to a physical disk storage location in another UCI for location of a global. Allows the same globals to be accessed from multiple UCIs.                                                                                                                                                                                                                                                                                                                                                        |
| VISTA                             | The Veterans Health Information Systems and Technology Architecture, within the Department of Veterans Affairs, is the component of the Veterans Health Administration that develops software and installs, maintains, and updates compatible computer systems in VA medical facilities. (Previously known as the Decentralized Hospital Computer Program \[DHCP\].)                                                                                                                                        |

<span id="_Toc108021509" class="anchor"></span>Index

^

^%ZOSF Global, xvi, 62, 66

^%ZOSF Node, 62

^DD Global, xvi, 65, 66

^DD(OS), 62

^DDA Global, xvi, 65

^DDD Global, xvi, 65

^DDE Global, xvi, 65

^DI Global, xvi, 66

^DIA Global, xvi, 66

^DIAR Global, xvi, 66

^DIBT Global, xvi, 66

^DIC Global, xvi, 66

^DIE Global, xvi, 66

^DIPT Global, xvi, 66

^DIST Global, xvi, 66

^DISV Global, xvi, 2, 65, 66

^DIT Global, 66

^DIZ Global, xvi, 66

^DMSQ Global, 66

^DOPT Global, xvi, 66

^DOSV Global, xvi, 2, 65, 66

^TMP Global, 66

^UTILITY Global, 66

A

ACTIVE by Custodial Package Option, 62

Alerts, 68

ALTERNATE EDITOR (#1.2) File, 6

APPLICATION ACTION (#1.61) File, 11

ARCHIVAL ACTIVITY (#1.11) File, 6, 58, 60, 61

Archiving, 60

Assumptions, xviii

AUDIT (#1.1) File, 6, 57, 60

B

BLOCK (#.404) File, 4, 54

BOOLEAN

SQLI DATA TYPE (#1.5211) File, 7

C

Callable Entry Points, 17

Callout Boxes, xiii

CHARACTER

SQLI DATA TYPE (#1.5211) File, 7

COMPILED ROUTINE (#.83) File, 5, 56

Conventions

Documentation, xii

Cross-references, 50

Custodial Package Menu, 62

D

Data Dictionary

Data Dictionary Utilities Menu, xvii

Listings, xvii

DATA TYPE (#.81) File, 5, 55

DATA TYPE METHOD (#.87) File, 5

DATA TYPE PROPERTY (#.86) File, 5

Database Server, 17

DATE

SQLI DATA TYPE (#1.5211) File, 7

DBA Approvals, 62

DBA IA CUSTODIAL MENU, 62

DBA IA CUSTODIAL Option, 62

DBA IA INQUIRY Option, 63

DBA IA ISC Menu, 62, 63

DBA IA SUBSCRIBER MENU, 63

DBA IA SUBSCRIBER Option, 63

DBA Menu, 62, 63

DD AUDIT (#.6) File, 4, 55, 60

DDE AUTO GEN ENTITY FOR A DD \# Option, ii

DDXP-DEFINE Security Key, 69

DESTINATION (#.2) File, 3

DEVICE (#3.5) File, 1

DI DDU Menu, xvii

DIALOG (#.84) File, 5, 10

DIEXTRACT Security Key, 69

DIFROM, 11

DILIST Option, xvii

DINIT Routine, xiv, xv, 1, 33, 68

DIPKINIT Routine, 11

Direct Mode Utilities, 38

Directives

VHA Directive 10-93-142, 17, 69

Disclaimers, xi

Software, xi, 68

DISYS Variable, 62, 64

DIUSER Menu, 43, 67

DMSQ MENU, 43

Documentation

Conventions, xii

Navigation, xiii

Symbols, xii

DT Variable, 64

DTIME Variable, 64

DUZ Variable, 64

DUZ(0) Variable, 64, 67

DUZ(LANG) Variable, 64

E

Electronic Signatures, 68

Enter or Edit File Entries Option, 27

ENTITY (#1.5) File, 6, 58

Entity Enter/Edit Option, ii

Entity Mapping Menu, ii

Entry Points, 17

EVE Menu, 43, 67

Exemptions

Standards and Conventions (SAC), 65

Export Tool, 69

Exported Options, 39

Exported PRINT Templates, 3

External Relationships, 61

Extract Tool, 60, 61

F

FILE (#1) File, 5, 19, 57

File Security, 69

Filegram, 62

FILEGRAM ERROR LOG (#1.13) File, 6

FILEGRAM HISTORY (#1.12) File, 6

FileMan

What is it?, ix

Files, 3

ALTERNATE EDITOR (#1.2), 6

APPLICATION ACTION (#1.61), 11

ARCHIVAL ACTIVITY (#1.11), 6, 58, 60, 61

AUDIT (#1.1), 6, 57, 60

BLOCK (#.404), 4, 54

COMPILED ROUTINE (#.83), 5, 56

DATA TYPE (#.81), 5, 55

DATA TYPE METHOD (#.87), 5

DATA TYPE PROPERTY (#.86), 5

DD AUDIT (#.6), 4, 55, 60

Description, 3

DESTINATION (#.2), 3

DEVICE (#3.5), 1

DIALOG (#.84), 5, 10

ENTITY (#1.5), 6, 58

FILE (#1), 5, 19, 57

FILEGRAM ERROR LOG (#1.13), 6

FILEGRAM HISTORY (#1.12), 6

FOREIGN FORMAT (#.44), 4, 55

FORM (#.403), 4, 54

FUNCTION (#.5), 4

IMPORT TEMPLATE (#.46), 4, 55

INDEX (#.11), 3, 50

INPUT TEMPLATE (#.402), 4, 53

KEY (#.31), 3, 51

LANGUAGE (#.85), 5, 56

Location, 3

META DATA DICTIONARY (#.9), 5, 56

MUMPS OPERATING SYSTEM (#.07), 61

MUMPS OPERATING SYSTEM (#.7), xiv, 4, 62, 64

NEW PERSON (#200), 61, 64

PACKAGE (#9.4), 11, 61

POLICY (#1.6), 10

POLICY FUNCTION (#1.62), 11

PRINT TEMPLATE (#.4), 3, 52

SORT TEMPLATE (#.401), 4, 53

SQLI_COLUMN (#1.5217), 9, 10, 59

SQLI_DATA_TYPE (#1.5211), 7

SQLI_DOMAIN (#1.5212), 7

SQLI_ERROR_LOG (#1.52192), 10

SQLI_ERROR_TEXT (#1.52191), 10

SQLI_FOREIGN_KEY (#1.5219), 10

SQLI_KEY_FORMAT (#1.5213), 8

SQLI_KEY_WORD (#1.52101), 6

SQLI_OUTPUT_FORMAT (#1.5214), 8

SQLI_PRIMARY_KEY (#1.5218), 9, 10, 59

SQLI_SCHEMA (#1.521), 6

SQLI_TABLE (#1.5215), 8

SQLI_TABLE_ELEMENT (#1.5216), 7, 8, 9, 10, 58

WORLD DAYLIGHT SAVINGS (#1.72), 11

WORLD TIMEZONES (#1.71), 11

FOREIGN FORMAT (#.44) File, 55

FOREIGN FORMAT (#.44)File, 4

FORM (#.403) File, 4, 54

FUNCTION (#.5) File, 4

G

Global Location, 3

Globals, 65

^%ZOSF, xvi, 62, 66

^DD, xvi, 65, 66

^DDA, xvi, 65

^DDD, xvi, 65

^DDE, xvi, 65

^DI, xvi, 66

^DIA, xvi, 66

^DIAR, xvi, 66

^DIBT, xvi, 66

^DIC, xvi, 66

^DIE, xvi, 66

^DIPT, xvi, 66

^DIST, xvi, 66

^DISV, xvi, 2, 65, 66

^DIT, 66

^DIZ, xvi, 66

^DMSQ, 66

^DOPT, xvi, 66

^DOSV, xvi, 2, 65, 66

^TMP, 66

^UTILITY, 66

H

Help

At Prompts, xvii, 70

Online, xvii, 70

Question Marks, xvii, 70

Home Pages

Adobe Website, xviii

VA Software Document Library (VDL) Website, xviii

How to

Obtain Technical Information Online, xvii, 70

Use this Manual, x

I

ICRs, 62

Implementation, 1

IMPORT TEMPLATE (#.46) File, 4, 55

INDEX (#.11) File, 3, 50

Initialization, 1

INPUT TEMPLATE (#.402) File, 4, 53

Inquire Option, 63

Inquire to File Entries Option, 31

Installing Standalone VA FileMan, 61

INTEGER

SQLI DATA TYPE (#1.5211) File, 7

Integration Agreements Menu, 62, 63

Integration Control Registrations (ICRs), 62

Current List for VA FileMan

Custodian, 62

Subscriber, 63

Detailed Information, 63

Intended Audience, x

Interfacing, 68

Internal Relationships, 63

Introduction, ix, 1

K

Kernel

KIDS, 1, 29

VA FileMan, 43

KEY (#.31) File, 3, 51

L

LANGUAGE (#.85) File, 5, 56

List File Attributes Option, xvii

M

Mail Groups, 68

Maintenance, 1

Management

Security, 68

Manuals

Reference, xviii

Mapping Routines, 39

MEMO

SQLI DATA TYPE (#1.5211) File, 7

Menu Structure, 39

Menus

Custodial Package Menu, 62

Data Dictionary Utilities, xvii

DBA, 62, 63

DBA IA CUSTODIAL MENU, 62

DBA IA ISC, 62, 63

DBA IA SUBSCRIBER MENU, 63

DI DDU, xvii

DIUSER, 43, 67

DMSQ MENU, 43

Entity Mapping, ii

EVE, 43, 67

Integration Agreements Menu, 62, 63

Subscriber Package Menu, 63

META DATA DICTIONARY (#.9) File, 5, 56

Modify File Attributes Option, 24, 25

MOMENT

SQLI DATA TYPE (#1.5211) File, 7

MUMPS OPERATING SYSTEM (#.07) File, 61

MUMPS OPERATING SYSTEM (#.7) File, xiv, 4, 62, 64

MUMPS-type Cross-references, 50

N

NEW PERSON (#200) File, 61, 64

New-Style Cross-references, 3

Nodes

^%ZOSF, 62

NUMERIC

SQLI DATA TYPE (#1.5211) File, 7

O

Official Policies, 69

Online

Documentation, xvii, 70

Technical Information, How to Obtain, xvii, 70

Options

ACTIVE by Custodial Package, 62

Custodial Package Menu, 62

Data Dictionary Utilities, xvii

DBA, 62, 63

DBA IA CUSTODIAL, 62

DBA IA CUSTODIAL MENU, 62

DBA IA INQUIRY, 63

DBA IA ISC, 62, 63

DBA IA SUBSCRIBER, 63

DBA IA SUBSCRIBER MENU, 63

DDE AUTO GEN ENTITY FOR A DD \#, ii

DI DDU, xvii

DILIST, xvii

DIUSER, 43, 67

DMSQ MENU, 43

Enter or Edit File Entries, 27

Entity Enter/Edit, ii

Entity Mapping, ii

EVE, 43, 67

Exported, 39

Inquire, 63

Inquire to File Entries, 31

Integration Agreements Menu, 62, 63

List File Attributes, xvii

Modify File Attributes, 24, 25

Print ACTIVE by Subscribing Package, 63

Search File Entries, 35

Standalone VA FileMan, 39

Subscriber Package Menu, 63

Orientation, x

P

PACKAGE (#9.4) File, 11, 61

Package-wide Variables, 64

Pointer Map, 12

Pointer Relationships, 12

POLICY (#1.6) File, 10

POLICY FUNCTION (#1.62) File, 11

PRIMARY_KEY

SQLI DATA TYPE (#1.5211) File, 7

Print ACTIVE by Subscribing Package Option, 63

PRINT TEMPLATE (#.4) File, 3, 52

PS Anonymous Directories, xix

Purging, 60

Q

Question Mark Help, xvii, 70

R

Reference Materials, xviii

References, 69

Relationships

External, 61

Internal, 63

Remote Systems, 68

Routines, 17

DINIT, xiv, xv, 1, 33, 68

DIPKINIT, 11

Mapping, 39

S

ScreenMan-Specific Utilities, 38

Search File Entries Option, 35

Security, 67

Security Keys, 68

DDXP-DEFINE, 69

DIEXTRACT, 69

XUAUDITING, 68

XUFILEGRAM, 68

XUMGR, 69

XUPROGMODE, 69

XUSCREENMAN, 69

Security Management, 68

Software Disclaimer, xi, 68

Software Product Security, 67

SORT TEMPLATE (#.401) File, 4, 53

SQLI DATA TYPE (#1.5211) File

BOOLEAN, 7

CHARACTER, 7

DATE, 7

INTEGER, 7

MEMO, 7

MOMENT, 7

NUMERIC, 7

PRIMARY_KEY, 7

TIME, 7

SQLI_COLUMN (#1.5217) File, 9, 10, 59

SQLI_DATA_TYPE (#1.5211) File, 7

SQLI_DOMAIN (#1.5212) File, 7

SQLI_ERROR_LOG (#1.52192) File, 10

SQLI_ERROR_TEXT (#1.52191) File, 10

SQLI_FOREIGN_KEY (#1.5219) File, 10

SQLI_KEY_FORMAT (#1.5213) File, 8

SQLI_KEY_WORD (#1.52101) File, 6

SQLI_OUTPUT_FORMAT (#1.5214) File, 8

SQLI_PRIMARY_KEY (#1.5218) File, 9, 10, 59

SQLI_SCHEMA (#1.521) File, 6

SQLI_TABLE (#1.5215) File, 8

SQLI_TABLE_ELEMENT (#1.5216) File, 7, 8, 9, 10, 58

Standalone VA FileMan

Options, 39

Standards and Conventions (SAC)

Exemptions, 65

Subscriber Package Menu, 63

Symbols

Found in the Documentation, xii

T

Templates

Exported PRINT, 3

TIME

SQLI DATA TYPE (#1.5211) File, 7

U

U Variable, 64

URLs

Adobe Website, xviii

VA Software Document Library (VDL) Website, xviii

Utilities

Direct Mode, 38

ScreenMan-Specific, 38

V

VA FileMan

What is it?, ix

VA FileMan with Kernel, 43

VA Software Document Library (VDL)

Website, xviii

Variables

DISYS, 62, 64

DT, 64

DTIME, 64

DUZ, 64

DUZ(0), 64, 67

DUZ(LANG), 64

Key, 64

Package-wide, 64

U, 64

VHA Directive 10-93-142, 3, 17, 69

W

Websites

Adobe Website, xviii

VA Software Document Library (VDL), xviii

What is VA FileMan?, ix

WORLD DAYLIGHT SAVINGS (#1.72) File, 11

WORLD TIMEZONES (#1.71) File, 11

X

XUAUDITING Security Key, 68

XUFILEGRAM Security Key, 68

XUMGR Security Key, 69

XUPROGMODE Security Key, 69

XUSCREENMAN Security Key, 69

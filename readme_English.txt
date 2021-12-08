===============================================================================
License Agreement
===============================================================================

The license agreement for this software (hereinafter referred to as the
SOFTWARE) is described as follows.

1. Intellectual property rights in the SOFTWARE shall remain in Fuji Xerox Co.,
   Ltd. (hereinafter referred to as Fuji Xerox) as well as the original
   copyright holders.

2. The SOFTWARE can only be used with compatible Fuji Xerox products
   (hereinafter referred to as the COMPATIBLE PRODUCTS) within the country of
   purchase of the COMPATIBLE PRODUCTS.

3. You are required to abide by the notes and restrictions (hereinafter referred
   to as the NOTES AND RESTRICTIONS) declared by Fuji Xerox while using the
   SOFTWARE.

4. You are not permitted to alter, modify, reverse engineer, decompile or
   disassemble the whole or any part of the SOFTWARE for the purpose of
   analyzing the SOFTWARE.

5. You are not permitted to distribute the SOFTWARE on a communication network,
   or transfer, sell, rent or license the SOFTWARE to any third party by
   duplicating the SOFTWARE on any media such as floppy disk or magnetic tape.

6. Fuji Xerox, Fuji Xerox Channel Partners, Authorized Dealers and the original
   copyright holders of the SOFTWARE shall not be liable for any loss or damage
   arising from matching of hardware or program that are not specified in the
   NOTES AND RESTRICTIONS of the SOFTWARE, or any modification to the SOFTWARE.

7. Fuji Xerox, Fuji Xerox Channel Partners, Authorized Dealers and the original
   copyright holders of the SOFTWARE shall not be responsible for any warranty
   or liability with respect to the SOFTWARE.

===============================================================================
PCL 6 Print Driver Ver.6.12.4 Additional Information
===============================================================================

This document provides information about the driver on the
following items:

1. Target Hardware Products
2. Requirements
3. General Comments
4. Limitations
5. Software Update

---------------------------------------------------
1. Target Hardware Products
---------------------------------------------------
FUJI XEROX ApeosPort-VII C7773
           ApeosPort-VII C6673
           ApeosPort-VII C5573
           ApeosPort-VII C4473
           ApeosPort-VII C3373
           ApeosPort-VII C3372
           ApeosPort-VII C2273
           DocuCentre-VII C7773
           DocuCentre-VII C6673
           DocuCentre-VII C5573
           DocuCentre-VII C4473
           DocuCentre-VII C3373
           DocuCentre-VII C3372
           DocuCentre-VII C2273

---------------------------------------------------
2. Requirements
---------------------------------------------------
Please note that this driver operates on a computer running on the following
operating system.

  Microsoft(R) Windows Server(R) 2008 x64 Editions
  Microsoft(R) Windows(R) 7 x64 Editions
  Microsoft(R) Windows Server(R) 2008 R2
  Microsoft(R) Windows Server(R) 2012
  Microsoft(R) Windows(R) 8.1 x64 Editions
  Microsoft(R) Windows Server(R) 2012 R2
  Microsoft(R) Windows(R) 10 x64 Editions
  Microsoft(R) Windows Server(R) 2016
  Microsoft(R) Windows Server(R) 2019

  Please visit our web site to check the latest software and supported
  operating systems.

---------------------------------------------------
3. General Comments
---------------------------------------------------
* Close all the running applications before installing the print driver.

* Always reboot the computer after installing an upgraded version of the print
  driver.

* If you have deleted an older version of the print driver, always reboot the
  computer before installing the new version.

* Some applications provide printing options pertaining to the number of copies
  and collated copies. Always select the printing options in the application
  unless the instructions specify otherwise. Use the print driver dialogs to
  select advanced options such as 2 Sided Print, Sample Set or options that
  are not available in the application.

* Always close the print driver dialogs and/or the application Print dialog box
  before you make any changes to the default settings of the print driver via
  the Control Panel.

* If your Job Offset output does not work well with the collated copies, you
  may try to deselect the [Collate] option in the application and check the
  [Collate] check box in the print driver.

* If a Fax Phonebook is not initialized or created by the current user, he/she
  may not be granted the authority to access it. For such inappropriate access
  by users, the driver will display an error message indicating that the default
  Fax Phonebook cannot be located or the specified Fax Phonebook cannot be
  recognized.
  On the other hand, if a user would like his/her Fax Phonebook to be accessed
  by other users, he/she has to specify the groups and users whose access
  he/she wants to allow, and must grant them at least the 'Change' permission
  to the Fax Phonebook data file.

* A fax job has to be sent separately to each recipient who is specified with 
  the F-code, Password or secure send attributes.
  Otherwise, the printer always disregards the F-code, Password and secure send
  attributes when sending a fax job to multiple recipients. The transmitted job
  is always printed directly at all specified destinations.

* For the installation through the networks, if you right-click
  on [Printer] folder, go to [Run as administrator] from the menu and select
  [Add printer...], printer icon may not be generated.

* Rename a Printer Icon should comply OS file naming convention. Use Symbols or
  special characters may incur renaming error or unexpected print driver
  behavior.

* Before installing a print driver in the Windows cluster environment, you need
  to install it on each node in the cluster.

---------------------------------------------------
4. Limitations
---------------------------------------------------
* Restrictions on Package-Aware Support Driver
  - The driver is not a Microsoft WHQL Certified Driver.
  For the above case in a Server-Client environment, when the printer driver
  is added or upgraded on the Server side, a dialog prompting user to install
  the printer driver or the User Account Control dialog may be displayed 
  on the Client side.

* About [Prioritize Application Specified Color when Output Color is Black & White]
  For print output that is consistent with color settings specified by application UI, set both
  [Print Using Application Specified Color] and [Prioritize Application Specified Color
  when Output Color is Black & White] to [On].

  The following describes the relationship between printer driver settings ([Output Color],
  [Print Using Application Specified Color], and [Prioritize Application Specified
  Color when Output Color is Black & White]) and print output.

  * [Print Using Application Specified Color]: [Off]
    Output Color specified by the application will be ignored, and driver UI's [Output Color]
    setting will be used for printing.

  * [Print Using Application Specified Color]: [On]
    - [Prioritize Application Specified Color when Output Color is Black & White]: [On]
      Output Color specified by the application will be used for printing.
      If no Output Color has been specified by the application, driver UI's [Output Color] setting
      will be used for printing.

    - [Prioritize Application Specified Color when Output Color is Black & White]: [Off]
      If driver UI's [Output Color] setting is [Color], Output Color specified by the application will
      be used for printing.
      If driver UI's [Output Color] setting is [Black and White], Output Color specified by the
      application will be ignored, and print output will be in black and white.
      If no Output Color has been specified by the application, driver UI's [Output Color] setting
      will be used for printing.

* On Microsoft Windows 7 or later versions select a printer from the [Devices
  and Printers] folder. Select Property of the printer and click the [Change
  Sharing Options] button on the [Sharing] tab.
  Then, specify Custom Paper Size.

* Default resolution of this driver is 600dpi. (Denoted by Auto.)
  When outputting through a driver, of which resolution is different from the
  one of this driver, errors such as the followings may be observed depending
  on specifications or limitations of an application.
  - Printed layout of the documents is changed.
  - Printed result of lines or patterns is changed.
  - Unnecessary lines are printed on the output.
  - Necessary lines are not printed on the output.

  In such case, the status may be improved by changing the settings of
  [Resolution] on the [Advanced] tab.

* When a printed pattern or diagram is different from what you see on the
  screen, changing the following settings may alleviate the problem.
  - Change the [Image Quality] setting on the [Color Options] tab.
  - Change the [Image Types] and the [Image Auto Correction] settings on the
    [Color Options] tab.
  - Set [High Speed Image Processing] on the [Advanced] tab to [Off].
  - Set [Draw the pattern with fine lines as per the resolution] on the
    [Advanced] tab to [On].
  - Change the [Resolution] setting in the [Image Options] group on the
    [Advanced] tab.
  - Change the [Halftone Print] setting in the [Image Options] group on the
    [Advanced] tab.

* Blank Separators
  If you set [EMF Spooling] to [Enabled] or specify Header, Footer and Watermark,
  and perform [2-Sided Print] with documents of odd number of pages, a blank page
  may be inserted on the last page depending on application or OS.

* The print layout may be changed when you change the [Image Quality] in the
  [Color Options] tab.

* Depending on the application, if the resolution of the driver is high, the
  size of the print data may become huge and printing cannot be done properly.
  When this happens, specify the following settings:
  - Specify the [Resolution] in the [Image Options] group in the [Advanced] tab
    to [300dpi] or [200dpi].

* For some applications, if a pasted image is printed at high resolution, the
  print data expands and may result in an extremely slow printing speed.
  The print data size of the output may be improved by changing the following
  settings of [Image Options] group on the [Advanced] tab.
  - Specify the [Image Compression] to [Standard] or [Photo] or [Resolution] to
    [300dpi] or [200dpi].

* When printing from the application of QuarkXPress 6.1E, if the [Image Quality]
  setting is [High Resolution] and the resolution of the driver is [1200dpi],
  the document may be printed as blank pages. This issue can be avoided by
  changing the resolution of the driver to [Auto].

* When doing a print job by specifying Paper Source as Auto, be sure to set
  Paper Size in the application to the Paper Size that the driver supports to
  enable the automatic paper feed feature.

* When using the Form Overlay feature, use form data of the same Paper Size,
  Resolution, and Image Settings as those of the document you want to print.
  If these settings are different between form data and the page where the form
  data is incorporated, expected print results may not be obtained.

* When using Form Overlay, as some applications paint the background in white
  to print, forms with overlay may be hidden. Such applications include
  Internet Explorer and WordPad.

* The print result may overlap if Pages Per Sheet (N-Up) and Margins [Standard]
  are selected when printing a document that has exceeded the print area of the
  print driver. When this happens, choose [None] of the [Margins] radio button
  group on the [Image Options] tab.

* When you cancel a fax job in progress from the driver, the application may
  display a warning dialog box. It may indicate a printer error message,
  although there is no error in the printer. In this case, ignore the warning
  message and continue operation.

* To use the [Store in Remote Folder] feature, you must obtain the be
  registered recipient's folder number and passcode in advance.
  Refer to the machine administrator guide on how to create a folder.

* Depending on the application used by the customer, blank pages for page
  adjustment will be inserted automatically according to the conditions like
  the number of copies specified when outputting 2-sided prints.
  In this case, the blank inserts will be included by the application.
  The performance may be improved by changing the setting below.
  - Check [Skip Blank Pages] on [Advanced] tab.

* Even with [Skip Blank Pages] selected, blank pages may still be printed in
  the following situations.
  - The page contains only line feeds.
  - The page contains only spaces.
  - The page contains only line feeds and spaces.
  - A white background drawing instruction is sent from the application.

* With Microsoft Word, even if [Skip Blank Pages] is specified, when a blank
  page is included in documents, it may be output.

* For customers using Microsoft Windows Server 2008 Cluster Environment

  <1> To specify custom paper size in a cluster environment, specify a common
      setting for all physical nodes in the cluster environment.

  <2> When [Search Printer] dialog box appears at the press of the [Get
      Information from Printer] button, enter the printer network address.

  <3> Deleting driver in cluster environment
      After the driver on the virtual server is deleted, delete the drivers
      on all standby nodes.
      ** Deleting driver from the standby node
        (1) Change the standby node to active node.
        (2) Install printer on virtual server.
        (3) Delete driver from virtual server.

  <4> Deleting driver
      After the printer icon is deleted, delete the driver from [Server
      Properties]. Then, restart the computer.

* [Cancel] button on [User Details Setup] Dialog
  For some applications, if [Enter User Details] dialog is cancelled when
  printing with the settings of [Prompt User for Entry when Submitting job] on
  [User Details Setup] dialog, a warning dialog may be displayed.
  This warning dialog may indicate a printer error, however, the printer
  actually has no problem.

  In that case, ignore the warning and continue.

* When [EMF Spooling] of [Advanced] tab is set to [Disabled], some documents
  with complex structure may have troubles such as distorted output image and
  failure of the output.

* To change the settings of Custom Paper Size, you need the Administrator
  access rights. On Windows Server 2008, select printer from the printer folder,
  right-click to go [Run as administrator] and select [Properties].
  After clicking [Continue] in [User Account Control], you can change
  the settings from Property.

  When Custom Paper Size equal to the standard paper size is specified in Paper
  Size, the print job may be performed as if a [standard] paper size was
  specified.
  To output as a Custom Paper Size, specify Custom Paper Size in Output Size.

* With the default settings of Firewall, data in cross-subnet broadcast cannot
  be retrieved.
  For cross-subnet data retrieval, please do not use broadcast and specify
  address directly.

* There are feature restrictions below on the execution of Fax print in
  Protected Mode of Microsoft Internet Explorer.
  - A warning message may be displayed right after the execution of Fax print.
  - The location for storage of Fax Phonebook is not a Public Folder, which is
    usually used for storage but a folder such as personal Folder, which can be
    used for file creation. Therefore, the contents of Fax Phonebook are
    different from the one registered with other applications.
  - Import To List feature of Fax Phonebook does not function.

* There is a restriction in creating file from Microsoft Internet Explorer.
  You cannot save form data file in the folder specified as the default in
  [Create / Register Forms]. Change the folder into one that can be used for
  creating file (such as "Document Folder") before creating/registering form
  data file.

* The following functions are restricted with use of Microsoft Internet Explorer
  in Protected Mode.
  - The setting items for [Job Type] ([Secure Print] / [Sample Set] /
    [Delayed Print] / [Store in Remote Folder]) can not be edited.
  - The functions of [Saved Settings], [Save] and [Edit] are disabled.
  - The functions of [Watermark], [New], [Edit] and [Delete] are disabled.
  - The setting of [Notify Job Completion by E-mail] can not be changed.
  To change the settings of these functions, open the default setting of
  the document from the Printer Folder.

* Notes and limitations about the server-client environment
- Server-Client Environment Issue (1)
  If the printer is being used as a shared printer and the server's operating
  system is being upgraded, a message indicating that the driver has to be
  updated may appear on the client, causing printing to fail.
  In this case, the print driver has to be reinstall on the client to be able
  to print again.

- Server-Client Environment Issue (2)
  In the Server-Client environment, after a print driver is added or upgraded
  on the Server side, printing may not be performed with a displayed message
  requiring print driver upgrade on the Client side.
  This problem can be avoided by the settings below.

  < Change of Group Policy Settings on Client PC >
  1. Log on as an Administrator on Client PC.
  2. Open command prompt and execute "gpedit.msc". to open [Local Group Policy
     Editor].
  3. Open the tree on the left side in the following order.
     [User Configuration]
     [Administrative Templates]
     [Control Panel]
     [Printers]
  4. Double-click [Point and Print Restrictions] in the right pane.
  5. Click the [Disabled] radio button.
  6. Click [OK] to close the window.
  7. Close [Local Group Policy Editor].

* Limitation on printing with the settings of Staple and Hole Punch at the same
  time
  Staple and Hole Punch may not function when 1 Staple and Hole Punch are
  specified at the same time for some paper sizes.

* Output Color Settings from Application
  To print in color from Application of Windows Store, open [Devices and Printers]
  from Windows Desktop, right-click on your printer to select [Printing Preferences]
  and then confirm that [Output Color] on the [Paper/Output] tab of the
  [Printing Preferences] dialog is set to [Color].
  If the setting of [Output Color] on the [Paper/Output] tab of the [Printing
  Preferences] dialog remains [Black and White], the output will be in black and
  white even if you specify Color Mode to [Color] on the printing setting screen
  shown after you select printer from the device charm.

* Limitations on Adobe Acrobat/Reader
  When you specify [2] or more pages for [Copies] on the [Print] dialog of
  Adobe Acrobat/Reader, Fax may not be transmitted normally.

* Microsoft Outlook
  When printing Schedule, the parts to be printed in color may appear printed
  in black and white with color missing.
  If color toner is used to make it look like gray-colored, the meter will
  count the job as a color printing.
 
  In such cases, the problem may be avoided with the following method.
  1. Close Outlook.
  2. Right-click the printer icon in [Devices and Printers], and open [Printing
     preferences].
  3. Click the [OK] button to close [Printing preferences].

  In the case of using shared printer icon, a new user of the shared printer
  may avoid the problem with the following method. (Only administrator is
  allowed to do.)
  1. Right-click the printer icon in [Devices and Printers] and open [Printer
     properties].
  2. Go to the [Advanced] tab and open [Printing Defaults].
  3. Click the [OK] button to close [Printing Defaults].
  4. Close [Printer properties].

* Limitation on printing with the setting of [Envelope] for [Paper Type]
  When printing with the setting of [Envelope] for [Paper Type] or [Type],
  the print job may not be performed correctly.
  To print on the paper of envelope types, open the [Advanced Paper
  Selection] dialog box, set [Paper Tray] to [Tray 5 (Bypass)] and then set
  [Bypass Paper Type] to [Envelope].

* Annotation and Watermark may not be printed even if [Annotation] and
  [Watermark] are specified.
  To make them function, set [EMF Spooling] to [Enabled] on the [Advanced] tab.

---------------------------------------------------
5. Software Update
---------------------------------------------------
    The latest software is available on our web site.

        https://www.fujixerox.com/

    Communication charges will be borne by the customer.

-------------------------------------------------------------------------------
Microsoft, Windows, Windows Server, Word, Excel, PowerPoint, Internet Explorer
and Visio are either registered trademarks or trademarks of Microsoft
Corporation in the United States and/or other countries.

Adobe, Acrobat and Reader are either registered trademarks or trademarks of
Adobe Systems Incorporated in the United States and/or other countries.

CentreWare is a registered trademark of Xerox Corporation.

Other company names and product names are trademarks or registered
trademarks of the respective companies.

libjpeg 6b
----------
This software is based in part on the work of the Independent JPEG Group.

(C) Fuji Xerox Co., Ltd. 2018-2020

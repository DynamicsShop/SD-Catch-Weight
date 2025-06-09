### 3.0.0

#### Enhancements

- AppSource App - The existing project code was converted from C/AL to AL.

- AppSource App - ISV Licensing was added.

- AppSource App - A change was made to the licence expiry notification. The logic for checking for expiry dates was reworked.

- AppSource App - The ISV About page was added.

- AppSource App - Permission sets were created.

- AppSource App - The Usage Category was added to the SD Catch Weight pages for the Tell Me search.

- AppSource App - Enhancements were made to the App Request Subscription page.

- AppSource App - Additional phrases were added as search phrases for the SD Catch Weight pages.

- AppSource App - The Item Ledger Entry table was extended to surface Units and the Item Units table was retired.

- AppSource App - Lot No, Expiration Date, and Item Category Code are now shown by default on the Item Ledger Entry List.

- AppSource App - Functionality was added to allow for modification of Units and Remaining Units on the Item Ledger Entry. Changes made are written to a Log table.

- AppSource App - The Catch Weight Units field and functionality was added to the Item Reclassification Journal.

- AppSource App - The Catch Weight Units, Units on Purchase Order and Units on Sales Order were surfaced on the Item Card. 

- AppSource App - Default Freeze Journal Template and Batch and Default Campaign Journal Template and Batch were added to the SD Catch Weight Setup Card.

- AppSource App - KPIs for Catch Weight Items and Shelf Life Items were added to the Setup Card.

- AppSource App - The SD Catch Weight Item FactBox was surfaced on the Item Card and Item List pages.

- AppSource App - The Enforce Catch Weight field was surfaced on the Item List page.

- AppSource App - New actions, fields and KPIs were surfaced on the Setup Card.

- AppSource App - Additional fields were added to the SD Catch Weight FastTab on the extension to the Item Card.

- AppSource App - The Campaign Journal on the Item Card now filters down to Item Journals of Type of Transfer rather than to Type of Item.

- AppSource App - The user is prompted that they need to turn on Lot Tracking for the Item if Enforce Shelf Life on an Item is enabled. 

- AppSource App - A Catch Weight Tolerance table and related functionality was created.

- AppSource App - The tolerance message raised on the extended pages was updated.

- AppSource App - Various UI changes were made to the Role Centre.

- AppSource App - The SD Catch Weight Shelf Life Expiration functionality on the item tracking lines was reworked. 

- AppSource App - Changes were made to the logic and UI when Confirming Alerts in the Shelf Life Worksheet. 

- AppSource App - The logic used to drive the Get Items action in the Shelf Life Worksheet was changed to use the Short Shelf Life Date from the Item Card if a value does not exist in the Minimum Shelf Life on the Item Shelf Life table.

- AppSource App - Various UI changes were made to the Item Shelf Life Worksheet. 

- AppSource App - The Shelf Life Message raised in the Item Tracking Lines page 6510 was updated.

- AppSource App - ToolTips were updated in the About, Activation and Subscription pages.

- AppSource App - ToolTips were updated in the SD Catch Weight Setup card.

- AppSource App - ToolTips were updated in the Shelf Life Worksheet.

- AppSource App - ToolTips were updated in the Shelf Life list.

- AppSource App - A new Activate Licence and Setup Wizard was created.

- AppSource App - A new action was added to the Setup Card called View Our Apps. This action opens a page on AppSource pointing to all our Simply Dynamics Ltd apps.

- AppSource App - The Lead Subscription Link from the Request Subscription action in the Product Activation page was updated.

- AppSource App - Changes were made to the Manage Subscriptions page.

- AppSource App - The notification to activate the app, displayed on fresh install of SD Inventory Cockpit, was added to the standard Business Central role centres.

### 2.0.0

#### Enhancements

- The Catch Weight module of SD Food and Beverage was split into its own project.

- Created a new extension table for Units.

- Created a custom PO List and Card using the new extension table.

- Created a Custom SO List and Card using the new extension table.

- Role Centre Activity Groups were split out into individual pages.

- A change was made in the SD-FBCW Item List to display records with a Catch Weight or a Shelf Life in bold.

- Added Catch Weight functionality to the Sales Return Orders.

- Made a change to copy the number of units per line when using copy doc functionality.

- Allow users to drill through on the Catch Weight and Shelf Life Activity Cues.

- The Stock Units Worksheet Action and the Shelf Life Worksheet Action were added to the Ribbon on the SD-FBCW Item List.

- Improved user experience/usability when creating Catch Weight Items and Shelf Life Items in SD-FBCW Item Card (43020204).

- Fixed a compile error of objects in a NAV 2018 environment.


#### Bug Fixes

- Fixed an issue were on some versions of NAV, the Item Extended sync was raising a "Transaction Error" when the Item Card was launched.

- Fixed an issue in the Item Units Stock Worksheet were entries were not appearing in the Items Unit Worksheet if no location was specified on the transaction line.

- Fixed an issue where the event trigger for unit weight was causing some lines on the Sales Order to reset.

- Fixed an issue where the number of units was not re-setting after the Journal line was posted.

- Fixed an issue with lines inserted when populating the Item Units Stock Worksheet SD-FBCW Units Stock Wksheet (43020209).

- Fixed an issue when populating the Item Units Stock Worksheet SD-FBCW Units Stock Wksheet (43020209) where the total quantity was doubled and entered into the quantity for blank locations.


### 1.0.0

#### Enhancements

Catch Weight and Expiry Dates module: 
- Created new tables, pages and associated functionality for Item Extended FANDB, Item Units, Item Shelf Life, Item Shelf Life Worksheet, Item Units Worksheet 
Created Readme.txt. 

- Reordered pages. 

- Keep extended item table in sync with item table using events. 

- Created a chart for the Catch Weight and Expiry Dates module and display in the Role Centre. 

- Created XMLports for Import/Export of Setup and Data. 

- Created a Role Center. 

- Generated Help files. 

- Created and Item List Page. 

- Created Extended Item Card Part Page. 

- Fixed the vertical alignment of the fields in the SD-FB Item Card. 

- In the Item Card SD-FB Item Card fixed the width of the SD FB fields in the Catch Weight Fast tab (the Avg and Min Weight fields). 

- In the SD-FB Item Shelf Life List page, displayed the Item description of the Item in Item No. 

- In the Stock Units Worksheet, displayed the Item Description for the Item No. 

- In the SD-FB Item List, moved the Catch Weight Enforcement and Shelf Life Enforcement columns beside the Item Description column.

LTA module: 
- Upgraded, renamed and renumbered code for LTA module. 

- Initial Code Merge. 

- Created Readme.txt. 

- Reordered pages. 

- Code restructure. 

- Created Event Hooks for LTA module. 

- Created and LTA Setup Card and table.
 
- Created Charts for the LTA module and display in the Role Centre. 

- Created XMLports for Import/Export of Setup and Data. 

- Created a Role Center.

- Generated Help files. 

- Add an option to open Sales Invoices and Credit Memos from the LTA Ledger Entry Lines on the LTA Ledger Entry Card. 

- UI improvements to the LTA Book Card. 

- Reordered fields in the General FastTab of the LTA Book Card for ease of user input. 

- Display the Item No. and the Item Description fields by default in the SD-FB LTA Price Group Line Page. 

MGP module: 
- Upgraded, renamed and renumbered code for MGP module.
 
- Initial Code Merge. 

- Created Readme.txt.
 
- Reordered pages. 

- Code restructure. 

- Renamed the List option to Standard to reflect functionality. 

- Created Charts for the MGP module and display in the Role Centre. 

- Created XMLports for Import/Export of Setup and Data. 

- Created a Role Center.
 
- Generated Help files. 

- Added a new flowField on the MGP Price Group table to count the number of records on the Price Group Line. 

- Group the Price List report by Item Category Code.
 
- In the Price Group Line Page - ensure the start and end dates are within the price book header start and end dates. 

- In the Price Group Line Page, to facilitate ease of data entry, on insert of a new line, default the UOM to the Item Sales UOM. 

- In the Price Group List, show the number of price lines associated with the Price Book. Allow KPI drill down to the Price Line Page. 

- In the Price Line Worksheet, change the Action Caption from Select prices to Get Prices. 

- Price Line Worksheet to allow the user to filter and make price changes easier, flow fields to the Item Category and Product Group were added to the table to allow users to filter and select for easier price changes. 

#### Bug Fixes

Catch Weight and Expiry Dates module: 
- Fix spelling mistake in the SD-FB Item Card. 

- In the Freeze Down Journal and the Reclass Journal fields in the SD-FB Item Extended Card and the SD-FB Item Card incorrect Journal Templates are displaying on drilldown. The Freeze Down Journal displays a list of Journals with a Journal Template Name of "RECLASS". While the Reclass Journal displays a list of Journals with a Journal Template Name of "Phys. Inv". 

- In the SD-FB Item Shelf Life List Page, fields are not being re-set/updated on change of Cross-Reference Type. 

- Drilling down on the Customer Min Shelf Life rules and the Vendor Min Shelf Life Rules from these pages is showing records for all Item Nos and not the Item that the user is currently on. 

- In the SD-FB Item Card selecting the Catch Weights and Shelf Life Action raises an error.
 
- Users should not be able to insert records into the Item Units Page. This page should be read only. 

- The following fields were moved from the Item Extended table to a Setup table - Freeze Down Journal Template, Freeze Down Journal Batch, Campaign Location Code, Campaign Reclass Journal Temp., Campaign Reclass Journal Batch.
 
- SD-FB Item Shelf Life WrkSheet - do not allow manual record input into this page. The only field users can update is the Confirm Action Checkbox. 

- A rename record message is raised on input of record into the SD-FB Item Shelf Life List Page. 

- The Description field on the Item-Cross References Page should be non-editable. 

- The Description field on the Item Shelf Life Worksheet should be non-editable. 

- In the Role Centre in the Catch Weights and Shelf Life Activity Group, the Cue link was renamed to Item Shelf Life to match the Navigation Pane. 

- Removed the New Item Unit link in the Role Centre from the Catch Weights and Shelf Life Activity Group as users cannot manually create an Item Unit Ledger. 

- Unit Stock Worksheet - when entries are calculated, records that have no stock location are not brought into the worksheet. 

- The Item Units Stock Worksheet should calculate the current unit item count up to the specified posting date (..Posting Date). 

- In the Goods In Shelf Life functionality, when receiving a PO the Expiration Date, calculated off the Default Purchase Shelf Life for the Item, is raising an error as the Expiration Date calculation (using the default Shelf Life) and the Shelf Life check is using different logic. 

- The Shelf Life functionality on the Purchase Line is re-setting the user updated Expiration Dates back to the system calculated date. 

- There is a blank Description field on the SD-FB Item Shelf Life Worksheet Page. 

LTA module: 
- Fixed bug whereby filters were not applying correctly if two LTA Books exist for the same Customer. 

- Settlement Amount and Total Settlement Amounts are calculating incorrectly. 

- In the LTA Book Page, in the Accrual/Settlement Fast Tab, the Field Captions are not displaying in full. 

- Fix the LTA Setup - No. Series to act as per standard NAV number series. 

- Calculation issue with LTA - refactored the code and restructured it to improve the functionality and to make it easier to understand from an end users point of view. 

- G/L Account not being stamped in the LTA Ledger Card - when the LTA Worksheet generates Accruals or Settlements, the G/L account on the LTA Book is not being stamped on the LTA Ledger Entry. 

- Error thrown when selecting the Accrual/Settlement Report Action from the LTA Worksheet. 

- Start and end dates on the Price Group Line should be within Price Group Header start and end dates. 

- Display the Item No. and Item Description by default in the SD-FB LTA Price Group Line Page, currently users would have to select choose columns to display the Item No. and Item Description. 

- LTA - Accrual Calculation - A Credit Memo quantity is treated as an Invoice quantity in the Accrual and Settlement Calculations. The amount for Credit Memo is being calculated as a positive amount rather than as a negative amount. 






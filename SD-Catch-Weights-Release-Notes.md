### 2.0.0

#### Enhancements



### 1.0.0

#### Enhancements

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
- Group the Price List report by Item Category Code 
- In the Price Group Line Page - ensure the start and end dates are within the price book header start and end dates. 
- In the Price Group Line Page, to facilitate ease of data entry, on insert of a new line, default the UOM to the Item Sales UOM. 
- In the Price Group List, show the number of price lines associated with the Price Book. Allow KPI drill down to the Price Line Page. 
- In the Price Line Worksheet, change the Action Caption from Select prices to Get Prices. 
- Price Line Worksheet to allow the user to filter and make price changes easier, flow fields to the Item Category and Product Group were added to the table to allow users to filter and select for easier price changes. 

Catch Weight and Expiry Dates module: 
- Created new tables, pages and associated functionality for Item Extended FANDB, Item Units, Item Shelf Life, Item Shelf Life Worksheet, Item Units Worksheet Created Readme.txt. 
- Reordered pages. 
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

#### Bug Fixes

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
- Movements for Catch Weight Items received in are not being stamped to the SD-FB Item Unit Ledger table.


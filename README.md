# Bond Store Excel Workbook

Macro-enabled Excel workbook for maintaining a ship’s bond store account.

The workbook is designed to track monthly bond store stock, crew purchases, representative issues, closing stock, stock value, and currency conversion. It combines formula-based calculations with VBA automation for routine monthly operations.

## Main features

* Monthly bond store stock accounting
* Opening stock, closing stock, and final stock calculation
* Crew bond tracking for up to 22 crew members
* Representative bond tracking in a separate section
* Automatic calculation of issued quantities and monetary value
* Rate of exchange field with automatic decimal separator normalization
* Printable price / stock list sheet
* One-click clearing of crew or representative bond entries
* Automatic hiding and unhiding of unused product rows
* Automatic hiding and unhiding of unused crew / representative columns
* “Create New Month” function to transfer remaining stock into the next month
* Keyboard shortcuts for fast entry:

  * `+` increases selected bond quantity by 1
  * `-` decreases selected bond quantity by 1

## Workbook structure

### WORKING

Main operational sheet.
It contains the opening stock, crew issue columns, representative issue columns, total calculations, closing stock, final stock, and stock value.

### PRICE

Printable stock / price list generated from the main working sheet.
It shows the remaining available stock in a cleaner format.

### Data

Reference sheet for crew list, representative list, and internal workbook settings.

## VBA automation

The workbook contains VBA macros for:

* clearing monthly issue data;
* hiding unused rows and columns;
* transferring closing stock to opening stock for the next month;
* updating the accounting month;
* entering a new rate of exchange;
* handling `+` / `-` keyboard shortcuts for faster data entry;
* normalizing decimal separators in price and exchange-rate cells.

## Typical monthly workflow

1. Enter or verify opening stock.
2. Enter crew and representative bond issues during the month.
3. Review calculated totals and final stock.
4. Print or export the price / stock list if required.
5. Run `Create New Month` to transfer remaining stock to the next month.
6. Enter the new rate of exchange when prompted.

## Notes

This workbook is intended for practical onboard bond store accounting and is optimized for fast manual use in Microsoft Excel with macros enabled.

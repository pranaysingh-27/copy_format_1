# copy_format_1
GOOGLE APP SCRIPT (Sheets): Copy Format from specific cells to required cells automatically. (Code for repetitive task).

Explanation of the code:

> Function Definition: The function `copyAndApplyFormat()` is designed to copy formatting from a specific range and apply it to a target range in a Google Spreadsheet.

> Active Spreadsheet and Sheet Selection:  
 - The function gets the active spreadsheet and selects the sheet named `'black_friday'`.

> Format Range Selection:  
 - The format to be copied is from the range `'A114:J120'`.

> Starting Row for Formatting:  
 - The formatting starts at row 121.

> Loop for Applying Format (50 iterations):  
 - A loop runs 50 times, incrementing the target row by 7 for each iteration (5 rows formatted, 2 rows skipped).

> Target Range for Format Application:  
 - For each iteration, the target range is calculated for 5 rows at a time, starting at `targetRow` and covering the next 4 rows (`targetRow + 4`).

> Format Application:  
 - The format from the source range (`A114:J120`) is copied and applied to the target range using `copyTo()` with the `{formatOnly: true}` option to only copy the format (not the data).

> Outcome:  
 - This process applies the copied format to 50 target blocks of 5 rows each, spaced by 2 rows, starting from row 121.

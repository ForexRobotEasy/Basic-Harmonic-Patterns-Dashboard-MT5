# Basic Harmonic Patterns Dashboard MT5

This code is a basic harmonic patterns dashboard for the MetaTrader 5 (MT5) trading platform. It is developed by the Forex Robot Easy Team and can be found on their website at [forexroboteasy.com](https://forexroboteasy.com).

## External Parameters

- `deviationLimit`: The deviation limit for pattern detection.

## Constants

- `MAX_SYMBOLS`: The maximum number of symbols to monitor.
- `MAX_PATTERNS`: The maximum number of patterns to detect.

## Pattern Structure

The `CPattern` structure is used to store information about each detected pattern. It includes the following properties:

- `type`: The type of the pattern.
- `entryPrice`: The recommended entry price for the pattern.
- `stopLossPrice`: The stop-loss price for the pattern.
- `takeProfitPrices`: An array of three take-profit prices for the pattern.
- `currentPrice`: The current price of the symbol.
- `ageOfPattern`: The age of the pattern in bars.
- `alertSettings`: The alert settings for pattern detection.

## Pattern Information Storage

The `patterns` array is used to store pattern information for each symbol. It is a two-dimensional array with dimensions `[MAX_SYMBOLS][MAX_PATTERNS]`. Each element of the array is an instance of the `CPattern` structure.

## Functions

1. `UpdatePattern`: This function is used to update pattern information for a symbol. It takes the symbol index, pattern type, entry price, stop-loss price, take-profit prices, current price, age of the pattern, and alert settings as parameters. It finds an empty pattern slot in the `patterns` array for the symbol and updates the corresponding elements with the provided information.

2. `DisplayDashboard`: This function is used to display the dashboard with the required columns. The code for displaying the dashboard is not provided in this code snippet.

3. `SortDashboard`: This function is used to sort the dashboard by a specific column. It takes the column index as a parameter. The code for sorting the dashboard is not provided in this code snippet.

4. `DisplayPatternOnChart`: This function is used to display the pattern on the chart for visual representation. It takes the symbol index and pattern index as parameters. The code for displaying the pattern on the chart is not provided in this code snippet.

## Main Function

The `OnStart` function is the main function of the code. It is executed when the script is started. The main loop of the code is inside this function. It performs the following steps:

1. Select symbols for monitoring.
2. Customize the color scheme.
3. Enter a loop that runs until the script is stopped.
   - Retrieve data for each selected symbol.
   - Detect harmonic patterns for each symbol.
   - Update pattern information for each symbol.
   - Display the dashboard.
   - Sort the dashboard if required.
   - Display the pattern on the chart if required.
   - Sleep for 1 second before the next iteration.

## Product Description

This code is a basic harmonic patterns dashboard for the MT5 trading platform. It allows traders to monitor multiple symbols for the detection of harmonic patterns. The dashboard displays information about detected patterns, including the pattern type, recommended entry price, stop-loss price, take-profit prices, current price of the symbol, and age of the pattern.

Traders can customize the color scheme of the dashboard to their preference. The dashboard can be sorted by different columns to prioritize patterns based on specific criteria. Traders can also choose to display the detected patterns on the chart for a visual representation.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please refer to the MQL5 platform. For detailed reviews and trading results of this product, you can visit the [product review page](https://forexroboteasy.com/forex-robot-review/review-basic-harmonic-patterns-dashboard-mt5-forex-tool/) on the Forex Robot Easy website.

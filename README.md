# LEGO-Set-Explorer
📊 Business case: This project revolves around a comprehensive dataset of LEGO sets released between 1970 and 2022. Rich with essential details such as themes, piece counts, recommended age ranges, retail prices, and images, this dataset forms the backbone of an innovative tool, consists of a single table containing 18,459 records across 14 fields. The primary objective is to develop an interactive tool that allows users to efficiently explore the entire range of LEGO sets and refine their choices based on specific criteria.

🔹 Key Steps & Technical Highlights: 

✅Load and prepare the data for analysis:

•	The initial objective is to load and review the raw LEGO dataset, utilizing Power Query to clean and profile the data. This includes performing essential data preparation tasks, such as refining columns and ensuring data accuracy. Additionally, calculated columns and DAX measures will be created to facilitate in-depth analysis.

•	Connect to the lego_sets CSV file. Remove the minifigs, bricksetURL and thumbnailURL fields, review data types for accuracy, and filter out records with no price, age, pieces or image URL values.

•	Create conditional columns for Age Range (“Over 18”, “10 to 17”, “5 to 9”, “1 to 4”) and Price Range (>$500 = “$”, >$100 = “$”, >$50 = “$”, >$25 = “$”, otherwise “$”).

•	Add measures to calculate the number of distinct sets (Total Sets) and theme groups (Total Groups), as well as the average age (Avg. Age), price (Avg. Price) and pieces (Avg. Pieces).

✅Design the layout and visuals

•	The second objective is to create a well-structured report layout, incorporate visually engaging elements and interactive filters into the canvas, and carefully configure cross-filtering behavior to ensure seamless interaction and data exploration between visuals.

•	Insert card visuals to show Total Sets, Avg. Pieces and Avg. Price.

•	Add slicers to filter based on the theme group, theme and age range.

•	Insert a table to show name, set_id, theme, Age Range, Avg. Pieces, Avg. Price and Price Range.

•	Add a report section to show details for a selected set, including the name, image, price, year, pieces and age.

•	Edit visual interactions to prevent table selections from filtering the top-level cards.

✅Add interactive components

•	The final objective is to enhance the report's interactivity by incorporating advanced features such as parameters, tooltips, bookmark actions, and page navigation buttons.

•	Create a numeric range parameter (Max Price) ranging from 0-850 and incrementing by 5. Add a slicer to the page, and a measure that allows you to filter the table based on the maximum price selected.

•	Enable tooltips on the table to display the image of each LEGO set on hover.

•	Use bookmarks and button actions to allow users to reset all filters on the page.

•	Create a new report page with a decomposition tree visual to analyze Total Sets by category, theme group, theme and name, and add buttons to navigate between pages.

✅Key Insights: 

•	Data at a Glance: 4,385 LEGO sets analyzed, with an average of 411 pieces per set and an average price of $45.

•	Top Themes: Star Wars emerged as the most popular theme, especially in the "Over 18" age range.

•	Top Price Tag: The AT-AT, a Star Wars-themed set, is the most expensive at $849.99.

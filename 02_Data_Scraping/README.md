# Experiment 2 - Data Scraping

**Run:** Open `project.json` and click **Run**. The demo reads the included `Data/sample_table.html` and writes `Output/scraped_table.csv`.

**Native UiPath activity chain for your practical:** `Use Application/Browser` -> `Extract Table Data` -> store in a `DataTable` variable (e.g. `scrapedData`) -> `Output Data Table` (optional) -> `Write Range` to Excel.

**Important distinction:** The included automatic demo parses the supplied local HTML fixture so it can run without depending on a third-party website changing. It is not a live-browser `Extract Table Data` recording. To reproduce the exact lab activity on a live site, indicate the table with UiPath's extraction wizard and save the generated target. Pages 6-8 of your record show this native activity flow.

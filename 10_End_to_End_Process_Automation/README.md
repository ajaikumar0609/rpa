# Experiment 10 - End-to-End Process Automation

**Run:** Open `project.json` and click **Run**. It reads `Data/requests.csv`, validates required values, applies a 5% fee to valid amounts, catches row-level errors, and generates three outputs: `Output/processed_requests.csv`, `Output/rejected_requests.csv`, and `Output/summary.txt`.

**Native UiPath activity chain for your practical:** Read the input file/Excel -> `For Each Row in Data Table` -> validate required fields -> apply a business rule -> write valid and rejected records -> generate summary -> wrap risky operations in `Try Catch` and log useful errors.

This local demo is intentionally deterministic so you can practise the complete data flow without an external system. Pages 30-31 of your record show the end-to-end workflow and output.

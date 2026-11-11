# Experiment 3 - Email Automation

**Run:** Open `project.json` and click **Run**. It creates `Output/RPA_Lab_Test_Email_DRAFT.eml`. The sample recipient is intentionally a placeholder; the project does **not** send an email automatically.

**Native UiPath activity chain for your practical:** Assign `toAddress`, `subject`, `body`, and optional `attachmentPath` -> configure the email account/connection -> `Send Outlook Mail Message` (or the provider-specific activity) -> verify the Sent folder and recipient inbox.

Do not put passwords or API secrets in the workflow. Replace the placeholder recipient only with an authorized test address. Outlook version, account configuration and package availability determine which mail activity works; the record's screenshot uses `Send Outlook Mail Message`. Pages 9-11 show this workflow.

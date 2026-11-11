# RPA Lab - 10 Experiment Activity Map

These projects are **Windows / Visual Basic UiPath starter projects**. Local demonstration workflows run without live account credentials. Activities that need desktop targets, provider connections, or Orchestrator permissions must be captured/configured on the lab computer.

| Ex. | Experiment | Main UiPath activities to practise | What the included one-click demo does |
|---|---|---|---|
| 1 | UiPath Studio Familiarization | Sequence, Assign, Message Box | Fully builds and displays the welcome message. |
| 2 | Data Scraping | Use Application/Browser, Extract Table Data, Output Data Table, Write Range | Parses the included HTML table into CSV; use the extraction wizard for a live website. |
| 3 | Email Automation | Assign, Send Outlook Mail Message | Creates an `.eml` draft; sending requires your authorized mail configuration. |
| 4 | Excel/PDF Automation | Read Range, For Each Row in Data Table, Write Range, Read PDF Text | Processes sample rows and a PDF text fixture; use the provided XLSX/PDF with the native activities. |
| 5 | Web Automation | Use Application/Browser, Type Into, Click, Get Text | Opens a browser search URL; capture live selectors in Studio. |
| 6 | Image Recognition | Find Image, Click Image, If/verification | Opens a local practice page with a stable blue target; capture the target on your screen. |
| 7 | Multi-Bot Collaboration | ProducerBot, ConsumerBot; optionally Add Queue Item / Get Transaction Item | Two separate projects exchange a CSV work queue. |
| 8 | UiPath Orchestrator | Publish, Processes, Jobs, Schedules, Queues, Assets, Logs | Generates a lab checklist; real tenant actions require institutional access. |
| 9 | UiPath AI Fabric Integration | Approved AI activity / Invoke OpenAI AI Model; validate response | Offline fallback by default; optional API request when a key is configured. |
| 10 | End-to-End Process Automation | Read input, For Each Row, If, Try Catch, Write outputs, summary | Validates records, calculates totals, separates rejected rows, writes summary. |

## How to open a project

1. Extract the ZIP to a normal folder, e.g. `Documents\RPA_Lab_10_Experiments`.
2. Open UiPath Studio Desktop and sign in.
3. Choose **Open** / **Open Local Project**, then select that experiment's `project.json`.
4. Allow Studio to restore `UiPath.System.Activities` from the configured official package feed.
5. Open `Main.xaml` and click **Run**.
6. Local outputs are written into that experiment's `Output` folder.

Experiment 7 contains two independent projects: run `ProducerBot\project.json` first, then `ConsumerBot\project.json`.

## Compatibility / limitations

- The project metadata targets `Windows` compatibility and Visual Basic expressions. These projects are not Windows-Legacy projects.
- The XAML demos use the UiPath `Invoke Code` activity for deterministic local sample processing. Read each experiment README for the exact native activities to use in your practical.
- This package was generated and structurally checked here, but it has **not been executed inside UiPath Studio on your Windows computer**. A clean project restore/build and a run on your machine are still required.
- Live website selectors, image targets, Outlook credentials, Excel installation/COM support, Orchestrator tenant access, and AI provider credentials vary by computer/account. Do not expect those external services to run without setup.
- The Email project creates a draft only; it does not send an email to a placeholder address. The AI experiment's default offline output is labelled as a mock and is not an AI model response.

## Sample external docs

- Project compatibility and project files: https://docs.uipath.com/studio/standalone/latest/user-guide/about-automation-projects
- Project.json: https://docs.uipath.com/studio/standalone/latest/user-guide/about-the-projectjson-file
- Excel activities: https://docs.uipath.com/activities/other/latest/productivity/about-the-excel-activities-pack
- Extract Table Data: https://docs.uipath.com/activities/other/latest/ui-automation/n-extract-data
- Read PDF Text: https://docs.uipath.com/activities/other/latest/document-understanding/read-pdf-text
- Outlook email activity: https://docs.uipath.com/activities/other/latest/productivity/send-outlook-mail
- Orchestrator queues: https://docs.uipath.com/orchestrator/automation-cloud/latest/user-guide/studio-activities-used-with-queues

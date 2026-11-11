# Experiment 7 - Multi-Bot Collaboration

This experiment contains **two separate UiPath projects**.

**Run in order:**
1. Open `ProducerBot/project.json` and Run. It creates `Shared/queue_input.csv`.
2. Open `ConsumerBot/project.json` and Run. It reads the shared file and creates `Shared/queue_output.csv`.

This is the file-based coordination option allowed in your lab record. For the Orchestrator queue version shown in the screenshots, replace the shared-file handoff with `Add Queue Item` in ProducerBot and `Get Transaction Item`/`Set Transaction Status` in ConsumerBot. The robot must be connected to Orchestrator and have queue permissions; queue activities do not work offline. Pages 21-23 show the producer/consumer queue design.

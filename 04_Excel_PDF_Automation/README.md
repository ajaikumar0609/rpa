# Experiment 4 - Excel/PDF Automation

**Run:** Open `project.json` and click **Run**. The included demonstration processes the sample rows and creates `Output/processed_students.csv`; it also copies the matching text fixture to `Output/pdf_text_fixture_output.txt`.

**Included inputs:** `Data/StudentMarks.xlsx`, `Data/students.csv`, `Data/SampleDocument.pdf`, and `Data/sample_pdf_text.txt`. The PDF is a text-based sample.

**Native UiPath activity chain for your practical:** `Use Excel File` -> `Read Range` into a `DataTable` -> `For Each Row in Data Table` -> process values -> `Write DataTable to Excel`/`Write Range`; then `Read PDF Text` with `Data/SampleDocument.pdf` as `FileName` and a String variable as `Text`; display/save the extracted text.

**Important distinction:** The auto-run demonstration uses CSV for its local row-processing fallback and the text sidecar for a deterministic PDF example. It does not itself invoke the Excel or PDF-specific UiPath packages. Use the listed native activities to reproduce the exact lab record. Your record's pages 12-14 show Excel Read/Write and PDF text extraction.

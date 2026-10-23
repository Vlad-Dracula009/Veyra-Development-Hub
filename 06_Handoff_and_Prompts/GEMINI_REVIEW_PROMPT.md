# Gemini — Independent Verification Prompt

Independently verify the current Veyra task using the supplied project documents and relevant code/logs. Do not rely on conclusions from other assistants without checking evidence.

Return:
1. Confirmed facts with file/log evidence.
2. Assumptions or missing evidence.
3. Alternative explanations for the reported behavior.
4. Findings ranked by severity, with precise file paths and relevant code locations.
5. The smallest safe next step and a test plan.
6. Any disagreement with the current documented diagnosis, and the evidence that supports your view.

Do not modify code unless explicitly asked. Do not request secrets or `.env` values. Do not enable API billing or purchase credits. Keep the investigation read-only and follow one-change-at-a-time testing rules if a later change is authorized.

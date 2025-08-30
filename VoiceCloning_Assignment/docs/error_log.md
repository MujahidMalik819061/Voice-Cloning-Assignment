
# Error Log

Log every error you encounter when running the notebook or scripts. For each entry include:
- Timestamp (ISO)
- Step / Command
- Full error message (copy-paste)
- Short diagnosis
- Fix attempted and result

Example entry:
- 2025-08-30T12:34:56+05:30
- Step: `pip install openvoice-cli`
- Error: `Could not find a version...`
- Diagnosis: PyPI / Python compatibility
- Fix: Installed with `--pre` or used a different torch wheel

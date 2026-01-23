# SOS Assignment 3 SOMs

## General Notes

Please create and activate a virtual environment before running the notebooks.

### Virtual Environment Setup
1. Navigate to your project folder
2. Create a virtual environment  
   `python3 -m venv <your_venv_name>`
3. Activate the virtual environment  
   `source <your_venv_name>/bin/activate`
4. Upgrade pip  
   `pip install --upgrade pip`
5. Install required packages  
   `pip install -r requirements.txt`

If you install new packages during development:
- Update the requirements file using  
  `python -m pip freeze > requirements.txt`
- Mention the update in the commit message
- Add `<your_venv_name>/` to `.gitignore`

---

## Notes for Part A - Ontology and Setup

### SOM Toolbox Source

The SOM Toolbox files were taken from the TUWEL-provided version, not directly from the public GitHub repository.  
Some file names differ between the two versions.

Observed differences:
- `training_assignment.ipynb` (GitHub) → `SOM_analysis_report.ipynb` (TUWEL)
- `coding_assignment.ipynb` → merged into `SOM_analysis_report.ipynb`
- `pysomvis.py` → `somtoolbox.py`
- `minisom-py`, `SOMTool_Parse.py` are unchanged
- Additional files in the TUWEL version:
  - `styling_linear_mappers.html`
  - `temps.xlsx`
  - `timeseries.ipynb`

The purpose of these additional files is currently unclear and they are not required for this assignment.

---

### Provenance and Ontology Tracking

The ontology-based provenance tracking is implemented directly in the main analysis notebook `MainNB.ipynb`.

The structure is based on the example provided in:
- `TemplateNotebookProvenanceDoc.ipynb`

All activities (Business Understanding, Data Understanding, Data Preprocessing, and later SOM Training) are documented using:
- **PROV-O** for process and agent tracking
- **schema.org** for dataset descriptions
- **Croissant** for describing dataset structure and feature groups

This ensures that all analysis steps and transformations are logged in a machine-readable way.

---

### Starvers / Triple Store

The notebook uses `starvers.starvers.TripleStoreEngine` to upload RDF triples to the TU Wien Starvers knowledge graph.

Although the `starvers` package is not available via pip or GitHub, it is provided in the TU Wien environment and works as required for the assignment.

---

### Important Execution Note

If you work in `MainNB.ipynb`, **always update and execute the cell defining the `executed_by` variable** with your student ID:

```python
executed_by = 'stud-id_XXXXXXXX'
```

## Notes for B (Dataset)

Fars: https://www.openml.org/d/40672

The dataset needs to meet the following requirements:
- 1000 instances
- 20 features 
- 4 classes

It has
- 100968 instances
- 30 features
- 8 classes
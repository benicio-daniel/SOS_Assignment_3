# SOS Assignment 3 SOMs

## General Notes
Please download the requirement.txt to your venv.\
Remeber that it is:
1. Navigate to your desired folder in zsh
2. `python3 venv <your venv name>`
3. `source <your venv name>/bin/activate`
4. `pip install --upgrade pip`
5. `pip install -r requirements.txt`\
If you download new packages while working, please type:
- `python -m pip freeze > requirements.txt`\
and mention it in the commit message that you updated it.  
Also add the "your venv name" to the .gitignore file


## Notes for A (Onthologie and Setup)
### Github Repo SOM Toolbox
I have downloaded the version of SOM TOOLBOX repo from tuwel, not from github. The file names are different than from github, and I track them here. I have choosen the Tuwel version that has a buch more stuff in it that I dont know if we need them
- The required in the original github repo "training_assignment.ipynb" is called "SOM_analysis_report.ipynb" in the tuwel version
- "coding_assingment.ipynb" is "SOM_analyis_report"
- "pysomvis.py" is "somtoolbox.py"
- "minisom-py", "SOMTool_Parse.py" are the same
- New are: "styling_linear_mappers.html" "temps.xlsx" "timeseries.ipynb"\
I still have no clue what they do

### The template for onthology tracking of what we do
Is in "TemplateNotebookProvenanceDoc.ipynb" which is the example of how we should conduct this exercise.
I have adapted everything in A) so far into "MainNB.ipynb" except I have no Idea where the starverse file is.

### Ontologies
The ontologies are established in the same notebook "MainNB" that we do all of our work of analysis in. This ensures that all of our work and changes are uploaded to a onthology. See the "TemplateNotebookProvenanceDoc.ipynb" to how it should be done\
For some reason in the notebook they used starvers.starvers, which is the engine to add the triples to the starverse which is a onthology of the TU were they store that. The file of starvers that has the TriplesStoresEngine is not in the repo, not in pip or on tuwel, googeling doesnt bring anythin up. I asked in the forum to see if there is a mistake.\

*Important* If you do work in the notebook, please excecute the  the cell with the `excecuted_by` variable to your MA number so that the verse can log what you did.
## Notes for B (Dataset)

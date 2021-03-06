# se-2018-class-profile
An analysis of se 2018 class profile survey results.

## Workflow
The data first gets normalized by hand so that it can be processed a lot easier. This is a back and forth process, and is documented in [here](https://github.com/chrisjluc/se-2018-class-profile/blob/master/Normalization_Plan.md).

After data is preprocessed using `Data Preprocessing.ipynb` it will output a CSV that can be read by the various notebooks. These notebooks should handle a specific category of the analysis (highlighted in the [analysis plan](https://paper.dropbox.com/doc/Analysis-Plan-FFNs8uboDURRprv4qbZGQ)) to allow for concurrent development. Data that is shared across notebooks can be added to `Data Preprocessing.ipynb`. Functions may be copied across notebooks to speed up workflow.

## Directory Structure
### Private
Directory that is not checked in. This private folder is used to store any data that the project works with. 

### Data
Store test and intermediary data. **Note**: Never commit real data to this repo.

### Analyses
Holds notebooks that process data and output final charts, graphs to used in the final report. Notebooks should be divided into modular pieces that allows for concurrent workflow to avoid version control issues.

### Utils
Any tools or utilities used to help facilitate and ease analyses. Shared utilities across analyses can go here such as data preprocessing that creates shared data columns like `coop_salary_avg`.

## Running the project
### Installation
Make sure you have `jupyter` installed. If you're on macOS, you can install it
with homebrew. Otherwise, you can probably install it with `pip`.

### Running Jupyter
Once you have `jupyter` installed, you can run
```
jupyter notebook
```

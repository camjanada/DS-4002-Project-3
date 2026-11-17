# Scripts

| Notebook | Purpose | When to run |
|---|---|---|
| [`metpulldata.ipynb`](metpulldata.ipynb) | Collects painting images and metadata from the Met API and exports `met_sample_balanced.zip`. | Run if you want to repeat data collection. |
| [`ds_project_3.ipynb`](ds_project_3.ipynb) | Extracts ResNet-18 features, trains and evaluates logistic regression, compares feature counts with cross-validation, and exports the model results. | Run to reproduce the reported results using the archived dataset. |

## Running the analysis

1. Download the archived dataset using the instructions in [`DATA/README.md`](../DATA/README.md).
2. Open `ds_project_3.ipynb` in Google Colab. Rename the archive to `paintings.zip` and upload it through Colab’s Files panel.
3. Run the setup, painting-level analysis, and artist-grouped analysis cells. Run the artist-grouped cross-validation before the ungrouped cross-validation, then run the final export cell.

See the [main README](../README.md) for package versions, expected results, and output locations.
